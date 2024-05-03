# Comparing `tmp/pye57-0.4.4.tar.gz` & `tmp/pye57-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pye57-0.4.4.tar", last modified: Tue Mar 12 20:59:55 2024, max compression
+gzip compressed data, was "pye57-0.4.5.tar", last modified: Fri May  3 19:30:19 2024, max compression
```

## Comparing `pye57-0.4.4.tar` & `pye57-0.4.5.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.239356 pye57-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-12 20:59:48.000000 pye57-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-12 20:59:48.000000 pye57-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-03-12 20:59:55.239356 pye57-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-03-12 20:59:48.000000 pye57-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.211356 pye57-0.4.4/libE57Format/
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/LICENSE-MIT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.203356 pye57-0.4.4/libE57Format/extern/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.211356 pye57-0.4.4/libE57Format/extern/CRCpp/
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/extern/CRCpp/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/extern/CRCpp/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.211356 pye57-0.4.4/libE57Format/extern/CRCpp/inc/
--rw-r--r--   0 runner    (1001) docker     (127)    84333 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/extern/CRCpp/inc/CRC.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.211356 pye57-0.4.4/libE57Format/include/
--rw-r--r--   0 runner    (1001) docker     (127)    21052 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/include/E57Exception.h
--rw-r--r--   0 runner    (1001) docker     (127)    30276 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/include/E57Format.h
--rw-r--r--   0 runner    (1001) docker     (127)    41131 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/include/E57SimpleData.h
--rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/include/E57SimpleReader.h
--rw-r--r--   0 runner    (1001) docker     (127)     9560 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/include/E57SimpleWriter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/include/E57Version.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.223356 pye57-0.4.4/libE57Format/src/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/ASTMVersion.h
--rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/BlobNode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8836 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/BlobNodeImpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/BlobNodeImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    21315 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/CheckedFile.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/CheckedFile.h
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/Common.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/Common.h
--rw-r--r--   0 runner    (1001) docker     (127)    18737 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/CompressedVectorNode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13435 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/CompressedVectorNodeImpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/CompressedVectorNodeImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    14443 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/CompressedVectorReader.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    23216 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/CompressedVectorReaderImpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/CompressedVectorReaderImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/CompressedVectorWriter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    27619 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/CompressedVectorWriterImpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/CompressedVectorWriterImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/DecodeChannel.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/DecodeChannel.h
--rw-r--r--   0 runner    (1001) docker     (127)    36064 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/Decoder.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/Decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)    17464 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/E57Exception.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/E57SimpleData.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/E57SimpleReader.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11201 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/E57SimpleWriter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/E57Version.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    33274 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/E57XmlParser.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/E57XmlParser.h
--rw-r--r--   0 runner    (1001) docker     (127)    35187 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/Encoder.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/Encoder.h
--rw-r--r--   0 runner    (1001) docker     (127)    12330 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/FloatNode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/FloatNodeImpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/FloatNodeImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    27142 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/ImageFile.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    28271 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/ImageFileImpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/ImageFileImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    10508 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/IntegerNode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/IntegerNodeImpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/IntegerNodeImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    23188 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/Node.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/NodeImpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/NodeImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    26982 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/Packet.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/Packet.h
--rw-r--r--   0 runner    (1001) docker     (127)    69177 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/ReaderImpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/ReaderImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    16399 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/ScaledIntegerNode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/ScaledIntegerNodeImpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/ScaledIntegerNodeImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/SectionHeaders.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/SectionHeaders.h
--rw-r--r--   0 runner    (1001) docker     (127)    20846 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/SourceDestBuffer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    38011 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/SourceDestBufferImpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/SourceDestBufferImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/StringFunctions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/StringFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     8033 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/StringNode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/StringNodeImpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/StringNodeImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    13582 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/StructureNode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/StructureNodeImpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/StructureNodeImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    14519 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/VectorNode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/VectorNodeImpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/VectorNodeImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    53515 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/WriterImpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/src/WriterImpl.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.223356 pye57-0.4.4/libE57Format/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/test/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.207356 pye57-0.4.4/libE57Format/test/extern/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.223356 pye57-0.4.4/libE57Format/test/extern/googletest/
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.223356 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.223356 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.207356 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.227356 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/
--rw-r--r--   0 runner    (1001) docker     (127)    87908 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-actions.h
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-cardinalities.h
--rw-r--r--   0 runner    (1001) docker     (127)    25756 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-function-mocker.h
--rw-r--r--   0 runner    (1001) docker     (127)   210002 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-matchers.h
--rw-r--r--   0 runner    (1001) docker     (127)    38344 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-more-actions.h
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-more-matchers.h
--rw-r--r--   0 runner    (1001) docker     (127)    10840 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-nice-strict.h
--rw-r--r--   0 runner    (1001) docker     (127)    80896 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-spec-builders.h
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.227356 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.227356 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/custom/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/custom/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/custom/gmock-generated-actions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/custom/gmock-matchers.h
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/custom/gmock-port.h
--rw-r--r--   0 runner    (1001) docker     (127)    19264 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/gmock-internal-utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/gmock-port.h
--rw-r--r--   0 runner    (1001) docker     (127)    13491 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/gmock-pp.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.227356 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/test/gmock-matchers_test.h
--rw-r--r--   0 runner    (1001) docker     (127)    19544 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/test/gmock_link_test.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.227356 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/
--rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.227356 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.207356 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.231356 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/
--rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-assertion-result.h
--rw-r--r--   0 runner    (1001) docker     (127)    14886 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-death-test.h
--rw-r--r--   0 runner    (1001) docker     (127)    33614 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-matchers.h
--rw-r--r--   0 runner    (1001) docker     (127)     8146 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-message.h
--rw-r--r--   0 runner    (1001) docker     (127)    24008 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-param-test.h
--rw-r--r--   0 runner    (1001) docker     (127)    39640 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-printers.h
--rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-spi.h
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-test-part.h
--rw-r--r--   0 runner    (1001) docker     (127)    15889 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-typed-test.h
--rw-r--r--   0 runner    (1001) docker     (127)    90771 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest.h
--rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest_pred_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest_prod.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.235356 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.235356 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/custom/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/custom/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/custom/gtest-port.h
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/custom/gtest-printers.h
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/custom/gtest.h
--rw-r--r--   0 runner    (1001) docker     (127)    13910 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-death-test-internal.h
--rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-filepath.h
--rw-r--r--   0 runner    (1001) docker     (127)    63416 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-internal.h
--rw-r--r--   0 runner    (1001) docker     (127)    38068 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-param-util.h
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-port-arch.h
--rw-r--r--   0 runner    (1001) docker     (127)    88791 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-port.h
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-string.h
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-type-util.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.235356 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/samples/
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/samples/prime_tables.h
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/samples/sample1.h
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/samples/sample2.h
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/samples/sample3-inl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/samples/sample4.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.235356 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/src/
--rw-r--r--   0 runner    (1001) docker     (127)    47881 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/src/gtest-internal-inl.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.235356 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/test/googletest-param-test-test.h
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/test/gtest-typed-test_test.h
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-03-12 20:59:52.000000 pye57-0.4.4/libE57Format/test/extern/googletest/googletest/test/production.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.235356 pye57-0.4.4/libE57Format/test/include/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/test/include/Helpers.h
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/test/include/RandomNum.h
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/test/include/TestData.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.235356 pye57-0.4.4/libE57Format/test/src/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/test/src/RandomNum.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/test/src/TestData.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/test/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11774 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/test/src/test_SimpleData.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10132 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/test/src/test_SimpleReader.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    22808 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/test/src/test_SimpleWriter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-03-12 20:59:49.000000 pye57-0.4.4/libE57Format/test/src/test_StringFunctions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-12 20:59:48.000000 pye57-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 20:59:55.239356 pye57-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-03-12 20:59:48.000000 pye57-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.207356 pye57-0.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.239356 pye57-0.4.4/src/pye57/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-12 20:59:48.000000 pye57-0.4.4/src/pye57/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-12 20:59:48.000000 pye57-0.4.4/src/pye57/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18528 2024-03-12 20:59:48.000000 pye57-0.4.4/src/pye57/e57.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-12 20:59:48.000000 pye57-0.4.4/src/pye57/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    34489 2024-03-12 20:59:48.000000 pye57-0.4.4/src/pye57/libe57_wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-03-12 20:59:48.000000 pye57-0.4.4/src/pye57/scan_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-03-12 20:59:48.000000 pye57-0.4.4/src/pye57/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.239356 pye57-0.4.4/src/pye57.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-03-12 20:59:55.000000 pye57-0.4.4/src/pye57.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-03-12 20:59:55.000000 pye57-0.4.4/src/pye57.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 20:59:55.000000 pye57-0.4.4/src/pye57.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 20:59:55.000000 pye57-0.4.4/src/pye57.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-12 20:59:55.000000 pye57-0.4.4/src/pye57.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-12 20:59:55.000000 pye57-0.4.4/src/pye57.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:59:55.239356 pye57-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10922 2024-03-12 20:59:48.000000 pye57-0.4.4/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.858227 pye57-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-03 19:30:12.000000 pye57-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-03 19:30:12.000000 pye57-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-05-03 19:30:19.858227 pye57-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-03 19:30:12.000000 pye57-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.830227 pye57-0.4.5/libE57Format/
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/LICENSE-MIT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.826227 pye57-0.4.5/libE57Format/extern/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.830227 pye57-0.4.5/libE57Format/extern/CRCpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/extern/CRCpp/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/extern/CRCpp/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.830227 pye57-0.4.5/libE57Format/extern/CRCpp/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)    84333 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/extern/CRCpp/inc/CRC.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.834227 pye57-0.4.5/libE57Format/include/
+-rw-r--r--   0 runner    (1001) docker     (127)    21052 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/include/E57Exception.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30276 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/include/E57Format.h
+-rw-r--r--   0 runner    (1001) docker     (127)    41131 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/include/E57SimpleData.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/include/E57SimpleReader.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9560 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/include/E57SimpleWriter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/include/E57Version.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.846227 pye57-0.4.5/libE57Format/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/ASTMVersion.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/BlobNode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8836 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/BlobNodeImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/BlobNodeImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21315 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/CheckedFile.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/CheckedFile.h
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/Common.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/Common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18737 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/CompressedVectorNode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13435 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/CompressedVectorNodeImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/CompressedVectorNodeImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14443 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/CompressedVectorReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23216 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/CompressedVectorReaderImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/CompressedVectorReaderImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/CompressedVectorWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    27619 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/CompressedVectorWriterImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/CompressedVectorWriterImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/DecodeChannel.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/DecodeChannel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    36064 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/Decoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/Decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17464 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/E57Exception.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/E57SimpleData.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/E57SimpleReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11201 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/E57SimpleWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/E57Version.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    33274 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/E57XmlParser.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/E57XmlParser.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35187 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/Encoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/Encoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12330 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/FloatNode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/FloatNodeImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/FloatNodeImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27142 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/ImageFile.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    28271 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/ImageFileImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/ImageFileImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10508 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/IntegerNode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/IntegerNodeImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/IntegerNodeImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23188 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/Node.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/NodeImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/NodeImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26982 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/Packet.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/Packet.h
+-rw-r--r--   0 runner    (1001) docker     (127)    69177 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/ReaderImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/ReaderImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16399 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/ScaledIntegerNode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/ScaledIntegerNodeImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/ScaledIntegerNodeImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/SectionHeaders.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/SectionHeaders.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20846 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/SourceDestBuffer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    38011 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/SourceDestBufferImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/SourceDestBufferImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/StringFunctions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/StringFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8033 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/StringNode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/StringNodeImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/StringNodeImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13582 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/StructureNode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/StructureNodeImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/StructureNodeImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14519 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/VectorNode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/VectorNodeImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/VectorNodeImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    53515 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/WriterImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/src/WriterImpl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.846227 pye57-0.4.5/libE57Format/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/test/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.826227 pye57-0.4.5/libE57Format/test/extern/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.846227 pye57-0.4.5/libE57Format/test/extern/googletest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.846227 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.846227 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.826227 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.846227 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/
+-rw-r--r--   0 runner    (1001) docker     (127)    87908 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-actions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-cardinalities.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25756 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-function-mocker.h
+-rw-r--r--   0 runner    (1001) docker     (127)   210002 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-matchers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38344 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-more-actions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-more-matchers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10840 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-nice-strict.h
+-rw-r--r--   0 runner    (1001) docker     (127)    80896 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-spec-builders.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.846227 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.850227 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/custom/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/custom/gmock-generated-actions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/custom/gmock-matchers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/custom/gmock-port.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19264 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/gmock-internal-utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/gmock-port.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13491 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/gmock-pp.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.850227 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/test/gmock-matchers_test.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19544 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/test/gmock_link_test.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.850227 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/
+-rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.850227 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.826227 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.850227 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/
+-rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-assertion-result.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14886 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-death-test.h
+-rw-r--r--   0 runner    (1001) docker     (127)    33614 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-matchers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8146 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-message.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24008 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-param-test.h
+-rw-r--r--   0 runner    (1001) docker     (127)    39640 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-printers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-spi.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-test-part.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15889 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-typed-test.h
+-rw-r--r--   0 runner    (1001) docker     (127)    90771 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest_pred_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest_prod.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.854227 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.854227 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/custom/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/custom/gtest-port.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/custom/gtest-printers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/custom/gtest.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13910 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-death-test-internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-filepath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    63416 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38068 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-param-util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-port-arch.h
+-rw-r--r--   0 runner    (1001) docker     (127)    88791 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-port.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-string.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-type-util.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.854227 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/samples/prime_tables.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/samples/sample1.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/samples/sample2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/samples/sample3-inl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/samples/sample4.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.854227 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    47881 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/src/gtest-internal-inl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.854227 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/test/googletest-param-test-test.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/test/gtest-typed-test_test.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-03 19:30:14.000000 pye57-0.4.5/libE57Format/test/extern/googletest/googletest/test/production.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.854227 pye57-0.4.5/libE57Format/test/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/test/include/Helpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/test/include/RandomNum.h
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/test/include/TestData.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.858227 pye57-0.4.5/libE57Format/test/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/test/src/RandomNum.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/test/src/TestData.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/test/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11774 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/test/src/test_SimpleData.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10132 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/test/src/test_SimpleReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    22808 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/test/src/test_SimpleWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-03 19:30:13.000000 pye57-0.4.5/libE57Format/test/src/test_StringFunctions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-03 19:30:12.000000 pye57-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:30:19.858227 pye57-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-03 19:30:12.000000 pye57-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.826227 pye57-0.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.858227 pye57-0.4.5/src/pye57/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-03 19:30:12.000000 pye57-0.4.5/src/pye57/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 19:30:12.000000 pye57-0.4.5/src/pye57/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18528 2024-05-03 19:30:12.000000 pye57-0.4.5/src/pye57/e57.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-03 19:30:12.000000 pye57-0.4.5/src/pye57/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34649 2024-05-03 19:30:12.000000 pye57-0.4.5/src/pye57/libe57_wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-05-03 19:30:12.000000 pye57-0.4.5/src/pye57/scan_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-03 19:30:12.000000 pye57-0.4.5/src/pye57/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.858227 pye57-0.4.5/src/pye57.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-05-03 19:30:19.000000 pye57-0.4.5/src/pye57.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-05-03 19:30:19.000000 pye57-0.4.5/src/pye57.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:30:19.000000 pye57-0.4.5/src/pye57.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:30:19.000000 pye57-0.4.5/src/pye57.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 19:30:19.000000 pye57-0.4.5/src/pye57.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 19:30:19.000000 pye57-0.4.5/src/pye57.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:30:19.858227 pye57-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14438 2024-05-03 19:30:12.000000 pye57-0.4.5/tests/test_main.py
```

### Comparing `pye57-0.4.4/LICENSE` & `pye57-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/PKG-INFO` & `pye57-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pye57
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python .e57 files reader/writer
 Home-page: https://www.github.com/davidcaron/pye57
 Author: David Caron
 Author-email: dcaron05@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pye57-0.4.4/README.md` & `pye57-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/LICENSE-MIT.md` & `pye57-0.4.5/libE57Format/LICENSE-MIT.md`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/LICENSE.md` & `pye57-0.4.5/libE57Format/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/README.md` & `pye57-0.4.5/libE57Format/README.md`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/extern/CRCpp/LICENSE` & `pye57-0.4.5/libE57Format/extern/CRCpp/LICENSE`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/extern/CRCpp/README.md` & `pye57-0.4.5/libE57Format/extern/CRCpp/README.md`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/extern/CRCpp/inc/CRC.h` & `pye57-0.4.5/libE57Format/extern/CRCpp/inc/CRC.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/include/E57Exception.h` & `pye57-0.4.5/libE57Format/include/E57Exception.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/include/E57Format.h` & `pye57-0.4.5/libE57Format/include/E57Format.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/include/E57SimpleData.h` & `pye57-0.4.5/libE57Format/include/E57SimpleData.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/include/E57SimpleReader.h` & `pye57-0.4.5/libE57Format/include/E57SimpleReader.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/include/E57SimpleWriter.h` & `pye57-0.4.5/libE57Format/include/E57SimpleWriter.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/include/E57Version.h` & `pye57-0.4.5/libE57Format/include/E57Version.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/ASTMVersion.h` & `pye57-0.4.5/libE57Format/src/ASTMVersion.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/BlobNode.cpp` & `pye57-0.4.5/libE57Format/src/BlobNode.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/BlobNodeImpl.cpp` & `pye57-0.4.5/libE57Format/src/BlobNodeImpl.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/BlobNodeImpl.h` & `pye57-0.4.5/libE57Format/src/BlobNodeImpl.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/CheckedFile.cpp` & `pye57-0.4.5/libE57Format/src/CheckedFile.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/CheckedFile.h` & `pye57-0.4.5/libE57Format/src/CheckedFile.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/Common.cpp` & `pye57-0.4.5/libE57Format/src/Common.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/Common.h` & `pye57-0.4.5/libE57Format/src/Common.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/CompressedVectorNode.cpp` & `pye57-0.4.5/libE57Format/src/CompressedVectorNode.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/CompressedVectorNodeImpl.cpp` & `pye57-0.4.5/libE57Format/src/CompressedVectorNodeImpl.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/CompressedVectorNodeImpl.h` & `pye57-0.4.5/libE57Format/src/CompressedVectorNodeImpl.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/CompressedVectorReader.cpp` & `pye57-0.4.5/libE57Format/src/CompressedVectorReader.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/CompressedVectorReaderImpl.cpp` & `pye57-0.4.5/libE57Format/src/CompressedVectorReaderImpl.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/CompressedVectorReaderImpl.h` & `pye57-0.4.5/libE57Format/src/CompressedVectorReaderImpl.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/CompressedVectorWriter.cpp` & `pye57-0.4.5/libE57Format/src/CompressedVectorWriter.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/CompressedVectorWriterImpl.cpp` & `pye57-0.4.5/libE57Format/src/CompressedVectorWriterImpl.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/CompressedVectorWriterImpl.h` & `pye57-0.4.5/libE57Format/src/CompressedVectorWriterImpl.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/DecodeChannel.cpp` & `pye57-0.4.5/libE57Format/src/DecodeChannel.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/DecodeChannel.h` & `pye57-0.4.5/libE57Format/src/DecodeChannel.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/Decoder.cpp` & `pye57-0.4.5/libE57Format/src/Decoder.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/Decoder.h` & `pye57-0.4.5/libE57Format/src/Decoder.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/E57Exception.cpp` & `pye57-0.4.5/libE57Format/src/E57Exception.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/E57SimpleData.cpp` & `pye57-0.4.5/libE57Format/src/E57SimpleData.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/E57SimpleReader.cpp` & `pye57-0.4.5/libE57Format/src/E57SimpleReader.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/E57SimpleWriter.cpp` & `pye57-0.4.5/libE57Format/src/E57SimpleWriter.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/E57Version.cpp` & `pye57-0.4.5/libE57Format/src/E57Version.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/E57XmlParser.cpp` & `pye57-0.4.5/libE57Format/src/E57XmlParser.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/E57XmlParser.h` & `pye57-0.4.5/libE57Format/src/E57XmlParser.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/Encoder.cpp` & `pye57-0.4.5/libE57Format/src/Encoder.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/Encoder.h` & `pye57-0.4.5/libE57Format/src/Encoder.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/FloatNode.cpp` & `pye57-0.4.5/libE57Format/src/FloatNode.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/FloatNodeImpl.cpp` & `pye57-0.4.5/libE57Format/src/FloatNodeImpl.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/FloatNodeImpl.h` & `pye57-0.4.5/libE57Format/src/FloatNodeImpl.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/ImageFile.cpp` & `pye57-0.4.5/libE57Format/src/ImageFile.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/ImageFileImpl.cpp` & `pye57-0.4.5/libE57Format/src/ImageFileImpl.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/ImageFileImpl.h` & `pye57-0.4.5/libE57Format/src/ImageFileImpl.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/IntegerNode.cpp` & `pye57-0.4.5/libE57Format/src/IntegerNode.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/IntegerNodeImpl.cpp` & `pye57-0.4.5/libE57Format/src/IntegerNodeImpl.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/IntegerNodeImpl.h` & `pye57-0.4.5/libE57Format/src/IntegerNodeImpl.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/Node.cpp` & `pye57-0.4.5/libE57Format/src/Node.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/NodeImpl.cpp` & `pye57-0.4.5/libE57Format/src/NodeImpl.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/NodeImpl.h` & `pye57-0.4.5/libE57Format/src/NodeImpl.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/Packet.cpp` & `pye57-0.4.5/libE57Format/src/Packet.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/Packet.h` & `pye57-0.4.5/libE57Format/src/Packet.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/ReaderImpl.cpp` & `pye57-0.4.5/libE57Format/src/ReaderImpl.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/ReaderImpl.h` & `pye57-0.4.5/libE57Format/src/ReaderImpl.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/ScaledIntegerNode.cpp` & `pye57-0.4.5/libE57Format/src/ScaledIntegerNode.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/ScaledIntegerNodeImpl.cpp` & `pye57-0.4.5/libE57Format/src/ScaledIntegerNodeImpl.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/ScaledIntegerNodeImpl.h` & `pye57-0.4.5/libE57Format/src/ScaledIntegerNodeImpl.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/SectionHeaders.cpp` & `pye57-0.4.5/libE57Format/src/SectionHeaders.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/SectionHeaders.h` & `pye57-0.4.5/libE57Format/src/SectionHeaders.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/SourceDestBuffer.cpp` & `pye57-0.4.5/libE57Format/src/SourceDestBuffer.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/SourceDestBufferImpl.cpp` & `pye57-0.4.5/libE57Format/src/SourceDestBufferImpl.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/SourceDestBufferImpl.h` & `pye57-0.4.5/libE57Format/src/SourceDestBufferImpl.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/StringFunctions.cpp` & `pye57-0.4.5/libE57Format/src/StringFunctions.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/StringFunctions.h` & `pye57-0.4.5/libE57Format/src/StringFunctions.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/StringNode.cpp` & `pye57-0.4.5/libE57Format/src/StringNode.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/StringNodeImpl.cpp` & `pye57-0.4.5/libE57Format/src/StringNodeImpl.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/StringNodeImpl.h` & `pye57-0.4.5/libE57Format/src/StringNodeImpl.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/StructureNode.cpp` & `pye57-0.4.5/libE57Format/src/StructureNode.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/StructureNodeImpl.cpp` & `pye57-0.4.5/libE57Format/src/StructureNodeImpl.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/StructureNodeImpl.h` & `pye57-0.4.5/libE57Format/src/StructureNodeImpl.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/VectorNode.cpp` & `pye57-0.4.5/libE57Format/src/VectorNode.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/VectorNodeImpl.cpp` & `pye57-0.4.5/libE57Format/src/VectorNodeImpl.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/VectorNodeImpl.h` & `pye57-0.4.5/libE57Format/src/VectorNodeImpl.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/WriterImpl.cpp` & `pye57-0.4.5/libE57Format/src/WriterImpl.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/src/WriterImpl.h` & `pye57-0.4.5/libE57Format/src/WriterImpl.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/README.md` & `pye57-0.4.5/libE57Format/test/README.md`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/LICENSE` & `pye57-0.4.5/libE57Format/test/extern/googletest/LICENSE`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/README.md` & `pye57-0.4.5/libE57Format/test/extern/googletest/README.md`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/README.md` & `pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/README.md`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-actions.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-actions.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-cardinalities.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-cardinalities.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-function-mocker.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-function-mocker.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-matchers.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-matchers.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-more-actions.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-more-actions.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-more-matchers.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-more-matchers.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-nice-strict.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-nice-strict.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-spec-builders.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock-spec-builders.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/gmock.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/custom/gmock-matchers.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/custom/gmock-matchers.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/custom/gmock-port.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/custom/gmock-port.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/gmock-internal-utils.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/gmock-internal-utils.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/gmock-port.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/gmock-port.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/gmock-pp.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/include/gmock/internal/gmock-pp.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/test/gmock-matchers_test.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/test/gmock-matchers_test.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googlemock/test/gmock_link_test.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googlemock/test/gmock_link_test.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/README.md` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/README.md`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-assertion-result.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-assertion-result.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-death-test.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-death-test.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-matchers.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-matchers.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-message.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-message.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-param-test.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-param-test.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-printers.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-printers.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-spi.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-spi.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-test-part.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-test-part.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-typed-test.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest-typed-test.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest_pred_impl.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest_pred_impl.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/gtest_prod.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/gtest_prod.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/custom/README.md` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/custom/README.md`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/custom/gtest-port.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/custom/gtest-port.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/custom/gtest-printers.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/custom/gtest-printers.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/custom/gtest.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/custom/gtest.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-death-test-internal.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-death-test-internal.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-filepath.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-filepath.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-internal.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-internal.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-param-util.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-param-util.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-port-arch.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-port-arch.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-port.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-port.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-string.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-string.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-type-util.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/include/gtest/internal/gtest-type-util.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/samples/prime_tables.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/samples/prime_tables.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/samples/sample1.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/samples/sample1.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/samples/sample2.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/samples/sample2.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/samples/sample3-inl.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/samples/sample3-inl.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/samples/sample4.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/samples/sample4.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/src/gtest-internal-inl.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/src/gtest-internal-inl.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/test/googletest-param-test-test.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/test/googletest-param-test-test.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/test/gtest-typed-test_test.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/test/gtest-typed-test_test.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/extern/googletest/googletest/test/production.h` & `pye57-0.4.5/libE57Format/test/extern/googletest/googletest/test/production.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/include/Helpers.h` & `pye57-0.4.5/libE57Format/test/include/Helpers.h`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/src/RandomNum.cpp` & `pye57-0.4.5/libE57Format/test/src/RandomNum.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/src/TestData.cpp` & `pye57-0.4.5/libE57Format/test/src/TestData.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/src/main.cpp` & `pye57-0.4.5/libE57Format/test/src/main.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/src/test_SimpleData.cpp` & `pye57-0.4.5/libE57Format/test/src/test_SimpleData.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/src/test_SimpleReader.cpp` & `pye57-0.4.5/libE57Format/test/src/test_SimpleReader.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/src/test_SimpleWriter.cpp` & `pye57-0.4.5/libE57Format/test/src/test_SimpleWriter.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/libE57Format/test/src/test_StringFunctions.cpp` & `pye57-0.4.5/libE57Format/test/src/test_StringFunctions.cpp`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/pyproject.toml` & `pye57-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/setup.py` & `pye57-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/src/pye57/e57.py` & `pye57-0.4.5/src/pye57/e57.py`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/src/pye57/libe57_wrapper.cpp` & `pye57-0.4.5/src/pye57/libe57_wrapper.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -193,14 +193,17 @@
     }, "pathName"_a, "n"_a);
     cls_StructureNode.def("set", [](StructureNode &node, const std::string &pathName, FloatNode &n){
         node.set(pathName, n);
     }, "pathName"_a, "n"_a);
     cls_StructureNode.def("set", [](StructureNode &node, const std::string &pathName, StringNode &n){
         node.set(pathName, n);
     }, "pathName"_a, "n"_a);
+    cls_StructureNode.def("set", [](StructureNode &node, const std::string &pathName, BlobNode &n){
+        node.set(pathName, n);
+    }, "pathName"_a, "n"_a);
     cls_StructureNode.def(py::init<const e57::Node &>(), "n"_a);
     cls_StructureNode.def("isRoot", &StructureNode::isRoot);
     cls_StructureNode.def("parent", &StructureNode::parent);
     cls_StructureNode.def("pathName", &StructureNode::pathName);
     cls_StructureNode.def("elementName", &StructureNode::elementName);
     cls_StructureNode.def("destImageFile", &StructureNode::destImageFile);
     cls_StructureNode.def("isAttached", &StructureNode::isAttached);
```

