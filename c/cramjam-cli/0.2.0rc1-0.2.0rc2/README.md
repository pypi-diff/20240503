# Comparing `tmp/cramjam_cli-0.2.0rc1.tar.gz` & `tmp/cramjam_cli-0.2.0rc2.tar.gz`

## Comparing `cramjam_cli-0.2.0rc1.tar` & `cramjam_cli-0.2.0rc2.tar`

### file list

```diff
@@ -1,25 +1,11 @@
--rw-r--r--   0     1001      127     2093 2024-04-28 19:18:27.000000 cramjam_cli-0.2.0rc1/libcramjam/Cargo.toml
--rw-r--r--   0     1001      127     1070 2024-04-28 19:18:27.000000 cramjam_cli-0.2.0rc1/libcramjam/LICENSE
--rw-r--r--   0     1001      127      402 2024-04-28 19:18:27.000000 cramjam_cli-0.2.0rc1/libcramjam/README.md
--rw-r--r--   0     1001      127       78 2024-04-28 19:18:27.000000 cramjam_cli-0.2.0rc1/libcramjam/cbindgen.toml
--rw-r--r--   0     1001      127     2179 2024-04-28 19:18:27.000000 cramjam_cli-0.2.0rc1/libcramjam/src/blosc2.rs
--rw-r--r--   0     1001      127     1315 2024-04-28 19:18:27.000000 cramjam_cli-0.2.0rc1/libcramjam/src/brotli.rs
--rw-r--r--   0     1001      127      846 2024-04-28 19:18:27.000000 cramjam_cli-0.2.0rc1/libcramjam/src/bzip2.rs
--rw-r--r--   0     1001      127    37607 2024-04-28 19:18:27.000000 cramjam_cli-0.2.0rc1/libcramjam/src/capi.rs
--rw-r--r--   0     1001      127     1178 2024-04-28 19:18:27.000000 cramjam_cli-0.2.0rc1/libcramjam/src/deflate.rs
--rw-r--r--   0     1001      127     1848 2024-04-28 19:18:27.000000 cramjam_cli-0.2.0rc1/libcramjam/src/gzip.rs
--rw-r--r--   0     1001      127     4839 2024-04-28 19:18:27.000000 cramjam_cli-0.2.0rc1/libcramjam/src/lib.rs
--rw-r--r--   0     1001      127     7205 2024-04-28 19:18:27.000000 cramjam_cli-0.2.0rc1/libcramjam/src/lz4.rs
--rw-r--r--   0     1001      127     1690 2024-04-28 19:18:27.000000 cramjam_cli-0.2.0rc1/libcramjam/src/snappy.rs
--rw-r--r--   0     1001      127     3339 2024-04-28 19:18:27.000000 cramjam_cli-0.2.0rc1/libcramjam/src/xz.rs
--rw-r--r--   0     1001      127      978 2024-04-28 19:18:27.000000 cramjam_cli-0.2.0rc1/libcramjam/src/zstd.rs
--rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 cramjam_cli-0.2.0rc1/cramjam-cli/Cargo.toml
--rw-r--r--   0     1001      127     1070 2024-04-28 19:18:27.000000 cramjam_cli-0.2.0rc1/cramjam-cli/LICENSE
--rw-r--r--   0     1001      127     1136 2024-04-28 19:18:27.000000 cramjam_cli-0.2.0rc1/cramjam-cli/README.md
--rw-r--r--   0     1001      127     7460 2024-04-28 19:18:27.000000 cramjam_cli-0.2.0rc1/cramjam-cli/src/main.rs
--rw-r--r--   0     1001      127     2577 2024-04-28 19:18:27.000000 cramjam_cli-0.2.0rc1/cramjam-cli/tests/test_cli.py
--rw-r--r--   0     1001      127    32314 2024-04-28 19:18:31.000000 cramjam_cli-0.2.0rc1/Cargo.lock
--rw-r--r--   0        0        0      234 1970-01-01 00:00:00.000000 cramjam_cli-0.2.0rc1/Cargo.toml
--rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 cramjam_cli-0.2.0rc1/pyproject.toml
--rw-r--r--   0     1001      127     1070 2024-04-28 19:18:27.000000 cramjam_cli-0.2.0rc1/LICENSE
--rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 cramjam_cli-0.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 cramjam_cli-0.2.0rc2/Cargo.toml
+-rw-r--r--   0     1001      127      440 2024-05-03 06:10:20.000000 cramjam_cli-0.2.0rc2/.cargo/config
+-rw-r--r--   0     1001      127    14520 2024-05-03 06:10:20.000000 cramjam_cli-0.2.0rc2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127     1876 2024-05-03 06:10:20.000000 cramjam_cli-0.2.0rc2/.gitignore
+-rw-r--r--   0     1001      127    22980 2024-05-03 06:10:27.000000 cramjam_cli-0.2.0rc2/Cargo.lock
+-rw-r--r--   0     1001      127     1070 2024-05-03 06:10:20.000000 cramjam_cli-0.2.0rc2/LICENSE
+-rw-r--r--   0     1001      127     1136 2024-05-03 06:10:20.000000 cramjam_cli-0.2.0rc2/README.md
+-rw-r--r--   0     1001      127     7460 2024-05-03 06:10:20.000000 cramjam_cli-0.2.0rc2/src/main.rs
+-rw-r--r--   0     1001      127     2577 2024-05-03 06:10:20.000000 cramjam_cli-0.2.0rc2/tests/test_cli.py
+-rw-r--r--   0     1001      127      612 2024-05-03 06:10:20.000000 cramjam_cli-0.2.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 cramjam_cli-0.2.0rc2/PKG-INFO
```

