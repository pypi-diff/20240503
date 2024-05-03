# Comparing `tmp/ytpb-2024.4.20.tar.gz` & `tmp/ytpb-2024.5.3.tar.gz`

## Comparing `ytpb-2024.4.20.tar` & `ytpb-2024.5.3.tar`

### file list

```diff
@@ -1,141 +1,140 @@
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ytpb-2024.4.20/.gitattributes
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 ytpb-2024.4.20/.pre-commit-config.yaml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ytpb-2024.4.20/.readthedocs.yaml
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 ytpb-2024.4.20/CHANGELOG.rst
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 ytpb-2024.4.20/CONTRIBUTING.rst
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 ytpb-2024.4.20/Makefile
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 ytpb-2024.4.20/config.toml.example
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/changelog.rst
--rw-r--r--   0        0        0    22920 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/cli.rst
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/conf.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/contributing.rst
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/cookbook.rst
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/index.rst
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/quick.rst
--rw-r--r--   0        0        0     8474 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/reference.rst
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/why.rst
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/index.rst
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/usage.rst
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/index.rst
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.actions.rst
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.cache.rst
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.download.rst
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.errors.rst
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.fetchers.rst
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.info.rst
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.locate.rst
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.merge.rst
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.playback.rst
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.representations.rst
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.rst
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.segment.rst
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.streams.rst
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 ytpb-2024.4.20/etc/Containerfile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.20/notebooks/shared/.gitkeep
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/__main__.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/api.py
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/cache.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/conditional.py
--rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/config.py
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/download.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/errors.py
--rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/fetchers.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/ffmpeg.py
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/info.py
--rw-r--r--   0        0        0    10576 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/locate.py
--rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/merge.py
--rw-r--r--   0        0        0    23882 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/playback.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/representations.py
--rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/segment.py
--rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/streams.py
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/types.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/actions/__init__.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/actions/capture.py
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/actions/compose.py
--rw-r--r--   0        0        0     7744 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/actions/download.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/cli/__init__.py
--rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/cli/common.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/cli/options.py
--rw-r--r--   0        0        0     7874 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/cli/parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/cli/commands/__init__.py
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/cli/commands/capture.py
--rw-r--r--   0        0        0    15726 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/cli/commands/download.py
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/cli/commands/mpd.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/utils/__init__.py
--rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/utils/date.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/utils/other.py
--rw-r--r--   0        0        0     8625 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/utils/path.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/utils/remote.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/utils/url.py
--rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/conftest.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/helpers.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_cache.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_download.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_fetchers.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_info.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_locate.py
--rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_merge.py
--rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_playback.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_playback_session.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_representations.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_segment.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_streams.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/actions/__init__.py
--rw-r--r--   0        0        0     8653 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/actions/test_compose.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/actions/test_download.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/cli/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/cli/conftest.py
--rw-r--r--   0        0        0    43550 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/cli/test_download_command.py
--rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/cli/test_parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/cli/capture/__init__.py
--rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/cli/capture/test_frame_command.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/cli/mpd/__init__.py
--rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/cli/mpd/test_compose_command.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/cli/mpd/test_refresh_command.py
--rw-r--r--   0        0        0    56372 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/info-1695928670.json
--rw-r--r--   0        0        0  2978627 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/manifest-1695928670.mpd
--rw-r--r--   0        0        0   701494 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/webpage-1695928670.html
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244].out
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_compose_mpd[itag%20eq%20140-none].out
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244].out
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_compose_mpd_with_no_streams.out
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244].out
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none].out
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4].out
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_dry_run_option.out
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_no_cut_option.out
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_no_merge_option.out
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_refresh_mpd.out
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/gap-cases/gap-case-1-fixture.csv
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/gap-cases/gap-case-2-fixture.csv
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/gap-cases/gap-case-3-fixture.csv
--rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/segments/7959120.i140.mp4
--rw-r--r--   0        0        0   172355 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/segments/7959120.i244.webm
--rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/segments/7959121.i140.mp4
--rw-r--r--   0        0        0   171647 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/segments/7959121.i244.webm
--rw-r--r--   0        0        0    42602 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/segments/7959122.i140.mp4
--rw-r--r--   0        0        0   173730 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/segments/7959122.i244.webm
--rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/segments/7959123.i140.mp4
--rw-r--r--   0        0        0   172126 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/segments/7959123.i244.webm
--rw-r--r--   0        0        0    42602 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/segments/7959203.i140.mp4
--rw-r--r--   0        0        0   172036 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/segments/7959203.i244.webm
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/utils/__init__.py
--rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/utils/test_date.py
--rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/utils/test_path.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/utils/test_remote.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/utils/test_url.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 ytpb-2024.4.20/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 ytpb-2024.4.20/LICENSE
--rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 ytpb-2024.4.20/README.rst
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 ytpb-2024.4.20/pyproject.toml
--rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 ytpb-2024.4.20/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ytpb-2024.5.3/.gitattributes
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 ytpb-2024.5.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ytpb-2024.5.3/.readthedocs.yaml
+-rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 ytpb-2024.5.3/CHANGELOG.rst
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 ytpb-2024.5.3/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 ytpb-2024.5.3/Makefile
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 ytpb-2024.5.3/config.toml.example
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/changelog.rst
+-rw-r--r--   0        0        0    24143 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/cli.rst
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/conf.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/contributing.rst
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/cookbook.rst
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/index.rst
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/quick.rst
+-rw-r--r--   0        0        0     8474 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/reference.rst
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/why.rst
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/index.rst
+-rw-r--r--   0        0        0     6897 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/usage.rst
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/index.rst
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.actions.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.cache.rst
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.download.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.errors.rst
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.fetchers.rst
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.info.rst
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.locate.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.merge.rst
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.playback.rst
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.representations.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.rst
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.segment.rst
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.streams.rst
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 ytpb-2024.5.3/etc/Containerfile
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/__main__.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/api.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cache.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/conditional.py
+-rw-r--r--   0        0        0     6089 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/config.py
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/download.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/errors.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/fetchers.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/ffmpeg.py
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/info.py
+-rw-r--r--   0        0        0    10576 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/locate.py
+-rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/merge.py
+-rw-r--r--   0        0        0    23882 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/playback.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/representations.py
+-rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/segment.py
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/streams.py
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/types.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/actions/__init__.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/actions/capture.py
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/actions/compose.py
+-rw-r--r--   0        0        0     7755 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/actions/download.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/__init__.py
+-rw-r--r--   0        0        0     7424 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/common.py
+-rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/options.py
+-rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/commands/__init__.py
+-rw-r--r--   0        0        0    17114 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/commands/capture.py
+-rw-r--r--   0        0        0    24033 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/commands/download.py
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/commands/mpd.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/utils/__init__.py
+-rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/utils/date.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/utils/other.py
+-rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/utils/path.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/utils/remote.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/utils/url.py
+-rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/conftest.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/helpers.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_cache.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_download.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_fetchers.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_info.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_locate.py
+-rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_merge.py
+-rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_playback.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_playback_session.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_representations.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_segment.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_streams.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/actions/__init__.py
+-rw-r--r--   0        0        0     8653 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/actions/test_compose.py
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/actions/test_download.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/__init__.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/conftest.py
+-rw-r--r--   0        0        0    60600 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/test_download_command.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/test_parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/capture/__init__.py
+-rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/capture/test_frame_command.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/mpd/__init__.py
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/mpd/test_compose_command.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/mpd/test_refresh_command.py
+-rw-r--r--   0        0        0    56372 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/info-1695928670.json
+-rw-r--r--   0        0        0  2978627 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/manifest-1695928670.mpd
+-rw-r--r--   0        0        0   701494 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/webpage-1695928670.html
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244].out
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_compose_mpd[itag%20eq%20140-none].out
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244].out
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_compose_mpd_with_no_streams.out
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244].out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none].out
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244].out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4].out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4].out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4].out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4].out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4].out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4].out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4].out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4].out
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_dry_run_option.out
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_no_cut_option.out
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_no_merge_option.out
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_refresh_mpd.out
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/gap-cases/gap-case-1-fixture.csv
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/gap-cases/gap-case-2-fixture.csv
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/gap-cases/gap-case-3-fixture.csv
+-rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959120.i140.mp4
+-rw-r--r--   0        0        0   172355 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959120.i244.webm
+-rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959121.i140.mp4
+-rw-r--r--   0        0        0   171647 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959121.i244.webm
+-rw-r--r--   0        0        0    42602 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959122.i140.mp4
+-rw-r--r--   0        0        0   173730 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959122.i244.webm
+-rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959123.i140.mp4
+-rw-r--r--   0        0        0   172126 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959123.i244.webm
+-rw-r--r--   0        0        0    42602 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959203.i140.mp4
+-rw-r--r--   0        0        0   172036 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959203.i244.webm
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/utils/__init__.py
+-rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/utils/test_date.py
+-rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/utils/test_path.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/utils/test_remote.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/utils/test_url.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 ytpb-2024.5.3/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 ytpb-2024.5.3/LICENSE
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 ytpb-2024.5.3/README.rst
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 ytpb-2024.5.3/pyproject.toml
+-rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 ytpb-2024.5.3/PKG-INFO
```

### Comparing `ytpb-2024.4.20/CHANGELOG.rst` & `ytpb-2024.5.3/CHANGELOG.rst`

 * *Files 14% similar despite different names*

