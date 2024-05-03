# Comparing `tmp/mutation-profile-0.1.0.tar.gz` & `tmp/mutation-profile-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutation-profile-0.1.0.tar", max compression
+gzip compressed data, was "mutation-profile-0.2.0.tar", max compression
```

## Comparing `mutation-profile-0.1.0.tar` & `mutation-profile-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    35149 2022-07-04 00:38:03.955821 mutation-profile-0.1.0/LICENSE
--rw-r--r--   0        0        0     7726 2022-07-04 02:07:23.909761 mutation-profile-0.1.0/README.md
--rw-r--r--   0        0        0     6148 2022-07-04 01:20:26.898322 mutation-profile-0.1.0/mutation_profile/.DS_Store
--rw-r--r--   0        0        0       22 2022-07-04 00:14:44.544084 mutation-profile-0.1.0/mutation_profile/__init__.py
--rw-r--r--   0        0        0     5694 2022-07-04 01:16:27.315712 mutation-profile-0.1.0/mutation_profile/__main__.py
--rw-r--r--   0        0        0    13251 2022-07-04 00:56:46.990245 mutation-profile-0.1.0/mutation_profile/mutation_profile.py
--rw-r--r--   0        0        0      640 2022-07-04 01:47:29.244627 mutation-profile-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8816 2022-07-04 02:07:45.976201 mutation-profile-0.1.0/setup.py
--rw-r--r--   0        0        0     8565 2022-07-04 02:07:45.976614 mutation-profile-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0    35149 2024-05-03 10:11:33.825111 mutation-profile-0.2.0/LICENSE
+-rwxr-xr-x   0        0        0     8052 2024-05-03 10:11:33.843537 mutation-profile-0.2.0/README.md
+-rwxr-xr-x   0        0        0       22 2024-05-03 10:11:34.098472 mutation-profile-0.2.0/mutation_profile/__init__.py
+-rwxr-xr-x   0        0        0     5694 2024-05-03 10:11:34.102472 mutation-profile-0.2.0/mutation_profile/__main__.py
+-rwxr-xr-x   0        0        0    13256 2024-05-03 10:37:25.973619 mutation-profile-0.2.0/mutation_profile/mutation_profile.py
+-rwxr-xr-x   0        0        0      661 2024-05-03 11:02:47.336525 mutation-profile-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9184 2024-05-03 11:21:36.935315 mutation-profile-0.2.0/setup.py
+-rw-r--r--   0        0        0     8933 2024-05-03 11:21:36.935728 mutation-profile-0.2.0/PKG-INFO
```

### Comparing `mutation-profile-0.1.0/LICENSE` & `mutation-profile-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mutation-profile-0.1.0/README.md` & `mutation-profile-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Mutation profile
 
-This tool was developed during Monkeypox 2022 outbreak to explore the mutational profiles/signatures of this virus, but can be of broad application to other species. It can be used to rapidly obtain the sequence context (size defined by the user) flanking SNPs of interest and determine their mutational profile according to the user's specifications (e.g. APOBEC3-mediated viral genome editing GA>AA and TC>TT replacements)
+This repository comprises the script(s) developed during Monkeypox 2022 outbreak to explore the mutational profiles/signatures of this virus, but that can be of broad application to other species. Currently, it comprises the script(s):
+- _get_mutation_profile.py_ that can be used to rapidly obtain the sequence context (size defined by the user) flanking SNPs of interest and determine their mutational profile according to the user's specifications (e.g. APOBEC3-mediated viral genome editing GA>AA and TC>TT replacements)
 
 ## Input/Output of _get_mutation_profile.py_
 									
 **OPTION1**   
 _Inputs:_    
 1. TSV file with the columns POS REF ALT (i.e. 1-indexed reference position, reference allele and alternative allele)
 2. Fasta file including the reference genome
@@ -36,15 +37,25 @@
 
 
 ## Dependencies and installation
 To run the _get_mutation_profile.py_ you will need:
 - biopython
 - pandas
 
+### pip installation
+```bash
+pip install mutation-profile
+mutation-profile -h
+```
 
