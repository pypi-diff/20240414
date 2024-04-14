# Comparing `tmp/pyPublicDecompWT-2.8.1.4.tar.gz` & `tmp/pypublicdecompwt-2.8.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPublicDecompWT-2.8.1.4.tar", last modified: Mon Oct 17 16:31:33 2022, max compression
+gzip compressed data, was "pypublicdecompwt-2.8.1.5.tar", last modified: Sun Apr 14 06:56:24 2024, max compression
```

## Comparing `pyPublicDecompWT-2.8.1.4.tar` & `pypublicdecompwt-2.8.1.5.tar`

### file list

```diff
@@ -1,136 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:31:33.884562 pyPublicDecompWT-2.8.1.4/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2457 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1001 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:31:33.876562 pyPublicDecompWT-2.8.1.4/COMP/
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:31:33.876562 pyPublicDecompWT-2.8.1.4/COMP/Inc/
--rw-r--r--   0 runner    (1001) docker     (121)    11000 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/Inc/Bitlevel.h
--rw-r--r--   0 runner    (1001) docker     (121)     5006 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/Inc/CBlock.h
--rw-r--r--   0 runner    (1001) docker     (121)    16092 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/Inc/CBuffer.h
--rw-r--r--   0 runner    (1001) docker     (121)    15292 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/Inc/CImage.h
--rw-r--r--   0 runner    (1001) docker     (121)     4012 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/Inc/CQualityInfo.h
--rw-r--r--   0 runner    (1001) docker     (121)     3525 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/Inc/CQualityMeasures.h
--rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/Inc/Compress.h
--rw-r--r--   0 runner    (1001) docker     (121)     2589 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/Inc/RMAErrorHandling.h
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/Inc/vssver.scc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:31:33.876562 pyPublicDecompWT-2.8.1.4/COMP/JPEG/
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:31:33.876562 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/
--rw-r--r--   0 runner    (1001) docker     (121)     5412 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/CHOptim.h
--rw-r--r--   0 runner    (1001) docker     (121)     8476 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/CHcodec.h
--rw-r--r--   0 runner    (1001) docker     (121)     5222 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/CHufftables.h
--rw-r--r--   0 runner    (1001) docker     (121)     6913 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/CJBlock.h
--rw-r--r--   0 runner    (1001) docker     (121)     3350 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/CJPEGCoder.h
--rw-r--r--   0 runner    (1001) docker     (121)     7316 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/CJPEGDecoder.h
--rw-r--r--   0 runner    (1001) docker     (121)     3644 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/CJPEGLossLessCoder.h
--rw-r--r--   0 runner    (1001) docker     (121)     3168 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/CJPEGLossyCoder.h
--rw-r--r--   0 runner    (1001) docker     (121)     5948 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/CQuantizationTable.h
--rw-r--r--   0 runner    (1001) docker     (121)    12236 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/CompressJPEG.h
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/JPEGConst.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:31:33.876562 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Src/
--rw-r--r--   0 runner    (1001) docker     (121)    10849 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Src/CHOptim.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3774 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Src/CHcodec.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    10404 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Src/CHufftables.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     8995 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Src/CJBlock.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    31868 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Src/CJPEGDecoder.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     7237 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Src/CJPEGLossLessCoder.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6051 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Src/CJPEGLossyCoder.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4017 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Src/CQuantizationTable.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     5534 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/JPEG/Src/CompressJPEG.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:31:33.876562 pyPublicDecompWT-2.8.1.4/COMP/Src/
--rw-r--r--   0 runner    (1001) docker     (121)     4917 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/Src/CBuffer.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    11186 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/Src/CImage.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3468 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/Src/CQualityMeasures.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:31:33.876562 pyPublicDecompWT-2.8.1.4/COMP/T4/
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/T4/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:31:33.876562 pyPublicDecompWT-2.8.1.4/COMP/T4/Inc/
--rw-r--r--   0 runner    (1001) docker     (121)    10464 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/T4/Inc/CBitBuffer.h
--rw-r--r--   0 runner    (1001) docker     (121)     3433 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/T4/Inc/CompressT4.h
--rw-r--r--   0 runner    (1001) docker     (121)     4185 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/T4/Inc/T4Coder.h
--rw-r--r--   0 runner    (1001) docker     (121)    12315 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/T4/Inc/T4Codes.h
--rw-r--r--   0 runner    (1001) docker     (121)     4690 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/T4/Inc/T4Decoder.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:31:33.880562 pyPublicDecompWT-2.8.1.4/COMP/T4/Src/
--rw-r--r--   0 runner    (1001) docker     (121)     5950 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/T4/Src/CBitBuffer.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1598 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/T4/Src/CompressT4.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4437 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/T4/Src/T4Coder.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    11371 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/T4/Src/T4Codes.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     7273 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/T4/Src/T4Decoder.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:31:33.880562 pyPublicDecompWT-2.8.1.4/COMP/WT/
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:31:33.880562 pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/
--rw-r--r--   0 runner    (1001) docker     (121)     5831 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/CACCoder.h
--rw-r--r--   0 runner    (1001) docker     (121)     5570 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/CACDecoder.h
--rw-r--r--   0 runner    (1001) docker     (121)     6268 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/CACModel.h
--rw-r--r--   0 runner    (1001) docker     (121)     3532 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/CVLCCodec.h
--rw-r--r--   0 runner    (1001) docker     (121)     5771 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/CVLCCoder.h
--rw-r--r--   0 runner    (1001) docker     (121)     6866 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/CVLCDecoder.h
--rw-r--r--   0 runner    (1001) docker     (121)    14098 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/CWBlock.h
--rw-r--r--   0 runner    (1001) docker     (121)     3611 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/CWTCoder.h
--rw-r--r--   0 runner    (1001) docker     (121)     5283 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/CWTDecoder.h
--rw-r--r--   0 runner    (1001) docker     (121)     7505 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/CompressWT.h
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/WTConst.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:31:33.880562 pyPublicDecompWT-2.8.1.4/COMP/WT/Src/
--rw-r--r--   0 runner    (1001) docker     (121)     1652 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/Src/CACCoder.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1566 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/Src/CACDecoder.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1919 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/Src/CACModel.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     5355 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/Src/CVLCCoder.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    12197 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/Src/CVLCDecoder.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    19025 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/Src/CWBlock.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6036 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/Src/CWTCoder.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    12763 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/Src/CWTDecoder.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/COMP/WT/Src/CompressWT.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:31:33.884562 pyPublicDecompWT-2.8.1.4/DISE/
--rw-r--r--   0 runner    (1001) docker     (121)    19053 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/CDataField.h
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5351 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/CSpacecraftID.h
--rw-r--r--   0 runner    (1001) docker     (121)     4792 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/CSpectralChannelID.h
--rw-r--r--   0 runner    (1001) docker     (121)     5704 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/CxRITAnnotation.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     5785 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/CxRITAnnotation.h
--rw-r--r--   0 runner    (1001) docker     (121)     7438 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/CxRITFile.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6284 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/CxRITFile.h
--rw-r--r--   0 runner    (1001) docker     (121)     3895 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/CxRITFileCompressed.h
--rw-r--r--   0 runner    (1001) docker     (121)     3797 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/CxRITFileDecompressed.h
--rw-r--r--   0 runner    (1001) docker     (121)    23508 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/CxRITFileHeaderRecords.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    21546 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/CxRITFileHeaderRecords.h
--rw-r--r--   0 runner    (1001) docker     (121)     1466 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/ErrorHandling.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3914 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/ErrorHandling.h
--rw-r--r--   0 runner    (1001) docker     (121)    25745 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/GSDS_Volume_F_NBO.h
--rw-r--r--   0 runner    (1001) docker     (121)    29186 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/MSGTime.h
--rw-r--r--   0 runner    (1001) docker     (121)    44747 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/MSGTime_impl.h
--rw-r--r--   0 runner    (1001) docker     (121)     5591 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/SmartPtr.h
--rw-r--r--   0 runner    (1001) docker     (121)     2194 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/TimeSpan.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4245 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/TimeSpan.h
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/Types.h
--rw-r--r--   0 runner    (1001) docker     (121)     6261 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/UTCTime.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     9051 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/UTCTime.h
--rw-r--r--   0 runner    (1001) docker     (121)     3981 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/DISE/YYYYMMDDhhmm.h
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4825 2022-10-17 16:31:33.884562 pyPublicDecompWT-2.8.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/PublicDecompWT.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     3406 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:31:33.872562 pyPublicDecompWT-2.8.1.4/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:31:33.884562 pyPublicDecompWT-2.8.1.4/cmake/modules/
--rw-r--r--   0 runner    (1001) docker     (121)    22219 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/cmake/modules/FindPythonExtensions.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    11404 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/cmake/modules/UsePythonExtensions.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    17931 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/cmake/modules/targetLinkLibrariesWithDynamicLookup.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:31:33.884562 pyPublicDecompWT-2.8.1.4/pyPublicDecompWT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4825 2022-10-17 16:31:33.000000 pyPublicDecompWT-2.8.1.4/pyPublicDecompWT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2839 2022-10-17 16:31:33.000000 pyPublicDecompWT-2.8.1.4/pyPublicDecompWT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 16:31:33.000000 pyPublicDecompWT-2.8.1.4/pyPublicDecompWT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 16:31:33.000000 pyPublicDecompWT-2.8.1.4/pyPublicDecompWT.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-17 16:31:33.000000 pyPublicDecompWT-2.8.1.4/pyPublicDecompWT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-17 16:31:33.000000 pyPublicDecompWT-2.8.1.4/pyPublicDecompWT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:31:33.884562 pyPublicDecompWT-2.8.1.4/pybind/
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/pybind/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/pybind/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)     5270 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/pybind/libxRITDecompress.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:31:33.884562 pyPublicDecompWT-2.8.1.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/scripts/xRITDecompress
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-17 16:31:33.884562 pyPublicDecompWT-2.8.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     8289 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:31:33.884562 pyPublicDecompWT-2.8.1.4/xRITDecompress/
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/xRITDecompress/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3958 2022-10-17 16:31:24.000000 pyPublicDecompWT-2.8.1.4/xRITDecompress/xRITDecompress.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.777002 pypublicdecompwt-2.8.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.757002 pypublicdecompwt-2.8.1.5/COMP/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.757002 pypublicdecompwt-2.8.1.5/COMP/Inc/
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/Inc/Bitlevel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/Inc/CBlock.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16092 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/Inc/CBuffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/Inc/CImage.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/Inc/CQualityInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/Inc/CQualityMeasures.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/Inc/Compress.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/Inc/RMAErrorHandling.h
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/Inc/vssver.scc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.757002 pypublicdecompwt-2.8.1.5/COMP/JPEG/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.761002 pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/CHOptim.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/CHcodec.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/CHufftables.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/CJBlock.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/CJPEGCoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/CJPEGDecoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/CJPEGLossLessCoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/CJPEGLossyCoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/CQuantizationTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12236 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/CompressJPEG.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/JPEGConst.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.761002 pypublicdecompwt-2.8.1.5/COMP/JPEG/Src/
+-rw-r--r--   0 runner    (1001) docker     (127)    10849 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/Src/CHOptim.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/Src/CHcodec.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/Src/CHufftables.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/Src/CJBlock.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    31868 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/Src/CJPEGDecoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/Src/CJPEGLossLessCoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/Src/CJPEGLossyCoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/Src/CQuantizationTable.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/JPEG/Src/CompressJPEG.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.761002 pypublicdecompwt-2.8.1.5/COMP/Src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/Src/CBuffer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11186 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/Src/CImage.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/Src/CQualityMeasures.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.761002 pypublicdecompwt-2.8.1.5/COMP/T4/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/T4/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.765002 pypublicdecompwt-2.8.1.5/COMP/T4/Inc/
+-rw-r--r--   0 runner    (1001) docker     (127)    10464 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/T4/Inc/CBitBuffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/T4/Inc/CompressT4.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/T4/Inc/T4Coder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/T4/Inc/T4Codes.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/T4/Inc/T4Decoder.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.765002 pypublicdecompwt-2.8.1.5/COMP/T4/Src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/T4/Src/CBitBuffer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/T4/Src/CompressT4.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/T4/Src/T4Coder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11371 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/T4/Src/T4Codes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7273 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/T4/Src/T4Decoder.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.765002 pypublicdecompwt-2.8.1.5/COMP/WT/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.765002 pypublicdecompwt-2.8.1.5/COMP/WT/Inc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/Inc/CACCoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/Inc/CACDecoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/Inc/CACModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/Inc/CVLCCodec.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/Inc/CVLCCoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/Inc/CVLCDecoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/Inc/CWBlock.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/Inc/CWTCoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/Inc/CWTDecoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/Inc/CompressWT.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/Inc/WTConst.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.769002 pypublicdecompwt-2.8.1.5/COMP/WT/Src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/Src/CACCoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/Src/CACDecoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/Src/CACModel.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/Src/CVLCCoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12197 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/Src/CVLCDecoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19025 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/Src/CWBlock.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/Src/CWTCoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12763 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/Src/CWTDecoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/COMP/WT/Src/CompressWT.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.773002 pypublicdecompwt-2.8.1.5/DISE/
+-rw-r--r--   0 runner    (1001) docker     (127)    19053 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/CDataField.h
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/CSpacecraftID.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/CSpectralChannelID.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/CxRITAnnotation.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/CxRITAnnotation.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10191 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/CxRITFile.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/CxRITFile.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/CxRITFileCompressed.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/CxRITFileDecompressed.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23508 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/CxRITFileHeaderRecords.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    21546 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/CxRITFileHeaderRecords.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/ErrorHandling.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/ErrorHandling.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25745 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/GSDS_Volume_F_NBO.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29186 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/MSGTime.h
+-rw-r--r--   0 runner    (1001) docker     (127)    44747 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/MSGTime_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/SmartPtr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/TimeSpan.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/TimeSpan.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/Types.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6261 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/UTCTime.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9051 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/UTCTime.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/DISE/YYYYMMDDhhmm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-14 06:56:24.777002 pypublicdecompwt-2.8.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/PublicDecompWT.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.753002 pypublicdecompwt-2.8.1.5/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.773002 pypublicdecompwt-2.8.1.5/cmake/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)    22219 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/cmake/modules/FindPythonExtensions.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/cmake/modules/UsePythonExtensions.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    17931 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/cmake/modules/targetLinkLibrariesWithDynamicLookup.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.773002 pypublicdecompwt-2.8.1.5/pyPublicDecompWT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-14 06:56:24.000000 pypublicdecompwt-2.8.1.5/pyPublicDecompWT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-14 06:56:24.000000 pypublicdecompwt-2.8.1.5/pyPublicDecompWT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 06:56:24.000000 pypublicdecompwt-2.8.1.5/pyPublicDecompWT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 06:56:24.000000 pypublicdecompwt-2.8.1.5/pyPublicDecompWT.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 06:56:24.000000 pypublicdecompwt-2.8.1.5/pyPublicDecompWT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-14 06:56:24.000000 pypublicdecompwt-2.8.1.5/pyPublicDecompWT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.773002 pypublicdecompwt-2.8.1.5/pybind/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/pybind/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/pybind/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/pybind/libxRITDecompress.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.773002 pypublicdecompwt-2.8.1.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/scripts/xRITDecompress
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 06:56:24.777002 pypublicdecompwt-2.8.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.773002 pypublicdecompwt-2.8.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:56:24.773002 pypublicdecompwt-2.8.1.5/xRITDecompress/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/xRITDecompress/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-14 06:56:21.000000 pypublicdecompwt-2.8.1.5/xRITDecompress/xRITDecompress.cpp
```

### Comparing `pyPublicDecompWT-2.8.1.4/CHANGELOG.md` & `pypublicdecompwt-2.8.1.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/CMakeLists.txt` & `pypublicdecompwt-2.8.1.5/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/CMakeLists.txt` & `pypublicdecompwt-2.8.1.5/COMP/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 set_property(TARGET ${LIBNAME} PROPERTY POSITION_INDEPENDENT_CODE ON)
 target_link_libraries(${LIBNAME} LINK_PUBLIC "DISE")
 target_include_directories(${LIBNAME} PUBLIC Inc)
 set_property(TARGET ${LIBNAME} APPEND PROPERTY INTERFACE_INCLUDE_DIRECTORIES
         $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/Inc>
         $<INSTALL_INTERFACE:Inc>  # <prefix>/Inc
         )