```diff
@@ -2,214 +2,257 @@
 00000010: 2323 230a 0a56 6572 7369 6f6e 7320 666f  ###..Versions fo
 00000020: 6c6c 6f77 2060 4361 6c65 6e64 6172 2056  llow `Calendar V
 00000030: 6572 7369 6f6e 696e 6760 5f20 7769 7468  ersioning`_ with
 00000040: 2074 6865 2060 6059 5959 592e 4d2e 4460   the ``YYYY.M.D`
 00000050: 6020 7363 6865 6d65 2e0a 0a2e 2e20 5f43  ` scheme..... _C
 00000060: 616c 656e 6461 7220 5665 7273 696f 6e69  alendar Versioni
 00000070: 6e67 3a20 6874 7470 733a 2f2f 6361 6c76  ng: https://calv
-00000080: 6572 2e6f 7267 0a0a 6032 3032 342e 342e  er.org..`2024.4.
-00000090: 3230 605f 0a2a 2a2a 2a2a 2a2a 2a2a 2a2a  20`_.***********
-000000a0: 2a0a 0a2d 2046 6978 2077 726f 6e67 2066  *..- Fix wrong f
-000000b0: 7261 6d65 2072 6174 6520 7661 6c75 6573  rame rate values
-000000c0: 206f 6620 7468 6520 7669 6465 6f2d 6f6e   of the video-on
-000000d0: 6c79 206d 6572 6765 6420 6669 6c65 7320  ly merged files 
-000000e0: 7768 656e 2062 6f75 6e64 6172 790a 2020  when boundary.  
-000000f0: 7365 676d 656e 7473 2061 7265 2063 7574  segments are cut
-00000100: 2061 6e64 2065 6e63 6f64 6564 2077 6974   and encoded wit
-00000110: 6820 482e 3236 3420 2860 6531 3132 3062  h H.264 (`e1120b
-00000120: 660a 2020 3c68 7474 7073 3a2f 2f67 6974  f.  <https://git
-00000130: 6875 622e 636f 6d2f 7879 6d61 7869 6d2f  hub.com/xymaxim/
-00000140: 7974 7062 2f63 6f6d 6d69 742f 6531 3132  ytpb/commit/e112
-00000150: 3062 6634 3531 3433 3333 6666 3361 6335  0bf4514333ff3ac5
-00000160: 6434 6561 6338 3632 6363 6236 6139 6435  d4eac862ccb6a9d5
-00000170: 6636 3036 3e60 5f5f 290a 2d20 4164 6420  f606>`__).- Add 
-00000180: 6d65 7461 6461 7461 2074 6167 7320 7769  metadata tags wi
-00000190: 7468 2062 6173 6963 2061 6e64 2072 6577  th basic and rew
-000001a0: 696e 6420 696e 666f 726d 6174 696f 6e20  ind information 
-000001b0: 746f 206d 6572 6765 6420 6669 6c65 7320  to merged files 
-000001c0: 2860 6161 3761 6466 310a 2020 3c68 7474  (`aa7adf1.  <htt
-000001d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000001e0: 7879 6d61 7869 6d2f 7974 7062 2f63 6f6d  xymaxim/ytpb/com
-000001f0: 6d69 742f 6161 3761 6466 3135 3830 6535  mit/aa7adf1580e5
-00000200: 6138 3363 3961 6261 6137 3666 3238 3336  a83c9abaa76f2836
-00000210: 6239 6130 3537 3063 6334 6261 3e60 5f5f  b9a0570cc4ba>`__
-00000220: 290a 2020 0a60 3230 3234 2e34 2e31 3260  ).  .`2024.4.12`
-00000230: 5f0a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 0a0a  _.************..
-00000240: 2d20 4164 6420 7468 6520 6050 7974 686f  - Add the `Pytho
-00000250: 6e20 7061 636b 6167 650a 2020 3c68 7474  n package.  <htt
-00000260: 7073 3a2f 2f79 7470 622e 7265 6164 7468  ps://ytpb.readth
-00000270: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00000280: 7374 2f70 6163 6b61 6765 2f69 6e64 6578  st/package/index
-00000290: 2e68 746d 6c3e 605f 5f20 7061 6765 2077  .html>`__ page w
-000002a0: 6974 6820 7468 650a 2020 6261 7369 6320  ith the.  basic 
-000002b0: 7573 6167 6520 616e 6420 4150 4920 7265  usage and API re
-000002c0: 6665 7265 6e63 650a 2d20 4164 6420 7468  ference.- Add th
-000002d0: 6520 6060 2d2d 7665 7273 696f 6e60 6020  e ``--version`` 
-000002e0: 434c 4920 6f70 7469 6f6e 2074 6f20 7368  CLI option to sh
-000002f0: 6f77 2076 6572 7369 6f6e 206e 756d 6265  ow version numbe
-00000300: 720a 2d20 4164 6420 3a61 7474 723a 6079  r.- Add :attr:`y
-00000310: 7470 622e 7265 7072 6573 656e 7461 7469  tpb.representati
-00000320: 6f6e 732e 5265 7072 6573 656e 7461 7469  ons.Representati
-00000330: 6f6e 496e 666f 2e74 7970 6560 2070 726f  onInfo.type` pro
-00000340: 7065 7274 790a 2d20 4164 6420 3a61 7474  perty.- Add :att
-00000350: 723a 6079 7470 622e 706c 6179 6261 636b  r:`ytpb.playback
-00000360: 2e52 6577 696e 6449 6e74 6572 7661 6c2e  .RewindInterval.
-00000370: 6475 7261 7469 6f6e 6020 616e 640a 2020  duration` and.  
-00000380: 3a61 7474 723a 607e 7974 7062 2e70 6c61  :attr:`~ytpb.pla
-00000390: 7962 6163 6b2e 5265 7769 6e64 496e 7465  yback.RewindInte
-000003a0: 7276 616c 2e73 6571 7565 6e63 6573 6020  rval.sequences` 
-000003b0: 7072 6f70 6572 7469 6573 0a2d 2041 6363  properties.- Acc
-000003c0: 6570 7420 556e 6978 2074 696d 6573 7461  ept Unix timesta
-000003d0: 6d70 7320 666f 7220 6d6f 6d65 6e74 7320  mps for moments 
-000003e0: 616e 6420 696e 7465 7276 616c 7320 2860  and intervals (`
-000003f0: 6237 6463 6261 660a 2020 3c68 7474 7073  b7dcbaf.  <https
-00000400: 3a2f 2f67 6974 6875 622e 636f 6d2f 7879  ://github.com/xy
-00000410: 6d61 7869 6d2f 7974 7062 2f63 6f6d 6d69  maxim/ytpb/commi
-00000420: 742f 6237 6463 6261 6636 6565 6265 3366  t/b7dcbaf6eebe3f
-00000430: 3630 3232 6237 6661 3865 6566 6539 3866  6022b7fa8eefe98f
-00000440: 3462 3861 6637 6334 6362 3e60 5f5f 290a  4b8af7c4cb>`__).
-00000450: 2d20 4164 6420 3a63 6c61 7373 3a60 7974  - Add :class:`yt
-00000460: 7062 2e70 6c61 7962 6163 6b2e 5265 7769  pb.playback.Rewi
-00000470: 6e64 5472 6565 4d61 7060 2074 6f20 6b65  ndTreeMap` to ke
-00000480: 6570 2072 6577 696e 6420 6869 7374 6f72  ep rewind histor
-00000490: 7920 2860 3931 6664 3037 380a 2020 3c68  y (`91fd078.  <h
-000004a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000004b0: 6d2f 7879 6d61 7869 6d2f 7974 7062 2f63  m/xymaxim/ytpb/c
-000004c0: 6f6d 6d69 742f 3931 6664 3037 3863 6166  ommit/91fd078caf
-000004d0: 3337 6633 3166 6565 3136 3765 3063 3261  37f31fee167e0c2a
-000004e0: 3230 6133 3861 6132 6261 6463 6438 3e60  20a38aa2badcd8>`
-000004f0: 5f5f 290a 0a42 7265 616b 696e 6720 6368  __)..Breaking ch
-00000500: 616e 6765 730a 3d3d 3d3d 3d3d 3d3d 3d3d  anges.==========
-00000510: 3d3d 3d3d 3d3d 0a0a 2d20 5265 6e61 6d65  ======..- Rename
-00000520: 203a 6d6f 643a 6079 7470 622e 6d70 6460   :mod:`ytpb.mpd`
-00000530: 2074 6f20 3a6d 6f64 3a60 7974 7062 2e72   to :mod:`ytpb.r
-00000540: 6570 7265 7365 6e74 6174 696f 6e73 600a  epresentations`.
-00000550: 2d20 5265 6e61 6d65 203a 6d6f 643a 6079  - Rename :mod:`y
-00000560: 7470 622e 6578 6365 7074 696f 6e73 6020  tpb.exceptions` 
-00000570: 746f 203a 6d6f 643a 6079 7470 622e 6572  to :mod:`ytpb.er
-00000580: 726f 7273 600a 2d20 5265 6e61 6d65 203a  rors`.- Rename :
-00000590: 6d65 7468 3a60 7974 7062 2e70 6c61 7962  meth:`ytpb.playb
-000005a0: 6163 6b2e 506c 6179 6261 636b 2e67 6574  ack.Playback.get
-000005b0: 5f64 6f77 6e6c 6f61 6465 645f 7365 676d  _downloaded_segm
-000005c0: 656e 7460 2074 6f0a 2020 3a6d 6574 683a  ent` to.  :meth:
-000005d0: 607e 7974 7062 2e70 6c61 7962 6163 6b2e  `~ytpb.playback.
-000005e0: 506c 6179 6261 636b 2e67 6574 5f73 6567  Playback.get_seg
-000005f0: 6d65 6e74 600a 2d20 5265 6e61 6d65 203a  ment`.- Rename :
-00000600: 6d65 7468 3a60 7974 7062 2e72 6570 7265  meth:`ytpb.repre
-00000610: 7365 6e74 6174 696f 6e73 2e65 7874 7261  sentations.extra
-00000620: 6374 5f72 6570 7265 7365 6e74 6174 696f  ct_representatio
-00000630: 6e73 5f69 6e66 6f60 2074 6f0a 2020 3a6d  ns_info` to.  :m
-00000640: 6574 683a 607e 7974 7062 2e72 6570 7265  eth:`~ytpb.repre
-00000650: 7365 6e74 6174 696f 6e73 2e65 7874 7261  sentations.extra
-00000660: 6374 5f72 6570 7265 7365 6e74 6174 696f  ct_representatio
-00000670: 6e73 600a 2d20 5265 6d6f 7665 2075 6e75  ns`.- Remove unu
-00000680: 7365 6420 3a6d 6574 683a 6079 7470 622e  sed :meth:`ytpb.
-00000690: 7265 7072 6573 656e 7461 7469 6f6e 732e  representations.
-000006a0: 7374 7269 705f 6d61 6e69 6665 7374 600a  strip_manifest`.
-000006b0: 0a60 3230 3234 2e33 2e32 3760 5f0a 2a2a  .`2024.3.27`_.**
-000006c0: 2a2a 2a2a 2a2a 2a2a 2a2a 0a0a 2d20 4164  **********..- Ad
-000006d0: 6420 436f 6e74 6169 6e65 7266 696c 6520  d Containerfile 
-000006e0: 7769 7468 2069 6e73 7472 7563 7469 6f6e  with instruction
-000006f0: 7320 746f 2062 7569 6c64 2070 6174 6368  s to build patch
-00000700: 6564 2046 466d 7065 6720 616e 6420 4d50  ed FFmpeg and MP
-00000710: 560a 0a42 7265 616b 696e 6720 6368 616e  V..Breaking chan
-00000720: 6765 730a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ges.============
-00000730: 3d3d 3d3d 0a0a 2d20 4368 616e 6765 2072  ====..- Change r
-00000740: 6574 7572 6e20 7661 6c75 6520 6f66 0a20  eturn value of. 
-00000750: 203a 6d65 7468 3a60 7974 7062 2e6c 6f63   :meth:`ytpb.loc
-00000760: 6174 652e 5365 676d 656e 744c 6f63 6174  ate.SegmentLocat
-00000770: 6f72 2e66 696e 645f 7365 7175 656e 6365  or.find_sequence
-00000780: 5f62 795f 7469 6d65 6020 746f 0a20 203a  _by_time` to.  :
-00000790: 636c 6173 733a 607e 7974 7062 2e6c 6f63  class:`~ytpb.loc
-000007a0: 6174 652e 4c6f 6361 7465 5265 7375 6c74  ate.LocateResult
-000007b0: 600a 0a60 3230 3234 2e33 2e31 3660 5f0a  `..`2024.3.16`_.
-000007c0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 0a0a 2d20  ************..- 
-000007d0: 4164 6420 6f70 7469 6f6e 7320 746f 2064  Add options to d
-000007e0: 756d 7020 6261 7365 2028 6060 2d2d 6475  ump base (``--du
-000007f0: 6d70 2d62 6173 652d 7572 6c73 6060 2920  mp-base-urls``) 
-00000800: 616e 6420 7365 676d 656e 740a 2020 2860  and segment.  (`
-00000810: 602d 2d64 756d 702d 7365 676d 656e 742d  `--dump-segment-
-00000820: 7572 6c73 6060 2920 5552 4c73 2074 6f20  urls``) URLs to 
-00000830: 7468 6520 6060 646f 776e 6c6f 6164 6060  the ``download``
-00000840: 2063 6f6d 6d61 6e64 2028 6023 3130 0a20   command (`#10. 
-00000850: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
-00000860: 2e63 6f6d 2f78 796d 6178 696d 2f79 7470  .com/xymaxim/ytp
-00000870: 622f 7075 6c6c 2f31 303e 605f 5f29 0a2d  b/pull/10>`__).-
-00000880: 2041 6464 2074 6865 2060 436f 6f6b 626f   Add the `Cookbo
-00000890: 6f6b 605f 2064 6f63 756d 656e 7461 7469  ok`_ documentati
-000008a0: 6f6e 2070 6167 650a 0a2e 2e20 5f43 6f6f  on page.... _Coo
-000008b0: 6b62 6f6f 6b3a 2068 7474 7073 3a2f 2f79  kbook: https://y
-000008c0: 7470 622e 7265 6164 7468 6564 6f63 732e  tpb.readthedocs.
-000008d0: 696f 2f65 6e2f 6c61 7465 7374 2f63 6f6f  io/en/latest/coo
-000008e0: 6b62 6f6f 6b2e 6874 6d6c 0a0a 6032 3032  kbook.html..`202
-000008f0: 342e 332e 3133 605f 0a2a 2a2a 2a2a 2a2a  4.3.13`_.*******
-00000900: 2a2a 2a2a 2a0a 0a2d 2041 6464 2074 6865  *****..- Add the
-00000910: 2063 6f6e 6669 672e 746f 6d6c 2e65 7861   config.toml.exa
-00000920: 6d70 6c65 2066 696c 650a 2d20 4164 6420  mple file.- Add 
-00000930: 6162 696c 6974 7920 746f 2075 7365 2060  ability to use `
-00000940: 6375 7374 6f6d 2061 6c69 6173 6573 605f  custom aliases`_
-00000950: 2069 6e20 666f 726d 6174 2073 7065 6373   in format specs
-00000960: 0a2d 2041 6464 2060 616c 6961 7365 7360  .- Add `aliases`
-00000970: 5f20 666f 7220 6974 6167 7320 2860 6040  _ for itags (``@
-00000980: 3c69 7461 673e 6060 2920 6173 2060 6479  <itag>``) as `dy
-00000990: 6e61 6d69 6320 616c 6961 7365 7360 5f0a  namic aliases`_.
-000009a0: 2d20 4669 7820 616c 6c6f 7769 6e67 2065  - Fix allowing e
-000009b0: 6d70 7479 2072 6570 7265 7365 6e74 6174  mpty representat
-000009c0: 696f 6e73 2069 6e20 7468 6520 434c 4920  ions in the CLI 
-000009d0: 636f 6d6d 616e 6473 0a0a 2e2e 205f 6375  commands.... _cu
-000009e0: 7374 6f6d 2061 6c69 6173 6573 3a20 6874  stom aliases: ht
-000009f0: 7470 733a 2f2f 7974 7062 2e72 6561 6474  tps://ytpb.readt
-00000a00: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00000a10: 6573 742f 7265 6665 7265 6e63 652e 6874  est/reference.ht
-00000a20: 6d6c 2363 7573 746f 6d2d 616c 6961 7365  ml#custom-aliase
-00000a30: 730a 2e2e 205f 616c 6961 7365 733a 2068  s... _aliases: h
-00000a40: 7474 7073 3a2f 2f79 7470 622e 7265 6164  ttps://ytpb.read
-00000a50: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00000a60: 7465 7374 2f72 6566 6572 656e 6365 2e68  test/reference.h
-00000a70: 746d 6c23 6974 6167 730a 2e2e 205f 6479  tml#itags... _dy
-00000a80: 6e61 6d69 6320 616c 6961 7365 733a 2068  namic aliases: h
-00000a90: 7474 7073 3a2f 2f79 7470 622e 7265 6164  ttps://ytpb.read
-00000aa0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00000ab0: 7465 7374 2f72 6566 6572 656e 6365 2e68  test/reference.h
-00000ac0: 746d 6c23 616c 6961 7365 730a 0a60 3230  tml#aliases..`20
-00000ad0: 3234 2e33 2e39 605f 0a2a 2a2a 2a2a 2a2a  24.3.9`_.*******
-00000ae0: 2a2a 2a2a 0a0a 2d20 4164 6420 7468 6520  ****..- Add the 
-00000af0: 4348 414e 4745 4c4f 4720 6669 6c65 2061  CHANGELOG file a
-00000b00: 6e64 2064 6f63 756d 656e 7461 7469 6f6e  nd documentation
-00000b10: 2070 6167 650a 2d20 4368 616e 6765 2074   page.- Change t
-00000b20: 6865 2066 6972 7374 2073 6567 6d65 6e74  he first segment
-00000b30: 206c 6f63 6174 696e 6720 7374 6570 3a20   locating step: 
-00000b40: 646f 6e27 7420 6c69 6d69 7420 6974 2074  don't limit it t
-00000b50: 6f20 7477 6f20 6a75 6d70 7320 2860 2338  o two jumps (`#8
-00000b60: 0a20 203c 6874 7470 733a 2f2f 6769 7468  .  <https://gith
-00000b70: 7562 2e63 6f6d 2f78 796d 6178 696d 2f79  ub.com/xymaxim/y
-00000b80: 7470 622f 7075 6c6c 2f38 3e60 5f5f 290a  tpb/pull/8>`__).
-00000b90: 0a2e 2e20 5f32 3032 342e 342e 3230 3a20  ... _2024.4.20: 
-00000ba0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000bb0: 6f6d 2f78 796d 6178 696d 2f79 7470 622f  om/xymaxim/ytpb/
-00000bc0: 636f 6d70 6172 652f 7632 3032 342e 342e  compare/v2024.4.
-00000bd0: 3132 2e2e 7632 3032 342e 342e 3230 2020  12..v2024.4.20  
-00000be0: 0a2e 2e20 5f32 3032 342e 342e 3132 3a20  ... _2024.4.12: 
-00000bf0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000c00: 6f6d 2f78 796d 6178 696d 2f79 7470 622f  om/xymaxim/ytpb/
-00000c10: 636f 6d70 6172 652f 7632 3032 342e 332e  compare/v2024.3.
-00000c20: 3237 2e2e 7632 3032 342e 342e 3132 0a2e  27..v2024.4.12..
-00000c30: 2e20 5f32 3032 342e 332e 3237 3a20 6874  . _2024.3.27: ht
-00000c40: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000c50: 2f78 796d 6178 696d 2f79 7470 622f 636f  /xymaxim/ytpb/co
-00000c60: 6d70 6172 652f 7632 3032 342e 332e 3136  mpare/v2024.3.16
-00000c70: 2e2e 7632 3032 342e 332e 3237 0a2e 2e20  ..v2024.3.27... 
-00000c80: 5f32 3032 342e 332e 3136 3a20 6874 7470  _2024.3.16: http
-00000c90: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f78  s://github.com/x
-00000ca0: 796d 6178 696d 2f79 7470 622f 636f 6d70  ymaxim/ytpb/comp
-00000cb0: 6172 652f 7632 3032 342e 332e 3133 2e2e  are/v2024.3.13..
-00000cc0: 7632 3032 342e 332e 3136 0a2e 2e20 5f32  v2024.3.16... _2
-00000cd0: 3032 342e 332e 3133 3a20 6874 7470 733a  024.3.13: https:
-00000ce0: 2f2f 6769 7468 7562 2e63 6f6d 2f78 796d  //github.com/xym
-00000cf0: 6178 696d 2f79 7470 622f 636f 6d70 6172  axim/ytpb/compar
-00000d00: 652f 7632 3032 342e 332e 392e 2e76 3230  e/v2024.3.9..v20
-00000d10: 3234 2e33 2e31 330a 2e2e 205f 3230 3234  24.3.13... _2024
-00000d20: 2e33 2e39 3a20 6874 7470 733a 2f2f 6769  .3.9: https://gi
-00000d30: 7468 7562 2e63 6f6d 2f78 796d 6178 696d  thub.com/xymaxim
-00000d40: 2f79 7470 622f 636f 6d70 6172 652f 7632  /ytpb/compare/v2
-00000d50: 3032 342e 332e 372e 2e76 3230 3234 2e33  024.3.7..v2024.3
-00000d60: 2e39 0a                                  .9.
+00000080: 6572 2e6f 7267 0a0a 6032 3032 342e 352e  er.org..`2024.5.
+00000090: 3360 5f0a 2a2a 2a2a 2a2a 2a2a 2a2a 2a0a  3`_.***********.
+000000a0: 0a2d 2041 6464 2073 7570 706f 7274 2066  .- Add support f
+000000b0: 6f72 2072 6573 756d 6162 6c65 2064 6f77  or resumable dow
+000000c0: 6e6c 6f61 6473 2028 6023 3133 0a20 203c  nloads (`#13.  <
+000000d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000000e0: 6f6d 2f78 796d 6178 696d 2f79 7470 622f  om/xymaxim/ytpb/
+000000f0: 7075 6c6c 2f31 333e 605f 5f29 0a2d 2043  pull/13>`__).- C
+00000100: 6861 6e67 6520 7468 6520 7365 676d 656e  hange the segmen
+00000110: 7473 206f 7574 7075 7420 6469 7265 6374  ts output direct
+00000120: 6f72 7920 6672 6f6d 2074 6865 2072 756e  ory from the run
+00000130: 2074 656d 706f 7261 7279 2064 6972 6563   temporary direc
+00000140: 746f 7279 2074 6f20 610a 2020 6469 7265  tory to a.  dire
+00000150: 6374 6f72 7920 756e 6465 7220 7468 6520  ctory under the 
+00000160: 6375 7272 656e 7420 776f 726b 696e 6720  current working 
+00000170: 6f6e 650a 2d20 4164 6420 6060 2d2d 6967  one.- Add ``--ig
+00000180: 6e6f 7265 2d72 6573 756d 6560 602c 2060  nore-resume``, `
+00000190: 602d 5320 2f20 2d2d 6b65 6570 2d73 6567  `-S / --keep-seg
+000001a0: 6d65 6e74 7360 602c 2061 6e64 0a20 2060  ments``, and.  `
+000001b0: 602d 2d73 6567 6d65 6e74 732d 6f75 7470  `--segments-outp
+000001c0: 7574 2d64 6972 6060 206f 7074 696f 6e73  ut-dir`` options
+000001d0: 0a2d 2043 6861 6e67 6520 7468 6520 6465  .- Change the de
+000001e0: 6661 756c 7420 6f75 7470 7574 2070 6174  fault output pat
+000001f0: 6820 746f 2060 603c 7469 746c 653e 5f3c  h to ``<title>_<
+00000200: 6964 3e5f 3c69 6e70 7574 5f73 7461 7274  id>_<input_start
+00000210: 5f64 6174 653e 6060 0a2d 2052 656e 616d  _date>``.- Renam
+00000220: 6520 7468 6520 6060 2d2d 6e6f 2d63 6c65  e the ``--no-cle
+00000230: 616e 7570 6060 206f 7074 696f 6e20 746f  anup`` option to
+00000240: 2060 602d 2d6b 6565 702d 7465 6d70 6060   ``--keep-temp``
+00000250: 0a2d 2052 6570 6c61 6365 2074 6865 2060  .- Replace the `
+00000260: 602d 2d70 7265 7669 6577 6060 206f 7074  `--preview`` opt
+00000270: 696f 6e20 7769 7468 2060 602d 2d70 7265  ion with ``--pre
+00000280: 7669 6577 2d73 7461 7274 6060 2061 6e64  view-start`` and
+00000290: 0a20 2060 602d 2d70 7265 7669 6577 2d65  .  ``--preview-e
+000002a0: 6e64 6060 0a0a 6032 3032 342e 342e 3230  nd``..`2024.4.20
+000002b0: 605f 0a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a0a  `_.************.
+000002c0: 0a2d 2046 6978 2077 726f 6e67 2066 7261  .- Fix wrong fra
+000002d0: 6d65 2072 6174 6520 7661 6c75 6573 206f  me rate values o
+000002e0: 6620 7468 6520 7669 6465 6f2d 6f6e 6c79  f the video-only
+000002f0: 206d 6572 6765 6420 6669 6c65 7320 7768   merged files wh
+00000300: 656e 2062 6f75 6e64 6172 790a 2020 7365  en boundary.  se
+00000310: 676d 656e 7473 2061 7265 2063 7574 2061  gments are cut a
+00000320: 6e64 2065 6e63 6f64 6564 2077 6974 6820  nd encoded with 
+00000330: 482e 3236 3420 2860 6531 3132 3062 660a  H.264 (`e1120bf.
+00000340: 2020 3c68 7474 7073 3a2f 2f67 6974 6875    <https://githu
+00000350: 622e 636f 6d2f 7879 6d61 7869 6d2f 7974  b.com/xymaxim/yt
+00000360: 7062 2f63 6f6d 6d69 742f 6531 3132 3062  pb/commit/e1120b
+00000370: 6634 3531 3433 3333 6666 3361 6335 6434  f4514333ff3ac5d4
+00000380: 6561 6338 3632 6363 6236 6139 6435 6636  eac862ccb6a9d5f6
+00000390: 3036 3e60 5f5f 290a 2d20 5772 6974 6520  06>`__).- Write 
+000003a0: 6d65 7461 6461 7461 2074 6167 7320 7769  metadata tags wi
+000003b0: 7468 2062 6173 6963 2061 6e64 2072 6577  th basic and rew
+000003c0: 696e 6420 696e 666f 726d 6174 696f 6e20  ind information 
+000003d0: 746f 206d 6572 6765 6420 6669 6c65 7320  to merged files 
+000003e0: 2860 6161 3761 6466 310a 2020 3c68 7474  (`aa7adf1.  <htt
+000003f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000400: 7879 6d61 7869 6d2f 7974 7062 2f63 6f6d  xymaxim/ytpb/com
+00000410: 6d69 742f 6161 3761 6466 3135 3830 6535  mit/aa7adf1580e5
+00000420: 6138 3363 3961 6261 6137 3666 3238 3336  a83c9abaa76f2836
+00000430: 6239 6130 3537 3063 6334 6261 3e60 5f5f  b9a0570cc4ba>`__
+00000440: 290a 2d20 4164 6420 7468 6520 6060 2d2d  ).- Add the ``--
+00000450: 6e6f 2d6d 6574 6164 6174 6160 6020 6f70  no-metadata`` op
+00000460: 7469 6f6e 2074 6f20 6e6f 7420 7772 6974  tion to not writ
+00000470: 6520 6d65 7461 6461 7461 2074 6167 7320  e metadata tags 
+00000480: 746f 206d 6572 6765 6420 6669 6c65 730a  to merged files.
+00000490: 0a60 3230 3234 2e34 2e31 3260 5f0a 2a2a  .`2024.4.12`_.**
+000004a0: 2a2a 2a2a 2a2a 2a2a 2a2a 0a0a 2d20 4164  **********..- Ad
+000004b0: 6420 7468 6520 6050 7974 686f 6e20 7061  d the `Python pa
+000004c0: 636b 6167 650a 2020 3c68 7474 7073 3a2f  ckage.  <https:/
+000004d0: 2f79 7470 622e 7265 6164 7468 6564 6f63  /ytpb.readthedoc
+000004e0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f70  s.io/en/latest/p
+000004f0: 6163 6b61 6765 2f69 6e64 6578 2e68 746d  ackage/index.htm
+00000500: 6c3e 605f 5f20 7061 6765 2077 6974 6820  l>`__ page with 
+00000510: 7468 650a 2020 6261 7369 6320 7573 6167  the.  basic usag
+00000520: 6520 616e 6420 4150 4920 7265 6665 7265  e and API refere
+00000530: 6e63 650a 2d20 4164 6420 7468 6520 6060  nce.- Add the ``
+00000540: 2d2d 7665 7273 696f 6e60 6020 434c 4920  --version`` CLI 
+00000550: 6f70 7469 6f6e 2074 6f20 7368 6f77 2076  option to show v
+00000560: 6572 7369 6f6e 206e 756d 6265 720a 2d20  ersion number.- 
+00000570: 4164 6420 3a61 7474 723a 6079 7470 622e  Add :attr:`ytpb.
+00000580: 7265 7072 6573 656e 7461 7469 6f6e 732e  representations.
+00000590: 5265 7072 6573 656e 7461 7469 6f6e 496e  RepresentationIn
+000005a0: 666f 2e74 7970 6560 2070 726f 7065 7274  fo.type` propert
+000005b0: 790a 2d20 4164 6420 3a61 7474 723a 6079  y.- Add :attr:`y
+000005c0: 7470 622e 706c 6179 6261 636b 2e52 6577  tpb.playback.Rew
+000005d0: 696e 6449 6e74 6572 7661 6c2e 6475 7261  indInterval.dura
+000005e0: 7469 6f6e 6020 616e 640a 2020 3a61 7474  tion` and.  :att
+000005f0: 723a 607e 7974 7062 2e70 6c61 7962 6163  r:`~ytpb.playbac
+00000600: 6b2e 5265 7769 6e64 496e 7465 7276 616c  k.RewindInterval
+00000610: 2e73 6571 7565 6e63 6573 6020 7072 6f70  .sequences` prop
+00000620: 6572 7469 6573 0a2d 2041 6363 6570 7420  erties.- Accept 
+00000630: 556e 6978 2074 696d 6573 7461 6d70 7320  Unix timestamps 
+00000640: 666f 7220 6d6f 6d65 6e74 7320 616e 6420  for moments and 
+00000650: 696e 7465 7276 616c 7320 2860 6237 6463  intervals (`b7dc
+00000660: 6261 660a 2020 3c68 7474 7073 3a2f 2f67  baf.  <https://g
+00000670: 6974 6875 622e 636f 6d2f 7879 6d61 7869  ithub.com/xymaxi
+00000680: 6d2f 7974 7062 2f63 6f6d 6d69 742f 6237  m/ytpb/commit/b7
+00000690: 6463 6261 6636 6565 6265 3366 3630 3232  dcbaf6eebe3f6022
+000006a0: 6237 6661 3865 6566 6539 3866 3462 3861  b7fa8eefe98f4b8a
+000006b0: 6637 6334 6362 3e60 5f5f 290a 2d20 4164  f7c4cb>`__).- Ad
+000006c0: 6420 3a63 6c61 7373 3a60 7974 7062 2e70  d :class:`ytpb.p
+000006d0: 6c61 7962 6163 6b2e 5265 7769 6e64 5472  layback.RewindTr
+000006e0: 6565 4d61 7060 2074 6f20 6b65 6570 2072  eeMap` to keep r
+000006f0: 6577 696e 6420 6869 7374 6f72 7920 2860  ewind history (`
+00000700: 3931 6664 3037 380a 2020 3c68 7474 7073  91fd078.  <https
+00000710: 3a2f 2f67 6974 6875 622e 636f 6d2f 7879  ://github.com/xy
+00000720: 6d61 7869 6d2f 7974 7062 2f63 6f6d 6d69  maxim/ytpb/commi
+00000730: 742f 3931 6664 3037 3863 6166 3337 6633  t/91fd078caf37f3
+00000740: 3166 6565 3136 3765 3063 3261 3230 6133  1fee167e0c2a20a3
+00000750: 3861 6132 6261 6463 6438 3e60 5f5f 290a  8aa2badcd8>`__).
+00000760: 0a42 7265 616b 696e 6720 6368 616e 6765  .Breaking change
+00000770: 730a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  s.==============
+00000780: 3d3d 0a0a 2d20 5265 6e61 6d65 203a 6d6f  ==..- Rename :mo
+00000790: 643a 6079 7470 622e 6d70 6460 2074 6f20  d:`ytpb.mpd` to 
+000007a0: 3a6d 6f64 3a60 7974 7062 2e72 6570 7265  :mod:`ytpb.repre
+000007b0: 7365 6e74 6174 696f 6e73 600a 2d20 5265  sentations`.- Re
+000007c0: 6e61 6d65 203a 6d6f 643a 6079 7470 622e  name :mod:`ytpb.
+000007d0: 6578 6365 7074 696f 6e73 6020 746f 203a  exceptions` to :
+000007e0: 6d6f 643a 6079 7470 622e 6572 726f 7273  mod:`ytpb.errors
+000007f0: 600a 2d20 5265 6e61 6d65 203a 6d65 7468  `.- Rename :meth
+00000800: 3a60 7974 7062 2e70 6c61 7962 6163 6b2e  :`ytpb.playback.
+00000810: 506c 6179 6261 636b 2e67 6574 5f64 6f77  Playback.get_dow
+00000820: 6e6c 6f61 6465 645f 7365 676d 656e 7460  nloaded_segment`
+00000830: 2074 6f0a 2020 3a6d 6574 683a 607e 7974   to.  :meth:`~yt
+00000840: 7062 2e70 6c61 7962 6163 6b2e 506c 6179  pb.playback.Play
+00000850: 6261 636b 2e67 6574 5f73 6567 6d65 6e74  back.get_segment
+00000860: 600a 2d20 5265 6e61 6d65 203a 6d65 7468  `.- Rename :meth
+00000870: 3a60 7974 7062 2e72 6570 7265 7365 6e74  :`ytpb.represent
+00000880: 6174 696f 6e73 2e65 7874 7261 6374 5f72  ations.extract_r
+00000890: 6570 7265 7365 6e74 6174 696f 6e73 5f69  epresentations_i
+000008a0: 6e66 6f60 2074 6f0a 2020 3a6d 6574 683a  nfo` to.  :meth:
+000008b0: 607e 7974 7062 2e72 6570 7265 7365 6e74  `~ytpb.represent
+000008c0: 6174 696f 6e73 2e65 7874 7261 6374 5f72  ations.extract_r
+000008d0: 6570 7265 7365 6e74 6174 696f 6e73 600a  epresentations`.
+000008e0: 2d20 5265 6d6f 7665 2075 6e75 7365 6420  - Remove unused 
+000008f0: 3a6d 6574 683a 6079 7470 622e 7265 7072  :meth:`ytpb.repr
+00000900: 6573 656e 7461 7469 6f6e 732e 7374 7269  esentations.stri
+00000910: 705f 6d61 6e69 6665 7374 600a 0a60 3230  p_manifest`..`20
+00000920: 3234 2e33 2e32 3760 5f0a 2a2a 2a2a 2a2a  24.3.27`_.******
+00000930: 2a2a 2a2a 2a2a 0a0a 2d20 4164 6420 436f  ******..- Add Co
+00000940: 6e74 6169 6e65 7266 696c 6520 7769 7468  ntainerfile with
+00000950: 2069 6e73 7472 7563 7469 6f6e 7320 746f   instructions to
+00000960: 2062 7569 6c64 2070 6174 6368 6564 2046   build patched F
+00000970: 466d 7065 6720 616e 6420 4d50 560a 0a42  Fmpeg and MPV..B
+00000980: 7265 616b 696e 6720 6368 616e 6765 730a  reaking changes.
+00000990: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000009a0: 0a0a 2d20 4368 616e 6765 2072 6574 7572  ..- Change retur
+000009b0: 6e20 7661 6c75 6520 6f66 0a20 203a 6d65  n value of.  :me
+000009c0: 7468 3a60 7974 7062 2e6c 6f63 6174 652e  th:`ytpb.locate.
+000009d0: 5365 676d 656e 744c 6f63 6174 6f72 2e66  SegmentLocator.f
+000009e0: 696e 645f 7365 7175 656e 6365 5f62 795f  ind_sequence_by_
+000009f0: 7469 6d65 6020 746f 0a20 203a 636c 6173  time` to.  :clas
+00000a00: 733a 607e 7974 7062 2e6c 6f63 6174 652e  s:`~ytpb.locate.
+00000a10: 4c6f 6361 7465 5265 7375 6c74 600a 0a60  LocateResult`..`
+00000a20: 3230 3234 2e33 2e31 3660 5f0a 2a2a 2a2a  2024.3.16`_.****
+00000a30: 2a2a 2a2a 2a2a 2a2a 0a0a 2d20 4164 6420  ********..- Add 
+00000a40: 6f70 7469 6f6e 7320 746f 2064 756d 7020  options to dump 
+00000a50: 6261 7365 2028 6060 2d2d 6475 6d70 2d62  base (``--dump-b
+00000a60: 6173 652d 7572 6c73 6060 2920 616e 6420  ase-urls``) and 
+00000a70: 7365 676d 656e 740a 2020 2860 602d 2d64  segment.  (``--d
+00000a80: 756d 702d 7365 676d 656e 742d 7572 6c73  ump-segment-urls
+00000a90: 6060 2920 5552 4c73 2074 6f20 7468 6520  ``) URLs to the 
+00000aa0: 6060 646f 776e 6c6f 6164 6060 2063 6f6d  ``download`` com
+00000ab0: 6d61 6e64 2028 6023 3130 0a20 203c 6874  mand (`#10.  <ht
+00000ac0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000ad0: 2f78 796d 6178 696d 2f79 7470 622f 7075  /xymaxim/ytpb/pu
+00000ae0: 6c6c 2f31 303e 605f 5f29 0a2d 2041 6464  ll/10>`__).- Add
+00000af0: 2074 6865 2060 436f 6f6b 626f 6f6b 605f   the `Cookbook`_
+00000b00: 2064 6f63 756d 656e 7461 7469 6f6e 2070   documentation p
+00000b10: 6167 650a 0a2e 2e20 5f43 6f6f 6b62 6f6f  age.... _Cookboo
+00000b20: 6b3a 2068 7474 7073 3a2f 2f79 7470 622e  k: https://ytpb.
+00000b30: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+00000b40: 6e2f 6c61 7465 7374 2f63 6f6f 6b62 6f6f  n/latest/cookboo
+00000b50: 6b2e 6874 6d6c 0a0a 6032 3032 342e 332e  k.html..`2024.3.
+00000b60: 3133 605f 0a2a 2a2a 2a2a 2a2a 2a2a 2a2a  13`_.***********
+00000b70: 2a0a 0a2d 2041 6464 2074 6865 2063 6f6e  *..- Add the con
+00000b80: 6669 672e 746f 6d6c 2e65 7861 6d70 6c65  fig.toml.example
+00000b90: 2066 696c 650a 2d20 4164 6420 6162 696c   file.- Add abil
+00000ba0: 6974 7920 746f 2075 7365 2060 6375 7374  ity to use `cust
+00000bb0: 6f6d 2061 6c69 6173 6573 605f 2069 6e20  om aliases`_ in 
+00000bc0: 666f 726d 6174 2073 7065 6373 0a2d 2041  format specs.- A
+00000bd0: 6464 2060 616c 6961 7365 7360 5f20 666f  dd `aliases`_ fo
+00000be0: 7220 6974 6167 7320 2860 6040 3c69 7461  r itags (``@<ita
+00000bf0: 673e 6060 2920 6173 2060 6479 6e61 6d69  g>``) as `dynami
+00000c00: 6320 616c 6961 7365 7360 5f0a 2d20 4669  c aliases`_.- Fi
+00000c10: 7820 616c 6c6f 7769 6e67 2065 6d70 7479  x allowing empty
+00000c20: 2072 6570 7265 7365 6e74 6174 696f 6e73   representations
+00000c30: 2069 6e20 7468 6520 434c 4920 636f 6d6d   in the CLI comm
+00000c40: 616e 6473 0a0a 2e2e 205f 6375 7374 6f6d  ands.... _custom
+00000c50: 2061 6c69 6173 6573 3a20 6874 7470 733a   aliases: https:
+00000c60: 2f2f 7974 7062 2e72 6561 6474 6865 646f  //ytpb.readthedo
+00000c70: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00000c80: 7265 6665 7265 6e63 652e 6874 6d6c 2363  reference.html#c
+00000c90: 7573 746f 6d2d 616c 6961 7365 730a 2e2e  ustom-aliases...
+00000ca0: 205f 616c 6961 7365 733a 2068 7474 7073   _aliases: https
+00000cb0: 3a2f 2f79 7470 622e 7265 6164 7468 6564  ://ytpb.readthed
+00000cc0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00000cd0: 2f72 6566 6572 656e 6365 2e68 746d 6c23  /reference.html#
+00000ce0: 6974 6167 730a 2e2e 205f 6479 6e61 6d69  itags... _dynami
+00000cf0: 6320 616c 6961 7365 733a 2068 7474 7073  c aliases: https
+00000d00: 3a2f 2f79 7470 622e 7265 6164 7468 6564  ://ytpb.readthed
+00000d10: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00000d20: 2f72 6566 6572 656e 6365 2e68 746d 6c23  /reference.html#
+00000d30: 616c 6961 7365 730a 0a60 3230 3234 2e33  aliases..`2024.3
+00000d40: 2e39 605f 0a2a 2a2a 2a2a 2a2a 2a2a 2a2a  .9`_.***********
+00000d50: 0a0a 2d20 4164 6420 7468 6520 4348 414e  ..- Add the CHAN
+00000d60: 4745 4c4f 4720 6669 6c65 2061 6e64 2064  GELOG file and d
+00000d70: 6f63 756d 656e 7461 7469 6f6e 2070 6167  ocumentation pag
+00000d80: 650a 2d20 4368 616e 6765 2074 6865 2066  e.- Change the f
+00000d90: 6972 7374 2073 6567 6d65 6e74 206c 6f63  irst segment loc
+00000da0: 6174 696e 6720 7374 6570 3a20 646f 6e27  ating step: don'
+00000db0: 7420 6c69 6d69 7420 6974 2074 6f20 7477  t limit it to tw
+00000dc0: 6f20 6a75 6d70 7320 2860 2338 0a20 203c  o jumps (`#8.  <
+00000dd0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000de0: 6f6d 2f78 796d 6178 696d 2f79 7470 622f  om/xymaxim/ytpb/
+00000df0: 7075 6c6c 2f38 3e60 5f5f 290a 0a2e 2e20  pull/8>`__).... 
+00000e00: 5f32 3032 342e 352e 333a 2068 7474 7073  _2024.5.3: https
+00000e10: 3a2f 2f67 6974 6875 622e 636f 6d2f 7879  ://github.com/xy
+00000e20: 6d61 7869 6d2f 7974 7062 2f63 6f6d 7061  maxim/ytpb/compa
+00000e30: 7265 2f76 3230 3234 2e34 2e32 302e 2e76  re/v2024.4.20..v
+00000e40: 3230 3234 2e35 2e33 0a2e 2e20 5f32 3032  2024.5.3... _202
+00000e50: 342e 342e 3230 3a20 6874 7470 733a 2f2f  4.4.20: https://
+00000e60: 6769 7468 7562 2e63 6f6d 2f78 796d 6178  github.com/xymax
+00000e70: 696d 2f79 7470 622f 636f 6d70 6172 652f  im/ytpb/compare/
+00000e80: 7632 3032 342e 342e 3132 2e2e 7632 3032  v2024.4.12..v202
+00000e90: 342e 342e 3230 0a2e 2e20 5f32 3032 342e  4.4.20... _2024.
+00000ea0: 342e 3132 3a20 6874 7470 733a 2f2f 6769  4.12: https://gi
+00000eb0: 7468 7562 2e63 6f6d 2f78 796d 6178 696d  thub.com/xymaxim
+00000ec0: 2f79 7470 622f 636f 6d70 6172 652f 7632  /ytpb/compare/v2
+00000ed0: 3032 342e 332e 3237 2e2e 7632 3032 342e  024.3.27..v2024.
+00000ee0: 342e 3132 0a2e 2e20 5f32 3032 342e 332e  4.12... _2024.3.
+00000ef0: 3237 3a20 6874 7470 733a 2f2f 6769 7468  27: https://gith
+00000f00: 7562 2e63 6f6d 2f78 796d 6178 696d 2f79  ub.com/xymaxim/y
+00000f10: 7470 622f 636f 6d70 6172 652f 7632 3032  tpb/compare/v202
+00000f20: 342e 332e 3136 2e2e 7632 3032 342e 332e  4.3.16..v2024.3.
+00000f30: 3237 0a2e 2e20 5f32 3032 342e 332e 3136  27... _2024.3.16
+00000f40: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00000f50: 2e63 6f6d 2f78 796d 6178 696d 2f79 7470  .com/xymaxim/ytp
+00000f60: 622f 636f 6d70 6172 652f 7632 3032 342e  b/compare/v2024.
+00000f70: 332e 3133 2e2e 7632 3032 342e 332e 3136  3.13..v2024.3.16
+00000f80: 0a2e 2e20 5f32 3032 342e 332e 3133 3a20  ... _2024.3.13: 
+00000f90: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000fa0: 6f6d 2f78 796d 6178 696d 2f79 7470 622f  om/xymaxim/ytpb/
+00000fb0: 636f 6d70 6172 652f 7632 3032 342e 332e  compare/v2024.3.
+00000fc0: 392e 2e76 3230 3234 2e33 2e31 330a 2e2e  9..v2024.3.13...
+00000fd0: 205f 3230 3234 2e33 2e39 3a20 6874 7470   _2024.3.9: http
+00000fe0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f78  s://github.com/x
+00000ff0: 796d 6178 696d 2f79 7470 622f 636f 6d70  ymaxim/ytpb/comp
+00001000: 6172 652f 7632 3032 342e 332e 372e 2e76  are/v2024.3.7..v
+00001010: 3230 3234 2e33 2e39 0a                   2024.3.9.
```

