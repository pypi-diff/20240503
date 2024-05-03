# Comparing `tmp/manim_slides-5.1.6.tar.gz` & `tmp/manim_slides-5.1.7.tar.gz`

## Comparing `manim_slides-5.1.6.tar` & `manim_slides-5.1.7.tar`

### file list

```diff
@@ -1,142 +1,141 @@
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.bumpversion.cfg
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.mdlc.json
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.python-version
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.readthedocs.yaml
--rw-r--r--   0        0        0    11657 2020-02-02 00:00:00.000000 manim_slides-5.1.6/CHANGELOG.md
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 manim_slides-5.1.6/CITATION.cff
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 manim_slides-5.1.6/custom_config.yml
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 manim_slides-5.1.6/example.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim-slides.qrc
--rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 manim_slides-5.1.6/requirements-dev.lock
--rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 manim_slides-5.1.6/requirements.lock
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.github/FUNDING.yml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.github/dependabot.yml
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.github/pull_request_template.md
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.github/ISSUE_TEMPLATE/documentation.yml
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.github/ISSUE_TEMPLATE/support.yml
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.github/scripts/check_github_issues.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.github/workflows/clearcache.yml
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.github/workflows/draft-pdf.yml
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.github/workflows/languagetool.yml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.github/workflows/latest_tag.yml
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.github/workflows/publish.yml
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docker/Dockerfile
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docker/README.md
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docker/texlive-profile.txt
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/make.bat
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/changelog.md
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/conf.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/docutils.conf
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/faq.md
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/features_table.md
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/gallery.md
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/index.md
--rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/installation.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/license.md
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/manim_or_manimgl.md
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/quickstart.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/_static/favicon.png -> ../../../static/favicon.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/_static/logo.png -> ../../../static/logo.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/_static/logo_dark_docs.png -> ../../../static/logo_dark_docs.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/_static/logo_dark_github.png -> ../../../static/logo_dark_github.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/_static/logo_dark_transparent.png -> ../../../static/logo_dark_transparent.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/_static/logo_light_transparent.png -> ../../../static/logo_light_transparent.png
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/_static/template.diff
--rw-r--r--   0        0        0    17358 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/_static/template.html
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/_static/wizard_dark.png -> ../../../static/wizard_dark.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/_static/wizard_light.png -> ../../../static/wizard_light.png
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/contributing/index.md
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/contributing/internals.md
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/contributing/workflow.md
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/reference/api.md
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/reference/cli.md
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/reference/customize_html.md
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/reference/examples.md
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/reference/gui.md
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/reference/html.md
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/reference/index.md
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/reference/ipython_magic.md
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/reference/magic_example.ipynb
--rw-r--r--   0        0        0     6947 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/reference/sharing.md
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 manim_slides-5.1.6/docs/source/reference/sphinx_extension.md
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/__init__.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/__version__.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/commons.py
--rw-r--r--   0        0        0    11123 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/config.py
--rw-r--r--   0        0        0    21228 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/convert.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/defaults.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/logger.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/qt_utils.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/render.py
--rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/resources.py
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/docs/__init__.py
--rw-r--r--   0        0        0    16359 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/docs/manim_slides_directive.py
--rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/ipython/ipython_magic.py
--rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/present/__init__.py
--rw-r--r--   0        0        0    18061 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/present/player.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/slide/__init__.py
--rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/slide/animation.py
--rw-r--r--   0        0        0    20762 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/slide/base.py
--rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/slide/manim.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/slide/manimlib.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/templates/__init__.py
--rw-r--r--   0        0        0    14662 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/templates/revealjs.html
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/wizard/__init__.py
--rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 manim_slides-5.1.6/manim_slides/wizard/wizard.py
--rw-r--r--   0        0        0   161325 2020-02-02 00:00:00.000000 manim_slides-5.1.6/paper/docs.png
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 manim_slides-5.1.6/paper/paper.bib
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 manim_slides-5.1.6/paper/paper.md
--rw-r--r--   0        0        0   181998 2020-02-02 00:00:00.000000 manim_slides-5.1.6/static/docs.png
--rw-r--r--   0        0        0   496568 2020-02-02 00:00:00.000000 manim_slides-5.1.6/static/example.gif
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 manim_slides-5.1.6/static/favicon.png
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 manim_slides-5.1.6/static/icon.png
--rw-r--r--   0        0        0    92151 2020-02-02 00:00:00.000000 manim_slides-5.1.6/static/logo.png
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 manim_slides-5.1.6/static/logo.py
--rw-r--r--   0        0        0    88069 2020-02-02 00:00:00.000000 manim_slides-5.1.6/static/logo_dark_docs.png
--rw-r--r--   0        0        0    88377 2020-02-02 00:00:00.000000 manim_slides-5.1.6/static/logo_dark_github.png
--rw-r--r--   0        0        0   112081 2020-02-02 00:00:00.000000 manim_slides-5.1.6/static/logo_dark_transparent.png
--rw-r--r--   0        0        0   104821 2020-02-02 00:00:00.000000 manim_slides-5.1.6/static/logo_light_transparent.png
--rwxr-xr-x   0        0        0      231 2020-02-02 00:00:00.000000 manim_slides-5.1.6/static/make_favicon.sh
--rwxr-xr-x   0        0        0     1364 2020-02-02 00:00:00.000000 manim_slides-5.1.6/static/make_logo.sh
--rw-r--r--   0        0        0    29891 2020-02-02 00:00:00.000000 manim_slides-5.1.6/static/windows_quality_fix.png
--rw-r--r--   0        0        0    26333 2020-02-02 00:00:00.000000 manim_slides-5.1.6/static/wizard_dark.png
--rw-r--r--   0        0        0    24815 2020-02-02 00:00:00.000000 manim_slides-5.1.6/static/wizard_light.png
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/conftest.py
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/test_base_slide.py
--rw-r--r--   0        0        0     3443 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/test_commons.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/test_config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/test_convert.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/test_defaults.py
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/test_main.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/test_manim.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/test_player.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/test_present.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/test_qt_utils.py
--rw-r--r--   0        0        0     9760 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/test_slide.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/test_utils.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/test_wizard.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/data/slides.py
--rw-r--r--   0        0        0    30504 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/data/video.mp4
--rw-r--r--   0        0        0    40695 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/data/video_data_uri.txt
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/data/slides/BasicSlide.json
--rw-r--r--   0        0        0    50327 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511.mp4
--rw-r--r--   0        0        0    45042 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511_reversed.mp4
--rw-r--r--   0        0        0    23621 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c.mp4
--rw-r--r--   0        0        0    23195 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c_reversed.mp4
--rw-r--r--   0        0        0    17527 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077.mp4
--rw-r--r--   0        0        0    17349 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077_reversed.mp4
--rw-r--r--   0        0        0    36367 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368.mp4
--rw-r--r--   0        0        0    30504 2020-02-02 00:00:00.000000 manim_slides-5.1.6/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368_reversed.mp4
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 manim_slides-5.1.6/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 manim_slides-5.1.6/LICENSE.md
--rw-r--r--   0        0        0     9076 2020-02-02 00:00:00.000000 manim_slides-5.1.6/README.md
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 manim_slides-5.1.6/pyproject.toml
--rw-r--r--   0        0        0    12829 2020-02-02 00:00:00.000000 manim_slides-5.1.6/PKG-INFO
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 manim_slides-5.1.7/.mdlc.json
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 manim_slides-5.1.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 manim_slides-5.1.7/.python-version
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 manim_slides-5.1.7/.readthedocs.yaml
+-rw-r--r--   0        0        0    11907 2020-02-02 00:00:00.000000 manim_slides-5.1.7/CHANGELOG.md
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 manim_slides-5.1.7/CITATION.cff
+-rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 manim_slides-5.1.7/README.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 manim_slides-5.1.7/custom_config.yml
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 manim_slides-5.1.7/example.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim-slides.qrc
+-rw-r--r--   0        0        0     8375 2020-02-02 00:00:00.000000 manim_slides-5.1.7/requirements-dev.lock
+-rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 manim_slides-5.1.7/requirements.lock
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 manim_slides-5.1.7/.github/FUNDING.yml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 manim_slides-5.1.7/.github/dependabot.yml
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 manim_slides-5.1.7/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 manim_slides-5.1.7/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 manim_slides-5.1.7/.github/ISSUE_TEMPLATE/documentation.yml
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 manim_slides-5.1.7/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 manim_slides-5.1.7/.github/ISSUE_TEMPLATE/support.yml
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 manim_slides-5.1.7/.github/scripts/check_github_issues.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 manim_slides-5.1.7/.github/workflows/clearcache.yml
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 manim_slides-5.1.7/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 manim_slides-5.1.7/.github/workflows/draft-pdf.yml
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 manim_slides-5.1.7/.github/workflows/languagetool.yml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 manim_slides-5.1.7/.github/workflows/latest_tag.yml
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 manim_slides-5.1.7/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 manim_slides-5.1.7/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docker/Dockerfile
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docker/README.md
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docker/texlive-profile.txt
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/make.bat
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/changelog.md
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/conf.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/docutils.conf
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/faq.md
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/features_table.md
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/gallery.md
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/index.md
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/installation.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/license.md
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/manim_or_manimgl.md
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/quickstart.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/_static/favicon.png -> ../../../static/favicon.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/_static/logo.png -> ../../../static/logo.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/_static/logo_dark_docs.png -> ../../../static/logo_dark_docs.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/_static/logo_dark_github.png -> ../../../static/logo_dark_github.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/_static/logo_dark_transparent.png -> ../../../static/logo_dark_transparent.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/_static/logo_light_transparent.png -> ../../../static/logo_light_transparent.png
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/_static/template.diff
+-rw-r--r--   0        0        0    17358 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/_static/template.html
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/_static/wizard_dark.png -> ../../../static/wizard_dark.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/_static/wizard_light.png -> ../../../static/wizard_light.png
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/contributing/index.md
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/contributing/internals.md
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/contributing/workflow.md
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/reference/api.md
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/reference/cli.md
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/reference/customize_html.md
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/reference/examples.md
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/reference/gui.md
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/reference/html.md
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/reference/index.md
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/reference/ipython_magic.md
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/reference/magic_example.ipynb
+-rw-r--r--   0        0        0     6947 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/reference/sharing.md
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 manim_slides-5.1.7/docs/source/reference/sphinx_extension.md
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/__init__.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/__version__.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/commons.py
+-rw-r--r--   0        0        0    11123 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/config.py
+-rw-r--r--   0        0        0    21228 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/convert.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/defaults.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/logger.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/qt_utils.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/render.py
+-rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/resources.py
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/docs/__init__.py
+-rw-r--r--   0        0        0    16359 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/docs/manim_slides_directive.py
+-rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/ipython/ipython_magic.py
+-rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/present/__init__.py
+-rw-r--r--   0        0        0    18061 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/present/player.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/slide/__init__.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/slide/animation.py
+-rw-r--r--   0        0        0    20762 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/slide/base.py
+-rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/slide/manim.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/slide/manimlib.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/templates/__init__.py
+-rw-r--r--   0        0        0    14662 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/templates/revealjs.html
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/wizard/__init__.py
+-rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 manim_slides-5.1.7/manim_slides/wizard/wizard.py
+-rw-r--r--   0        0        0   161325 2020-02-02 00:00:00.000000 manim_slides-5.1.7/paper/docs.png
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 manim_slides-5.1.7/paper/paper.bib
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 manim_slides-5.1.7/paper/paper.md
+-rw-r--r--   0        0        0   181998 2020-02-02 00:00:00.000000 manim_slides-5.1.7/static/docs.png
+-rw-r--r--   0        0        0   496568 2020-02-02 00:00:00.000000 manim_slides-5.1.7/static/example.gif
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 manim_slides-5.1.7/static/favicon.png
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 manim_slides-5.1.7/static/icon.png
+-rw-r--r--   0        0        0    92151 2020-02-02 00:00:00.000000 manim_slides-5.1.7/static/logo.png
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 manim_slides-5.1.7/static/logo.py
+-rw-r--r--   0        0        0    88069 2020-02-02 00:00:00.000000 manim_slides-5.1.7/static/logo_dark_docs.png
+-rw-r--r--   0        0        0    88377 2020-02-02 00:00:00.000000 manim_slides-5.1.7/static/logo_dark_github.png
+-rw-r--r--   0        0        0   112081 2020-02-02 00:00:00.000000 manim_slides-5.1.7/static/logo_dark_transparent.png
+-rw-r--r--   0        0        0   104821 2020-02-02 00:00:00.000000 manim_slides-5.1.7/static/logo_light_transparent.png
+-rwxr-xr-x   0        0        0      231 2020-02-02 00:00:00.000000 manim_slides-5.1.7/static/make_favicon.sh
+-rwxr-xr-x   0        0        0     1364 2020-02-02 00:00:00.000000 manim_slides-5.1.7/static/make_logo.sh
+-rw-r--r--   0        0        0    29891 2020-02-02 00:00:00.000000 manim_slides-5.1.7/static/windows_quality_fix.png
+-rw-r--r--   0        0        0    26333 2020-02-02 00:00:00.000000 manim_slides-5.1.7/static/wizard_dark.png
+-rw-r--r--   0        0        0    24815 2020-02-02 00:00:00.000000 manim_slides-5.1.7/static/wizard_light.png
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/conftest.py
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/test_base_slide.py
+-rw-r--r--   0        0        0     3443 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/test_commons.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/test_config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/test_convert.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/test_defaults.py
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/test_main.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/test_manim.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/test_player.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/test_present.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/test_qt_utils.py
+-rw-r--r--   0        0        0     9760 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/test_slide.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/test_utils.py
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/test_wizard.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/data/slides.py
+-rw-r--r--   0        0        0    30504 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/data/video.mp4
+-rw-r--r--   0        0        0    40695 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/data/video_data_uri.txt
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/data/slides/BasicSlide.json
+-rw-r--r--   0        0        0    50327 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511.mp4
+-rw-r--r--   0        0        0    45042 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511_reversed.mp4
+-rw-r--r--   0        0        0    23621 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c.mp4
+-rw-r--r--   0        0        0    23195 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c_reversed.mp4
+-rw-r--r--   0        0        0    17527 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077.mp4
+-rw-r--r--   0        0        0    17349 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077_reversed.mp4
+-rw-r--r--   0        0        0    36367 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368.mp4
+-rw-r--r--   0        0        0    30504 2020-02-02 00:00:00.000000 manim_slides-5.1.7/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368_reversed.mp4
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 manim_slides-5.1.7/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 manim_slides-5.1.7/LICENSE.md
+-rw-r--r--   0        0        0     5563 2020-02-02 00:00:00.000000 manim_slides-5.1.7/pyproject.toml
+-rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 manim_slides-5.1.7/PKG-INFO
```