-install(TARGETS ${LIBNAME} DESTINATION .)
+install(TARGETS ${LIBNAME} DESTINATION lib)
 
 
 # add subdirs
 add_subdirectory(T4)
 add_subdirectory(JPEG)
 add_subdirectory(WT)
```

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/Inc/Bitlevel.h` & `pypublicdecompwt-2.8.1.5/COMP/Inc/Bitlevel.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/Inc/CBlock.h` & `pypublicdecompwt-2.8.1.5/COMP/Inc/CBlock.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/Inc/CBuffer.h` & `pypublicdecompwt-2.8.1.5/COMP/Inc/CBuffer.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/Inc/CImage.h` & `pypublicdecompwt-2.8.1.5/COMP/Inc/CImage.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/Inc/CQualityInfo.h` & `pypublicdecompwt-2.8.1.5/COMP/Inc/CQualityInfo.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/Inc/CQualityMeasures.h` & `pypublicdecompwt-2.8.1.5/COMP/Inc/CQualityMeasures.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/Inc/Compress.h` & `pypublicdecompwt-2.8.1.5/COMP/Inc/Compress.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/Inc/RMAErrorHandling.h` & `pypublicdecompwt-2.8.1.5/COMP/Inc/RMAErrorHandling.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/CMakeLists.txt` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/CHOptim.h` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/CHOptim.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/CHcodec.h` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/CHcodec.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/CHufftables.h` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/CHufftables.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/CJBlock.h` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/CJBlock.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/CJPEGCoder.h` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/CJPEGCoder.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/CJPEGDecoder.h` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/CJPEGDecoder.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/CJPEGLossLessCoder.h` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/CJPEGLossLessCoder.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/CJPEGLossyCoder.h` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/CJPEGLossyCoder.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/CQuantizationTable.h` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/CQuantizationTable.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/CompressJPEG.h` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/CompressJPEG.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/Inc/JPEGConst.h` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/Inc/JPEGConst.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/Src/CHOptim.cpp` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/Src/CHOptim.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/Src/CHcodec.cpp` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/Src/CHcodec.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/Src/CHufftables.cpp` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/Src/CHufftables.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/Src/CJBlock.cpp` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/Src/CJBlock.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/Src/CJPEGDecoder.cpp` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/Src/CJPEGDecoder.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/Src/CJPEGLossLessCoder.cpp` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/Src/CJPEGLossLessCoder.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/Src/CJPEGLossyCoder.cpp` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/Src/CJPEGLossyCoder.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/Src/CQuantizationTable.cpp` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/Src/CQuantizationTable.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/JPEG/Src/CompressJPEG.cpp` & `pypublicdecompwt-2.8.1.5/COMP/JPEG/Src/CompressJPEG.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/Src/CBuffer.cpp` & `pypublicdecompwt-2.8.1.5/COMP/Src/CBuffer.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/Src/CImage.cpp` & `pypublicdecompwt-2.8.1.5/COMP/Src/CImage.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/Src/CQualityMeasures.cpp` & `pypublicdecompwt-2.8.1.5/COMP/Src/CQualityMeasures.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/T4/CMakeLists.txt` & `pypublicdecompwt-2.8.1.5/COMP/T4/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/T4/Inc/CBitBuffer.h` & `pypublicdecompwt-2.8.1.5/COMP/T4/Inc/CBitBuffer.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/T4/Inc/CompressT4.h` & `pypublicdecompwt-2.8.1.5/COMP/T4/Inc/CompressT4.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/T4/Inc/T4Coder.h` & `pypublicdecompwt-2.8.1.5/COMP/T4/Inc/T4Coder.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/T4/Inc/T4Codes.h` & `pypublicdecompwt-2.8.1.5/COMP/T4/Inc/T4Codes.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/T4/Inc/T4Decoder.h` & `pypublicdecompwt-2.8.1.5/COMP/T4/Inc/T4Decoder.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/T4/Src/CBitBuffer.cpp` & `pypublicdecompwt-2.8.1.5/COMP/T4/Src/CBitBuffer.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/T4/Src/CompressT4.cpp` & `pypublicdecompwt-2.8.1.5/COMP/T4/Src/CompressT4.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/T4/Src/T4Coder.cpp` & `pypublicdecompwt-2.8.1.5/COMP/T4/Src/T4Coder.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/T4/Src/T4Codes.cpp` & `pypublicdecompwt-2.8.1.5/COMP/T4/Src/T4Codes.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/T4/Src/T4Decoder.cpp` & `pypublicdecompwt-2.8.1.5/COMP/T4/Src/T4Decoder.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/CMakeLists.txt` & `pypublicdecompwt-2.8.1.5/COMP/WT/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/CACCoder.h` & `pypublicdecompwt-2.8.1.5/COMP/WT/Inc/CACCoder.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/CACDecoder.h` & `pypublicdecompwt-2.8.1.5/COMP/WT/Inc/CACDecoder.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/CACModel.h` & `pypublicdecompwt-2.8.1.5/COMP/WT/Inc/CACModel.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/CVLCCodec.h` & `pypublicdecompwt-2.8.1.5/COMP/WT/Inc/CVLCCodec.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/CVLCCoder.h` & `pypublicdecompwt-2.8.1.5/COMP/WT/Inc/CVLCCoder.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/CVLCDecoder.h` & `pypublicdecompwt-2.8.1.5/COMP/WT/Inc/CVLCDecoder.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/CWBlock.h` & `pypublicdecompwt-2.8.1.5/COMP/WT/Inc/CWBlock.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/CWTCoder.h` & `pypublicdecompwt-2.8.1.5/COMP/WT/Inc/CWTCoder.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/CWTDecoder.h` & `pypublicdecompwt-2.8.1.5/COMP/WT/Inc/CWTDecoder.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/CompressWT.h` & `pypublicdecompwt-2.8.1.5/COMP/WT/Inc/CompressWT.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/Inc/WTConst.h` & `pypublicdecompwt-2.8.1.5/COMP/WT/Inc/WTConst.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/Src/CACCoder.cpp` & `pypublicdecompwt-2.8.1.5/COMP/WT/Src/CACCoder.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/Src/CACDecoder.cpp` & `pypublicdecompwt-2.8.1.5/COMP/WT/Src/CACDecoder.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/Src/CACModel.cpp` & `pypublicdecompwt-2.8.1.5/COMP/WT/Src/CACModel.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/Src/CVLCCoder.cpp` & `pypublicdecompwt-2.8.1.5/COMP/WT/Src/CVLCCoder.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/Src/CVLCDecoder.cpp` & `pypublicdecompwt-2.8.1.5/COMP/WT/Src/CVLCDecoder.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/Src/CWBlock.cpp` & `pypublicdecompwt-2.8.1.5/COMP/WT/Src/CWBlock.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/Src/CWTCoder.cpp` & `pypublicdecompwt-2.8.1.5/COMP/WT/Src/CWTCoder.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/Src/CWTDecoder.cpp` & `pypublicdecompwt-2.8.1.5/COMP/WT/Src/CWTDecoder.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/COMP/WT/Src/CompressWT.cpp` & `pypublicdecompwt-2.8.1.5/COMP/WT/Src/CompressWT.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/CDataField.h` & `pypublicdecompwt-2.8.1.5/DISE/CDataField.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/CMakeLists.txt` & `pypublicdecompwt-2.8.1.5/DISE/CMakeLists.txt`

 * *Files 12% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 add_library(${LIBNAME} STATIC ${SOURCE_FILES})
 set_property(TARGET ${LIBNAME} PROPERTY POSITION_INDEPENDENT_CODE ON)
 target_include_directories(${LIBNAME} PUBLIC .)
 set_property(TARGET ${LIBNAME} APPEND PROPERTY INTERFACE_INCLUDE_DIRECTORIES
         $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/>
         $<INSTALL_INTERFACE:>  # <prefix>/
         )