+### conda installation
+```bash
+conda create -n mutation-profile -c vmixao mutation-profile
+conda activate mutation-profile # if you created the conda environment
+mutation-profile -h
 ```
 
 ## Usage
 
 ```bash
   -h, --help            show this help message and exit
 
@@ -82,28 +93,28 @@
 
 ## Examples using Monkeypox 2022 outbreak data available at [_examples/_](https://github.com/insapathogenomics/mutation_profile/tree/main/examples)
 
 ### Option 1 (this option reflects part of the analysis performed in the publication)
 Providing a TSV file with the columns POS REF ALT (i.e. 1-indexed reference position, reference allele and alternative allele) and a fasta file including the reference genome (can be the same alignment or a normal fasta sequence).
 
 ```bash
-python get_mutation_profile.py -f alignment_Figure1B.fasta -m positions_of_interest_POS_REF_ALT.txt -r 'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome' -b 10 -a 10 -o OPTION1
+mutation-profile -f alignment_Figure1B.fasta -m positions_of_interest_POS_REF_ALT.txt -r 'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome' -b 10 -a 10 -o OPTION1
 ```
 
 _Output:_    
 1. TSV file with the mutation context and profile
 <p align="center">
 	<img width="636" alt="Captura de ecrã 2022-06-17, às 15 17 41" src="https://user-images.githubusercontent.com/19263468/174316512-056bb280-a89e-4d81-9ba3-6065f6a9a0f1.png">
 </p>
 
 ### Option 2
 Providing a TSV file with the columns ID POS REF ALT (i.e. samples id, 1-indexed reference position, reference allele and alternative allele) and a fasta file including the reference genome (can be the same alignment or a normal fasta sequence).
 
 ```bash
-python get_mutation_profile.py -f alignment_Figure1B.fasta -m positions_of_interest_ID_POS_REF_ALT.txt -r 'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome' -b 10 -a 10 -o OPTION2
+mutation-profile -f alignment_Figure1B.fasta -m positions_of_interest_ID_POS_REF_ALT.txt -r 'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome' -b 10 -a 10 -o OPTION2
 ```
 
 _Outputs:_    
 1. TSV file with the mutation context and profile for each sample present in the TSV input
 <p align="center">
 	<img width="849" alt="Captura de ecrã 2022-06-17, às 15 21 20" src="https://user-images.githubusercontent.com/19263468/174317025-e090f7f8-17a4-4001-863f-cd965dfff9a6.png">
 </p>
@@ -113,15 +124,15 @@
 	<img width="1145" alt="Captura de ecrã 2022-06-17, às 15 23 07" src="https://user-images.githubusercontent.com/19263468/174317375-d17183e8-0f9c-46a6-ab83-9f1e212c4854.png">
 </p>
 
 ### Option 3
 Providing a single-column file with a list of 1-indexed reference positions of interest and a fasta Multiple Sequence Alignment including the reference genome.
 
 ```bash
-python get_mutation_profile.py -f alignment_Figure1B.fasta -m Monkeypox_positions_of_interest.tsv -r 'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome' -b 10 -a 10 -o OPTION3
+mutation-profile -f alignment_Figure1B.fasta -m Monkeypox_positions_of_interest.tsv -r 'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome' -b 10 -a 10 -o OPTION3
 ```
 
 _Outputs:_     
 1. TSV file with the mutation context and profile for each sample present in the alignment
 <p align="center">
 	<img width="1106" alt="Captura de ecrã 2022-06-17, às 15 31 56" src="https://user-images.githubusercontent.com/19263468/174319330-2702cf97-af7d-44e9-b7ca-2bf2f0f612ed.png">
 </p>
@@ -135,10 +146,11 @@
 
 ```bash
 python ReporTree/scripts/alignment_processing.py -align alignment_Figure1B.fasta -o Monkeypox --use-reference-coords -r 'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome' --keep-gaps --get-positions-interest
 ```
 
 ## Citation
 
-If you use this tool please cite the article where it was first described:
+If you use this script please cite the article where it was first described:
 
-Isidro, J., Borges, V., Pinto, M. et al. (2022) Phylogenomic characterization and signs of microevolution in the 2022 multi-country outbreak of monkeypox virus. _Nature Medicine_. https://doi.org/10.1038/s41591-022-01907-y
+Isidro, J., Borges, V., Pinto, M. et al. Phylogenomic characterization and signs of microevolution in the 2022 multi-country outbreak of monkeypox virus.  
+_Nature Medicine_ (2022). https://doi.org/10.1038/s41591-022-01907-y
```