### Comparing `pye57-0.4.4/src/pye57/scan_header.py` & `pye57-0.4.5/src/pye57/scan_header.py`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/src/pye57.egg-info/PKG-INFO` & `pye57-0.4.5/src/pye57.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pye57
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python .e57 files reader/writer
 Home-page: https://www.github.com/davidcaron/pye57
 Author: David Caron
 Author-email: dcaron05@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pye57-0.4.4/src/pye57.egg-info/SOURCES.txt` & `pye57-0.4.5/src/pye57.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pye57-0.4.4/tests/test_main.py` & `pye57-0.4.5/tests/test_main.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import time
 
 import numpy as np
 
 import pye57
 from pye57 import libe57
+from pye57.utils import get_node, copy_node
 
 try:
     from exceptions import WindowsError
 except ImportError:
     class WindowsError(OSError):
         pass
 
@@ -33,18 +34,26 @@
             os.remove(path)
 
 
 @pytest.fixture
 def e57_path():
     return sample_data("test.e57")
 
+
 @pytest.fixture
 def e57_spherical_path():
     return sample_data("testSpherical.e57")
 
+
+@pytest.fixture
+def e57_with_data_and_images_path():
+    # From http://www.libe57.org/data.html
+    return sample_data("pumpAVisualReferenceImage.e57")
+
+
 @pytest.fixture
 def temp_e57_write(request):
     path = sample_data("test_write.e57")
     request.addfinalizer(lambda: delete_retry(path))
     return path
 
 