### Comparing `ytpb-2024.4.20/CONTRIBUTING.rst` & `ytpb-2024.5.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/config.toml.example` & `ytpb-2024.5.3/config.toml.example`

 * *Files 8% similar despite different names*

```diff
@@ -13,33 +13,34 @@
 # command or sub-command. See help of a command for all options. Note that
 # values provided here can be overriden by the corresponding CLI option.
 [options]
 
 [options.download]
 audio_format = "itag eq 140"
 video_format = "best(@mp4 and <=1080p and @30fps)"
-output_path = "<title>_<input_start_date>"
+output_path = "<title>_<id>_<input_start_date>"
 
 [options.capture.frame]
 video_format = "best(@mp4 and @30fps)"
-output_path = "<title>_<moment_date>.jpg"
+output_path = "<title>_<id>_<moment_date>.jpg"
 
 [options.capture.timelapse]
 video_format = "best(@mp4 and @30fps)"
-output_path = "<title>/<input_start_date>/<every>/<title>_<input_start_date>_<every>_%04d.jpg"
+output_path = "<title>_<id>/<input_start_date>/<every>/<title>_<id>_<input_start_date>_<every>_%04d.jpg"
 
 [options.mpd.compose]
 audio_formats = "itag eq 140"
 video_formats = "@webm and [@720p or @1080p] and @30fps"
-output_path = "<title>_<input_start_date>.mpd"
+output_path = "<title>_<id>_<input_start_date>.mpd"
 
 # General settings.
 [general]
 
-# Preview duration for the --preview option (in seconds).
+# Preview duration for the preview start (--preview-start) and end
+# (--preview-end) modes (in seconds).
 preview_duration = 10
 # The User-Agent header.
 user_agent = "Mozilla/5.0 (Android 14; Mobile; rv:68.0) Gecko/68.0 Firefox/120.0"
 
 # Custom aliases used in format specs. See
 # https://ytpb.readthedocs.io/en/latest/reference.html#format-spec.
 [general.aliases]
```

#### html2text {}

```diff
@@ -5,25 +5,26 @@
 content) of this file to # $XDG_CONFIG_HOME/ytpb/config.toml. # # See https://
 ytpb.readthedocs.io/en/latest/cli.html#configuring for more # information on
 configuring. # Default values for the CLI options. Each section corresponds to
 its own # command or sub-command. See help of a command for all options. Note
 that # values provided here can be overriden by the corresponding CLI option.
 [options] [options.download] audio_format = "itag eq 140" video_format = "best
 (@mp4 and <=1080p and @30fps)" output_path = "
-" [options.capture.frame] video_format = "best(@mp4 and @30fps)" output_path =
+_" [options.capture.frame] video_format = "best(@mp4 and @30fps)" output_path =
 "
-.jpg" [options.capture.timelapse] video_format = "best(@mp4 and @30fps)"
+_.jpg" [options.capture.timelapse] video_format = "best(@mp4 and @30fps)"
 output_path = "
-//
-__%04d.jpg" [options.mpd.compose] audio_formats = "itag eq 140" video_formats =
-"@webm and [@720p or @1080p] and @30fps" output_path = "
-.mpd" # General settings. [general] # Preview duration for the --preview option
-(in seconds). preview_duration = 10 # The User-Agent header. user_agent =
-"Mozilla/5.0 (Android 14; Mobile; rv:68.0) Gecko/68.0 Firefox/120.0" # Custom
-aliases used in format specs. See # https://ytpb.readthedocs.io/en/latest/
+///
+___%04d.jpg" [options.mpd.compose] audio_formats = "itag eq 140" video_formats
+= "@webm and [@720p or @1080p] and @30fps" output_path = "
+_.mpd" # General settings. [general] # Preview duration for the preview start
+(--preview-start) and end # (--preview-end) modes (in seconds).
+preview_duration = 10 # The User-Agent header. user_agent = "Mozilla/5.0
+(Android 14; Mobile; rv:68.0) Gecko/68.0 Firefox/120.0" # Custom aliases used
+in format specs. See # https://ytpb.readthedocs.io/en/latest/
 reference.html#format-spec. [general.aliases] custom-alias = "[@720p or @1080p]
 and @webm" another-alias = "@custom-alias and @30fps" # Output settings.
 [output] # Output date formatting settings. See # https://ytpb.readthedocs.io/
 en/latest/cli.html#formatting-dates. [output.date] # Set of styles that refer
 to ISO 8601-related formatting. Available styles that # can be combined:
 'basic' or 'extended', 'complete' or 'reduced', 'hh' or # 'hhmm', 'z'. styles =
 "basic,complete,hh" # Output title formatting settings. See # https://
```

### Comparing `ytpb-2024.4.20/docs/cli.rst` & `ytpb-2024.5.3/docs/cli.rst`

 * *Files 3% similar despite different names*