### Comparing `mutation-profile-0.1.0/mutation_profile/__main__.py` & `mutation-profile-0.2.0/mutation_profile/__main__.py`

 * *Files identical despite different names*

### Comparing `mutation-profile-0.1.0/mutation_profile/mutation_profile.py` & `mutation-profile-0.2.0/mutation_profile/mutation_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 	
 def mut_profile(sequences, before, after, ref, ref_seq, coords, profiles, mutation_df):
 	""" obtain a dataframe with a summary of the mutation profile
 	input: fasta and mutations
 	output: dataframe """
 	
 	prof = profiles.split(",")
-	ref_seq_nogaps = ref_seq.ungap("-")
-	
+	ref_seq_nogaps = ref_seq.replace("-", "")
+
 	if "POS" in mutation_df.columns and "ALT" in mutation_df.columns and "REF" in mutation_df.columns:
 		mutations = mutation_df["POS"].values.tolist()
 		ref_nucl = mutation_df["REF"].values.tolist()
 		alt_nucl = mutation_df["ALT"].values.tolist()
 		if "ID" in mutation_df.columns:
 			samples = mutation_df[mutation_df.columns[0]].values.tolist()
 			info = {"sample": samples, "ref_position": mutations, "ref": ref_nucl, "alt": alt_nucl, "motif_ref": [], "observed_profile": [],  "profile_of_interest": []}
```

### Comparing `mutation-profile-0.1.0/pyproject.toml` & `mutation-profile-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "mutation-profile"
-version = "0.1.0"
+version = "0.2.0"
 description = "A bioinformatics solution to determine SNP flanking sequences and mutation profile"
 authors = ["Veronica Mixao <vmixao@gmail.com>"]
 license = "GPL-3.0-only"
 
 readme = "README.md"
 
 repository = "https://github.com/insapathogenomics/mutation_profile"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-biopython = "^1.70"
+biopython = "^1.80"
 pandas = "^1.4.3"
 textwrap3 = "^0.9.2"
+requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mutation-profile-0.1.0/setup.py` & `mutation-profile-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 packages = \
 ['mutation_profile']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['biopython>=1.70,<2.0', 'pandas>=1.4.3,<2.0.0', 'textwrap3>=0.9.2,<0.10.0']