### Comparing `cramjam_cli-0.2.0rc1/libcramjam/LICENSE` & `cramjam_cli-0.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `cramjam_cli-0.2.0rc1/cramjam-cli/Cargo.toml` & `cramjam_cli-0.2.0rc2/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 [package]
 name = "cramjam-cli"
-version = "0.2.0-rc1"
+version = "0.2.0-rc2"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [features]
-default = ["blosc2-shared", "blosc2-static"]
-extension-module = []  # only here for uniformity w/ cramjam-python's feat set
+default = ["blosc2-static"]
 use-system-blosc2 = ["libcramjam/use-system-blosc2"]
 blosc2-static = ["libcramjam/blosc2-static"]
 blosc2-shared = ["libcramjam/blosc2-shared"]
 
 [dependencies]
 clap = { version = "^4.2", features = ["derive"] }
 bytesize = "^1"
-libcramjam = { path = "../libcramjam" }
-# libcramjam = "0.3.0"
+libcramjam = { version = "0.4.2" }
+
+[profile.release]
+strip = true
+lto = "fat"
+codegen-units = 1
+opt-level = 3
```

### Comparing `cramjam_cli-0.2.0rc1/cramjam-cli/README.md` & `cramjam_cli-0.2.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `cramjam_cli-0.2.0rc1/cramjam-cli/src/main.rs` & `cramjam_cli-0.2.0rc2/src/main.rs`

 * *Files identical despite different names*

### Comparing `cramjam_cli-0.2.0rc1/cramjam-cli/tests/test_cli.py` & `cramjam_cli-0.2.0rc2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cramjam_cli-0.2.0rc1/Cargo.lock` & `cramjam_cli-0.2.0rc2/Cargo.lock`

 * *Files 16% similar despite different names*