### Comparing `manim_slides-5.1.6/.pre-commit-config.yaml` & `manim_slides-5.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/CHANGELOG.md` & `manim_slides-5.1.7/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,24 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 <!-- start changelog -->
 
 (unreleased)=
-## [Unreleased](https://github.com/jeertmans/manim-slides/compare/v5.1.6...HEAD)
+## [Unreleased](https://github.com/jeertmans/manim-slides/compare/5.1.7...HEAD)
+
+(v5.1.7)=
+## [v5.1.7](https://github.com/jeertmans/manim-slides/compare/v5.1.6...v5.1.7)
+
+(v5.1.7-chore)=
+### Chore
+
+- Improved the CI for bumping the version and README rendering on PyPI.
+  [#425](https://github.com/jeertmans/manim-slides/pull/425)
 
 (v5.1.6)=
 ## [v5.1.6](https://github.com/jeertmans/manim-slides/compare/v5.1.5...v5.1.6)
 
 (v5.1.6-added)=
 ### Added
```

### Comparing `manim_slides-5.1.6/CITATION.cff` & `manim_slides-5.1.7/CITATION.cff`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 keywords:
   - Education
   - Math Animations
   - Presentation Tool
   - PowerPoint
   - Python
 license: MIT
-version: v5.1.6
+version: v5.1.7
 preferred-citation:
   publisher:
     name: The Open Journal
   type: article
   authors:
     - name: Jérome Eertmans
       orcid: 'https://orcid.org/0000-0002-5579-5360'
```

### Comparing `manim_slides-5.1.6/example.py` & `manim_slides-5.1.7/example.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/requirements-dev.lock` & `manim_slides-5.1.7/requirements-dev.lock`

 * *Files 11% similar despite different names*

```diff
@@ -22,26 +22,30 @@
 babel==2.14.0
     # via sphinx
 beautifulsoup4==4.12.3
     # via furo
     # via nbconvert
 bleach==6.1.0
     # via nbconvert
-bump2version==1.0.1
+bracex==2.4
+    # via wcmatch
+bump-my-version==0.21.0
 certifi==2024.2.2
     # via requests
 cfgv==3.4.0
     # via pre-commit
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
+    # via bump-my-version
     # via click-default-group
     # via cloup
     # via manim
     # via manim-slides
+    # via rich-click
     # via sphinx-click
 click-default-group==1.2.4
     # via manim
     # via manim-slides
 cloup==0.13.1
     # via manim
 colour==0.1.5
@@ -77,27 +81,25 @@
 fastjsonschema==2.19.1
     # via nbformat
 filelock==3.13.4
     # via virtualenv
 fonttools==4.51.0
     # via matplotlib
 furo==2024.1.29
-    # via manim-slides
 glcontext==2.5.0
     # via moderngl
 identify==2.5.35
     # via pre-commit
 idna==3.7
     # via requests
 imagesize==1.4.1
     # via sphinx
 iniconfig==2.0.0
     # via pytest
 ipykernel==6.29.4
-    # via manim-slides
 ipython==8.18.1
     # via ipykernel
     # via manim-slides
     # via manimgl
 isosurfaces==0.1.0
     # via manim
     # via manimgl
@@ -165,25 +167,23 @@
     # via manim
     # via manimgl
 mpmath==1.3.0
     # via sympy
 multipledispatch==1.0.0
     # via pyrr
 myst-parser==2.0.0
-    # via manim-slides
 nbclient==0.10.0
     # via nbconvert
 nbconvert==7.16.3
     # via nbsphinx
 nbformat==5.10.4
     # via nbclient
     # via nbconvert
     # via nbsphinx
 nbsphinx==0.9.3
-    # via manim-slides
 nest-asyncio==1.6.0
     # via ipykernel
 networkx==2.8.8
     # via manim
 nodeenv==1.8.0
     # via pre-commit
 numpy==1.26.4
@@ -201,15 +201,14 @@
     # via ipykernel
     # via matplotlib
     # via nbconvert
     # via pytest
     # via qtpy
     # via sphinx
 pandoc==2.3
-    # via manim-slides
 pandocfilters==1.5.1
     # via nbconvert
 parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
 pillow==9.5.0
@@ -228,29 +227,34 @@
 plumbum==1.8.2
     # via pandoc
 ply==3.11
     # via pandoc
 pre-commit==3.7.0
 prompt-toolkit==3.0.43
     # via ipython
+    # via questionary
 psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 pycairo==1.26.0
     # via manim
 pydantic==2.7.0
+    # via bump-my-version
     # via manim-slides
     # via pydantic-extra-types
+    # via pydantic-settings
 pydantic-core==2.18.1
     # via pydantic
 pydantic-extra-types==2.6.0
     # via manim-slides
+pydantic-settings==2.2.1
+    # via bump-my-version
 pydub==0.25.1
     # via manim
     # via manimgl
 pyglet==2.0.15
     # via moderngl-window
 pygments==2.17.2
     # via furo
@@ -287,36 +291,44 @@
 pytest-cov==5.0.0
 pytest-env==1.1.3
 pytest-qt==4.4.0
 pytest-xdist==3.5.0
 python-dateutil==2.9.0.post0
     # via jupyter-client
     # via matplotlib
+python-dotenv==1.0.1
+    # via pydantic-settings
 python-pptx==0.6.23
     # via manim-slides
 pyyaml==6.0.1
     # via manimgl
     # via myst-parser
     # via pre-commit
 pyzmq==26.0.0
     # via ipykernel
     # via jupyter-client
 qtpy==2.4.1
     # via manim-slides
+questionary==1.10.0
+    # via bump-my-version
 referencing==0.34.0
     # via jsonschema
     # via jsonschema-specifications
 requests==2.31.0
     # via manim
     # via manim-slides
     # via sphinx
 rich==13.7.1
+    # via bump-my-version
     # via manim
     # via manim-slides
     # via manimgl
+    # via rich-click
+rich-click==1.8.0
+    # via bump-my-version
 rpds-py==0.18.0
     # via jsonschema
     # via referencing
 rtoml==0.10.0
     # via manim-slides
 scipy==1.13.0
     # via manim
@@ -339,52 +351,50 @@
     # via manimgl
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
 sphinx==7.3.6
     # via furo
-    # via manim-slides
     # via myst-parser
     # via nbsphinx
     # via sphinx-basic-ng
     # via sphinx-click
     # via sphinx-copybutton
     # via sphinxext-opengraph
 sphinx-basic-ng==1.0.0b2
     # via furo
 sphinx-click==5.1.0
-    # via manim-slides
 sphinx-copybutton==0.5.2
-    # via manim-slides
 sphinxcontrib-applehelp==1.0.8
     # via sphinx
 sphinxcontrib-devhelp==1.0.6
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
 sphinxext-opengraph==0.9.1
-    # via manim-slides
 srt==3.5.3
     # via manim
 stack-data==0.6.3
     # via ipython
 svgelements==1.9.6
     # via manim
     # via manimgl
 sympy==1.12
     # via manimgl
 tinycss2==1.2.1
     # via nbconvert
+tomlkit==0.12.4
+    # via bump-my-version
 tornado==6.4
     # via ipykernel
     # via jupyter-client
 tqdm==4.66.2
     # via manim
     # via manim-slides
     # via manimgl
@@ -398,22 +408,25 @@
     # via nbclient
     # via nbconvert
     # via nbformat
     # via nbsphinx
 typing-extensions==4.11.0
     # via pydantic
     # via pydantic-core
+    # via rich-click
 urllib3==2.2.1
     # via requests
 validators==0.28.0
     # via manimgl
 virtualenv==20.25.3
     # via pre-commit
 watchdog==2.3.1
     # via manim
+wcmatch==8.5.1
+    # via bump-my-version
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
     # via tinycss2
 xlsxwriter==3.2.0
     # via python-pptx
```

### Comparing `manim_slides-5.1.6/.github/pull_request_template.md` & `manim_slides-5.1.7/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/.github/ISSUE_TEMPLATE/bug.yml` & `manim_slides-5.1.7/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/.github/ISSUE_TEMPLATE/documentation.yml` & `manim_slides-5.1.7/.github/ISSUE_TEMPLATE/documentation.yml`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/.github/ISSUE_TEMPLATE/feature_request.yml` & `manim_slides-5.1.7/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/.github/scripts/check_github_issues.py` & `manim_slides-5.1.7/.github/scripts/check_github_issues.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/.github/workflows/clearcache.yml` & `manim_slides-5.1.7/.github/workflows/clearcache.yml`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/.github/workflows/codeql-analysis.yml` & `manim_slides-5.1.7/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/.github/workflows/draft-pdf.yml` & `manim_slides-5.1.7/.github/workflows/draft-pdf.yml`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/.github/workflows/publish.yml` & `manim_slides-5.1.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/.github/workflows/tests.yml` & `manim_slides-5.1.7/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docker/Dockerfile` & `manim_slides-5.1.7/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/Makefile` & `manim_slides-5.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/make.bat` & `manim_slides-5.1.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/conf.py` & `manim_slides-5.1.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/faq.md` & `manim_slides-5.1.7/docs/source/faq.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/features_table.md` & `manim_slides-5.1.7/docs/source/features_table.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/gallery.md` & `manim_slides-5.1.7/docs/source/gallery.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/index.md` & `manim_slides-5.1.7/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/installation.md` & `manim_slides-5.1.7/docs/source/installation.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/manim_or_manimgl.md` & `manim_slides-5.1.7/docs/source/manim_or_manimgl.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/quickstart.md` & `manim_slides-5.1.7/docs/source/quickstart.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/_static/template.diff` & `manim_slides-5.1.7/docs/source/_static/template.diff`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/_static/template.html` & `manim_slides-5.1.7/docs/source/_static/template.html`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/contributing/index.md` & `manim_slides-5.1.7/docs/source/contributing/index.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/contributing/internals.md` & `manim_slides-5.1.7/docs/source/contributing/internals.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/contributing/workflow.md` & `manim_slides-5.1.7/docs/source/contributing/workflow.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/reference/api.md` & `manim_slides-5.1.7/docs/source/reference/api.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/reference/customize_html.md` & `manim_slides-5.1.7/docs/source/reference/customize_html.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/reference/examples.md` & `manim_slides-5.1.7/docs/source/reference/examples.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/reference/gui.md` & `manim_slides-5.1.7/docs/source/reference/gui.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/reference/html.md` & `manim_slides-5.1.7/docs/source/reference/html.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/reference/index.md` & `manim_slides-5.1.7/docs/source/reference/index.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/reference/magic_example.ipynb` & `manim_slides-5.1.7/docs/source/reference/magic_example.ipynb`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/docs/source/reference/sharing.md` & `manim_slides-5.1.7/docs/source/reference/sharing.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/__init__.py` & `manim_slides-5.1.7/manim_slides/__init__.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/__main__.py` & `manim_slides-5.1.7/manim_slides/__main__.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/commons.py` & `manim_slides-5.1.7/manim_slides/commons.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/config.py` & `manim_slides-5.1.7/manim_slides/config.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/convert.py` & `manim_slides-5.1.7/manim_slides/convert.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/logger.py` & `manim_slides-5.1.7/manim_slides/logger.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/render.py` & `manim_slides-5.1.7/manim_slides/render.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/resources.py` & `manim_slides-5.1.7/manim_slides/resources.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/utils.py` & `manim_slides-5.1.7/manim_slides/utils.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/docs/manim_slides_directive.py` & `manim_slides-5.1.7/manim_slides/docs/manim_slides_directive.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/ipython/ipython_magic.py` & `manim_slides-5.1.7/manim_slides/ipython/ipython_magic.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/present/__init__.py` & `manim_slides-5.1.7/manim_slides/present/__init__.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/present/player.py` & `manim_slides-5.1.7/manim_slides/present/player.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/slide/__init__.py` & `manim_slides-5.1.7/manim_slides/slide/__init__.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/slide/animation.py` & `manim_slides-5.1.7/manim_slides/slide/animation.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/slide/base.py` & `manim_slides-5.1.7/manim_slides/slide/base.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/slide/manim.py` & `manim_slides-5.1.7/manim_slides/slide/manim.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/slide/manimlib.py` & `manim_slides-5.1.7/manim_slides/slide/manimlib.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/templates/revealjs.html` & `manim_slides-5.1.7/manim_slides/templates/revealjs.html`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/wizard/__init__.py` & `manim_slides-5.1.7/manim_slides/wizard/__init__.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/manim_slides/wizard/wizard.py` & `manim_slides-5.1.7/manim_slides/wizard/wizard.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/paper/docs.png` & `manim_slides-5.1.7/paper/docs.png`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/paper/paper.bib` & `manim_slides-5.1.7/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/paper/paper.md` & `manim_slides-5.1.7/paper/paper.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/static/docs.png` & `manim_slides-5.1.7/static/docs.png`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/static/example.gif` & `manim_slides-5.1.7/static/example.gif`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/static/favicon.png` & `manim_slides-5.1.7/static/favicon.png`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/static/icon.png` & `manim_slides-5.1.7/static/icon.png`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/static/logo.png` & `manim_slides-5.1.7/static/logo.png`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/static/logo.py` & `manim_slides-5.1.7/static/logo.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/static/logo_dark_docs.png` & `manim_slides-5.1.7/static/logo_dark_docs.png`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/static/logo_dark_github.png` & `manim_slides-5.1.7/static/logo_dark_github.png`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/static/logo_dark_transparent.png` & `manim_slides-5.1.7/static/logo_dark_transparent.png`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/static/logo_light_transparent.png` & `manim_slides-5.1.7/static/logo_light_transparent.png`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/static/make_logo.sh` & `manim_slides-5.1.7/static/make_logo.sh`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/static/windows_quality_fix.png` & `manim_slides-5.1.7/static/windows_quality_fix.png`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/static/wizard_dark.png` & `manim_slides-5.1.7/static/wizard_dark.png`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/static/wizard_light.png` & `manim_slides-5.1.7/static/wizard_light.png`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/conftest.py` & `manim_slides-5.1.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/test_base_slide.py` & `manim_slides-5.1.7/tests/test_base_slide.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/test_commons.py` & `manim_slides-5.1.7/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/test_config.py` & `manim_slides-5.1.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/test_convert.py` & `manim_slides-5.1.7/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/test_main.py` & `manim_slides-5.1.7/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/test_manim.py` & `manim_slides-5.1.7/tests/test_manim.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/test_present.py` & `manim_slides-5.1.7/tests/test_present.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/test_slide.py` & `manim_slides-5.1.7/tests/test_slide.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/test_utils.py` & `manim_slides-5.1.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/test_wizard.py` & `manim_slides-5.1.7/tests/test_wizard.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/data/slides.py` & `manim_slides-5.1.7/tests/data/slides.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/data/video.mp4` & `manim_slides-5.1.7/tests/data/video.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/data/video_data_uri.txt` & `manim_slides-5.1.7/tests/data/video_data_uri.txt`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/data/slides/BasicSlide.json` & `manim_slides-5.1.7/tests/data/slides/BasicSlide.json`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511.mp4` & `manim_slides-5.1.7/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511_reversed.mp4` & `manim_slides-5.1.7/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511_reversed.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c.mp4` & `manim_slides-5.1.7/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c_reversed.mp4` & `manim_slides-5.1.7/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c_reversed.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077.mp4` & `manim_slides-5.1.7/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077_reversed.mp4` & `manim_slides-5.1.7/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077_reversed.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368.mp4` & `manim_slides-5.1.7/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368_reversed.mp4` & `manim_slides-5.1.7/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368_reversed.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/.gitignore` & `manim_slides-5.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/LICENSE.md` & `manim_slides-5.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.6/README.md` & `manim_slides-5.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/jeertmans/manim-slides/main/static/logo_dark_transparent.png">
   <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/jeertmans/manim-slides/main/static/logo_light_transparent.png">
   <img alt="Manim Slides Logo" src="https://raw.githubusercontent.com/jeertmans/manim-slides/main/static/logo.png">
 </picture>
 
+<!-- start pypi -->
+
 [![Latest Release][pypi-version-badge]][pypi-version-url]
 [![Python version][pypi-python-version-badge]][pypi-version-url]
 [![PyPI - Downloads][pypi-download-badge]][pypi-version-url]
 [![Documentation][documentation-badge]][documentation-url]
 [![DOI][doi-badge]][doi-url]
 [![JOSE Paper][jose-badge]][jose-url]
 [![codecov][codecov-badge]][codecov-url]
```

### Comparing `manim_slides-5.1.6/PKG-INFO` & `manim_slides-5.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.3
 Name: manim-slides
-Version: 5.1.6
+Version: 5.1.7
 Summary: Tool for live presentations using manim
 Project-URL: Changelog, https://github.com/jeertmans/manim-slides/releases
 Project-URL: Documentation, https://eertmans.be/manim-slides
 Project-URL: Founding, https://github.com/sponsors/jeertmans
 Project-URL: Homepage, https://github.com/jeertmans/manim-slides
 Project-URL: Repository, https://github.com/jeertmans/manim-slides
 Author-email: Jérome Eertmans <jeertmans@icloud.com>
-License: MIT
+License-Expression: MIT
 License-File: LICENSE.md
 Keywords: manim,manimgl,plugin,slides
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -33,27 +33,14 @@
 Requires-Dist: pydantic>=2.0.1
 Requires-Dist: python-pptx>=0.6.21
 Requires-Dist: qtpy>=2.4.1
 Requires-Dist: requests>=2.28.1
 Requires-Dist: rich>=13.3.2
 Requires-Dist: rtoml>=0.9.0
 Requires-Dist: tqdm>=4.64.1
-Provides-Extra: docs
-Requires-Dist: docutils>=0.20.1; extra == 'docs'
-Requires-Dist: furo>=2023.5.20; extra == 'docs'
-Requires-Dist: ipykernel>=6.25.1; extra == 'docs'
-Requires-Dist: ipython>=8.12.2; extra == 'docs'
-Requires-Dist: manim>=0.17.3; extra == 'docs'
-Requires-Dist: myst-parser>=2.0.0; extra == 'docs'
-Requires-Dist: nbsphinx>=0.9.2; extra == 'docs'
-Requires-Dist: pandoc>=2.3; extra == 'docs'
-Requires-Dist: sphinx-click>=4.4.0; extra == 'docs'
-Requires-Dist: sphinx-copybutton>=0.5.1; extra == 'docs'
-Requires-Dist: sphinx>=7.0.1; extra == 'docs'
-Requires-Dist: sphinxext-opengraph>=0.7.5; extra == 'docs'
 Provides-Extra: full
 Requires-Dist: docutils>=0.20.1; extra == 'full'
 Requires-Dist: ipython>=8.12.2; extra == 'full'
 Requires-Dist: manim>=0.17.3; extra == 'full'
 Provides-Extra: full-gl
 Requires-Dist: docutils>=0.20.1; extra == 'full-gl'
 Requires-Dist: ipython>=8.12.2; extra == 'full-gl'
@@ -81,19 +68,20 @@
 Requires-Dist: manim>=0.17.3; extra == 'pyside6-full'
 Requires-Dist: pyside6<6.5.3,>=6.5.1; (python_version < '3.12') and extra == 'pyside6-full'
 Provides-Extra: sphinx-directive
 Requires-Dist: docutils>=0.20.1; extra == 'sphinx-directive'
 Requires-Dist: manim>=0.17.3; extra == 'sphinx-directive'
 Description-Content-Type: text/markdown
 
-<picture>
-  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/jeertmans/manim-slides/main/static/logo_dark_transparent.png">
-  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/jeertmans/manim-slides/main/static/logo_light_transparent.png">
-  <img alt="Manim Slides Logo" src="https://raw.githubusercontent.com/jeertmans/manim-slides/main/static/logo.png">
-</picture>
+<p align="center">
+  <a href="https://www.github.com/jeertmans/manin-slides">
+    <img src="https://raw.githubusercontent.com/jeertmans/manim-slides/main/static/logo.png"/>
+  </a>
+</p>
+
 
 [![Latest Release][pypi-version-badge]][pypi-version-url]
 [![Python version][pypi-python-version-badge]][pypi-version-url]
 [![PyPI - Downloads][pypi-download-badge]][pypi-version-url]
 [![Documentation][documentation-badge]][documentation-url]
 [![DOI][doi-badge]][doi-url]
 [![JOSE Paper][jose-badge]][jose-url]
@@ -103,15 +91,15 @@
 # Manim Slides
 
 Tool for live presentations using either
 [Manim (community edition)](https://www.manim.community/)
 or [ManimGL](https://3b1b.github.io/manim/).
 Manim Slides will *automatically* detect the one you are using!
 
-> [!NOTE]
+> **NOTE:**
 > This project extends the work of
 > [`manim-presentation`](https://github.com/galatolofederico/manim-presentation),
 > with a lot more features!
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Comparison with Similar Tools](#comparison-with-similar-tools)
@@ -173,15 +161,15 @@
 ```bash
 manim-slides render example.py BasicExample
 # or use ManimGL
 manim-slides render --GL example.py BasicExample
 ```
 <!-- end usage -->
 
-> [!NOTE]
+> **NOTE:**
 > Using `manim-slides render` makes sure to use the `manim`
 > (or `manimlib`) library that was installed in the same Python environment.
 > Put simply, this is a wrapper around
 > `manim render [ARGS]...` (or `manimgl [ARGS]...`).
 
 <!-- start more-usage -->
```