-install(TARGETS ${LIBNAME} DESTINATION .)
+install(TARGETS ${LIBNAME} DESTINATION lib)
```

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/CSpacecraftID.h` & `pypublicdecompwt-2.8.1.5/DISE/CSpacecraftID.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/CSpectralChannelID.h` & `pypublicdecompwt-2.8.1.5/DISE/CSpectralChannelID.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/CxRITAnnotation.cpp` & `pypublicdecompwt-2.8.1.5/DISE/CxRITAnnotation.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/CxRITAnnotation.h` & `pypublicdecompwt-2.8.1.5/DISE/CxRITAnnotation.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/CxRITFile.h` & `pypublicdecompwt-2.8.1.5/DISE/CxRITFile.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/CxRITFileCompressed.h` & `pypublicdecompwt-2.8.1.5/DISE/CxRITFileCompressed.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/CxRITFileDecompressed.h` & `pypublicdecompwt-2.8.1.5/DISE/CxRITFileDecompressed.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/CxRITFileHeaderRecords.cpp` & `pypublicdecompwt-2.8.1.5/DISE/CxRITFileHeaderRecords.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/CxRITFileHeaderRecords.h` & `pypublicdecompwt-2.8.1.5/DISE/CxRITFileHeaderRecords.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/ErrorHandling.cpp` & `pypublicdecompwt-2.8.1.5/DISE/ErrorHandling.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/ErrorHandling.h` & `pypublicdecompwt-2.8.1.5/DISE/ErrorHandling.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/GSDS_Volume_F_NBO.h` & `pypublicdecompwt-2.8.1.5/DISE/GSDS_Volume_F_NBO.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/MSGTime.h` & `pypublicdecompwt-2.8.1.5/DISE/MSGTime.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/MSGTime_impl.h` & `pypublicdecompwt-2.8.1.5/DISE/MSGTime_impl.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/SmartPtr.h` & `pypublicdecompwt-2.8.1.5/DISE/SmartPtr.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/TimeSpan.cpp` & `pypublicdecompwt-2.8.1.5/DISE/TimeSpan.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/TimeSpan.h` & `pypublicdecompwt-2.8.1.5/DISE/TimeSpan.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/Types.h` & `pypublicdecompwt-2.8.1.5/DISE/Types.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/UTCTime.cpp` & `pypublicdecompwt-2.8.1.5/DISE/UTCTime.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/UTCTime.h` & `pypublicdecompwt-2.8.1.5/DISE/UTCTime.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/DISE/YYYYMMDDhhmm.h` & `pypublicdecompwt-2.8.1.5/DISE/YYYYMMDDhhmm.h`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/LICENSE` & `pypublicdecompwt-2.8.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/PKG-INFO` & `pypublicdecompwt-2.8.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPublicDecompWT
-Version: 2.8.1.4
+Version: 2.8.1.5
 Summary: Python bindings for EUMETSAT's PublicDecompWT
 Home-page: https://github.com/sbrodehl/pyPublicDecompWT
 Author: Sebastian Brodehl
 Author-email: foss@sbrodehl.de
 License: Apache-2.0 License
 Project-URL: Documentation, https://github.com/sbrodehl/pyPublicDecompWT
 Project-URL: Source, https://github.com/sbrodehl/pyPublicDecompWT