```diff
@@ -233,29 +233,32 @@
   $ ytpb download -i PT30S/2024-01-02T10:20:30+00 ...
 
 .. _Preview mode:
 
 C. Preview mode
 ---------------
 
-* ``--interval <start>/.. --preview``
-* ``--interval <start>/<end> --preview``
+* ``--interval <start>/<end> --preview-start``
+* ``--interval <start>/<end> --preview-end``
+* ``--interval <start>/.. --preview-start``
+* ``--interval ../<end> --preview-end``
 
 If you only need to preview a moment in a stream, which you can refer to later,
-the ``-p/--preview`` option exists. It's basically an alias for the short end
-duration.
+the ``-ps / --preview-start`` and ``-pe / --preview-end`` options exist. It's
+basically an alias for the short end duration.
 
-In the above, the closed intervals were used, while for the preview mode, you
+In the above, the closed intervals were used, while for the preview modes, you
 can define (not necessarily, though) intervals with an open end designated with
-the ".." literal: ::
+the '..' literal: ::
 
-  $ ytpb download -i 2024-01-02T10:20:00+00/.. -p ...
+  $ ytpb download -i 2024-01-02T10:20:00+00/.. -ps ...
+  $ ytpb download -i ../2024-01-02T10:20:00+00 -pe ...
 
-(In case of a closed interval, an end part will be ignored, and you'll see a
-note in the output that the preview mode is enabled.)
+(In case of a closed interval, the start or end part will be ignored, and you'll
+see a note in the output that the preview mode is enabled.)
 
 By default, the output preview duration varies from 10 to 10 + one segment
 duration seconds. The imprecision is due to the reliance on the full-length,
 uncut end segment (to reduce merging time). The minimal preview duration value
 can be changed via the ``general.preview_duration`` field in the ``config.toml``
 file.
 
@@ -360,18 +363,18 @@
   $ ytpb download -vf 'best(@mp4 and @30fps)' ...
 
 .. _Default format values:
 
 Default values
 --------------
 
-The format specs can be provided using the following ways (in order of increasing
-priority): (a) using the default, built-in option values, (b) parsing
-custom, user-defined configuration file, e.g. ``~/.config/ytpb/config.toml``,
-and (c) via ``-af/--audio-format(s)`` and ``-vf/--video-format(s)`` options.
+The format specs can be provided using the following ways (in order of
+increasing priority): (a) using the default, built-in option values, (b) parsing
+custom, user-defined :ref:`configuration <Configuring>` file, ``config.toml``, and (c) via ``-af/--audio-format(s)`` and
+``-vf/--video-format(s)`` options.
 
 The default option values are as follows:
 
 .. code:: TOML
 
 	  [options.download]
 	  audio_format = "@140"
@@ -383,26 +386,30 @@
           [options.capture.timelapse]
 	  video_format = "best(@mp4 and @30fps)"
 
 	  [options.mpd.compose]
 	  audio_formats = "@140"
 	  video_formats = "@webm and [@720p or @1080p] and @30fps"
 
-See `Configuring`_ for more information on configuring.
-
 Specifying output name
 ======================
 
-There are two options to change the default output naming: (a) specify a full output
-path or (b) provide a template output path (both without extension). The extension
-will be automatically determined during the merging stage. ::
-
-  $ ytpb download -o '<title>_<input_start_date>_<duration>' ...
-  $ ls
-  $ Stream-Title_20240102T102000+00_PT30S.mp4
+There are two options to change the output naming: (a) specify a full output
+path, (b) provide a template output path (both without extension). The extension
+will be automatically determined during the merging step.
+
+Specify values directly via the ``-o / --output`` option::
+
+  $ ytpb download -o '<title>_<input_start_date>' ... && ls
+  $ Stream-Title_20240102T102000+00.mp4
+
+Or set default option values in the ``config.toml`` file::
+
+  [options.download]
+  output = <title>_<input_start_date>
 
 See :ref:`reference:Output name context` for the available template variables.
 
 Formatting titles
 -----------------
 
 Titles can be formatted to adapt them for the output name: set maximum length,
@@ -509,16 +516,18 @@
 	  # 20240102T1020Z
           # 20240102T1220+02
 	  styles = "basic,reduced,z"
 
 Writing metadata tags
 =====================
 
-By default, metadata tags will be added to the output file by the ``ytpb
-download`` command.  Use the ``--no-metadata`` option to disable it.
+*Related command:* ``ytpb download``
+
+By default, metadata tags will be added to an output excerpt file. Use the
+``--no-metadata`` option to disable it.
 
 .. table:: Metadata tags overview
 
    +---------------------------+-------------------------------+---------------------------------------------+
    | Tag                       | Description                   |                   Example                   |
    +===========================+===============================+=============================================+
    | ``title``                 | Video's title                 | Stream Title                                |
@@ -541,14 +550,60 @@
    +---------------------------+-------------------------------+---------------------------------------------+
 
 The input and actual time values (represented as seconds since the epoch) are
 expected to be different in only two cases: if the boundary (start and end)
 points fall in gaps or the ``--no-cut`` option is requested. In the opposite
 cases, after accurate cut, they're supposed to be identical.
 
+Saving segment files
+====================
+
+*Related command:* ``ytpb download``
+
+After merging downloaded segment files to make an excerpt, the segments will be
+deleted. Do you want to keep them? There are two options here.
+
+*First*, download an excerpt and keep segment files by using the ``-S /
+--keep-segments`` option::
+
+  $ ytpb download ... -S <STREAM>
+  ...
+  Success! Saved to 'Stream-Title_abcdefgh123_20240102T102030+00.mkv'.
+  ~ Segments are kept in 'Stream-Title_abcdefgh123_20240102T102030+00'.
+
+The download destination can be changed via ``--segments-output-dir``::
+
+  $ ytpb download ... -S --segments-output-dir segments <STREAM>
+  ...
+  Success! Saved to 'Stream-Title_abcdefgh123_20240102T102030+00.mkv'.
+  ~ Segments are kept in 'segments'.
+
+*Second*, download only segment files without merging them::
+
+  $ ytpb download ... --no-merge <STREAM>
+  ...
+  Success! Segments saved to 'Stream-Title_abcdefgh123_20240102T102030+00'.
+
+Resuming unfinished downloads
+=============================
+
+*Related command:* ``ytpb download``
+
+If a download gets interrupted for some reason (network problems, unhandled
+exceptions, aborting with ``Ctrl+C``, etc.), you can continue the unfinished
+download by execution of the same command again. Each run creates a resume file
+used to keep information needed for resumption, which is cleaned after
+successful completion. The commands are matched based on the following input
+option values: ``--interval``, ``--audio-format``, ``--video-format``, and
+``--segments-output-dir``. Resuming behavior can be disabled by the
+``--ignore-resume`` option to avoid using an existing resume file and start
+download from scratch.
+
+.. _Configuring:
+
 Configuring
 ***********
 
 The configuration provides the way to set up default values of the command
 options and change other settings via configuration files. It's optional, and
 the default, built-in settings are used.
 
@@ -565,77 +620,53 @@
 
 Advanced usage
 **************
 
 Merging without cutting
 =======================
 
-By default, boundary segments are cutted to exact times during the merging step
-to produce an excerpt. It may take some time to re-encode boundary segments. If
-you don't need exact precision, it could be practical to omit cutting via the
+The boundary segments are cutted to exact times during the merging step to
+make an excerpt. It may take some time to re-encode boundary segments. If you
+don't need exact precision, it could be practical to omit cutting via the
 ``--no-cut`` option. In this case the accuracy will be slightly reduced, which
 will depend on the constant segment duration (or type of `live-streaming latency
 <https://support.google.com/youtube/answer/7444635?hl=en>`_): in the worst case,
 the error will be 1 (for ultra-low latency), 2 (low latency), or 5 (normal
 latency) seconds.
 
 ::
 
-   $ ytpb download ... --no-cut
-
-Keep segment files
-==================
-
-By default, after merging downloaded segment files to produce an excerpt, the
-segments will be deleted. Do you want to keep them? There are two options here.
-
-*First*, download only segment files without merging them (it also implies
-another option, ``--no-cleanup``): ::
-
-  $ ytpb download ... --no-merge
-  ...
-  Success! Segments saved to /tmp/.../segments/.
-  notice: No cleanup enabled, check /tmp/.../
-
-Actually, it keeps not only segments (in ``/tmp/.../segments``) but some other
-auxiliary files in the run temporary directory (``/tmp/...``). Note that, in
-this case, the temporary directory shall be removed manually afterward.
-
-*Second*, download an excerpt and keep segment files: ::
-
-  $ ytpb download ... --no-cleanup
-  ...
-  notice: No cleanup enabled, check /tmp/.../
-
+   $ ytpb download ... --no-cut <STREAM>
 
 Running without downloading
 ===========================
 
-There is a dry run mode to run without downloading. It could be useful if you
-are not interested in having an output excerpt file: for example, you want to
-locate the desired segments or debug just the first steps (by combining a dry
-run mode with the logging options; see the subsection below).
+There is a dry run mode (``-X / --dry-run``) to run without downloading. It
+could be useful if you are not interested in having an output excerpt file: for
+example, you want to locate the rewind interval or debug just the first steps
+(by combining a dry run mode with the ``--debug`` global option).
 
-For example, just to locate start and end segments, use: ::
+For example, just to locate start and end moments, use::
 
-  $ ytpb download ... --dry-run
+  $ ytpb download ... --dry-run <STREAM>
   ...
   (<<) Locating start and end in the stream... done.
   Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
-  notice: This is a dry run. Skip downloading and exit.
+  ~ This is a dry run. Skip downloading and exit.
 
-It can be combined with the ``--no-cleanup`` option as well: ::
+It can be combined with the ``--keep-temp`` option to keep temporary
+files::
 
-  $ ytpb download ... --dry-run --no-cleanup
+  $ ytpb download ... --dry-run --keep-temp <STREAM>
 
 Using cache
 ===========
 
-Using cache helps to avoid getting info about videos and downloading MPEG-DASH
-manifest on every run. The cached files contain the info and the base URLs for
-segments, and are stored under ``XDG_CACHE_HOME/ytpb``. It's a default
-behavior. The cache expiration is defined by the base URLs expiration time. The
-``--no-cache`` option allows avoiding touching cache: no reading and
-writing. Another option, ``--force-update-cache``, exists to trigger cache
-update.
+Using cache helps to avoid getting information about videos and downloading
+MPEG-DASH manifest on every run. The cached files contain the basic information
+and the base URLs for segments, and are stored under
+``$XDG_CACHE_HOME/ytpb``. It's a default behavior. The cache expiration is
+defined by the segment base URLs expiration time. The ``--no-cache`` option allows
+avoiding touching cache: no reading and writing. Another option,
+``--force-update-cache``, exists to trigger cache update.
```

### Comparing `ytpb-2024.4.20/docs/conf.py` & `ytpb-2024.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/docs/cookbook.rst` & `ytpb-2024.5.3/docs/cookbook.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/docs/quick.rst` & `ytpb-2024.5.3/docs/quick.rst`

 * *Files 4% similar despite different names*

```diff
@@ -8,30 +8,29 @@
 
 Download
 ********
 
 Let's start with downloading a 30-second excerpt of audio and video by
 specifying start and end dates and stream URL or ID: ::
 
-  $ ytpb download -i 2024-01-02T10:20:00+00/PT30S <STREAM>
-  $ ls
+  $ ytpb download -i 2024-01-02T10:20:00+00/PT30S <STREAM> && ls
   Stream-Title_20240102T102000+00.mp4
 
 By default, it will download an excerpt in the best :ref:`pre-defined
 <Default format values>` quality: 128k AAC audio and 1080p30 (or less) H.264
 video. See :ref:`cli:Specifying formats` on how to choose the formats to
 download.
 
 As for the start and end, they can be also defined in other ways (see
 :ref:`cli:Specifying rewind interval`). For example, it would be handy to locate
 the desired moments first by previewing them and only after download a full
 excerpt. To run downloading in the :ref:`preview mode <Preview mode>`, use the
-``-p/--preview`` option: ::
+``-ps / --preview-start`` or ``-ps / --preview-end`` options::
 
-  $ ytpb download -i 2024-01-02T10:20:00+00/.. -p <STREAM>
+  $ ytpb download -i 2024-01-02T10:20:00+00/PT30S -ps <STREAM>
 
 Check also out how to `download
 <https://ytpb.readthedocs.io/en/latest/cookbook.html#download-segments-with-curl>`__
 media segments with an external downloader.
 
 Compose and play
 ****************
@@ -73,16 +72,15 @@
 possible without making a video.
 
 One frame
 =========
 
 For example, let's take a picture of the moment happening right now: ::
 
-  $ ytpb capture frame --moment now <STREAM>
-  $ ls
+  $ ytpb capture frame --moment now <STREAM> && ls
   Stream-Title_20231227T012954+00.jpg
 
 Timelapse
 =========
 
 Capture not just a single frame, but a whole timelapse with one frame every
 period of time: ::
```

### Comparing `ytpb-2024.4.20/docs/reference.rst` & `ytpb-2024.5.3/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/docs/why.rst` & `ytpb-2024.5.3/docs/why.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/docs/package/index.rst` & `ytpb-2024.5.3/docs/package/index.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/docs/package/usage.rst` & `ytpb-2024.5.3/docs/package/usage.rst`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,15 @@
 
 Let's, for example, download a 30-seconds audio and video excerpt with showing
 download progress:
 
 .. code-block:: python
 
    from datetime import datetime, timedelta, timezone
+   from pathlib import Path
    from ytpb.actions.download import download_excerpt, RichProgressReporter
 
    rewind_interval = playback.locate_interval(
        datetime(2024, 1, 2, 12, tzinfo=timezone.utc),
        timedelta(minutes=30),
    )
 
@@ -187,10 +188,11 @@
 
    download_excerpt(
        rewind_interval,
        audio_stream=playback.streams.get_by_itag("140"),
        video_stream=playback.streams.query(
            "best(format eq webm and quality eq 720p)"
        ),
-       output_stem="path/to/output",
+       output_stem=Path("path/to/output"),
+       segments_directory=Path("path/to/segments"),
        progress_reporter=progress_reporter,
    )
```

### Comparing `ytpb-2024.4.20/etc/Containerfile` & `ytpb-2024.5.3/etc/Containerfile`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/api.py` & `ytpb-2024.5.3/src/ytpb/api.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/cache.py` & `ytpb-2024.5.3/src/ytpb/cache.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/conditional.py` & `ytpb-2024.5.3/src/ytpb/conditional.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/config.py` & `ytpb-2024.5.3/src/ytpb/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     **VIDEO_QUALITY_WITH_OPERATOR_ALIASES,
     **NAME_QUALITY_ALIASES,
     **FRAME_PER_SECOND_ALIASES,
 }
 
 ALL_ALIASES = {**BUILT_IN_ALIASES}
 