+['biopython>=1.80,<2.0',
+ 'pandas>=1.4.3,<2.0.0',
+ 'requests>=2.31.0,<3.0.0',
+ 'textwrap3>=0.9.2,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['mutation-profile = mutation_profile.__main__:main']}
 
 setup_kwargs = {
     'name': 'mutation-profile',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': 'A bioinformatics solution to determine SNP flanking sequences and mutation profile',
-    'long_description': '# Mutation profile\n\nThis tool was developed during Monkeypox 2022 outbreak to explore the mutational profiles/signatures of this virus, but can be of broad application to other species. It can be used to rapidly obtain the sequence context (size defined by the user) flanking SNPs of interest and determine their mutational profile according to the user\'s specifications (e.g. APOBEC3-mediated viral genome editing GA>AA and TC>TT replacements)\n\n## Input/Output of _get_mutation_profile.py_\n\t\t\t\t\t\t\t\t\t\n**OPTION1**   \n_Inputs:_    \n1. TSV file with the columns POS REF ALT (i.e. 1-indexed reference position, reference allele and alternative allele)\n2. Fasta file including the reference genome\n\n_Output:_    \n1. TSV file with the mutation context and profile\n\n**OPTION 2**     \n_Inputs:_   \n1. TSV file with the columns ID POS REF ALT (i.e. sample ID, 1-indexed reference position, reference allele and alternative allele)\n2. Fasta file including the reference genome\n\n_Outputs:_    \n1. TSV file with the mutation context and profile for each sample present in the TSV input\n2. TSV file with a summary report for each position of interest including the different patterns observed and their respective frequency\n\n_NOTE: For options 1 and 2 the order of the columns in the input 1 is not important but their name is (ID, POS, REF, ALT)!!_\n\n**OPTION 3**  \n_Inputs:_    \n1. Single-column file with a list of 1-indexed reference positions of interest   \n2. Multiple Sequence Alignment (fasta) including the reference genome    \n\t\t\t\t\t\t\t\t\t\n_Outputs:_     \n1. TSV file with the mutation context and profile for each sample present in the alignment\n2. TSV file with a summary report for each position of interest including the different patterns observed and their respective frequency\n\n_TIP: If you do not know your positions of interest, you can run the script _alignment_processing.py_ of [ReporTree](https://github.com/insapathogenomics/ReporTree) and it will provide a list of positions of interest according to your specifications._\n\n\n## Dependencies and installation\nTo run the _get_mutation_profile.py_ you will need:\n- biopython\n- pandas\n\n\n```\n\n## Usage\n\n```bash\n  -h, --help            show this help message and exit\n\nMutation profile:\n  Provide input/output specifications\n\n  -f FASTA, --fasta FASTA\n                        [MANDATORY] Input sequence file (fasta)\n  -m MUTATION, --mutation_list MUTATION\n                        [MANDATORY] Input mutation list that can be: 1)\n                        single-column file with 1-based reference position\n                        information (in this case the fasta file must be a\n                        multiple sequence alignment of all the sequences of\n                        interest); OR 2) tsv file with the columns POS, REF,\n                        and ALT where POS = 1-based reference position. If you\n                        want to include information for more than one sample\n                        per position, add also the column \'ID\' (note that the\n                        order of the columns is not important but their name\n                        is!)\n  -r REF, --reference REF\n                        [MANDATORY] Reference sequence name\n  -b BEFORE, --before BEFORE\n                        [OPTIONAL] Number of nucleotides to report BEFORE the\n                        mutation (default = 5)\n  -a AFTER, --after AFTER\n                        [OPTIONAL] Number of nucleotides to report AFTER the\n                        mutation (default = 5)\n  -p PROFILES, --profiles PROFILES\n                        [OPTIONAL] Comma-separated list of mutational profiles\n                        of interest (upper-case!). Default = \'GA>AA,TC>TT\'\n  -o OUTPUT, --output OUTPUT\n                        [OPTIONAL] Tag for output file name. Default =\n                        Mutation_profile\n```\n\n## Examples using Monkeypox 2022 outbreak data available at [_examples/_](https://github.com/insapathogenomics/mutation_profile/tree/main/examples)\n\n### Option 1 (this option reflects part of the analysis performed in the publication)\nProviding a TSV file with the columns POS REF ALT (i.e. 1-indexed reference position, reference allele and alternative allele) and a fasta file including the reference genome (can be the same alignment or a normal fasta sequence).\n\n```bash\npython get_mutation_profile.py -f alignment_Figure1B.fasta -m positions_of_interest_POS_REF_ALT.txt -r \'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome\' -b 10 -a 10 -o OPTION1\n```\n\n_Output:_    \n1. TSV file with the mutation context and profile\n<p align="center">\n\t<img width="636" alt="Captura de ecrã 2022-06-17, às 15 17 41" src="https://user-images.githubusercontent.com/19263468/174316512-056bb280-a89e-4d81-9ba3-6065f6a9a0f1.png">\n</p>\n\n### Option 2\nProviding a TSV file with the columns ID POS REF ALT (i.e. samples id, 1-indexed reference position, reference allele and alternative allele) and a fasta file including the reference genome (can be the same alignment or a normal fasta sequence).\n\n```bash\npython get_mutation_profile.py -f alignment_Figure1B.fasta -m positions_of_interest_ID_POS_REF_ALT.txt -r \'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome\' -b 10 -a 10 -o OPTION2\n```\n\n_Outputs:_    \n1. TSV file with the mutation context and profile for each sample present in the TSV input\n<p align="center">\n\t<img width="849" alt="Captura de ecrã 2022-06-17, às 15 21 20" src="https://user-images.githubusercontent.com/19263468/174317025-e090f7f8-17a4-4001-863f-cd965dfff9a6.png">\n</p>\n\n2. TSV file with a summary report for each position of interest including the different patterns observed and their respective frequency\n<p align="center">\n\t<img width="1145" alt="Captura de ecrã 2022-06-17, às 15 23 07" src="https://user-images.githubusercontent.com/19263468/174317375-d17183e8-0f9c-46a6-ab83-9f1e212c4854.png">\n</p>\n\n### Option 3\nProviding a single-column file with a list of 1-indexed reference positions of interest and a fasta Multiple Sequence Alignment including the reference genome.\n\n```bash\npython get_mutation_profile.py -f alignment_Figure1B.fasta -m Monkeypox_positions_of_interest.tsv -r \'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome\' -b 10 -a 10 -o OPTION3\n```\n\n_Outputs:_     \n1. TSV file with the mutation context and profile for each sample present in the alignment\n<p align="center">\n\t<img width="1106" alt="Captura de ecrã 2022-06-17, às 15 31 56" src="https://user-images.githubusercontent.com/19263468/174319330-2702cf97-af7d-44e9-b7ca-2bf2f0f612ed.png">\n</p>\n\n2. TSV file with a summary report for each position of interest including the different patterns observed and their respective frequency\n<p align="center">\n<img width="1359" alt="Captura de ecrã 2022-06-17, às 15 33 18" src="https://user-images.githubusercontent.com/19263468/174319340-d95fd034-a740-48f1-8cd5-53ea77e785e8.png">\t\n</p>\n\n_TIP: If you do not know your positions of interest, you can run the script _alignment_processing.py_ of [ReporTree](https://github.com/insapathogenomics/ReporTree) and it will provide a list of positions of interest according to your specifications. Example:_\n\n```bash\npython ReporTree/scripts/alignment_processing.py -align alignment_Figure1B.fasta -o Monkeypox --use-reference-coords -r \'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome\' --keep-gaps --get-positions-interest\n```\n\n## Citation\n\nIf you use this tool please cite the article where it was first described:\n\nIsidro, J., Borges, V., Pinto, M. et al. (2022) Phylogenomic characterization and signs of microevolution in the 2022 multi-country outbreak of monkeypox virus. _Nature Medicine_. https://doi.org/10.1038/s41591-022-01907-y\n',
+    'long_description': '# Mutation profile\n\nThis repository comprises the script(s) developed during Monkeypox 2022 outbreak to explore the mutational profiles/signatures of this virus, but that can be of broad application to other species. Currently, it comprises the script(s):\n- _get_mutation_profile.py_ that can be used to rapidly obtain the sequence context (size defined by the user) flanking SNPs of interest and determine their mutational profile according to the user\'s specifications (e.g. APOBEC3-mediated viral genome editing GA>AA and TC>TT replacements)\n\n## Input/Output of _get_mutation_profile.py_\n\t\t\t\t\t\t\t\t\t\n**OPTION1**   \n_Inputs:_    \n1. TSV file with the columns POS REF ALT (i.e. 1-indexed reference position, reference allele and alternative allele)\n2. Fasta file including the reference genome\n\n_Output:_    \n1. TSV file with the mutation context and profile\n\n**OPTION 2**     \n_Inputs:_   \n1. TSV file with the columns ID POS REF ALT (i.e. sample ID, 1-indexed reference position, reference allele and alternative allele)\n2. Fasta file including the reference genome\n\n_Outputs:_    \n1. TSV file with the mutation context and profile for each sample present in the TSV input\n2. TSV file with a summary report for each position of interest including the different patterns observed and their respective frequency\n\n_NOTE: For options 1 and 2 the order of the columns in the input 1 is not important but their name is (ID, POS, REF, ALT)!!_\n\n**OPTION 3**  \n_Inputs:_    \n1. Single-column file with a list of 1-indexed reference positions of interest   \n2. Multiple Sequence Alignment (fasta) including the reference genome    \n\t\t\t\t\t\t\t\t\t\n_Outputs:_     \n1. TSV file with the mutation context and profile for each sample present in the alignment\n2. TSV file with a summary report for each position of interest including the different patterns observed and their respective frequency\n\n_TIP: If you do not know your positions of interest, you can run the script _alignment_processing.py_ of [ReporTree](https://github.com/insapathogenomics/ReporTree) and it will provide a list of positions of interest according to your specifications._\n\n\n## Dependencies and installation\nTo run the _get_mutation_profile.py_ you will need:\n- biopython\n- pandas\n\n### pip installation\n```bash\npip install mutation-profile\nmutation-profile -h\n```\n\n### conda installation\n```bash\nconda create -n mutation-profile -c vmixao mutation-profile\nconda activate mutation-profile # if you created the conda environment\nmutation-profile -h\n```\n\n## Usage\n\n```bash\n  -h, --help            show this help message and exit\n\nMutation profile:\n  Provide input/output specifications\n\n  -f FASTA, --fasta FASTA\n                        [MANDATORY] Input sequence file (fasta)\n  -m MUTATION, --mutation_list MUTATION\n                        [MANDATORY] Input mutation list that can be: 1)\n                        single-column file with 1-based reference position\n                        information (in this case the fasta file must be a\n                        multiple sequence alignment of all the sequences of\n                        interest); OR 2) tsv file with the columns POS, REF,\n                        and ALT where POS = 1-based reference position. If you\n                        want to include information for more than one sample\n                        per position, add also the column \'ID\' (note that the\n                        order of the columns is not important but their name\n                        is!)\n  -r REF, --reference REF\n                        [MANDATORY] Reference sequence name\n  -b BEFORE, --before BEFORE\n                        [OPTIONAL] Number of nucleotides to report BEFORE the\n                        mutation (default = 5)\n  -a AFTER, --after AFTER\n                        [OPTIONAL] Number of nucleotides to report AFTER the\n                        mutation (default = 5)\n  -p PROFILES, --profiles PROFILES\n                        [OPTIONAL] Comma-separated list of mutational profiles\n                        of interest (upper-case!). Default = \'GA>AA,TC>TT\'\n  -o OUTPUT, --output OUTPUT\n                        [OPTIONAL] Tag for output file name. Default =\n                        Mutation_profile\n```\n\n## Examples using Monkeypox 2022 outbreak data available at [_examples/_](https://github.com/insapathogenomics/mutation_profile/tree/main/examples)\n\n### Option 1 (this option reflects part of the analysis performed in the publication)\nProviding a TSV file with the columns POS REF ALT (i.e. 1-indexed reference position, reference allele and alternative allele) and a fasta file including the reference genome (can be the same alignment or a normal fasta sequence).\n\n```bash\nmutation-profile -f alignment_Figure1B.fasta -m positions_of_interest_POS_REF_ALT.txt -r \'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome\' -b 10 -a 10 -o OPTION1\n```\n\n_Output:_    \n1. TSV file with the mutation context and profile\n<p align="center">\n\t<img width="636" alt="Captura de ecrã 2022-06-17, às 15 17 41" src="https://user-images.githubusercontent.com/19263468/174316512-056bb280-a89e-4d81-9ba3-6065f6a9a0f1.png">\n</p>\n\n### Option 2\nProviding a TSV file with the columns ID POS REF ALT (i.e. samples id, 1-indexed reference position, reference allele and alternative allele) and a fasta file including the reference genome (can be the same alignment or a normal fasta sequence).\n\n```bash\nmutation-profile -f alignment_Figure1B.fasta -m positions_of_interest_ID_POS_REF_ALT.txt -r \'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome\' -b 10 -a 10 -o OPTION2\n```\n\n_Outputs:_    \n1. TSV file with the mutation context and profile for each sample present in the TSV input\n<p align="center">\n\t<img width="849" alt="Captura de ecrã 2022-06-17, às 15 21 20" src="https://user-images.githubusercontent.com/19263468/174317025-e090f7f8-17a4-4001-863f-cd965dfff9a6.png">\n</p>\n\n2. TSV file with a summary report for each position of interest including the different patterns observed and their respective frequency\n<p align="center">\n\t<img width="1145" alt="Captura de ecrã 2022-06-17, às 15 23 07" src="https://user-images.githubusercontent.com/19263468/174317375-d17183e8-0f9c-46a6-ab83-9f1e212c4854.png">\n</p>\n\n### Option 3\nProviding a single-column file with a list of 1-indexed reference positions of interest and a fasta Multiple Sequence Alignment including the reference genome.\n\n```bash\nmutation-profile -f alignment_Figure1B.fasta -m Monkeypox_positions_of_interest.tsv -r \'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome\' -b 10 -a 10 -o OPTION3\n```\n\n_Outputs:_     \n1. TSV file with the mutation context and profile for each sample present in the alignment\n<p align="center">\n\t<img width="1106" alt="Captura de ecrã 2022-06-17, às 15 31 56" src="https://user-images.githubusercontent.com/19263468/174319330-2702cf97-af7d-44e9-b7ca-2bf2f0f612ed.png">\n</p>\n\n2. TSV file with a summary report for each position of interest including the different patterns observed and their respective frequency\n<p align="center">\n<img width="1359" alt="Captura de ecrã 2022-06-17, às 15 33 18" src="https://user-images.githubusercontent.com/19263468/174319340-d95fd034-a740-48f1-8cd5-53ea77e785e8.png">\t\n</p>\n\n_TIP: If you do not know your positions of interest, you can run the script _alignment_processing.py_ of [ReporTree](https://github.com/insapathogenomics/ReporTree) and it will provide a list of positions of interest according to your specifications. Example:_\n\n```bash\npython ReporTree/scripts/alignment_processing.py -align alignment_Figure1B.fasta -o Monkeypox --use-reference-coords -r \'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome\' --keep-gaps --get-positions-interest\n```\n\n## Citation\n\nIf you use this script please cite the article where it was first described:\n\nIsidro, J., Borges, V., Pinto, M. et al. Phylogenomic characterization and signs of microevolution in the 2022 multi-country outbreak of monkeypox virus.  \n_Nature Medicine_ (2022). https://doi.org/10.1038/s41591-022-01907-y\n',
     'author': 'Veronica Mixao',
     'author_email': 'vmixao@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/insapathogenomics/mutation_profile',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mutation-profile-0.1.0/PKG-INFO` & `mutation-profile-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: mutation-profile
-Version: 0.1.0
+Version: 0.2.0
 Summary: A bioinformatics solution to determine SNP flanking sequences and mutation profile
 Home-page: https://github.com/insapathogenomics/mutation_profile
 License: GPL-3.0-only
 Author: Veronica Mixao
 Author-email: vmixao@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: biopython (>=1.70,<2.0)
+Requires-Dist: biopython (>=1.80,<2.0)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: textwrap3 (>=0.9.2,<0.10.0)
 Project-URL: Repository, https://github.com/insapathogenomics/mutation_profile
 Description-Content-Type: text/markdown
 
 # Mutation profile
 
-This tool was developed during Monkeypox 2022 outbreak to explore the mutational profiles/signatures of this virus, but can be of broad application to other species. It can be used to rapidly obtain the sequence context (size defined by the user) flanking SNPs of interest and determine their mutational profile according to the user's specifications (e.g. APOBEC3-mediated viral genome editing GA>AA and TC>TT replacements)
+This repository comprises the script(s) developed during Monkeypox 2022 outbreak to explore the mutational profiles/signatures of this virus, but that can be of broad application to other species. Currently, it comprises the script(s):
+- _get_mutation_profile.py_ that can be used to rapidly obtain the sequence context (size defined by the user) flanking SNPs of interest and determine their mutational profile according to the user's specifications (e.g. APOBEC3-mediated viral genome editing GA>AA and TC>TT replacements)
 
 ## Input/Output of _get_mutation_profile.py_
 									
 **OPTION1**   
 _Inputs:_    
 1. TSV file with the columns POS REF ALT (i.e. 1-indexed reference position, reference allele and alternative allele)
 2. Fasta file including the reference genome
@@ -56,15 +58,25 @@
 
 
 ## Dependencies and installation
 To run the _get_mutation_profile.py_ you will need:
 - biopython
 - pandas
 
+### pip installation
+```bash
+pip install mutation-profile
+mutation-profile -h
+```
 
+### conda installation
+```bash
+conda create -n mutation-profile -c vmixao mutation-profile
+conda activate mutation-profile # if you created the conda environment
+mutation-profile -h
 ```
 
 ## Usage
 
 ```bash
   -h, --help            show this help message and exit
 
@@ -102,28 +114,28 @@
 
 ## Examples using Monkeypox 2022 outbreak data available at [_examples/_](https://github.com/insapathogenomics/mutation_profile/tree/main/examples)
 
 ### Option 1 (this option reflects part of the analysis performed in the publication)
 Providing a TSV file with the columns POS REF ALT (i.e. 1-indexed reference position, reference allele and alternative allele) and a fasta file including the reference genome (can be the same alignment or a normal fasta sequence).
 
 ```bash
-python get_mutation_profile.py -f alignment_Figure1B.fasta -m positions_of_interest_POS_REF_ALT.txt -r 'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome' -b 10 -a 10 -o OPTION1
+mutation-profile -f alignment_Figure1B.fasta -m positions_of_interest_POS_REF_ALT.txt -r 'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome' -b 10 -a 10 -o OPTION1
 ```
 
 _Output:_    
 1. TSV file with the mutation context and profile
 <p align="center">
 	<img width="636" alt="Captura de ecrã 2022-06-17, às 15 17 41" src="https://user-images.githubusercontent.com/19263468/174316512-056bb280-a89e-4d81-9ba3-6065f6a9a0f1.png">
 </p>
 
 ### Option 2
 Providing a TSV file with the columns ID POS REF ALT (i.e. samples id, 1-indexed reference position, reference allele and alternative allele) and a fasta file including the reference genome (can be the same alignment or a normal fasta sequence).
 
 ```bash
-python get_mutation_profile.py -f alignment_Figure1B.fasta -m positions_of_interest_ID_POS_REF_ALT.txt -r 'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome' -b 10 -a 10 -o OPTION2
+mutation-profile -f alignment_Figure1B.fasta -m positions_of_interest_ID_POS_REF_ALT.txt -r 'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome' -b 10 -a 10 -o OPTION2
 ```
 
 _Outputs:_    
 1. TSV file with the mutation context and profile for each sample present in the TSV input
 <p align="center">
 	<img width="849" alt="Captura de ecrã 2022-06-17, às 15 21 20" src="https://user-images.githubusercontent.com/19263468/174317025-e090f7f8-17a4-4001-863f-cd965dfff9a6.png">
 </p>
@@ -133,15 +145,15 @@
 	<img width="1145" alt="Captura de ecrã 2022-06-17, às 15 23 07" src="https://user-images.githubusercontent.com/19263468/174317375-d17183e8-0f9c-46a6-ab83-9f1e212c4854.png">
 </p>
 
 ### Option 3
 Providing a single-column file with a list of 1-indexed reference positions of interest and a fasta Multiple Sequence Alignment including the reference genome.
 
 ```bash
-python get_mutation_profile.py -f alignment_Figure1B.fasta -m Monkeypox_positions_of_interest.tsv -r 'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome' -b 10 -a 10 -o OPTION3
+mutation-profile -f alignment_Figure1B.fasta -m Monkeypox_positions_of_interest.tsv -r 'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome' -b 10 -a 10 -o OPTION3
 ```
 
 _Outputs:_     
 1. TSV file with the mutation context and profile for each sample present in the alignment
 <p align="center">
 	<img width="1106" alt="Captura de ecrã 2022-06-17, às 15 31 56" src="https://user-images.githubusercontent.com/19263468/174319330-2702cf97-af7d-44e9-b7ca-2bf2f0f612ed.png">
 </p>
@@ -155,11 +167,12 @@
 
 ```bash
 python ReporTree/scripts/alignment_processing.py -align alignment_Figure1B.fasta -o Monkeypox --use-reference-coords -r 'MT903344.1_Monkeypox_virus_isolate_MPXVUK_P2_complete_genome' --keep-gaps --get-positions-interest
 ```
 
 ## Citation
 
-If you use this tool please cite the article where it was first described:
+If you use this script please cite the article where it was first described:
 
-Isidro, J., Borges, V., Pinto, M. et al. (2022) Phylogenomic characterization and signs of microevolution in the 2022 multi-country outbreak of monkeypox virus. _Nature Medicine_. https://doi.org/10.1038/s41591-022-01907-y
+Isidro, J., Borges, V., Pinto, M. et al. Phylogenomic characterization and signs of microevolution in the 2022 multi-country outbreak of monkeypox virus.  
+_Nature Medicine_ (2022). https://doi.org/10.1038/s41591-022-01907-y
```