@@ -23,17 +23,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS.txt
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 # pyPublicDecompWT
 [![python versions](https://img.shields.io/pypi/pyversions/pyPublicDecompWT)](https://pypi.org/project/pyPublicDecompWT)
 [![wheel](https://img.shields.io/pypi/wheel/pyPublicDecompWT)](https://pypi.org/project/pyPublicDecompWT/#files)
 [![CI build](https://github.com/sbrodehl/pyPublicDecompWT/actions/workflows/trigger.yml/badge.svg)](https://github.com/sbrodehl/pyPublicDecompWT/actions/workflows/trigger.yml)
 
 This package provides python bindings for some of [EUMETSAT’s PublicDecompWT][2] tools.
@@ -43,15 +44,15 @@
 If you need other classes or functionalities, please open a [pull-request][3]!
 
 This repository contains / mirrors the source code for the complete [PublicDecompWT][2] tool, as well.
 Additionally, we provide CMake build files.
 
 ## Installation
 
-Install pyxRITDecompress via pip:
+Install pyPublicDecompWT via pip:
 ```bash
 pip install pyPublicDecompWT
 ```
 
 The following command will verify if the installation succeeded:
 
 ```bash
```

### Comparing `pyPublicDecompWT-2.8.1.4/PublicDecompWT.ABOUT` & `pypublicdecompwt-2.8.1.5/PublicDecompWT.ABOUT`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/README.md` & `pypublicdecompwt-2.8.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 If you need other classes or functionalities, please open a [pull-request][3]!
 
 This repository contains / mirrors the source code for the complete [PublicDecompWT][2] tool, as well.
 Additionally, we provide CMake build files.
 
 ## Installation
 
-Install pyxRITDecompress via pip:
+Install pyPublicDecompWT via pip:
 ```bash
 pip install pyPublicDecompWT
 ```
 
 The following command will verify if the installation succeeded:
 
 ```bash
```

### Comparing `pyPublicDecompWT-2.8.1.4/cmake/modules/FindPythonExtensions.cmake` & `pypublicdecompwt-2.8.1.5/cmake/modules/FindPythonExtensions.cmake`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/cmake/modules/UsePythonExtensions.cmake` & `pypublicdecompwt-2.8.1.5/cmake/modules/UsePythonExtensions.cmake`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/cmake/modules/targetLinkLibrariesWithDynamicLookup.cmake` & `pypublicdecompwt-2.8.1.5/cmake/modules/targetLinkLibrariesWithDynamicLookup.cmake`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/pyPublicDecompWT.egg-info/PKG-INFO` & `pypublicdecompwt-2.8.1.5/pyPublicDecompWT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPublicDecompWT
-Version: 2.8.1.4
+Version: 2.8.1.5
 Summary: Python bindings for EUMETSAT's PublicDecompWT
 Home-page: https://github.com/sbrodehl/pyPublicDecompWT
 Author: Sebastian Brodehl
 Author-email: foss@sbrodehl.de
 License: Apache-2.0 License
 Project-URL: Documentation, https://github.com/sbrodehl/pyPublicDecompWT
 Project-URL: Source, https://github.com/sbrodehl/pyPublicDecompWT
@@ -23,17 +23,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS.txt
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 # pyPublicDecompWT
 [![python versions](https://img.shields.io/pypi/pyversions/pyPublicDecompWT)](https://pypi.org/project/pyPublicDecompWT)
 [![wheel](https://img.shields.io/pypi/wheel/pyPublicDecompWT)](https://pypi.org/project/pyPublicDecompWT/#files)
 [![CI build](https://github.com/sbrodehl/pyPublicDecompWT/actions/workflows/trigger.yml/badge.svg)](https://github.com/sbrodehl/pyPublicDecompWT/actions/workflows/trigger.yml)
 
 This package provides python bindings for some of [EUMETSAT’s PublicDecompWT][2] tools.
@@ -43,15 +44,15 @@
 If you need other classes or functionalities, please open a [pull-request][3]!
 
 This repository contains / mirrors the source code for the complete [PublicDecompWT][2] tool, as well.
 Additionally, we provide CMake build files.
 
 ## Installation
 
-Install pyxRITDecompress via pip:
+Install pyPublicDecompWT via pip:
 ```bash
 pip install pyPublicDecompWT
 ```
 
 The following command will verify if the installation succeeded:
 
 ```bash
```

### Comparing `pyPublicDecompWT-2.8.1.4/pyPublicDecompWT.egg-info/SOURCES.txt` & `pypublicdecompwt-2.8.1.5/pyPublicDecompWT.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -106,9 +106,10 @@
 pyPublicDecompWT.egg-info/not-zip-safe
 pyPublicDecompWT.egg-info/requires.txt
 pyPublicDecompWT.egg-info/top_level.txt
 pybind/CMakeLists.txt
 pybind/VERSION
 pybind/libxRITDecompress.cpp
 scripts/xRITDecompress
+tests/test_api.py
 xRITDecompress/CMakeLists.txt
 xRITDecompress/xRITDecompress.cpp
```

### Comparing `pyPublicDecompWT-2.8.1.4/pybind/libxRITDecompress.cpp` & `pypublicdecompwt-2.8.1.5/pybind/libxRITDecompress.cpp`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/scripts/xRITDecompress` & `pypublicdecompwt-2.8.1.5/scripts/xRITDecompress`

 * *Files identical despite different names*

### Comparing `pyPublicDecompWT-2.8.1.4/setup.py` & `pypublicdecompwt-2.8.1.5/setup.py`

 * *Files identical despite different names*