-DEFAULT_OUTPUT_PATH = "<title>_<input_start_date>"
+DEFAULT_OUTPUT_PATH = "<title>_<id>_<input_start_date>"
 
 DEFAULT_CONFIG = AddressableDict(
     {
         "version": 1,
         "options": {
             "download": {
                 "audio_format": "itag eq 140",
@@ -104,21 +104,21 @@
                     "best(format eq mp4 and height le 1080 and frame_rate eq 30)"
                 ),
                 "output_path": DEFAULT_OUTPUT_PATH,
             },
             "capture": {
                 "frame": {
                     "video_format": "best(format eq mp4 and frame_rate eq 30)",
-                    "output_path": "<title>_<moment_date>.jpg",
+                    "output_path": "<title>_<id>_<moment_date>.jpg",
                 },
                 "timelapse": {
                     "video_format": "best(format eq mp4 and frame_rate eq 30)",
                     "output_path": (
-                        "<title>/<input_start_date>/<every>/"
-                        "<title>_<input_start_date>_<every>_%04d.jpg"
+                        "<title>_<id>/<input_start_date>/<every>/"
+                        "<title>_<id>_<input_start_date>_<every>_%04d.jpg"
                     ),
                 },
             },
             "mpd": {
                 "compose": {
                     "audio_formats": "itag eq 140",
                     "video_formats": (
```

### Comparing `ytpb-2024.4.20/src/ytpb/download.py` & `ytpb-2024.5.3/src/ytpb/download.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/errors.py` & `ytpb-2024.5.3/src/ytpb/errors.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/fetchers.py` & `ytpb-2024.5.3/src/ytpb/fetchers.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,17 +108,15 @@
         Args:
             video_url: A video URL.
             base_url: A segment base URL.
             session: A :class:`requests.Session` object.
             options: Options passed to :class:`yt_dlp.YoutubeDL`.
         """
         super().__init__(video_url, session)
-        if options is not None:
-            options = self.default_options.update(options)
-        self._ydl = YoutubeDL(options)
+        self._ydl = YoutubeDL(self.default_options | (options or {}))
         self._formats: list[dict] = []
 
     def fetch_video_info(self) -> YouTubeVideoInfo:
         try:
             extracted = self._ydl.extract_info(self.video_url, download=False)
         except DownloadError as exc:
             raise AssertionError from exc
```

### Comparing `ytpb-2024.4.20/src/ytpb/ffmpeg.py` & `ytpb-2024.5.3/src/ytpb/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/info.py` & `ytpb-2024.5.3/src/ytpb/info.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/locate.py` & `ytpb-2024.5.3/src/ytpb/locate.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/merge.py` & `ytpb-2024.5.3/src/ytpb/merge.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/playback.py` & `ytpb-2024.5.3/src/ytpb/playback.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/representations.py` & `ytpb-2024.5.3/src/ytpb/representations.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/segment.py` & `ytpb-2024.5.3/src/ytpb/segment.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/streams.py` & `ytpb-2024.5.3/src/ytpb/streams.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/types.py` & `ytpb-2024.5.3/src/ytpb/types.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/actions/capture.py` & `ytpb-2024.5.3/src/ytpb/actions/capture.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/actions/compose.py` & `ytpb-2024.5.3/src/ytpb/actions/compose.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/actions/download.py` & `ytpb-2024.5.3/src/ytpb/actions/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,27 +109,27 @@
                 yield next(it)
             except StopIteration:
                 return
 
 
 def download_segments(
     playback: Playback,
-    rewind_interval: RewindInterval,
+    sequence_numbers: Iterable[SegmentSequence],
     streams: Union[SetOfStreams, list[AudioOrVideoStream]],
     output_directory: Path | None = None,
     output_filename: Callable[
         [SegmentSequence, str], str
     ] = compose_default_segment_filename,
     progress_reporter: ProgressReporter | None = None,
 ) -> list[Path]:
     """Downloads segments.
 
     Args:
         playback: A playback.
-        rewind_interval: A rewound interval.
+        sequence_numbers: Segment sequence numbers to rewind.
         streams: Streams to download.
         output_directory: A directory where to save downloaded segments.
         output_filename: A callable to compose segment filenames.
         progress_reporter: An instance of :class:`ProgressReporter`-like class
           to show downloading progress. Defaults to dummy progress reporter.
 
     Returns:
@@ -142,18 +142,16 @@
         output_directory = playback.locations["segments"]
         output_directory.mkdir(parents=True, exist_ok=True)
 
     base_urls: list[str] = [s.base_url for s in streams]
     download_generator = chained_zip(
         *[
             zip(
-                iter_segments(
-                    rewind_interval.sequences, base_url, session=playback.session
-                ),
-                repeat(task, len(rewind_interval.sequences)),
+                iter_segments(sequence_numbers, base_url, session=playback.session),
+                repeat(task, len(sequence_numbers)),
             )
             for task, base_url in enumerate(base_urls)
         ]
     )
 
     downloaded_paths: list[list[Path]] = [[] for _ in base_urls]
     with progress_reporter:
@@ -167,31 +165,33 @@
     return downloaded_paths
 
 
 def download_excerpt(
     playback: Playback,
     rewind_interval: RewindInterval,
     output_stem: str | Path,
+    segments_directory: Path,
     audio_stream: AudioStream | None = None,
     video_stream: VideoStream | None = None,
     need_cut: bool = True,
     merge_kwargs: dict[str, Any] | None = None,
     progress_reporter: ProgressReporter | None = None,
 ) -> ExcerptDownloadResult:
     """Downloads and merges audio and/or video segments.
 
     Notes:
         Downloaded segments are not cleaned up after merging.
 
     Args:
         playback: A playback.
-        rewind_interval: A rewound interval.
+        rewind_interval: A rewind interval.
         output_stem: A full path stem of the merged excerpt file.
         audio_stream: An audio stream.
         video_stream: A video stream.
+        segments_directory: A directory where to store downloaded segments.
         need_cut: Whether to cut boundary segments to exact times.
         merge_kwargs: Arguments that :meth:`ytpb.merge.merge_segments` takes.
         progress_reporter: An instance of :class:`ProgressReporter`-like class
           to show downloading progress. Defaults to dummy progress reporter.
 
     Returns:
         An :class:`ExcerptDownloadResult` object.
@@ -200,19 +200,18 @@
         raise AssertionError("At least audio or video stream should be provided")
 
     if progress_reporter is None:
         progress_reporter = NullProgressReporter()
 
     all_streams = [x for x in [audio_stream, video_stream] if x is not None]
 
-    segments_output_directory = playback.locations["segments"]
-    segments_output_directory.mkdir(parents=True, exist_ok=True)
+    segments_directory.mkdir(parents=True, exist_ok=True)
 
     _downloaded_paths: list[list[Path]] = download_segments(
-        playback, rewind_interval, all_streams, segments_output_directory
+        playback, rewind_interval.sequences, all_streams, segments_directory
     )
     downloaded_paths: list[list[Path]] = [[], []]
     if audio_stream:
         downloaded_paths[0] = _downloaded_paths[0]
     if video_stream:
         downloaded_paths[1] = _downloaded_paths[1]
```

### Comparing `ytpb-2024.4.20/src/ytpb/cli/__init__.py` & `ytpb-2024.5.3/src/ytpb/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/cli/common.py` & `ytpb-2024.5.3/src/ytpb/cli/common.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 import email
 import os
 import sys
-import textwrap
 from datetime import datetime, timedelta
 from pathlib import Path
 
 import click
 import cloup
 import structlog
 
-from ytpb.download import compose_default_segment_filename
 from ytpb.errors import (
     BadCommandArgument,
     BaseUrlExpiredError,
     BroadcastStatusError,
     CachedItemNotFoundError,
     QueryError,
 )
 from ytpb.fetchers import YoutubeDLInfoFetcher, YtpbInfoFetcher
 from ytpb.info import BroadcastStatus
 from ytpb.playback import Playback, RewindInterval
-from ytpb.segment import Segment
 from ytpb.types import DateInterval, SetOfStreams
 from ytpb.utils.date import format_timedelta, round_date
 from ytpb.utils.url import extract_parameter_from_url, normalize_video_url
 
 logger = structlog.getLogger(__name__)
 
 
@@ -96,34 +93,14 @@
     "stream_url",
     metavar="STREAM",
     help="Stream URL or video ID.",
     callback=normalize_stream_url,
 )
 
 
-def check_end_options(start, end, duration, preview):
-    if not (end or duration or preview):
-        raise click.UsageError(
-            "One of --end, --duration, or --preview must be specified."
-        )
-
-    if isinstance(end, datetime) and isinstance(start, datetime):
-        if end <= start:
-            raise click.BadParameter(
-                "End date is ahead or equal to the start date.",
-                param_hint="'-e' / '--end'",
-            )
-
-
-def get_downloaded_segment(playback, sequence, base_url):
-    segment_filename = compose_default_segment_filename(sequence, base_url)
-    segment = Segment.from_file(playback.get_temp_directory() / segment_filename)
-    return segment
-
-
 def prepare_line_for_summary_info(
     date: datetime,
     input_actual_timedelta: timedelta,
     use_ms_precision: bool = False,
 ) -> str:
     if not use_ms_precision:
         date = round_date(date)
@@ -169,44 +146,14 @@
     )
     click.echo(
         "  Actual end: {}, seq. {}".format(
             end_time_info_line, rewind_interval.end.sequence
         )
     )
 
-    # total_duration = format_duration(
-    #     timedelta(seconds=actual_date_interval.duration),
-    #     DurationFormatPattern.IN_SENTENCE
-    # )
-    # click.echo(f"Total duration: {total_duration}, estimated size: ?")
-
-
-def check_streams_not_empty(
-    audio_stream, audio_format, video_stream, video_format, max_text_width=62
-):
-    if audio_format and not audio_stream:
-        message = (
-            "  Error! Found no audio formats matching requested format spec: "
-            f"{audio_format}."
-        )
-        if video_format and not video_stream:
-            message += " Same for the video: {video_format}."
-        click.echo(textwrap.fill(message, max_text_width))
-        click.echo("~" * max_text_width)
-        sys.exit(1)
-    elif video_format and not video_stream:
-        click.echo("~" * max_text_width)
-        message = (
-            "  Error! Found no video formats matching requested format spec: "
-            f"{video_format}."
-        )
-        click.echo(textwrap.fill(message, max_text_width))
-        click.echo("~" * max_text_width)
-        sys.exit(1)
-
 
 def query_streams_or_exit(
     streams: SetOfStreams,
     format_spec: str,
     param: str | None = None,
     allow_empty: bool = False,
     allow_many: bool = True,
@@ -277,7 +224,11 @@
     resolved_path = Path(output_path).expanduser().resolve()
     resolved_path.parent.mkdir(parents=True, exist_ok=True)
     return resolved_path
 
 
 def suppress_output() -> None:
     sys.stdout = open(os.devnull, "w")
+
+
+def echo_notice(message: str) -> None:
+    click.echo(f"~ {message}")
```

### Comparing `ytpb-2024.4.20/src/ytpb/cli/options.py` & `ytpb-2024.5.3/src/ytpb/cli/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,22 +70,14 @@
     metavar="INTERVAL",
     type=parameters.RewindIntervalParamType(),
     help="Time or segment interval.",
     required=True,
 )
 
 
-preview_option = click.option(
-    "-p",
-    "--preview",
-    help="Run in preview mode.",
-    is_flag=True,
-)
-
-
 def config_options(f):
     f = click.option(
         "--config",
         "config_path",
         help="Specifies a path to a configuration file.",
         type=click.Path(path_type=Path),
         is_eager=True,
@@ -140,10 +132,10 @@
 
 
 yt_dlp_option = click.option(
     "-Y", "--yt-dlp", is_flag=True, help="Use yt-dlp to extract info."
 )
 
 
-no_cleanup_option = click.option(
-    "--no-cleanup", is_flag=True, help="Do not clean up temporary files."
+keep_temp_option = click.option(
+    "--keep-temp", is_flag=True, help="Keep temporary files."
 )
```

### Comparing `ytpb-2024.4.20/src/ytpb/cli/parameters.py` & `ytpb-2024.5.3/src/ytpb/cli/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,25 +82,24 @@
                     previous = i + 1
 
         return date.replace(**components_to_replace)
 
     def _parse_interval_part(
         self,
         part: str,
-        end: bool = False,
     ) -> int | str | Literal["now", ".."] | datetime | timedelta | isotimedelta:
         match part:
             # Sequence number
             case x if x.isdecimal():
                 output = int(x)
             # Duration
             case x if x[0] == "P":
                 output = isotimedelta.fromisoformat(x)
             # Replacing components
-            case x if set(x) & set("DHMS"):
+            case x if set(x) & set("YMDHS"):
                 output = x
             # Time of today
             case x if x[0] == "T" or (":" in x and "-" not in x):
                 parsed_time = time.fromisoformat(x)
                 today = datetime.now()
                 output = today.replace(
                     hour=parsed_time.hour,
@@ -142,37 +141,45 @@
         except ValueError as exc:
             raise click.BadParameter(f"'{end_part}', {exc}.")
 
         match parsed_start, parsed_end:
             # Two durations
             case [timedelta(), timedelta()]:
                 raise click.BadParameter("Two durations are ambiguous.")
-            case ["now" | ".." as x, _]:
+            # Two '..' keywords
+            case ["..", ".."]:
+                raise click.BadParameter("Two '..' are ambiguous.")
+            case ["now" as x, _]:
                 raise click.BadParameter(
                     f"Keyword '{x}' is only allowed for the end part."
                 )
             # Duration and '..'
-            case [timedelta(), ".."]:
-                raise click.BadParameter("Keyword '..' not compatible with duration.")
+            case [timedelta(), ".."] | ["..", timedelta()]:
+                raise click.BadParameter(
+                    "Keyword '..' is not compatible with duration."
+                )
             # Anything compatible and 'now' or '..'
-            case [int() | datetime() | timedelta(), "now" | ".."]:
+            case [int() | datetime() | timedelta(), "now" | ".."] | [
+                "..",
+                int() | datetime() | timedelta(),
+            ]:
                 start = parsed_start
                 end = parsed_end
             # Replacing components and date and time
             case (str(), datetime()) | (datetime(), str()):
                 if isinstance(parsed_start, str):
                     end = parsed_end
                     start = self._replace_datetime_components(end, parsed_start)
                 else:
                     start = parsed_start
                     end = self._replace_datetime_components(start, parsed_end)
             # Replacing components and anything remaining, non-compatible
             case (str(), _) | (_, str()):
                 raise click.BadParameter(
-                    "Replacement components is only compatible with date and time."
+                    "Replacement components are only compatible with date and time."
                 )
             # Remaining and compatible
             case [_, _]:
                 start = parsed_start
                 end = parsed_end
 
         if type(start) == type(end) and start >= end:
```

### Comparing `ytpb-2024.4.20/src/ytpb/cli/commands/capture.py` & `ytpb-2024.5.3/src/ytpb/cli/commands/capture.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,26 +20,26 @@
 )
 from timedelta_isoformat import timedelta as isotimedelta
 
 from ytpb.actions.capture import capture_frames, extract_frame_as_image
 from ytpb.cli.commands.download import render_download_output_path_context
 from ytpb.cli.common import (
     create_playback,
+    echo_notice,
     get_parameter_by_name,
     prepare_line_for_summary_info,
     raise_for_sequence_ahead_of_current,
     raise_for_too_far_sequence,
     resolve_output_path,
     stream_argument,
 )
 from ytpb.cli.options import (
     cache_options,
     interval_option,
-    no_cleanup_option,
-    preview_option,
+    keep_temp_option,
     validate_image_output_path,
     yt_dlp_option,
 )
 from ytpb.cli.parameters import (
     FormatSpecParamType,
     FormatSpecType,
     InputRewindInterval,
@@ -176,25 +176,25 @@
     "--output",
     "output_path",
     type=click.Path(path_type=Path),
     help="Output path (with extension).",
     callback=validate_image_output_path(CaptureOutputPathContext),
 )
 @yt_dlp_option
-@no_cleanup_option
+@keep_temp_option
 @cache_options
 @stream_argument
 @click.pass_context
 def frame_command(
     ctx: click.Context,
     moment: AbsolutePointInStream | Literal["now"],
     video_format: str,
     output_path: Path,
     yt_dlp: bool,
-    no_cleanup: bool,
+    keep_temp: bool,
     force_update_cache: bool,
     no_cache: bool,
     stream_url: str,
 ):
     playback = create_playback(ctx)
 
     if video_format:
@@ -292,16 +292,16 @@
     try:
         saved_to_path_value = final_output_path.relative_to(Path.cwd())
     except ValueError:
         saved_to_path_value = final_output_path
     click.echo(f"\nSuccess! Saved to '{saved_to_path_value}'.")
 
     run_temp_directory = playback.get_temp_directory()
-    if no_cleanup:
-        click.echo(f"notice: No cleanup enabled, check {run_temp_directory}/")
+    if keep_temp:
+        echo_notice(f"No cleanup enabled, check {run_temp_directory}")
     else:
         try:
             shutil.rmtree(run_temp_directory)
         except OSError:
             logger.warning(
                 "Failed to remove %s temporary directory", run_temp_directory
             )
@@ -323,38 +323,43 @@
     cloup.option(
         "-vf",
         "--video-format",
         metavar="SPEC",
         type=FormatSpecParamType(FormatSpecType.VIDEO),
         help="Video format to capture.",
     ),
-    preview_option,
+    cloup.option(
+        "-p",
+        "--preview",
+        help="Run in preview mode.",
+        is_flag=True,
+    ),
 )
 @click.option(
     "-o",
     "--output",
     "output_path",
     type=click.Path(path_type=Path),
     help="Output path (with extension).",
     callback=validate_image_output_path(TimelapseOutputPathContext),
 )
 @yt_dlp_option
-@no_cleanup_option
+@keep_temp_option
 @cache_options
 @stream_argument
 @click.pass_context
 def timelapse_command(
     ctx: click.Context,
     interval: InputRewindInterval,
     every: timedelta,
     video_format: str,
     preview: bool,
     output_path: Path,
     yt_dlp: bool,
-    no_cleanup: bool,
+    keep_temp: bool,
     force_update_cache: bool,
     no_cache: bool,
     stream_url: str,
 ):
     playback = create_playback(ctx)
 
     if video_format:
@@ -439,15 +444,16 @@
 
     s, e = requested_date_interval.start, requested_date_interval.end
     dates_to_capture = [s + every * i for i in range((e - s) // every + 1)]
 
     print_timelapse_summary_info(dates_to_capture, requested_date_interval.end, every)
 
     if preview:
-        click.echo("info: Preview mode is enabled, only first 3 frames will be taken.")
+        click.echo()
+        echo_notice("Preview mode enabled, only first 3 frames will be taken.")
         dates_to_capture = dates_to_capture[:3]
 
     click.echo()
 
     # Absolute output path of images with a numeric pattern.
     final_output_path: Path
     if OUTPUT_PATH_PLACEHOLDER_RE.search(str(output_path)):
@@ -505,19 +511,19 @@
             _save_ith_frame_as_image(image, final_output_path, i)
             capturing_progress.advance(capturing_task)
 
     try:
         saved_to_path_value = final_output_path.parent.relative_to(Path.cwd())
     except ValueError:
         saved_to_path_value = final_output_path.parent
-    click.echo(f"\nSuccess! Saved to '{saved_to_path_value}/'.")
+    click.echo(f"\nSuccess! Saved to '{saved_to_path_value}'.")
 
     run_temp_directory = playback.get_temp_directory()
-    if no_cleanup:
-        click.echo(f"notice: No cleanup enabled, check {run_temp_directory}/")
+    if keep_temp:
+        echo_notice(f"No cleanup enabled, check {run_temp_directory}")
     else:
         try:
             shutil.rmtree(run_temp_directory)
         except OSError:
             logger.warning(
                 "Failed to remove %s temporary directory", run_temp_directory
             )
```

### Comparing `ytpb-2024.4.20/src/ytpb/cli/commands/download.py` & `ytpb-2024.5.3/src/ytpb/cli/commands/download.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,90 @@
+import pickle
 import shutil
 import sys
 from datetime import datetime, timedelta
 from functools import partial
 from pathlib import Path
 
 import click
 import cloup
 import structlog
-from cloup.constraints import constraint, require_any
+from cloup.constraints import constraint, mutually_exclusive, require_any
 
 from ytpb import actions
 from ytpb.cli.common import (
     create_playback,
+    echo_notice,
     get_parameter_by_name,
     print_summary_info,
     query_streams_or_exit,
     raise_for_sequence_ahead_of_current,
     raise_for_too_far_sequence,
     resolve_output_path,
     stream_argument,
     suppress_output,
 )
 from ytpb.cli.options import (
     cache_options,
     interval_option,
-    no_cleanup_option,
-    preview_option,
+    keep_temp_option,
     validate_output_path,
     yt_dlp_option,
 )
 from ytpb.cli.parameters import FormatSpecParamType, FormatSpecType, InputRewindInterval
+from ytpb.download import compose_default_segment_filename
 from ytpb.errors import SequenceLocatingError
 from ytpb.merge import merge_segments
 from ytpb.types import (
     AddressableMappingProtocol,
+    AudioOrVideoStream,
     DateInterval,
     RelativeSegmentSequence,
     SegmentSequence,
 )
 from ytpb.utils.other import resolve_relativity_in_interval
 from ytpb.utils.path import (
     expand_template_output_path,
     IntervalOutputPathContext,
     MinimalOutputPathContext,
     OUTPUT_PATH_PLACEHOLDER_RE,
+    remove_directories_between,
     render_interval_output_path_context,
     render_minimal_output_path_context,
+    try_get_relative_path,
 )
 from ytpb.utils.remote import request_reference_sequence
 from ytpb.utils.url import build_segment_url, extract_parameter_from_url
 
 logger = structlog.get_logger(__name__)
 
 
 class DownloadOutputPathContext(
     MinimalOutputPathContext, IntervalOutputPathContext
 ): ...
 
 
+def compose_resume_filename(
+    video_id: str, streams: list[AudioOrVideoStream | None]
+) -> str:
+    for i, arg in enumerate(sys.argv):
+        if arg in ("--interval", "-i"):
+            interval_option_value = sys.argv[i + 1]
+            break
+
+    interval_part = interval_option_value
+    for char in "-:@":
+        interval_part = interval_part.replace(char, "")
+    interval_part = interval_part.replace("/", "-")
+
+    itag_part = "".join([stream.itag for stream in streams if stream])
+
+    return f"{video_id}-{interval_part}-{itag_part}.resume"
+
+
 def render_download_output_path_context(
     context: DownloadOutputPathContext,
     config_settings: AddressableMappingProtocol,
 ) -> DownloadOutputPathContext:
     output = context
     output.update(render_minimal_output_path_context(context, config_settings))
     output.update(render_interval_output_path_context(context, config_settings))
@@ -82,36 +105,66 @@
     cloup.option(
         "-vf",
         "--video-format",
         metavar="SPEC",
         type=FormatSpecParamType(FormatSpecType.VIDEO),
         help="Video format to download.",
     ),
-    preview_option,
+    cloup.option(
+        "-ps",
+        "--preview-start",
+        help="Preview interval start.",
+        is_flag=True,
+    ),
+    cloup.option(
+        "-pe",
+        "--preview-end",
+        help="Preview interval end.",
+        is_flag=True,
+    ),
 )
 @cloup.option_group(
     "Dump options",
     cloup.option(
         "--dump-base-urls",
         is_flag=True,
         help="Print base URLs and exit.",
     ),
     cloup.option(
         "--dump-segment-urls",
         is_flag=True,
         help="Print segment URLs and exit.",
     ),
 )
-@click.option(
-    "-o",
-    "--output",
-    "output_path",
-    type=click.Path(path_type=Path),
-    help="Output path (without extension).",
-    callback=validate_output_path(DownloadOutputPathContext),
+@cloup.option_group(
+    "Output options",
+    cloup.option(
+        "-o",
+        "--output",
+        "output_path",
+        type=click.Path(path_type=Path),
+        help="Output path (without extension).",
+        callback=validate_output_path(DownloadOutputPathContext),
+    ),
+    cloup.option(
+        "-S", "--keep-segments", is_flag=True, help="Keep downloaded segments."
+    ),
+    cloup.option(
+        "--segments-output-dir",
+        "segments_output_dir_option",
+        type=click.Path(path_type=Path),
+        help="Location where to download segments to.",
+    ),
+    cloup.option("--no-metadata", is_flag=True, help="Do not write metadata tags."),
+    cloup.option("--no-cut", is_flag=True, help="Do not perform excerpt cutting."),
+    cloup.option(
+        "--no-merge",
+        is_flag=True,
+        help="Only download segments, without merging.",
+    ),
 )
 @click.option(
     "-m",
     "--from-manifest",
     metavar="PATH",
     type=click.Path(path_type=Path),
     help="Path to a MPEG-DASH manifest.",
@@ -119,51 +172,52 @@
 @click.option(
     "-X",
     "--dry-run",
     is_flag=True,
     help="Run without downloading.",
 )
 @yt_dlp_option
-@click.option("--no-metadata", is_flag=True, help="Do not write metadata tags.")
-@click.option("--no-cut", is_flag=True, help="Do not perform excerpt cutting.")
 @click.option(
-    "--no-merge",
-    is_flag=True,
-    help="Only download segments, without merging. This implies '--no-cleanup'.",
+    "--ignore-resume", is_flag=True, help="Avoid resuming unfinished download."
 )
-@no_cleanup_option
 @cache_options
+@keep_temp_option
 @stream_argument
 @constraint(require_any, ["audio_format", "video_format"])
+@constraint(mutually_exclusive, ["preview_start", "preview_end"])
 @click.pass_context
 def download_command(
     ctx: click.Context,
     interval: InputRewindInterval,
     audio_format: str,
     video_format: str,
-    preview: bool,
+    preview_start: bool,
+    preview_end: bool,
     dump_base_urls: bool,
     dump_segment_urls: bool,
     output_path: Path,
-    from_manifest: Path,
-    dry_run: bool,
-    yt_dlp: bool,
+    keep_segments: bool,
+    segments_output_dir_option: Path,
     no_metadata: bool,
     no_cut: bool,
     no_merge: bool,
-    no_cleanup: bool,
-    force_update_cache: bool,
+    from_manifest: Path,
+    dry_run: bool,
+    yt_dlp: bool,
+    ignore_resume: bool,
     no_cache: bool,
+    force_update_cache: bool,
+    keep_temp: bool,
     stream_url: str,
 ) -> int:
     if dump_base_urls or dump_segment_urls:
         suppress_output()
 
     if no_merge:
-        no_cleanup = True
+        keep_segments = True
 
     playback = create_playback(ctx)
 
     queried_audio_streams = []
     if audio_format:
         logger.debug("Query audio stream by format spec", spec=audio_format)
         queried_audio_streams = query_streams_or_exit(
@@ -206,14 +260,15 @@
         if audio_format:
             click.echo(audio_stream.base_url, ctx.obj.original_stdout)
         if video_format:
             click.echo(video_stream.base_url, ctx.obj.original_stdout)
         sys.exit()
 
     click.echo()
+
     click.echo("(<<) Locating start and end in the stream... ", nl=False)
 
     reference_stream = video_stream or audio_stream
     reference_base_url = reference_stream.base_url
     head_sequence = request_reference_sequence(reference_base_url, playback.session)
 
     requested_start, requested_end = resolve_relativity_in_interval(*interval)
@@ -227,53 +282,100 @@
         )
 
     match requested_end:
         case SegmentSequence() as x:
             raise_for_sequence_ahead_of_current(x, head_sequence, ctx, "interval")
         case "now":
             requested_end = head_sequence - 1
-        case "..":
-            if not preview:
+
+    preview_mode = preview_start or preview_end
+    if not preview_mode and (requested_start == ".." or requested_end == ".."):
+        raise click.BadParameter(
+            "Open interval is only valid in the preview mode.",
+            param=get_parameter_by_name("interval", ctx),
+        )
+
+    if preview_mode:
+        preview_duration_value = ctx.obj.config.traverse("general.preview_duration")
+        segment_duration = float(extract_parameter_from_url("dur", reference_base_url))
+        preview_segments = round(preview_duration_value / segment_duration)
+
+        if preview_start:
+            if requested_start == "..":
                 raise click.BadParameter(
-                    "Open interval is only valid in the preview mode",
+                    "Start '..' is only valid in the end preview mode.",
                     param=get_parameter_by_name("interval", ctx),
                 )
+            elif isinstance(requested_start, timedelta):
+                located_moment = playback.locate_moment(
+                    requested_end, reference_stream, is_end=True
+                )
+                requested_start = located_moment.date - requested_start
+            requested_end = RelativeSegmentSequence(preview_segments)
+        if preview_end:
+            if requested_end == "..":
+                raise click.BadParameter(
+                    "End '..' is only valid in the start preview mode.",
+                    param=get_parameter_by_name("interval", ctx),
+                )
+            elif isinstance(requested_end, timedelta):
+                located_moment = playback.locate_moment(
+                    requested_start, reference_stream
+                )
+                requested_end = located_moment.date + requested_end
+            requested_start = RelativeSegmentSequence(preview_segments)
 
-    if preview:
-        preview_duration_value = ctx.obj.config.traverse("general.preview_duration")
-        segment_duration = float(extract_parameter_from_url("dur", reference_base_url))
-        number_of_segments = round(preview_duration_value / segment_duration)
-        requested_end = RelativeSegmentSequence(number_of_segments)
+    resume_run: bool = False
+    resume_file_path = Path.cwd() / compose_resume_filename(
+        playback.video_id, (audio_stream, video_stream)
+    )
 
-    try:
-        rewind_interval = playback.locate_interval(
-            requested_start,
-            requested_end,
-            reference_stream,
-        )
-    except SequenceLocatingError:
-        message = "\nerror: An error occured during segment locating, exit."
-        click.echo(message, err=True)
-        sys.exit(1)
+    if not ignore_resume and resume_file_path.exists():
+        logger.debug("Load resume file from %s", resume_file_path)
+        with open(resume_file_path, "rb") as f:
+            resume_run = True
+            pickled = pickle.load(f)
+            rewind_interval = pickled["interval"]
+            previous_segments_output_directory = Path.absolute(
+                pickled["segments_output_directory"]
+            )
+
+    if not resume_run:
+        try:
+            # assert False, requested_start
+            rewind_interval = playback.locate_interval(
+                requested_start,
+                requested_end,
+                reference_stream,
+            )
+        except SequenceLocatingError:
+            message = "\nerror: An error occured during segment locating, exit."
+            click.echo(message, err=True)
+            sys.exit(1)
 
     click.echo("done.")
 
     if dump_segment_urls:
         range_part = "[{start}-{end}]".format(
             start=rewind_interval.start.sequence, end=rewind_interval.end.sequence
         )
         build_dump_url = lambda base_url: build_segment_url(base_url, range_part)
         if audio_format:
             click.echo(build_dump_url(audio_stream.base_url), ctx.obj.original_stdout)
         if video_format:
             click.echo(build_dump_url(video_stream.base_url), ctx.obj.original_stdout)
         sys.exit()
 
-    if preview and interval[1] != "..":
-        click.echo("info: The preview mode is enabled, interval end is ignored.")
+    # if preview_mode and interval[1] != "..":
+    if preview_mode:
+        echo_notice(
+            "Preview mode enabled, interval {} is ignored.".format(
+                "end" if preview_start else "start"
+            )
+        )
 
     start_segment = playback.get_segment(
         rewind_interval.start.sequence, reference_stream
     )
     end_segment = playback.get_segment(rewind_interval.end.sequence, reference_stream)
 
     requested_start_date: datetime
@@ -298,38 +400,42 @@
     actual_date_interval = DateInterval(
         start_segment.ingestion_start_date,
         end_segment.ingestion_end_date,
     )
 
     cut_kwargs: dict[str, float] = {}
     if not no_cut:
-        cut_at_start = rewind_interval.start.cut_at
-        if preview:
-            cut_at_end = 0
-        else:
-            cut_at_end = rewind_interval.end.cut_at
+        cut_at_start = rewind_interval.start.cut_at if preview_start else 0
+        cut_at_end = rewind_interval.end.cut_at if preview_end else 0
         cut_kwargs.update(
             {
                 "cut_at_start": cut_at_start,
                 "cut_at_end": cut_at_end,
             }
         )
         actual_date_interval = DateInterval(
             rewind_interval.start.date, rewind_interval.end.date
         )
 
     print_summary_info(requested_date_interval, actual_date_interval, rewind_interval)
     click.echo()
 
     if dry_run:
-        click.echo("notice: This is a dry run. Skip downloading and exit.")
+        echo_notice("This is a dry run. Skip downloading and exit.")
     else:
         # Absolute output path of an excerpt without extension.
         final_output_path: Path
 
+        if preview_mode:
+            default_output_path = ctx.obj.config.traverse(
+                "options.download.output_path"
+            )
+            if str(output_path) == default_output_path:
+                output_path = "<title>_<id>_preview"
+
         if OUTPUT_PATH_PLACEHOLDER_RE.search(str(output_path)):
             input_timezone = requested_date_interval.start.tzinfo
             template_context: DownloadOutputPathContext = {
                 "id": playback.video_id,
                 "title": playback.info.title,
                 "input_start_date": requested_date_interval.start,
                 "input_end_date": requested_date_interval.end,
@@ -345,58 +451,141 @@
                 render_download_output_path_context,
                 ctx.obj.config,
             )
         else:
             final_output_path = output_path
         final_output_path = resolve_output_path(final_output_path)
 
-        total_segments = (
-            rewind_interval.end.sequence - rewind_interval.start.sequence + 1
-        )
+        if preview_mode:
+            segments_output_directory = playback.get_temp_directory()
+        elif segments_output_dir_option:
+            segments_output_directory = segments_output_dir_option
+        elif keep_segments or no_merge:
+            segments_output_directory = final_output_path
+        else:
+            segments_output_directory = resume_file_path.with_name(
+                f"{resume_file_path.stem}"
+            )
+        segments_output_directory = segments_output_directory.absolute()
+        logger.debug("Segments output directory set to %s", segments_output_directory)
+
+        if resume_run:
+            click.echo(
+                f"~ Found unfinished download, continue from {resume_file_path.name}\n"
+            )
+            if segments_output_directory != previous_segments_output_directory:
+                click.echo(
+                    "fatal: The previous segments output directory is not "
+                    "the same as the current run:\n'{}' != '{}'.".format(
+                        try_get_relative_path(previous_segments_output_directory),
+                        try_get_relative_path(segments_output_directory),
+                    ),
+                    err=True,
+                )
+                click.echo(
+                    "\nUse '--segments-output-dir {}' or '--ignore-resume'.".format(
+                        try_get_relative_path(previous_segments_output_directory)
+                    ),
+                    err=True,
+                )
+                sys.exit(1)
+
+        if segments_output_dir_option is None or not segments_output_directory.exists():
+            need_to_remove_segments_directory = True
+            segments_directory_to_remove = segments_output_directory
+            for directory in segments_output_directory.parents:
+                if directory.exists():
+                    break
+                segments_directory_to_remove = directory
+            segments_output_directory.mkdir(parents=True, exist_ok=True)
+        else:
+            need_to_remove_segments_directory = False
+
+        if not resume_run and not preview_mode:
+            with open(resume_file_path, "wb") as f:
+                logger.debug("Write resume file to %s", resume_file_path)
+                to_pickle = {
+                    "interval": rewind_interval,
+                    "segments_output_directory": segments_output_directory,
+                }
+                pickle.dump(to_pickle, f)
+
+        if resume_run:
+            extract_sequence_number = lambda p: int(p.name.split(".")[0])
+            latest_sequence_number = extract_sequence_number(
+                sorted(
+                    segments_output_directory.glob(
+                        f"*.i{(audio_stream or video_stream).itag}*"
+                    ),
+                    key=extract_sequence_number,
+                )[-1]
+            )
+            sequences_to_download = range(
+                latest_sequence_number, rewind_interval.end.sequence + 1
+            )
+            completed_segments = latest_sequence_number - rewind_interval.start.sequence
+        else:
+            sequences_to_download = rewind_interval.sequences
+            completed_segments = 0
+
+        total_segments = len(rewind_interval.sequences)
+
         progress_reporter = actions.download.RichProgressReporter()
         if audio_stream:
-            progress_reporter.progress.add_task("   - Audio", total=total_segments)
+            progress_reporter.progress.add_task(
+                "   - Audio", total=total_segments, completed=completed_segments
+            )
         if video_stream:
-            progress_reporter.progress.add_task("   - Video", total=total_segments)
+            progress_reporter.progress.add_task(
+                "   - Video", total=total_segments, completed=completed_segments
+            )
+
         do_download_segments = partial(
             actions.download.download_segments,
-            playback,
-            rewind_interval,
-            [x for x in [audio_stream, video_stream] if x is not None],
+            playback=playback,
+            sequence_numbers=sequences_to_download,
+            streams=[x for x in [audio_stream, video_stream] if x is not None],
+            output_directory=segments_output_directory,
             progress_reporter=progress_reporter,
         )
 
         if no_merge:
             click.echo(
                 "(<<) Downloading segments {}-{} (no merge requested)...".format(
                     rewind_interval.start.sequence, rewind_interval.end.sequence
                 )
             )
-            downloaded_segment_paths = do_download_segments()
-            some_downloaded_path = downloaded_segment_paths[0][0]
+            do_download_segments()
             click.echo(
-                "\nSuccess! Segments saved to {}/.".format(some_downloaded_path.parent)
+                "\nSuccess! Segments saved to '{}'.".format(
+                    try_get_relative_path(segments_output_directory)
+                )
             )
         else:
             click.echo("(<<) Preparing and saving the excerpt...")
             click.echo(
                 "1. Downloading segments {}-{}:".format(
                     rewind_interval.start.sequence, rewind_interval.end.sequence
                 )
             )
 
-            downloaded_segment_paths = do_download_segments()
+            do_download_segments()
             audio_and_video_segment_paths: list[list[Path]] = [[], []]
-            match audio_stream, video_stream:
-                case _, None:
-                    audio_and_video_segment_paths[0] = downloaded_segment_paths[0]
-                case None, _:
-                    audio_and_video_segment_paths[1] = downloaded_segment_paths[0]
-                case _:
-                    audio_and_video_segment_paths = downloaded_segment_paths
+            if audio_stream:
+                audio_and_video_segment_paths[0] = [
+                    segments_output_directory
+                    / compose_default_segment_filename(sequence, audio_stream.base_url)
+                    for sequence in rewind_interval.sequences
+                ]
+            if video_stream:
+                audio_and_video_segment_paths[1] = [
+                    segments_output_directory
+                    / compose_default_segment_filename(sequence, video_stream.base_url)
+                    for sequence in rewind_interval.sequences
+                ]
 
             if no_cut:
                 click.echo("2. Merging segments (no cut requested)... ", nl=False)
             else:
                 click.echo("2. Merging segments (may take a while)... ", nl=False)
 
             metadata_tags: dict[str, str] = {}
@@ -429,24 +618,51 @@
                 output_stem=final_output_path.name,
                 temp_directory=playback.get_temp_directory(),
                 metadata_tags=metadata_tags,
                 **cut_kwargs,
             )
 
             click.echo("done.\n")
+            click.echo(f"Success! Saved to '{try_get_relative_path(merged_path)}'.")
 
-            try:
-                saved_to_path_value = f"{merged_path.relative_to(Path.cwd())}"
-            except ValueError:
-                saved_to_path_value = merged_path
-            click.echo(f"Success! Saved to '{saved_to_path_value}'.")
+            if keep_segments and not preview_mode:
+                click.echo(
+                    "~ Segments are kept in '{}'.".format(
+                        try_get_relative_path(segments_output_directory)
+                    )
+                )
 
     run_temp_directory = playback.get_temp_directory()
-    if no_cleanup:
-        click.echo(f"notice: No cleanup enabled, check {run_temp_directory}/")
+    if keep_temp:
+        echo_notice(f"No cleanup enabled, check {run_temp_directory}")
     else:
         try:
             shutil.rmtree(run_temp_directory)
         except OSError:
             logger.warning(
-                "Failed to remove %s temporary directory", run_temp_directory
+                "Failed to remove temporary directory: %s", run_temp_directory
+            )
+
+    if not dry_run and not preview_mode:
+        resume_file_path.unlink()
+
+    if not (dry_run or keep_segments or preview_mode):
+        try:
+            for paths in audio_and_video_segment_paths:
+                for path in paths:
+                    path.unlink()
+        except OSError:
+            logger.warning("Could not remove segment: %s", path)
+        try:
+            if need_to_remove_segments_directory:
+                logger.debug(
+                    "Remove created segments directory: %s",
+                    segments_directory_to_remove,
+                )
+                remove_directories_between(
+                    segments_directory_to_remove, segments_output_directory
+                )
+        except OSError:
+            logger.warning(
+                "Could not remove segments directory: %s",
+                segments_directory_to_remove,
             )
```

### Comparing `ytpb-2024.4.20/src/ytpb/cli/commands/mpd.py` & `ytpb-2024.5.3/src/ytpb/cli/commands/mpd.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/utils/date.py` & `ytpb-2024.5.3/src/ytpb/utils/date.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/utils/other.py` & `ytpb-2024.5.3/src/ytpb/utils/other.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/utils/path.py` & `ytpb-2024.5.3/src/ytpb/utils/path.py`

 * *Files 4% similar despite different names*

```diff
@@ -257,7 +257,22 @@
             )
             if lowercase:
                 output = output.lower()
         case _:
             raise ValueError(f"Unknown title formatting style: '{style}'")
 
     return output
+
+
+def try_get_relative_path(path: Path, other: Path | None = None) -> Path:
+    try:
+        return path.relative_to(other or Path.cwd())
+    except ValueError:
+        return path
+
+
+def remove_directories_between(top: Path, until: Path) -> None:
+    until.rmdir()
+    directory = until.resolve()
+    while directory != top.resolve():
+        directory = directory.parent
+        directory.rmdir()
```

### Comparing `ytpb-2024.4.20/src/ytpb/utils/remote.py` & `ytpb-2024.5.3/src/ytpb/utils/remote.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/src/ytpb/utils/url.py` & `ytpb-2024.5.3/src/ytpb/utils/url.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/conftest.py` & `ytpb-2024.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/helpers.py` & `ytpb-2024.5.3/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/test_cache.py` & `ytpb-2024.5.3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/test_download.py` & `ytpb-2024.5.3/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/test_fetchers.py` & `ytpb-2024.5.3/tests/test_fetchers.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/test_locate.py` & `ytpb-2024.5.3/tests/test_locate.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/test_merge.py` & `ytpb-2024.5.3/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/test_playback.py` & `ytpb-2024.5.3/tests/test_playback.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/test_playback_session.py` & `ytpb-2024.5.3/tests/test_playback_session.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/test_representations.py` & `ytpb-2024.5.3/tests/test_representations.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/test_segment.py` & `ytpb-2024.5.3/tests/test_segment.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/test_streams.py` & `ytpb-2024.5.3/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/test_types.py` & `ytpb-2024.5.3/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/actions/test_compose.py` & `ytpb-2024.5.3/tests/actions/test_compose.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/actions/test_download.py` & `ytpb-2024.5.3/tests/actions/test_download.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,71 +32,73 @@
 
 
 def test_download_audio_segments(
     fake_info_fetcher: "FakeInfoFetcher",
     add_responses_callback_for_segment_urls: Callable,
     stream_url: str,
     audio_base_url: str,
-    run_temp_directory: Path,
+    tmp_path: Path,
 ) -> None:
     # Given:
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
     # When:
     playback = Playback(stream_url, fetcher=fake_info_fetcher)
     playback.fetch_and_set_essential()
     output_paths = actions.download.download_segments(
         playback,
-        FakeRewindInterval(FakeRewindMoment(7959120), FakeRewindMoment(7959121)),
-        [FakeStream(audio_base_url)],
+        sequence_numbers=range(7959120, 7959122),
+        streams=[FakeStream(audio_base_url)],
+        output_directory=tmp_path,
     )
 
     # Then:
     assert output_paths == [
         [
-            run_temp_directory / "segments/7959120.i140.mp4",
-            run_temp_directory / "segments/7959121.i140.mp4",
+            tmp_path / "7959120.i140.mp4",
+            tmp_path / "7959121.i140.mp4",
         ]
     ]
 
 
 def test_download_audio_and_video_segments(
     fake_info_fetcher: "FakeInfoFetcher",
     add_responses_callback_for_segment_urls: Callable,
     stream_url: str,
     audio_base_url: str,
     video_base_url: str,
-    run_temp_directory: Path,
+    tmp_path: Path,
 ) -> None:
     # Given:
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
         urljoin(video_base_url, r"sq/\w+"),
     )
 
     # When:
     playback = Playback(stream_url, fetcher=fake_info_fetcher)
     playback.fetch_and_set_essential()
     output_paths = actions.download.download_segments(
         playback,
-        FakeRewindInterval(FakeRewindMoment(7959120), FakeRewindMoment(7959121)),
-        [FakeStream(audio_base_url), FakeStream(video_base_url)],
+        sequence_numbers=range(7959120, 7959122),
+        streams=[FakeStream(audio_base_url), FakeStream(video_base_url)],
+        output_directory=tmp_path,
     )
 
     # Then:
     assert output_paths == [
         [
-            run_temp_directory / "segments/7959120.i140.mp4",
-            run_temp_directory / "segments/7959121.i140.mp4",
+            tmp_path / "7959120.i140.mp4",
+            tmp_path / "7959121.i140.mp4",
         ],
         [
-            run_temp_directory / "segments/7959120.i244.webm",
-            run_temp_directory / "segments/7959121.i244.webm",
+            tmp_path / "7959120.i244.webm",
+            tmp_path / "7959121.i244.webm",
         ],
     ]
 
 
 def test_download_audio_excerpt_with_cutting(
     fake_info_fetcher: "FakeInfoFetcher",
     add_responses_callback_for_segment_urls: Callable,
@@ -109,29 +111,29 @@
     add_responses_callback_for_segment_urls(urljoin(audio_base_url, r"sq/\w+"))
 
     # When:
     playback = Playback(stream_url, fetcher=fake_info_fetcher)
     playback.fetch_and_set_essential()
     output_result = actions.download.download_excerpt(
         playback,
-        FakeRewindInterval(
-            FakeRewindMoment(7959120, cut_at=0.5),
-            FakeRewindMoment(7959121, cut_at=1.5),
+        rewind_interval=FakeRewindInterval(
+            FakeRewindMoment(7959120, cut_at=0.5), FakeRewindMoment(7959121, cut_at=1.5)
         ),
-        tmp_path / "output",
-        FakeStream(audio_base_url),
+        output_stem=tmp_path / "output",
+        audio_stream=FakeStream(audio_base_url),
+        segments_directory=tmp_path / "segments",
     )
 
     # Then:
     assert output_result == (
         None,
         tmp_path / "output.mp4",
         [
-            run_temp_directory / "segments/7959120.i140.mp4",
-            run_temp_directory / "segments/7959121.i140.mp4",
+            tmp_path / "segments/7959120.i140.mp4",
+            tmp_path / "segments/7959121.i140.mp4",
         ],
         [],
     )
     assert_approx_duration(output_result[1], 3)
 
 
 def test_download_audio_and_video_excerpt_without_cutting(
@@ -149,31 +151,32 @@
     )
 
     # When:
     playback = Playback(stream_url, fetcher=fake_info_fetcher)
     playback.fetch_and_set_essential()
     output_result = actions.download.download_excerpt(
         playback,
-        FakeRewindInterval(
+        rewind_interval=FakeRewindInterval(
             FakeRewindMoment(7959120, cut_at=0.5),
             FakeRewindMoment(7959121, cut_at=1.5),
         ),
-        tmp_path / "output",
-        FakeStream(audio_base_url),
-        FakeStream(video_base_url),
+        output_stem=tmp_path / "output",
+        audio_stream=FakeStream(audio_base_url),
+        video_stream=FakeStream(video_base_url),
+        segments_directory=tmp_path / "segments",
         need_cut=False,
     )
 
     # Then:
     assert output_result == (
         None,
         tmp_path / "output.mkv",
         [
-            run_temp_directory / "segments/7959120.i140.mp4",
-            run_temp_directory / "segments/7959121.i140.mp4",
+            tmp_path / "segments/7959120.i140.mp4",
+            tmp_path / "segments/7959121.i140.mp4",
         ],
         [
-            run_temp_directory / "segments/7959120.i244.webm",
-            run_temp_directory / "segments/7959121.i244.webm",
+            tmp_path / "segments/7959120.i244.webm",
+            tmp_path / "segments/7959121.i244.webm",
         ],
     )
     assert_approx_duration(output_result[1], 4)
```

### Comparing `ytpb-2024.4.20/tests/cli/conftest.py` & `ytpb-2024.5.3/tests/cli/conftest.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 """ Fixtures for the CLI tests."""
 
 import contextlib
 import os
-from collections.abc import Callable
+import sys
+from collections.abc import Callable, Sequence
 from functools import partial
 from pathlib import Path
 
 import pytest
-from click.testing import CliRunner
+from click import Command
+from click.testing import CliRunner, Result
 
 from ytpb.cli import cli
 
 
+class CustomCliRunner(CliRunner):
+    def invoke(
+        self, cli: Command, args: str | Sequence[str] | None = None, **kwargs
+    ) -> Result:
+        sys.argv = args
+        return super().invoke(cli, args, **kwargs)
+
+
 @contextlib.contextmanager
 def isolated_filesystem(path: Path):
     old_cwd = Path.cwd()
     os.chdir(path)
     try:
         yield
     finally:
         os.chdir(old_cwd)
 
 
 @pytest.fixture()
 def ytpb_cli_invoke(tmp_path: Path) -> Callable:
-    runner = CliRunner()
+    runner = CustomCliRunner()
     with isolated_filesystem(tmp_path):
         yield partial(runner.invoke, cli)
```

### Comparing `ytpb-2024.4.20/tests/cli/test_download_command.py` & `ytpb-2024.5.3/tests/cli/test_download_command.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import glob
 import os
+import pickle
 import re
+import shutil
+from datetime import datetime, timezone
 from pathlib import Path
 from typing import Callable
 from unittest.mock import MagicMock, patch
 from urllib.parse import urljoin
 
 import click
-
 import pytest
-
+import responses
 import toml
-from freezegun import freeze_time
 
+from conftest import TEST_DATA_PATH
+from freezegun import freeze_time
 from helpers import assert_approx_duration
 
 from ytpb.config import DEFAULT_CONFIG
 from ytpb.ffmpeg import ffprobe_show_entries
+from ytpb.playback import RewindInterval, RewindMoment
 
 
 @pytest.mark.parametrize(
     "interval,output_subpath",
     [
         # Segments and corresponding ingestion start dates:
         #             7959120       21       22
@@ -116,112 +120,230 @@
                 "none",
                 stream_url,
             ],
         )
 
     # Then:
     assert result.exit_code == 0
-    expected_path = tmp_path / "Webcam-Zurich-HB_20230325T233354+00.mp4"
+    expected_path = tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4"
     assert os.path.exists(expected_path)
     assert_approx_duration(expected_path, 4.0)
 
 
+@pytest.mark.parametrize(
+    "interval",
+    [
+        "7959120/7959200",
+        "2023-03-25T23:33:55+00/2023-03-26T00+00",
+        "2023-03-25T23:33:55+00/PT1H",
+        "2023-03-25T23:33:55+00/7959200",
+        "PT3S/2023-03-25T23:33:58+00",
+        "PT3S/7959121",
+        "7959120/..",
+    ],
+)
 @freeze_time("2023-03-26T00:00:00+00:00")
-def test_preview_option_with_open_interval(
+def test_preview_start_option(
+    interval: str,
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
     stream_url: str,
     audio_base_url: str,
     tmp_path: Path,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
-        urljoin(audio_base_url, r"sq/\w+"),
+        urljoin(audio_base_url, "sq/7959203"),
+        urljoin(audio_base_url, "sq/7959120"),
+        urljoin(audio_base_url, "sq/7959121"),
+        urljoin(audio_base_url, "sq/7959122"),
     )
 
-    # We only have three test segments of 2 second duration.
     DEFAULT_CONFIG["general"]["preview_duration"] = 4
 
     # When:
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
                 "--no-config",
                 "download",
                 "--no-cache",
                 "--interval",
-                "2023-03-25T23:33:55+00/..",
-                "--preview",
+                interval,
+                "--preview-start",
                 "-af",
                 "itag eq 140",
                 "-vf",
                 "none",
                 stream_url,
             ],
+            catch_exceptions=False,
+            standalone_mode=False,
         )
 
     # Then:
     assert result.exit_code == 0
-    expected_path = tmp_path / "Webcam-Zurich-HB_20230325T233355+00.mp4"
-    assert os.path.exists(expected_path)
-    assert_approx_duration(expected_path, 5.5)
+    if not ".." in interval:
+        assert "~ Preview mode enabled, interval end is ignored." in result.output
+    assert os.path.exists(tmp_path / "Webcam-Zurich-HB_kHwmzef842g_preview.mp4")
 
 
+@pytest.mark.parametrize(
+    "interval",
+    [
+        "7959000/7959122",
+        "2023-03-24T00+00/2023-03-25T23:33:58.500+00",
+        "PT1H/2023-03-25T23:33:58.500+00",
+        "7959000/2023-03-25T23:33:58.500+00",
+        "2023-03-25T23:33:55.500+00/PT3S",
+        "7959121/PT3S",
+    ],
+)
 @freeze_time("2023-03-26T00:00:00+00:00")
-def test_preview_option_with_closed_interval(
+def test_preview_end_option(
+    interval: str,
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
     stream_url: str,
     audio_base_url: str,
     tmp_path: Path,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
+        urljoin(audio_base_url, "sq/7959203"),
+        urljoin(audio_base_url, "sq/7959120"),
+        urljoin(audio_base_url, "sq/7959121"),
+        urljoin(audio_base_url, "sq/7959122"),
+    )
+
+    DEFAULT_CONFIG["general"]["preview_duration"] = 4
+
+    # When:
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "--no-config",
+                "download",
+                "--no-cache",
+                "--interval",
+                interval,
+                "--preview-end",
+                "-af",
+                "itag eq 140",
+                "-vf",
+                "none",
+                stream_url,
+            ],
+        )
+
+    # Then:
+    assert result.exit_code == 0
+    assert "~ Preview mode enabled, interval start is ignored." in result.output
+    assert os.path.exists(tmp_path / "Webcam-Zurich-HB_kHwmzef842g_preview.mp4")
+
+
+@freeze_time("2023-03-26T00:00:00+00:00")
+def test_preview_and_output_option(
+    ytpb_cli_invoke: Callable,
+    add_responses_callback_for_reference_base_url: Callable,
+    add_responses_callback_for_segment_urls: Callable,
+    fake_info_fetcher: MagicMock,
+    stream_url: str,
+    audio_base_url: str,
+    tmp_path: Path,
+) -> None:
+    # Given:
+    add_responses_callback_for_reference_base_url()
+    add_responses_callback_for_segment_urls(
+        urljoin(audio_base_url, "sq/7959203"),
+        urljoin(audio_base_url, "sq/7959120"),
+        urljoin(audio_base_url, "sq/7959121"),
+        urljoin(audio_base_url, "sq/7959122"),
+    )
+
+    DEFAULT_CONFIG["general"]["preview_duration"] = 4
+
+    # When:
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "--no-config",
+                "download",
+                "--no-cache",
+                "--interval",
+                "7959120/7959200",
+                "--preview-start",
+                "--output",
+                "preview",
+                "-af",
+                "itag eq 140",
+                "-vf",
+                "none",
+                stream_url,
+            ],
+        )
+
+    # Then:
+    assert result.exit_code == 0
+    assert os.path.exists(tmp_path / "preview.mp4")
+
+
+@freeze_time("2023-03-26T00:00:00+00:00")
+def test_save_segments_to_temp_in_preview_mode(
+    ytpb_cli_invoke: Callable,
+    add_responses_callback_for_reference_base_url: Callable,
+    add_responses_callback_for_segment_urls: Callable,
+    fake_info_fetcher: MagicMock,
+    stream_url: str,
+    audio_base_url: str,
+    run_temp_directory: Path,
+) -> None:
+    # Given:
+    add_responses_callback_for_reference_base_url()
+    add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
     # We only have three test segments of 2 second duration.
     DEFAULT_CONFIG["general"]["preview_duration"] = 4
 
     # When:
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
                 "--no-config",
                 "download",
                 "--no-cache",
+                "--keep-temp",
                 "--interval",
-                "2023-03-25T23:33:55+00/2023-03-25T23:33:57:00+00",
-                "--preview",
+                "7959120/7959122",
+                "--preview-start",
                 "-af",
                 "itag eq 140",
                 "-vf",
                 "none",
                 stream_url,
             ],
             catch_exceptions=False,
         )
 
     # Then:
     assert result.exit_code == 0
-
-    expected_path = tmp_path / "Webcam-Zurich-HB_20230325T233355+00.mp4"
-    assert os.path.exists(expected_path)
-    assert_approx_duration(expected_path, 5.5)
-
-    expected = "info: The preview mode is enabled, interval end is ignored."
-    assert expected in result.output
+    assert os.path.exists(run_temp_directory / "7959120.i140.mp4")
+    assert os.path.exists(run_temp_directory / "7959121.i140.mp4")
 
 
 @pytest.mark.parametrize(
     "audio_format,video_format",
     [("itag eq 140", "itag eq 244"), ("itag eq 140", "none"), ("none", "itag eq 244")],
 )
 @freeze_time("2023-03-26T00:00:00+00:00")
@@ -256,28 +378,22 @@
                 "--no-cut",
                 "--interval",
                 "7959120/7959121",
                 "-af",
                 audio_format,
                 "-vf",
                 video_format,
-                "--no-cleanup",
                 stream_url,
             ],
             catch_exceptions=False,
         )
 
     # Then:
     assert result.exit_code == 0
-    expected_output = re.sub(
-        r"notice: No cleanup enabled, check .+",
-        f"notice: No cleanup enabled, check {run_temp_directory}/",
-        expected_out._pattern_filename.read_text(),
-    )
-    assert expected_output == result.output
+    assert expected_out == result.output
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_download_to_custom_absolute_path(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
@@ -407,20 +523,20 @@
 
     # Then:
     assert result.exit_code == 0
     assert expected == str(next(tmp_path.glob("*.mp4")).name)
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
-def test_no_cleanup_option(
+def test_keep_temp_option(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
-    stream_url: str,
+    video_id: str,
     audio_base_url: str,
     tmp_path: Path,
     run_temp_directory: Path,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
@@ -431,28 +547,30 @@
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
                 "--no-config",
                 "download",
                 "--no-cache",
+                "--keep-temp",
                 "--interval",
                 "7959120/7959121",
                 "-af",
                 "itag eq 140",
                 "-vf",
                 "none",
-                "--no-cleanup",
-                stream_url,
+                video_id,
             ],
         )
 
     # Then:
     assert result.exit_code == 0
-    assert os.path.exists(tmp_path / "Webcam-Zurich-HB_20230325T233354+00.mp4")
+    assert os.path.exists(
+        tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4"
+    )
     assert os.path.exists(run_temp_directory / "7959120.i140.mp4")
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_no_merge_option(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
@@ -460,17 +578,14 @@
     fake_info_fetcher: MagicMock,
     stream_url: str,
     audio_base_url: str,
     tmp_path: Path,
     run_temp_directory: Path,
     expected_out,
 ) -> None:
-    """The expected output file for this test contains a template variable, and
-    needs to be updated manually."""
-
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
     # When:
@@ -490,28 +605,19 @@
                 "--no-merge",
                 stream_url,
             ],
         )
 
     # Then:
     assert result.exit_code == 0
-    assert not os.path.exists(tmp_path / "Webcam-Zurich-HB_20230325T233354+00.mp4")
-    assert os.path.exists(run_temp_directory / "7959120.i140.mp4")
-
-    expected_output = re.sub(
-        r"Success! Segments saved to .+\.",
-        f"Success! Segments saved to {run_temp_directory}/segments/.",
-        expected_out._pattern_filename.read_text(),
-    )
-    expected_output = re.sub(
-        r"notice: No cleanup enabled, check .+",
-        f"notice: No cleanup enabled, check {run_temp_directory}/",
-        expected_output,
+    assert not os.path.exists(
+        tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4"
     )
-    assert expected_output == result.output
+    assert not os.path.exists(run_temp_directory)
+    assert expected_out == result.output
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_dry_run_option(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
@@ -546,15 +652,17 @@
                 stream_url,
             ],
         )
 
     # Then:
     assert result.exit_code == 0
     assert result.output == expected_out
-    assert not os.path.exists(tmp_path / "Webcam-Zurich-HB_20230325T233355+00.mp4")
+    assert not os.path.exists(
+        tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4"
+    )
     assert not os.path.exists(run_temp_directory)
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_no_cut_option(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
@@ -589,15 +697,15 @@
                 "--no-cut",
                 stream_url,
             ],
         )
 
     # Then:
     assert result.exit_code == 0
-    expected_path = tmp_path / "Webcam-Zurich-HB_20230325T233355+00.mp4"
+    expected_path = tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4"
     assert os.path.exists(expected_path)
     assert_approx_duration(expected_path, 4.0)
 
     assert result.output == expected_out
 
 
 @freeze_time("2023-09-28T17:00:00+00:00")
@@ -674,15 +782,15 @@
                 "none",
                 stream_url,
             ],
         )
 
     # Then:
     assert result.exit_code == 0
-    expected_path = tmp_path / "Webcam-Zurich-HB_20230325T233354+00.mp4"
+    expected_path = tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4"
     assert os.path.exists(expected_path)
 
 
 @pytest.mark.parametrize(
     "audio_format,video_format",
     [
         ("format eq mp4", "quality gt 360p"),
@@ -758,15 +866,15 @@
                 "-vf",
                 "none",
                 stream_url,
             ],
         )
 
     assert result.exit_code == 0
-    expected_path = tmp_path / "Webcam-Zurich-HB_20230325T233354+00.mp4"
+    expected_path = tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4"
     assert os.path.exists(expected_path)
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_with_default_config_file(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
@@ -1417,15 +1525,17 @@
             ],
             catch_exceptions=False,
             standalone_mode=False,
         )
 
     # Then:
     format_tags = ffprobe_show_entries(
-        tmp_path / "Webcam-Zurich-HB_20230325T233355+00.mp4", "format_tags", "default"
+        tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4",
+        "format_tags",
+        "default",
     )
     assert "TAG:title=Webcam Zürich HB" in format_tags
     assert "TAG:author=David Gubler" in format_tags
     assert f"TAG:comment={stream_url}" in format_tags
     assert "TAG:input_start_time=1679787235.000000" in format_tags
     assert "TAG:input_end_time=1679787237.000000" in format_tags
     assert "TAG:actual_start_time=1679787235.000000" in format_tags
@@ -1470,18 +1580,471 @@
             ],
             catch_exceptions=False,
             standalone_mode=False,
         )
 
     # Then:
     format_tags = ffprobe_show_entries(
-        tmp_path / "Webcam-Zurich-HB_20230325T233355+00.mp4", "format_tags", "default"
+        tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4",
+        "format_tags",
+        "default",
     )
     assert "TAG:title=Webcam Zürich HB" in format_tags
     assert "TAG:author=David Gubler" in format_tags
     assert f"TAG:comment={stream_url}" in format_tags
     assert "TAG:input_start_time=1679787235.000000" in format_tags
     assert "TAG:input_end_time=1679787237.000000" in format_tags
     assert "TAG:actual_start_time=1679787234.491176" in format_tags
     assert "TAG:actual_end_time=1679787238.486826" in format_tags
     assert "TAG:start_sequence_number=7959120" in format_tags
     assert "TAG:end_sequence_number=7959121" in format_tags
+
+
+@freeze_time("2023-03-26T00:00:00+00:00")
+def test_resume_downloading(
+    ytpb_cli_invoke: Callable,
+    add_responses_callback_for_reference_base_url: Callable,
+    add_responses_callback_for_segment_urls: Callable,
+    mocked_responses: responses.RequestsMock,
+    fake_info_fetcher: MagicMock,
+    video_id: str,
+    audio_base_url: str,
+    tmp_path: Path,
+    expected_out,
+) -> None:
+    # Given:
+    add_responses_callback_for_reference_base_url()
+    add_responses_callback_for_segment_urls(
+        urljoin(audio_base_url, r"sq/\w+"),
+    )
+
+    resume_file_stem = f"{video_id}-7959120-20230325T233359+00-140"
+    with open(f"{resume_file_stem}.resume", "wb") as f:
+        end_date = datetime.fromisoformat("2023-03-25T23:33:59+00")
+        pickle.dump(
+            {
+                "interval": RewindInterval(
+                    start=RewindMoment(
+                        date=datetime.fromtimestamp(1679787234.491176, timezone.utc),
+                        sequence=7959120,
+                        cut_at=0,
+                        is_end=False,
+                    ),
+                    end=RewindMoment(
+                        date=end_date,
+                        sequence=7959122,
+                        cut_at=0,
+                        is_end=True,
+                    ),
+                ),
+                "segments_output_directory": Path(f"{resume_file_stem}"),
+            },
+            f,
+        )
+    segments_output_directory = tmp_path / f"{resume_file_stem}"
+    segments_output_directory.mkdir()
+    for segment in (7959120, 7959121):
+        shutil.copy(
+            TEST_DATA_PATH / f"segments/{segment}.i140.mp4",
+            segments_output_directory / f"{segment}.i140.mp4",
+        )
+
+    # When:
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "--no-config",
+                "download",
+                "--no-cache",
+                "--no-cut",
+                "--interval",
+                "7959120/2023-03-25T23:33:59+00",
+                "-af",
+                "itag eq 140",
+                "-vf",
+                "none",
+                video_id,
+            ],
+            catch_exceptions=False,
+            standalone_mode=False,
+        )
+
+    # Then:
+    assert result.exit_code == 0
+    assert (
+        f"~ Found unfinished download, continue from {resume_file_stem}.resume"
+    ) in result.output
+    expected_path = tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4"
+    assert os.path.exists(expected_path)
+    assert_approx_duration(expected_path, 6)
+    assert not os.path.exists(tmp_path / f"{resume_file_stem}")
+
+
+@freeze_time("2023-03-26T00:00:00+00:00")
+def test_keep_segments(
+    ytpb_cli_invoke: Callable,
+    add_responses_callback_for_reference_base_url: Callable,
+    add_responses_callback_for_segment_urls: Callable,
+    mocked_responses: responses.RequestsMock,
+    fake_info_fetcher: MagicMock,
+    video_id: str,
+    audio_base_url: str,
+    tmp_path: Path,
+    expected_out,
+) -> None:
+    # Given:
+    add_responses_callback_for_reference_base_url()
+    add_responses_callback_for_segment_urls(
+        urljoin(audio_base_url, r"sq/\w+"),
+    )
+
+    # When:
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "--no-config",
+                "download",
+                "--no-cache",
+                "--no-cut",
+                "--keep-segments",
+                "--interval",
+                "7959120/7959121",
+                "-af",
+                "itag eq 140",
+                "-vf",
+                "none",
+                video_id,
+            ],
+            catch_exceptions=False,
+            standalone_mode=False,
+        )
+
+    # Then:
+    assert result.exit_code == 0
+    segments_directory = tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00"
+    assert os.path.exists(segments_directory / "7959120.i140.mp4")
+    assert os.path.exists(segments_directory / "7959121.i140.mp4")
+
+
+@freeze_time("2023-03-26T00:00:00+00:00")
+def test_remove_default_segments_output_directory(
+    ytpb_cli_invoke: Callable,
+    add_responses_callback_for_reference_base_url: Callable,
+    add_responses_callback_for_segment_urls: Callable,
+    mocked_responses: responses.RequestsMock,
+    fake_info_fetcher: MagicMock,
+    video_id: str,
+    audio_base_url: str,
+    tmp_path: Path,
+    expected_out,
+) -> None:
+    # Given:
+    add_responses_callback_for_reference_base_url()
+    add_responses_callback_for_segment_urls(
+        urljoin(audio_base_url, r"sq/\w+"),
+    )
+
+    # When:
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "--no-config",
+                "download",
+                "--no-cache",
+                "--no-cut",
+                "--interval",
+                "7959120/7959121",
+                "-af",
+                "itag eq 140",
+                "-vf",
+                "none",
+                video_id,
+            ],
+            catch_exceptions=False,
+            standalone_mode=False,
+        )
+
+    # Then:
+    assert result.exit_code == 0
+    assert not os.path.exists(tmp_path / f"{video_id}-7959120-7959121-140")
+
+
+@pytest.mark.parametrize("segments_output_dir_option", ["a", "a/b", "./a", "../a/b"])
+@freeze_time("2023-03-26T00:00:00+00:00")
+def test_remove_created_segments_output_directory(
+    segments_output_dir_option: str,
+    monkeypatch: pytest.MonkeyPatch,
+    ytpb_cli_invoke: Callable,
+    add_responses_callback_for_reference_base_url: Callable,
+    add_responses_callback_for_segment_urls: Callable,
+    mocked_responses: responses.RequestsMock,
+    fake_info_fetcher: MagicMock,
+    video_id: str,
+    audio_base_url: str,
+    tmp_path: Path,
+    expected_out,
+) -> None:
+    # Given:
+    sub_tmp_path = tmp_path / "sub"
+    sub_tmp_path.mkdir()
+    monkeypatch.chdir(sub_tmp_path)
+
+    segments_output_directory = sub_tmp_path / segments_output_dir_option
+
+    add_responses_callback_for_reference_base_url()
+    add_responses_callback_for_segment_urls(
+        urljoin(audio_base_url, r"sq/\w+"),
+    )
+
+    # When:
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "--no-config",
+                "download",
+                "--no-cache",
+                "--no-cut",
+                "--interval",
+                "7959120/7959121",
+                "-af",
+                "itag eq 140",
+                "-vf",
+                "none",
+                "--segments-output-dir",
+                segments_output_dir_option,
+                video_id,
+            ],
+            catch_exceptions=False,
+            standalone_mode=False,
+        )
+
+    # Then:
+    assert result.exit_code == 0
+    if len(segments_output_directory.parts) > 1:
+        assert not os.path.exists(segments_output_directory)
+    else:
+        assert not os.path.exists(segments_output_directory.parent)
+
+
+def test_remove_only_rewound_segments(
+    ytpb_cli_invoke: Callable,
+    add_responses_callback_for_reference_base_url: Callable,
+    add_responses_callback_for_segment_urls: Callable,
+    mocked_responses: responses.RequestsMock,
+    fake_info_fetcher: MagicMock,
+    video_id: str,
+    audio_base_url: str,
+    tmp_path: Path,
+    expected_out,
+) -> None:
+    # Given:
+    add_responses_callback_for_reference_base_url()
+    add_responses_callback_for_segment_urls(
+        urljoin(audio_base_url, r"sq/\w+"),
+    )
+
+    segments_directory = tmp_path / f"{video_id}-7959120-7959121-140"
+    segments_directory.mkdir()
+    open(segments_directory / "0.i140.mp4", "x")
+
+    # When:
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "--no-config",
+                "download",
+                "--no-cache",
+                "--no-cut",
+                "--interval",
+                "7959120/7959121",
+                "-af",
+                "itag eq 140",
+                "-vf",
+                "none",
+                video_id,
+            ],
+            catch_exceptions=False,
+            standalone_mode=False,
+        )
+
+    # Then:
+    assert result.exit_code == 0
+    assert os.path.exists(segments_directory / "0.i140.mp4")
+    assert not os.path.exists(segments_directory / "7959120.i140.mp4")
+
+
+@freeze_time("2023-03-26T00:00:00+00:00")
+def test_do_not_remove_existing_directory(
+    ytpb_cli_invoke: Callable,
+    add_responses_callback_for_reference_base_url: Callable,
+    add_responses_callback_for_segment_urls: Callable,
+    mocked_responses: responses.RequestsMock,
+    fake_info_fetcher: MagicMock,
+    video_id: str,
+    audio_base_url: str,
+    tmp_path: Path,
+    expected_out,
+) -> None:
+    # Given:
+    add_responses_callback_for_reference_base_url()
+    add_responses_callback_for_segment_urls(
+        urljoin(audio_base_url, r"sq/\w+"),
+    )
+
+    segments_directory = tmp_path / "existing"
+    segments_directory.mkdir()
+
+    # When:
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "--no-config",
+                "download",
+                "--no-cache",
+                "--no-cut",
+                "--interval",
+                "7959120/7959121",
+                "-af",
+                "itag eq 140",
+                "-vf",
+                "none",
+                "--segments-output-dir",
+                "existing",
+                video_id,
+            ],
+            catch_exceptions=False,
+            standalone_mode=False,
+        )
+
+    # Then:
+    assert result.exit_code == 0
+    assert os.path.exists(segments_directory)
+    assert not os.path.exists(segments_directory / "7959120.i140.mp4")
+
+
+@freeze_time("2023-03-26T00:00:00+00:00")
+def test_ignore_resume_option(
+    ytpb_cli_invoke: Callable,
+    add_responses_callback_for_reference_base_url: Callable,
+    add_responses_callback_for_segment_urls: Callable,
+    mocked_responses: responses.RequestsMock,
+    fake_info_fetcher: MagicMock,
+    video_id: str,
+    audio_base_url: str,
+    tmp_path: Path,
+    expected_out,
+) -> None:
+    # Given:
+    add_responses_callback_for_reference_base_url()
+    add_responses_callback_for_segment_urls(
+        urljoin(audio_base_url, r"sq/\w+"),
+    )
+
+    # When:
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "--no-config",
+                "download",
+                "--no-cache",
+                "--no-cut",
+                "--ignore-resume",
+                "--interval",
+                "7959120/7959121",
+                "-af",
+                "itag eq 140",
+                "-vf",
+                "none",
+                video_id,
+            ],
+            catch_exceptions=False,
+            standalone_mode=False,
+        )
+
+    # Then:
+    assert result.exit_code == 0
+
+
+@freeze_time("2023-03-26T00:00:00+00:00")
+def test_ignore_resume_option_after_unfinished_run(
+    ytpb_cli_invoke: Callable,
+    add_responses_callback_for_reference_base_url: Callable,
+    add_responses_callback_for_segment_urls: Callable,
+    mocked_responses: responses.RequestsMock,
+    fake_info_fetcher: MagicMock,
+    video_id: str,
+    audio_base_url: str,
+    tmp_path: Path,
+    expected_out,
+) -> None:
+    # Given:
+    add_responses_callback_for_reference_base_url()
+    add_responses_callback_for_segment_urls(
+        urljoin(audio_base_url, r"sq/\w+"),
+    )
+
+    resume_file_stem = f"{video_id}-7959120-7959122-140"
+    with open(f"{resume_file_stem}.resume", "wb") as f:
+        pickle.dump(
+            {
+                "interval": RewindInterval(
+                    start=RewindMoment(
+                        date=datetime.fromtimestamp(1679787234.491176, timezone.utc),
+                        sequence=7959120,
+                        cut_at=0,
+                        is_end=False,
+                    ),
+                    end=RewindMoment(
+                        date=datetime.fromtimestamp(1679787238.491916, timezone.utc),
+                        sequence=7959122,
+                        cut_at=0,
+                        is_end=True,
+                    ),
+                ),
+                "segments_output_directory": Path(f"{resume_file_stem}"),
+            },
+            f,
+        )
+    segments_output_directory = tmp_path / f"{resume_file_stem}"
+    segments_output_directory.mkdir()
+    for segment in (7959120, 7959121):
+        shutil.copy(
+            TEST_DATA_PATH / f"segments/{segment}.i140.mp4",
+            segments_output_directory / f"{segment}.i140.mp4",
+        )
+
+    # When:
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "--no-config",
+                "download",
+                "--no-cache",
+                "--no-cut",
+                "--ignore-resume",
+                "--segments-output-dir",
+                "segments",
+                "--keep-segments",
+                "--interval",
+                "7959120/7959122",
+                "-af",
+                "itag eq 140",
+                "-vf",
+                "none",
+                video_id,
+            ],
+            catch_exceptions=False,
+            standalone_mode=False,
+        )
+
+    # Then:
+    assert result.exit_code == 0
+    assert os.path.exists(tmp_path / f"{video_id}-7959120-7959122-140")
+    assert os.path.exists(tmp_path / "segments")
```

### Comparing `ytpb-2024.4.20/tests/cli/test_parameters.py` & `ytpb-2024.5.3/tests/cli/test_parameters.py`

 * *Files 10% similar despite different names*

```diff
@@ -83,14 +83,18 @@
         ),
         ("PT30S/now", (timedelta(seconds=30), "now")),
         (
             "20240102T102000+00/..",
             (datetime(2024, 1, 2, 10, 20, tzinfo=timezone.utc), ".."),
         ),
         (
+            "../20240102T102000+00",
+            ("..", datetime(2024, 1, 2, 10, 20, tzinfo=timezone.utc)),
+        ),
+        (
             "@1704190800/@1704190830.123",
             (
                 datetime(2024, 1, 2, 10, 20, 0, tzinfo=timezone.utc),
                 datetime(2024, 1, 2, 10, 20, 30, 123000, tzinfo=timezone.utc),
             ),
         ),
     ],
@@ -147,7 +151,24 @@
         ("20240102T102030+00/PT30", "PT30"),
     ],
 )
 def test_invalid_rewind_interval(value: str, invalid_part: str):
     with pytest.raises(click.BadParameter) as exc_info:
         RewindIntervalParamType().convert(value, None, None)
     assert invalid_part in str(exc_info.value)
+
+
+@pytest.mark.parametrize(
+    "interval,error",
+    [
+        ("PT10M/PT20M", "Two durations"),
+        ("../..", "Two '..'"),
+        ("PT1H/..", "Keyword '..'"),
+        ("../PT1H", "Keyword '..'"),
+        ("2024Y/PT1H", "Replacement components"),
+        ("2024Y/..", "Replacement components"),
+    ],
+)
+def test_non_compatible_interval_parts(interval: str, error: str):
+    with pytest.raises(click.BadParameter) as exc_info:
+        RewindIntervalParamType().convert(interval, None, None)
+    assert error in str(exc_info.value)
```

### Comparing `ytpb-2024.4.20/tests/cli/capture/test_frame_command.py` & `ytpb-2024.5.3/tests/cli/capture/test_frame_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                 "-vf",
                 "itag eq 244",
                 stream_url,
             ],
         )
 
     assert result.exit_code == 0
-    actual_image_path = tmp_path / "Webcam-Zurich-HB_20230325T233354+00.jpg"
+    actual_image_path = tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.jpg"
     assert os.path.exists(actual_image_path)
 
     segment_path = TEST_DATA_PATH / "segments" / "7959120.i244.webm"
     assert_two_images(actual_image_path, segment_path, expected_frame=0)
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
@@ -110,15 +110,15 @@
                 "itag eq 244",
                 stream_url,
             ],
             catch_exceptions=False,
             standalone_mode=False,
         )
     assert result.exit_code == 0
-    actual_image_path = tmp_path / "Webcam-Zurich-HB_20230325T233355+00.jpg"
+    actual_image_path = tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.jpg"
     assert os.path.exists(actual_image_path)
 
     segment_path = TEST_DATA_PATH / "segments" / "7959120.i244.webm"
     assert_two_images(actual_image_path, segment_path, expected_frame=15)
 
 
 def test_unsupported_output_extension(
```

### Comparing `ytpb-2024.4.20/tests/cli/mpd/test_compose_command.py` & `ytpb-2024.5.3/tests/cli/mpd/test_compose_command.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/cli/mpd/test_refresh_command.py` & `ytpb-2024.5.3/tests/cli/mpd/test_refresh_command.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/data/info-1695928670.json` & `ytpb-2024.5.3/tests/data/info-1695928670.json`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/data/manifest-1695928670.mpd` & `ytpb-2024.5.3/tests/data/manifest-1695928670.mpd`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/data/webpage-1695928670.html` & `ytpb-2024.5.3/tests/data/webpage-1695928670.html`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244].out` & `ytpb-2024.5.3/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244].out`

 * *Files 15% similar despite different names*

```diff
@@ -13,9 +13,9 @@
     244     | webm          | vp9           | 480p          
 
 (<<) Locating start and end in the stream... done.
 Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Composing MPEG-DASH manifest...
-Success! Saved to 'Webcam-Zurich-HB_20230325T233354+00.mpd'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mpd'.
 ~ Note that the manifest will expire in 6 hours.
```

### Comparing `ytpb-2024.4.20/tests/data/expected/test_compose_mpd[itag%20eq%20140-none].out` & `ytpb-2024.5.3/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244].out`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Run playback for https://www.youtube.com/watch?v=kHwmzef842g
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
-This representation will be in the manifest:
-                          (Audio)                           
-    itag    | Format        | Codec         | Sampling      
+These 2 representations will be in the manifest:
+                          (Video)                           
+    itag    | Format        | Codec         | Quality       
 ------------|---------------|---------------|---------------
-    140     | mp4           | mp4a.40.2     | 44100 Hz      
+    243     | webm          | vp9           | 360p          
+    244     | webm          | vp9           | 480p          
 
 (<<) Locating start and end in the stream... done.
 Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Composing MPEG-DASH manifest...
-Success! Saved to 'Webcam-Zurich-HB_20230325T233354+00.mpd'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mpd'.
 ~ Note that the manifest will expire in 6 hours.
```

### Comparing `ytpb-2024.4.20/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244].out` & `ytpb-2024.5.3/tests/data/expected/test_compose_mpd[itag%20eq%20140-none].out`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Run playback for https://www.youtube.com/watch?v=kHwmzef842g
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
-These 2 representations will be in the manifest:
-                          (Video)                           
-    itag    | Format        | Codec         | Quality       
+This representation will be in the manifest:
+                          (Audio)                           
+    itag    | Format        | Codec         | Sampling      
 ------------|---------------|---------------|---------------
-    243     | webm          | vp9           | 360p          
-    244     | webm          | vp9           | 480p          
+    140     | mp4           | mp4a.40.2     | 44100 Hz      
 
 (<<) Locating start and end in the stream... done.
 Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Composing MPEG-DASH manifest...
-Success! Saved to 'Webcam-Zurich-HB_20230325T233354+00.mpd'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mpd'.
 ~ Note that the manifest will expire in 6 hours.
```

### Comparing `ytpb-2024.4.20/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244].out` & `ytpb-2024.5.3/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244].out`

 * *Files 12% similar despite different names*

```diff
@@ -11,9 +11,8 @@
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
    - Video ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (no cut requested)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_20230325T233354+00.mkv'.
-notice: No cleanup enabled, check /tmp/pytest-of-ms/pytest-4/test_download_audio_and_or_vid0/tmpe21_1mta/
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mkv'.
```

### Comparing `ytpb-2024.4.20/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244].out` & `ytpb-2024.5.3/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244].out`

 * *Files 14% similar despite different names*

```diff
@@ -9,9 +9,8 @@
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Video ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (no cut requested)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_20230325T233354+00.webm'.
-notice: No cleanup enabled, check /tmp/pytest-of-ms/pytest-4/test_download_audio_and_or_vid2/tmpmunjanzh/
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.webm'.
```

### Comparing `ytpb-2024.4.20/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4].out` & `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4].out`

 * *Files 3% similar despite different names*

```diff
@@ -9,8 +9,8 @@
   Actual end: 25 Mar 2023 23:33:57 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (may take a while)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_20230325T233355+00.mp4'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4'.
```

### Comparing `ytpb-2024.4.20/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4].out` & `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4].out`

 * *Files 4% similar despite different names*

```diff
@@ -9,8 +9,8 @@
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (may take a while)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_20230325T233355+00.mp4'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4'.
```

### Comparing `ytpb-2024.4.20/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4].out` & `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4].out`

 * *Files 4% similar despite different names*

```diff
@@ -9,8 +9,8 @@
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (may take a while)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_20230325T233355+00.mp4'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4'.
```

### Comparing `ytpb-2024.4.20/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4].out` & `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4].out`

 * *Files 4% similar despite different names*

```diff
@@ -9,8 +9,8 @@
   Actual end: 25 Mar 2023 23:33:57 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (may take a while)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_20230325T233354+00.mp4'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4'.
```

### Comparing `ytpb-2024.4.20/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4].out` & `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4].out`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
    - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
 Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
-  Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
+  Actual end: 25 Mar 2023 23:33:57 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (may take a while)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_20230325T233354+00.mp4'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4'.
```

### Comparing `ytpb-2024.4.20/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4].out` & `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4].out`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
    - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
 Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
-  Actual end: 25 Mar 2023 23:33:57 +0000, seq. 7959121
+  Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (may take a while)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_20230325T233354+00.mp4'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4'.
```

### Comparing `ytpb-2024.4.20/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4].out` & `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4].out`

 * *Files 4% similar despite different names*

```diff
@@ -9,8 +9,8 @@
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (may take a while)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_20230325T233355+00.mp4'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4'.
```

### Comparing `ytpb-2024.4.20/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4].out` & `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4].out`

 * *Files 4% similar despite different names*

```diff
@@ -9,8 +9,8 @@
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (may take a while)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_20230325T233355+00.mp4'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4'.
```

### Comparing `ytpb-2024.4.20/tests/data/expected/test_no_cut_option.out` & `ytpb-2024.5.3/tests/data/expected/test_no_merge_option.out`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Run playback for https://www.youtube.com/watch?v=kHwmzef842g
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
    - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
-Actual start: 25 Mar 2023 23:33:54 +0000 (-00:01), seq. 7959120
+Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
-(<<) Preparing and saving the excerpt...
-1. Downloading segments 7959120-7959121:
+(<<) Downloading segments 7959120-7959121 (no merge requested)...
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
-2. Merging segments (no cut requested)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_20230325T233355+00.mp4'.
+Success! Segments saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00'.
```

### Comparing `ytpb-2024.4.20/tests/data/gap-cases/gap-case-1-fixture.csv` & `ytpb-2024.5.3/tests/data/gap-cases/gap-case-1-fixture.csv`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/data/gap-cases/gap-case-2-fixture.csv` & `ytpb-2024.5.3/tests/data/gap-cases/gap-case-2-fixture.csv`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/data/gap-cases/gap-case-3-fixture.csv` & `ytpb-2024.5.3/tests/data/gap-cases/gap-case-3-fixture.csv`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/data/segments/7959120.i140.mp4` & `ytpb-2024.5.3/tests/data/segments/7959120.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/data/segments/7959120.i244.webm` & `ytpb-2024.5.3/tests/data/segments/7959120.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/data/segments/7959121.i140.mp4` & `ytpb-2024.5.3/tests/data/segments/7959121.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/data/segments/7959121.i244.webm` & `ytpb-2024.5.3/tests/data/segments/7959121.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/data/segments/7959122.i140.mp4` & `ytpb-2024.5.3/tests/data/segments/7959122.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/data/segments/7959122.i244.webm` & `ytpb-2024.5.3/tests/data/segments/7959122.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/data/segments/7959123.i140.mp4` & `ytpb-2024.5.3/tests/data/segments/7959123.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/data/segments/7959123.i244.webm` & `ytpb-2024.5.3/tests/data/segments/7959123.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/data/segments/7959203.i140.mp4` & `ytpb-2024.5.3/tests/data/segments/7959203.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/data/segments/7959203.i244.webm` & `ytpb-2024.5.3/tests/data/segments/7959203.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/utils/test_date.py` & `ytpb-2024.5.3/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/utils/test_path.py` & `ytpb-2024.5.3/tests/utils/test_path.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/utils/test_remote.py` & `ytpb-2024.5.3/tests/utils/test_remote.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/tests/utils/test_url.py` & `ytpb-2024.5.3/tests/utils/test_url.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/.gitignore` & `ytpb-2024.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/LICENSE` & `ytpb-2024.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.20/README.rst` & `ytpb-2024.5.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -55,22 +55,26 @@
 
 - Downloading a live stream excerpt (`link <https://asciinema.org/a/653861>`__)
 - Composing an MPEG-DASH MPD and transcoding it to MP4 (`link
   <https://asciinema.org/a/653865>`__)
 - Creating a time-lapse of a live stream excerpt (`link
   <https://asciinema.org/a/653869>`__)
 
-Install
-*******
+Installation
+************
 
 Ytpb requires Python 3.11 or higher. The recommended way is to use `pipx
-<https://pypa.github.io/pipx/>`_: ::
+<https://pypa.github.io/pipx/>`_::
 
   $ pipx install ytpb
 
+To upgrade to the newer version, do::
+
+  $ pipx upgrade ytpb
+
 Further reading
 ***************
 
 After installing, check out the `documentation`_. The `Why Ytpb?`_ page explains
 why the project exists. For main usage scenarios, see `Quick start`_. The
 `Command line application`_ page goes deeper into the usage. `Reference`_
 provides some general aspects and terms. `Cookbook`_ contains some useful
```

### Comparing `ytpb-2024.4.20/pyproject.toml` & `ytpb-2024.5.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [ "hatchling", "hatch-vcs" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "ytpb"
 description = "A playback for YouTube live streams"
 readme = "README.rst"
-version = "2024.4.20"
+version = "2024.5.3"
 authors = [ { name = "Maxim Stolyarchuk" } ]
 keywords = [ "youtube" ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Console",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.11",
```

### Comparing `ytpb-2024.4.20/PKG-INFO` & `ytpb-2024.5.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ytpb
-Version: 2024.4.20
+Version: 2024.5.3
 Summary: A playback for YouTube live streams
 Project-URL: Source, https://github.com/xymaxim/ytpb
 Project-URL: Documentation, https://ytpb.readthedocs.io
 Author: Maxim Stolyarchuk
 License: MIT License
         
         Copyright (c) 2024 Maxim Stolyarchuk
@@ -47,16 +47,20 @@
 Requires-Dist: rich>=13.7.0
 Requires-Dist: structlog>=23.3.0
 Requires-Dist: timedelta-isoformat>=0.6.2.11
 Requires-Dist: toml>=0.10.2
 Requires-Dist: unidecode>=1.3.7
 Requires-Dist: yt-dlp>=2023.12.30
 Provides-Extra: dev
+Requires-Dist: freezegun>=1.4.0; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
-Requires-Dist: ytpb[test]; extra == 'dev'
+Requires-Dist: pytest-matcher==2.0.1; extra == 'dev'
+Requires-Dist: pytest-socket>=0.6.0; extra == 'dev'
+Requires-Dist: pytest>=7.4.4; extra == 'dev'
+Requires-Dist: responses>=0.24.1; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: sphinx-toolbox==3.5.0; extra == 'docs'
 Requires-Dist: sphinx==7.2.6; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: freezegun>=1.4.0; extra == 'test'
 Requires-Dist: pytest-matcher==2.0.1; extra == 'test'
 Requires-Dist: pytest-socket>=0.6.0; extra == 'test'
@@ -121,22 +125,26 @@
 
 - Downloading a live stream excerpt (`link <https://asciinema.org/a/653861>`__)
 - Composing an MPEG-DASH MPD and transcoding it to MP4 (`link
   <https://asciinema.org/a/653865>`__)
 - Creating a time-lapse of a live stream excerpt (`link
   <https://asciinema.org/a/653869>`__)
 
-Install
-*******
+Installation
+************
 
 Ytpb requires Python 3.11 or higher. The recommended way is to use `pipx
-<https://pypa.github.io/pipx/>`_: ::
+<https://pypa.github.io/pipx/>`_::
 
   $ pipx install ytpb
 
+To upgrade to the newer version, do::
+
+  $ pipx upgrade ytpb
+
 Further reading
 ***************
 
 After installing, check out the `documentation`_. The `Why Ytpb?`_ page explains
 why the project exists. For main usage scenarios, see `Quick start`_. The
 `Command line application`_ page goes deeper into the usage. `Reference`_
 provides some general aspects and terms. `Cookbook`_ contains some useful
```