@@ -298,7 +307,115 @@
     with pytest.raises(ValueError):
         data = e57.read_scan(0, colors=True)
 
 
 def test_scan_position(e57_path):
     e57 = pye57.E57(e57_path)
     assert np.allclose(e57.scan_position(3), np.array([[3.01323456e+05, 5.04260184e+06, 1.56040279e+01]]))
+
+
+BUFFER_TYPES = {
+    libe57.FloatNode: 'd',
+    libe57.IntegerNode: 'l',
+    libe57.ScaledIntegerNode: 'd'
+}
+
+
+def make_buffer(node: libe57.Node, capacity: int):
+    node_type = type(node)
+    if node_type not in BUFFER_TYPES:
+        raise ValueError("Unsupported field type!")
+
+    buffer_type = BUFFER_TYPES[node_type]
+
+    np_array = np.empty(capacity, buffer_type)
+    buffer = libe57.SourceDestBuffer(
+        node.destImageFile(), node.elementName(), np_array, capacity, True, True)
+    return np_array, buffer
+
+
+def make_buffers(node: libe57.StructureNode, capacity: int):
+    data = {}
+    buffers = libe57.VectorSourceDestBuffer()
+    for i in range(node.childCount()):
+        field = get_node(node, i)
+        d, b = make_buffer(field, capacity)
+        data[field.elementName()] = d
+        buffers.append(b)
+    return data, buffers
+
+
+def copy_compressed_vector_data(in_node: libe57.Node, out_node: libe57.Node):
+    chunk_size = 100000
+
+    in_prototype = libe57.StructureNode(in_node.prototype())
+    out_prototype = libe57.StructureNode(out_node.prototype())
+
+    in_data, in_buffers = make_buffers(in_prototype, chunk_size)
+    out_data, out_buffers = make_buffers(out_prototype, chunk_size)
+
+    in_reader = in_node.reader(in_buffers)
+    out_writer = out_node.writer(out_buffers)
+
+    n_points = in_node.childCount()
+    current_index = 0
+    while current_index != n_points:
+        current_chunk = min(n_points - current_index, chunk_size)
+
+        in_reader.read()
+        for field in in_data:
+            out_data[field][:current_chunk] = in_data[field][:current_chunk]
+
+        out_writer.write(current_chunk)
+
+        current_index += current_chunk
+
+    in_reader.close()
+    out_writer.close()
+
+
+def copy_blob_data(in_node, out_node):
+    chunk_size = 100000
+
+    byte_count = in_node.byteCount()
+    blob_buffer = np.empty(chunk_size, np.ubyte)
+    current_index = 0
+    while current_index != byte_count:
+        current_chunk = min(byte_count - current_index, chunk_size)
+
+        in_node.read(blob_buffer, current_index, current_chunk)
+        out_node.write(blob_buffer, current_index, current_chunk)
+
+        current_index += current_chunk
+
+
+def test_clone_e57(e57_with_data_and_images_path, temp_e57_write):
+
+    in_image = libe57.ImageFile(e57_with_data_and_images_path, "r")
+    out_image = libe57.ImageFile(temp_e57_write, "w")
+
+    for i in range(in_image.extensionsCount()):
+        out_image.extensionsAdd(
+            in_image.extensionsPrefix(i),
+            in_image.extensionsUri(i)
+        )
+    
+    in_root = in_image.root()
+    out_root = out_image.root()
+
+    compressed_node_pairs = []
+    for i in range(in_root.childCount()):
+        in_child = get_node(in_root, i)
+        in_child_name = in_child.elementName()
+        out_child, out_child_compressed_node_pairs, out_child_blob_node_pairs = copy_node(in_child, out_image)
+
+        out_root.set(in_child_name, out_child)
+        compressed_node_pairs.extend(out_child_compressed_node_pairs)
+    
+    for compressed_node_pair in compressed_node_pairs:
+        copy_compressed_vector_data(compressed_node_pair['in'], compressed_node_pair['out'])
+
+    for blob_node_pair in out_child_blob_node_pairs:
+        copy_blob_data(blob_node_pair['in'], blob_node_pair['out'])
+
+    in_image.close()
+    out_image.close()
```