```diff
@@ -5,23 +5,14 @@
 [[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
-name = "aho-corasick"
-version = "1.1.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
-dependencies = [
- "memchr",
-]
-
-[[package]]
 name = "alloc-no-stdlib"
 version = "2.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cc7bb162ec39d46ab1ca8c77bf72e890535becd1751bb45f64c597edb4c8c6b3"
 
 [[package]]
 name = "alloc-stdlib"
@@ -30,75 +21,62 @@
 checksum = "94fb8275041c72129eb51b7d0322c29b8387a0386127718b096429201a5d6ece"
 dependencies = [
  "alloc-no-stdlib",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.6.13"
+version = "0.6.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d96bd03f33fe50a863e394ee9718a706f988b9079b20c3784fb726e7678b62fb"
+checksum = "418c75fa768af9c03be99d17643f93f79bbba589895012a80e3452a19ddda15b"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
+ "is_terminal_polyfill",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "1.0.6"
+version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
+checksum = "038dfcf04a5feb68e9c60b21c9625a54c2c0616e79b72b0fd87075a056ae1d1b"
 
 [[package]]
 name = "anstyle-parse"
-version = "0.2.3"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c75ac65da39e5fe5ab759307499ddad880d724eed2f6ce5b5e8a26f4f387928c"
+checksum = "c03a11a9034d92058ceb6ee011ce58af4a9bf61491aa7e1e59ecd24bd40d22d4"
 dependencies = [
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle-query"
-version = "1.0.2"
+version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e28923312444cdd728e4738b3f9c9cac739500909bb3d3c94b43551b16517648"
+checksum = "a64c907d4e79225ac72e2a354c9ce84d50ebb4586dee56c82b3ee73004f537f5"
 dependencies = [
  "windows-sys",
 ]
 
 [[package]]
 name = "anstyle-wincon"
-version = "3.0.2"
+version = "3.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1cd54b81ec8d6180e24654d0b371ad22fc3dd083b6ff8ba325b72e00c87660a7"
+checksum = "61a38449feb7068f52bb06c12759005cf459ee52bb4adc1d5a7c4322d716fb19"
 dependencies = [
  "anstyle",
  "windows-sys",
 ]
 
 [[package]]
-name = "assert_cmd"
-version = "1.0.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c98233c6673d8601ab23e77eb38f999c51100d46c5703b17288c57fddf3a1ffe"
-dependencies = [
- "bstr",
- "doc-comment",
- "predicates",
- "predicates-core",
- "predicates-tree",
- "wait-timeout",
-]
-
-[[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
 dependencies = [
  "hermit-abi",
  "libc",
@@ -121,29 +99,30 @@
 name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "blosc2-rs"
-version = "0.2.3+2.14.3"
+version = "0.2.5+2.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "51c3b2c50799095857cd6658e73403d5e2866f1c532211a2685b10b8229d7c75"
+checksum = "db3d12fe9a38e86a197a2cc14e366d9bcd6628f85ce5d23cda26600b06c156f9"
 dependencies = [
  "blosc2-sys",
  "parking_lot",
 ]
 
 [[package]]
 name = "blosc2-sys"
-version = "0.2.3+2.14.3"
+version = "0.2.5+2.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24b1bc7d65cbf139d694e2f899ae00fa6006d6e8ffcec7954fa5c5e2bba1be85"
+checksum = "2f1478a09e564ac5661d2ea7413786ff4a95eb1aec01659e25e7b955f3f8bd8d"
 dependencies = [
  "cmake",
+ "copy_dir",
  "libc",
  "pkg-config",
 ]
 
 [[package]]
 name = "brotli"
 version = "3.5.0"
@@ -162,25 +141,14 @@
 checksum = "4e2e4afe60d7dd600fdd3de8d0f08c2b7ec039712e3b6137ff98b7004e82de4f"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
 ]
 
 [[package]]
-name = "bstr"
-version = "0.2.17"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba3569f383e8f1598449f1a423e72e99569137b47740b1da11ef19af3d5c3223"
-dependencies = [
- "lazy_static",
- "memchr",
- "regex-automata 0.1.10",
-]
-
-[[package]]
 name = "bytesize"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3e368af43e418a04d52505cf3dbc23dda4e3407ae2fa99fd0e4f308ce546acc"
 
 [[package]]
 name = "bzip2"
@@ -220,17 +188,17 @@
  "syn 1.0.109",
  "tempfile",
  "toml",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.95"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
+checksum = "065a29261d53ba54260972629f9ca6bffa69bac13cd1fed61420f7fa68b9f8bd"
 dependencies = [
  "jobserver",
  "libc",
  "once_cell",
 ]
 
 [[package]]
@@ -310,64 +278,46 @@
 checksum = "a31c789563b815f77f4250caee12365734369f942439b7defd71e18a48197130"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "colorchoice"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+checksum = "0b6a852b24ab71dffc585bcb46eaf7959d175cb865a7152e35b348d1b2960422"
 
 [[package]]
-name = "cramjam-cli"
-version = "0.2.0-rc1"
+name = "copy_dir"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "543d1dd138ef086e2ff05e3a48cf9da045da2033d16f8538fd76b86cd49b2ca3"
 dependencies = [
- "bytesize",
- "clap 4.5.4",
- "libcramjam 0.4.0",
+ "walkdir",
 ]
 
 [[package]]
-name = "cramjam-python"
-version = "2.8.4-rc1"
+name = "cramjam-cli"
+version = "0.2.0-rc2"
 dependencies = [
- "libcramjam 0.4.0 (registry+https://github.com/rust-lang/crates.io-index)",
- "pyo3",
- "pyo3-build-config",
+ "bytesize",
+ "clap 4.5.4",
+ "libcramjam",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
-name = "difflib"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6184e33543162437515c2e2b48714794e37845ec9851711914eec9d308f6ebe8"
-
-[[package]]
-name = "doc-comment"
-version = "0.3.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fea41bba32d969b513997752735605054bc0dfa92b4c56bf1189f2e174be7a10"
-
-[[package]]
-name = "either"
-version = "1.11.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
-
-[[package]]
 name = "errno"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
 dependencies = [
  "libc",
  "windows-sys",
@@ -377,32 +327,23 @@
 name = "fastrand"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "flate2"
-version = "1.0.29"
+version = "1.0.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4556222738635b7a3417ae6130d8f52201e45a0c4d1a907f0826383adb5f85e7"
+checksum = "5f54427cfd1c7829e2a139fcefea601bf088ebca651d2bf53ebc600eac295dae"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
-name = "float-cmp"
-version = "0.9.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98de4bbd547a563b716d8dfa9aad1cb19bfab00f4fa09a6a4ed21dbcf44ce9c4"
-dependencies = [
- "num-traits",
-]
-
-[[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
 name = "heck"
@@ -432,55 +373,18 @@
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown",
 ]
 
 [[package]]
-name = "indoc"
-version = "2.0.5"
+name = "is_terminal_polyfill"
+version = "1.70.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
-
-[[package]]
-name = "inline-c"
-version = "0.1.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "340dd3d6102fa919bd20987024a6d84954c36ec691ac1efea37742ee983c8dd5"
-dependencies = [
- "assert_cmd",
- "cc",
- "inline-c-macro",
- "lazy_static",
- "predicates",
- "regex",
- "rustc_version",
- "target-lexicon 0.11.2",
- "tempfile",
-]
-
-[[package]]
-name = "inline-c-macro"
-version = "0.1.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17f5621ec7adacda881d7c2826c064f5c29c72fd44333f97df61b458a583ae15"
-dependencies = [
- "proc-macro2",
- "quote",
- "rustc_version",
-]
-
-[[package]]
-name = "itertools"
-version = "0.10.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
-dependencies = [
- "either",
-]
+checksum = "f8478577c03552c21db0e2724ffb8986a5ce7af88107e6be5d2ee6e158c12800"
 
 [[package]]
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
@@ -490,49 +394,24 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2b099aaa34a9751c5bf0878add70444e1ed2dd73f347be99003d4577277de6e"
 dependencies = [
  "libc",
 ]
 
 [[package]]
-name = "lazy_static"
-version = "1.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
-
-[[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "libcramjam"
-version = "0.4.0"
-dependencies = [
- "blosc2-rs",
- "brotli",
- "bzip2",
- "cbindgen",
- "flate2",
- "inline-c",
- "libc",
- "libdeflate-sys",
- "libdeflater",
- "lz4",
- "snap",
- "xz2",
- "zstd",
-]
-
-[[package]]
-name = "libcramjam"
-version = "0.4.0"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e14e4746c6e085387deaf03f50c15a44b7dcb77db5e371c3eaf54915fa3cdba1"
+checksum = "9ed734a70d1b4f6bd49ab6755f7eba542369bd8d5a2963ab835572ecd1bae48a"
 dependencies = [
  "blosc2-rs",
  "brotli",
  "bzip2",
  "cbindgen",
  "flate2",
  "libdeflate-sys",
@@ -611,53 +490,23 @@
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
 ]
 
 [[package]]
-name = "memchr"
-version = "2.7.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
-
-[[package]]
-name = "memoffset"
-version = "0.9.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
 name = "miniz_oxide"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
-name = "normalize-line-endings"
-version = "0.3.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61807f77802ff30975e01f4f071c8ba10c022052f98b3294119f3e615d13e5be"
-
-[[package]]
-name = "num-traits"
-version = "0.2.18"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "os_str_bytes"
@@ -685,149 +534,29 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
-name = "pest"
-version = "2.7.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "311fb059dee1a7b802f036316d790138c613a4e8b180c822e3925a662e9f0c95"
-dependencies = [
- "memchr",
- "thiserror",
- "ucd-trie",
-]
-
-[[package]]
 name = "pkg-config"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
 [[package]]
-name = "portable-atomic"
-version = "1.6.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
-
-[[package]]
-name = "predicates"
-version = "2.1.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "59230a63c37f3e18569bdb90e4a89cbf5bf8b06fea0b84e65ea10cc4df47addd"
-dependencies = [
- "difflib",
- "float-cmp",
- "itertools",
- "normalize-line-endings",
- "predicates-core",
- "regex",
-]
-
-[[package]]
-name = "predicates-core"
-version = "1.0.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b794032607612e7abeb4db69adb4e33590fa6cf1149e95fd7cb00e634b92f174"
-
-[[package]]
-name = "predicates-tree"
-version = "1.0.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "368ba315fb8c5052ab692e68a0eefec6ec57b23a36959c14496f0b0df2c0cecf"
-dependencies = [
- "predicates-core",
- "termtree",
-]
-
-[[package]]
 name = "proc-macro2"
 version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
-name = "pyo3"
-version = "0.20.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
-dependencies = [
- "cfg-if",
- "indoc",
- "libc",
- "memoffset",
- "parking_lot",
- "portable-atomic",
- "pyo3-build-config",
- "pyo3-ffi",
- "pyo3-macros",
- "unindent",
-]
-
-[[package]]
-name = "pyo3-build-config"
-version = "0.20.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
-dependencies = [
- "once_cell",
- "python3-dll-a",
- "target-lexicon 0.12.14",
-]
-
-[[package]]
-name = "pyo3-ffi"
-version = "0.20.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
-dependencies = [
- "libc",
- "pyo3-build-config",
-]
-
-[[package]]
-name = "pyo3-macros"
-version = "0.20.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
-dependencies = [
- "proc-macro2",
- "pyo3-macros-backend",
- "quote",
- "syn 2.0.60",
-]
-
-[[package]]
-name = "pyo3-macros-backend"
-version = "0.20.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
-dependencies = [
- "heck 0.4.1",
- "proc-macro2",
- "pyo3-build-config",
- "quote",
- "syn 2.0.60",
-]
-
-[[package]]
-name = "python3-dll-a"
-version = "0.2.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d5f07cd4412be8fa09a721d40007c483981bbe072cd6a21f2e83e04ec8f8343f"
-dependencies = [
- "cc",
-]
-
-[[package]]
 name = "quote"
 version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
@@ -838,58 +567,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags 2.5.0",
 ]
 
 [[package]]
-name = "regex"
-version = "1.10.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
-dependencies = [
- "aho-corasick",
- "memchr",
- "regex-automata 0.4.6",
- "regex-syntax",
-]
-
-[[package]]
-name = "regex-automata"
-version = "0.1.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
-
-[[package]]
-name = "regex-automata"
-version = "0.4.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
-dependencies = [
- "aho-corasick",
- "memchr",
- "regex-syntax",
-]
-
-[[package]]
-name = "regex-syntax"
-version = "0.8.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
-
-[[package]]
-name = "rustc_version"
-version = "0.3.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0dfe2087c51c460008730de8b57e6a320782fbfb312e1f4d520e6c6fae155ee"
-dependencies = [
- "semver",
-]
-
-[[package]]
 name = "rustix"
 version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
  "bitflags 2.5.0",
  "errno",
@@ -901,51 +586,42 @@
 [[package]]
 name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
-name = "scopeguard"
-version = "1.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
-
-[[package]]
-name = "semver"
-version = "0.11.0"
+name = "same-file"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f301af10236f6df4160f7c3f04eec6dbc70ace82d23326abad5edee88801c6b6"
+checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
- "semver-parser",
+ "winapi-util",
 ]
 
 [[package]]
-name = "semver-parser"
-version = "0.10.2"
+name = "scopeguard"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "00b0bef5b7f9e0df16536d3961cfb6e84331c065b4066afb39768d0e319411f7"
-dependencies = [
- "pest",
-]
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.199"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c9f6e76df036c77cd94996771fb40db98187f096dd0b9af39c6c6e452ba966a"
+checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.199"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11bd257a6541e141e42ca6d24ae26f7714887b47e89aa739099104c7e4d3b7fc"
+checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
@@ -1002,26 +678,14 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
-name = "target-lexicon"
-version = "0.11.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "422045212ea98508ae3d28025bc5aaa2bd4a9cdaecd442a08da2ee620ee9ea95"
-
-[[package]]
-name = "target-lexicon"
-version = "0.12.14"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
-
-[[package]]
 name = "tempfile"
 version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
  "cfg-if",
  "fastrand",
@@ -1035,85 +699,48 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06794f8f6c5c898b3275aebefa6b8a1cb24cd2c6c79397ab15774837a0bc5755"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
-name = "termtree"
-version = "0.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3369f5ac52d5eb6ab48c6b4ffdc8efbcad6b89c765749064ba298f2c68a16a76"
-
-[[package]]
 name = "textwrap"
 version = "0.16.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23d434d3f8967a09480fb04132ebe0a3e088c173e6d0ee7897abbdf4eab0f8b9"
 
 [[package]]
-name = "thiserror"
-version = "1.0.59"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
-dependencies = [
- "thiserror-impl",
-]
-
-[[package]]
-name = "thiserror-impl"
-version = "1.0.59"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.60",
-]
-
-[[package]]
 name = "toml"
 version = "0.5.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
 dependencies = [
  "serde",
 ]
 
 [[package]]
-name = "ucd-trie"
-version = "0.1.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed646292ffc8188ef8ea4d1e0e0150fb15a5c2e12ad9b8fc191ae7a8a7f3c4b9"
-
-[[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
-name = "unindent"
-version = "0.2.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
-
-[[package]]
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
-name = "wait-timeout"
-version = "0.2.0"
+name = "walkdir"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f200f5b12eb75f8c1ed65abd4b2db8a6e1b138a20de009dacee265a2498f3f6"
+checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
 dependencies = [
- "libc",
+ "same-file",
+ "winapi-util",
 ]
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
```

### Comparing `cramjam_cli-0.2.0rc1/pyproject.toml` & `cramjam_cli-0.2.0rc2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 [build-system]
 requires = ["maturin>=0.14"]
 build-backend = "maturin"
 
 [tool.maturin]
 bindings = "bin"
 strip = true
-manifest-path = "cramjam-cli/Cargo.toml"
 
 [project.optional-dependencies]
 dev = [
   "pytest>=5.30",
   "pytest-benchmark",
   "cramjam",
   "hypothesis"
```

### Comparing `cramjam_cli-0.2.0rc1/PKG-INFO` & `cramjam_cli-0.2.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cramjam-cli
-Version: 0.2.0rc1
+Version: 0.2.0rc2
 Requires-Dist: pytest >=5.30 ; extra == 'dev'
 Requires-Dist: pytest-benchmark ; extra == 'dev'
 Requires-Dist: cramjam ; extra == 'dev'
 Requires-Dist: hypothesis ; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE
 Keywords: compression,decompression,snappy,zstd,bz2,gzip,lz4,brotli,deflate
```

