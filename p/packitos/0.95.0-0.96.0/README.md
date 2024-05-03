# Comparing `tmp/packitos-0.95.0.tar.gz` & `tmp/packitos-0.96.0.tar.gz`

## Comparing `packitos-0.95.0.tar` & `packitos-0.96.0.tar`

### file list

```diff
@@ -1,408 +1,409 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 packitos-0.95.0/.git_archival.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 packitos-0.95.0/.gitattributes
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 packitos-0.95.0/.packit.yaml
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 packitos-0.95.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 packitos-0.95.0/.zuul.yaml
--rw-r--r--   0        0        0    57138 2020-02-02 00:00:00.000000 packitos-0.95.0/CHANGELOG.md
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 packitos-0.95.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 packitos-0.95.0/Containerfile
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 packitos-0.95.0/Containerfile.tests
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 packitos-0.95.0/DCO
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 packitos-0.95.0/LICENSE_HEADER.txt
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 packitos-0.95.0/Makefile
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 packitos-0.95.0/ansible.cfg
--rw-r--r--   0        0        0    13350 2020-02-02 00:00:00.000000 packitos-0.95.0/packit.spec
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 packitos-0.95.0/release-conf.yaml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 packitos-0.95.0/.fmf/version
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 packitos-0.95.0/.github/stale.yml
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 packitos-0.95.0/.github/workflows/build-and-push.yml
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 packitos-0.95.0/.github/workflows/check-release-notes.yml
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 packitos-0.95.0/.github/workflows/do_release.yml
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 packitos-0.95.0/.github/workflows/opened-issues-to-the-board.yml
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 packitos-0.95.0/.github/workflows/prepare-release.yml
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 packitos-0.95.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0  1843517 2020-02-02 00:00:00.000000 packitos-0.95.0/design/logo-packit.sketch
--rw-r--r--   0        0        0   135444 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/hexsticker.png
--rw-r--r--   0        0        0   132230 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-dark.png
--rw-r--r--   0        0        0    75002 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-extended.jpg
--rw-r--r--   0        0        0    48468 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-extended.png
--rw-r--r--   0        0        0    24881 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-extended.svg
--rw-r--r--   0        0        0   106567 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-guideline.pdf
--rw-r--r--   0        0        0    66141 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-no-borders.jpg
--rw-r--r--   0        0        0   143587 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-no-borders.png
--rw-r--r--   0        0        0    20683 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-small.png
--rw-r--r--   0        0        0    70268 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-square-small-borders.jpg
--rw-r--r--   0        0        0   150044 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-square-small-borders.png
--rw-r--r--   0        0        0    43972 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-stg-square-bigger-borders.svg
--rw-r--r--   0        0        0   107242 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-stg-square-small-borders.png
--rw-r--r--   0        0        0    43981 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-stg-square-small-borders.svg
--rw-r--r--   0        0        0    28826 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-stg.png
--rw-r--r--   0        0        0    24351 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-stg.svg
--rw-r--r--   0        0        0    18005 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-text.jpg
--rw-r--r--   0        0        0    14198 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-text.png
--rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-text.svg
--rw-r--r--   0        0        0   144552 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo-white.png
--rw-r--r--   0        0        0   158074 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo.png
--rw-r--r--   0        0        0    14697 2020-02-02 00:00:00.000000 packitos-0.95.0/design/export/logo.svg
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 packitos-0.95.0/files/install-requirements-git.yaml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 packitos-0.95.0/files/install-requirements-pip.yaml
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 packitos-0.95.0/files/install-requirements-rpms.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 packitos-0.95.0/files/local-tests-requirements.yaml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 packitos-0.95.0/files/packit-testing-farm-prepare-session-recording.yaml
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 packitos-0.95.0/files/packit-testing-farm-prepare.yaml
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 packitos-0.95.0/files/zuul-reverse-dep-packit-service.yaml
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 packitos-0.95.0/files/zuul-tests-session-recording.yaml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 packitos-0.95.0/files/zuul-tests.yaml
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 packitos-0.95.0/files/bash-completion/packit
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/build-rpm-deps.yaml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/centpkg.yaml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/generic-dnf-requirements.yaml
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/install-packit-service.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/install-packit.yaml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/ogr.yaml
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/packit-service-requirements.yaml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/project-dir.yaml
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/python-compile-deps.yaml
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/requre.yaml
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/rpm-test-deps.yaml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/sandcastle.yaml
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 packitos-0.95.0/files/tasks/specfile.yaml
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/__init__.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/actions.py
--rw-r--r--   0        0        0    90819 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/api.py
--rw-r--r--   0        0        0    29435 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/base_git.py
--rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/command_handler.py
--rw-r--r--   0        0        0     9167 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/constants.py
--rw-r--r--   0        0        0    20419 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/copr_helper.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/dist_git_instance.py
--rw-r--r--   0        0        0    25019 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/distgit.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/exceptions.py
--rw-r--r--   0        0        0    40197 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/local_project.py
--rw-r--r--   0        0        0    35127 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/patches.py
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/pkgtool.py
--rw-r--r--   0        0        0    29471 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/schema.py
--rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/security.py
--rw-r--r--   0        0        0    13547 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/source_git.py
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/status.py
--rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/sync.py
--rw-r--r--   0        0        0    53439 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/upstream.py
--rw-r--r--   0        0        0    10496 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/vm_image_build.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/__init__.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/build.py
--rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/create_update.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/dist_git.py
--rw-r--r--   0        0        0    15635 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/dist_git_init.py
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/init.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/packit_base.py
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/prepare_sources.py
--rw-r--r--   0        0        0     7011 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/propose_downstream.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/push_updates.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/source_git.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/source_git_init.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/source_git_status.py
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/srpm.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/status.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/sync_from_downstream.py
--rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/types.py
--rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/update_dist_git.py
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/update_source_git.py
--rw-r--r--   0        0        0    13599 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/utils.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/validate_config.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/builds/__init__.py
--rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/builds/copr_build.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/builds/in_image_builder.py
--rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/builds/koji_build.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/builds/local_build.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/cli/builds/mock_build.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/__init__.py
--rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/aliases.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/commands.py
--rw-r--r--   0        0        0    24627 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/common_package_config.py
--rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/config.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/job_config.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/notifications.py
--rw-r--r--   0        0        0    19870 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/package_config.py
--rw-r--r--   0        0        0     9005 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/package_config_validator.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/requirements.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/config/sources.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/data/__init__.py
--rwxr-xr-x   0        0        0     3233 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/data/_packitpatch
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/bodhi.py
--rw-r--r--   0        0        0    10708 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/changelog_helper.py
--rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/commands.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/decorators.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/extensions.py
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/koji_helper.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/logging.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/lookaside.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/monitoring.py
--rw-r--r--   0        0        0    18617 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/repo.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/source_script.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/upstream_version.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 packitos-0.95.0/packit/utils/versions.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 packitos-0.95.0/plans/README.md
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 packitos-0.95.0/plans/full.fmf
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 packitos-0.95.0/plans/git_reference.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 packitos-0.95.0/plans/main.fmf
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 packitos-0.95.0/plans/rpmlint.fmf
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 packitos-0.95.0/plans/session-recording.fmf
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 packitos-0.95.0/plans/smoke.fmf
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/__init__.py
--rw-r--r--   0        0        0     7163 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/conftest.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/full.fmf
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/smoke.fmf
--rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/smoke.sh
--rw-r--r--   0        0        0    22298 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/spellbook.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/copr_config
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cockpit-ostree/Makefile
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cockpit-ostree/cockpit-ostree.spec.dg
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cockpit-ostree/cockpit-ostree.spec.in
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cockpit-ostree/packit.yaml
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cronie/.cronie.metadata
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cronie/.gitignore
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cronie/SOURCES/cronie-1.5.2-context-role.patch
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cronie/SOURCES/cronie-1.5.2-restart-on-failure.patch
--rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cronie/SOURCES/fix-memory-leaks.patch
--rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cronie/SOURCES/fix-unsafe-code.patch
--rw-r--r--   0        0        0    19523 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/cronie/SPECS/cronie.spec
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/dg-ogr/.packit.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/dg-ogr/README.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/dg-ogr/README.packit
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/dg-ogr/python-ogr.spec
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/dg-ogr/sources
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/dist_git/.packit.yaml
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/dist_git/beer.spec
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/dist_git_with_autochangelog/.packit.yaml
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/dist_git_with_autochangelog/beer.spec
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/edd/.packit.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/edd/LICENSE
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/edd/Makefile
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/edd/README.rst
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/edd/edd
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/edd/edd.spec
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/edd/docs/man.rst
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/empty_changelog/.packit.yaml
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/empty_changelog/beer.spec
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/no_version_tag_in_spec/.packit.yaml
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/no_version_tag_in_spec/beer.spec
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/no_version_tag_in_spec/source
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/osbuild/.packit.yaml
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/osbuild/__init__.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/osbuild/osbuild.spec
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/osbuild/setup.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/osbuild/sources/test
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/previous/git-diff.patch
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/previous/missing-diff-line.patch
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/previous/unified-diff.patch
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/previous/weird-identical.patch
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/regenerated/git-diff.patch
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/regenerated/missing-diff-line.patch
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/regenerated/unified-diff.patch
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/regenerated/weird-identical.patch
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/rpms/hello/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/rpms/hello/hello.spec
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/src/hello/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/src/hello/.distro/hello.spec
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/patches/src/hello/.distro/source-git.yaml
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/rpms/hello/0017-Patch-This..patch
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/rpms/hello/from-git.patch
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/rpms/hello/hello.spec
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/rpms/hello/sources
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/rpms/hello/turn-into-fedora.patch
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/snapd/.packit.yaml
--rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/snapd/packaging/fedora/fix-spec
--rwxr-xr-x   0        0        0     1866 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/snapd/packaging/fedora/pack-source
--rw-r--r--   0        0        0    18386 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/snapd/packaging/fedora/snapd.spec
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/snapd/packaging/fedora/some-file-to-add
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/snapd/vendor/vendor.json
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/sourcegit/source_git/ignored_file.txt
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/sourcegit/source_git/.distro/beer.spec
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/sourcegit/source_git/.distro/source-git.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/sourcegit/upstream/big-source-file.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/spec_not_in_root/upstream/.packit.yaml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/spec_not_in_root/upstream/dir_with_spec/beer.spec
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/src/.gitignore
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/src/hello/Makefile
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/src/hello/README.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/src/hello/hello.rs
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/sync_files/a.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/sync_files/b.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/sync_files/c.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/sync_files/example_dir/d.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/sync_files/example_dir/e.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/sync_files/example_dir/f.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/upstream_git/.packit.yaml
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/upstream_git/beer.spec
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/upstream_git_macro_in_source/.packit.yaml
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/upstream_git_macro_in_source/beer.spec
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/upstream_git_weird_sources/.packit.yaml
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/upstream_git_weird_sources/beer.spec
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/upstream_git_with_multiple_sources/.packit.yaml
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/upstream_git_with_multiple_sources/beer.spec
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/.packit.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/AUDIT
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/BENCHMARKS
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/BUGS
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/COPYING
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Changelog
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/FAQ
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/INSTALL
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/README
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/README.security
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/REWARD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/SIZE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/SPEED
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/TODO
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/TUNING
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/vsftpd.8
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/vsftpd.conf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/vsftpd.conf.5
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/EXAMPLE/example
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd-generator
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd.ftpusers
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd.pam
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd.service
--rw-r--r--   0        0        0    27817 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd.spec
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd.target
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd.user_list
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd.xinetd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd@.service
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd_conf_migrate.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/RedHat/vsftpd.log
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/data/vsftpd/SECURITY/security
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/functional/README.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/functional/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/functional/spellbook.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/functional/test_local_build.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/functional/test_prepare_sources.py
--rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/functional/test_srpm.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/functional/test_validate_config.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/README.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/bodhi_latest_builds.py
--rw-r--r--   0        0        0    42198 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/bodhi_status_updates.py
--rw-r--r--   0        0        0    15059 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_actions.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_api.py
--rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_base_git.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_build.py
--rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_changelog_helper.py
--rw-r--r--   0        0        0    21951 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_copr_build.py
--rw-r--r--   0        0        0    15035 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_create_update.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_distgit.py
--rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_get_api.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_init.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_local_project.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_pagure.py
--rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_patches.py
--rw-r--r--   0        0        0    19018 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_push_updates.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_security.py
--rw-r--r--   0        0        0    24135 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_source_git.py
--rw-r--r--   0        0        0     8032 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_source_git_init.py
--rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_source_git_status.py
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_source_git_synch_push.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_source_git_update_source_git.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_spec.py
--rw-r--r--   0        0        0    18153 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_update.py
--rw-r--r--   0        0        0    20720 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_upstream.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_using_cockpit.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_using_examples.py
--rw-r--r--   0        0        0     7837 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_validate_config.py
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/test_validate_synced_files.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/integration/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/__init__.py
--rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/conftest.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_actions.py
--rw-r--r--   0        0        0    20019 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_api.py
--rw-r--r--   0        0        0    34220 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_base_git.py
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_cli.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_cli_utils.py
--rw-r--r--   0        0        0     5611 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_copr_helper.py
--rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_dg.py
--rw-r--r--   0        0        0     7735 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_dist_git_init.py
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_image_builder.py
--rw-r--r--   0        0        0    11886 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_iterate_packages.py
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_koji_build.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_load_authentication.py
--rw-r--r--   0        0        0    34254 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_local_project.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_login_with_kerberos.py
--rw-r--r--   0        0        0     7693 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_patches.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_prepare_sources.py
--rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_propose_downstream.py
--rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_security.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_specfile.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_status.py
--rw-r--r--   0        0        0     6146 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_sync.py
--rw-r--r--   0        0        0    19993 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_upstream.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/test_utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/config/__init__.py
--rw-r--r--   0        0        0    22698 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/config/test_config.py
--rw-r--r--   0        0        0    14916 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/config/test_config_aliases.py
--rw-r--r--   0        0        0    95205 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/config/test_package_config.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/__init__.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_changelog_helper.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_commands.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_decorators.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_dist_git_instance.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_exceptions.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_koji_helper.py
--rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_lookaside.py
--rw-r--r--   0        0        0    16223 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_repo.py
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_source_script.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_upstream_version.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 packitos-0.95.0/tests/unit/utils/test_versions.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/README.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/__init__.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/main.fmf
--rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_api.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_base_git.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_image_builder.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_local_project.py
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_repository_cache.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_status.py
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/testbase.py
--rw-r--r--   0        0        0   513530 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml
--rw-r--r--   0        0        0    53824 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.packit-dist-git2k0adr0g_1.tar.xz
--rw-r--r--   0        0        0  1387468 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.tmpg_51_3z9_1.tar.xz
--rw-r--r--   0        0        0   162050 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.packit-dist-gitfnk035np_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
--rw-r--r--   0        0        0  1425896 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0    86697 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml
--rw-r--r--   0        0        0    64940 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.tmp5bwaoc9m_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_base_git/ProposeUpdate.test_download_remote_sources_via_spec.yaml
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_bad_request.yaml
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_get_token.yaml
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_token_auto_refresh.yaml
--rw-r--r--   0        0        0    34569 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr.yaml
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr_no_merge.yaml
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml.python-requre_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.clone2_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.python-requre_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
--rw-r--r--   0        0        0  2668265 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml.tmpgtdjxv_x_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0    43243 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml.packit-dist-gitzea090jp_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml.tmpv3zw6n9v_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0   155977 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml.packit-dist-gitl12hm88e_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml.tmpyqn3l5sr_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0   152944 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml.tmp9u1xyoyx_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0    40654 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_status.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_status.yaml.tmp620nfd0i_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0    70501 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml.tmpco60quxn_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 packitos-0.95.0/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 packitos-0.95.0/LICENSE
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 packitos-0.95.0/README.md
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 packitos-0.95.0/pyproject.toml
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 packitos-0.95.0/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 packitos-0.96.0/.git_archival.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 packitos-0.96.0/.gitattributes
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 packitos-0.96.0/.packit.yaml
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 packitos-0.96.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 packitos-0.96.0/.zuul.yaml
+-rw-r--r--   0        0        0    57486 2020-02-02 00:00:00.000000 packitos-0.96.0/CHANGELOG.md
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 packitos-0.96.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 packitos-0.96.0/Containerfile
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 packitos-0.96.0/Containerfile.tests
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 packitos-0.96.0/DCO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 packitos-0.96.0/LICENSE_HEADER.txt
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 packitos-0.96.0/Makefile
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 packitos-0.96.0/ansible.cfg
+-rw-r--r--   0        0        0    13441 2020-02-02 00:00:00.000000 packitos-0.96.0/packit.spec
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 packitos-0.96.0/release-conf.yaml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 packitos-0.96.0/.fmf/version
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 packitos-0.96.0/.github/stale.yml
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 packitos-0.96.0/.github/workflows/build-and-push.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 packitos-0.96.0/.github/workflows/check-release-notes.yml
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 packitos-0.96.0/.github/workflows/do_release.yml
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 packitos-0.96.0/.github/workflows/opened-issues-to-the-board.yml
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 packitos-0.96.0/.github/workflows/prepare-release.yml
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 packitos-0.96.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0  1843517 2020-02-02 00:00:00.000000 packitos-0.96.0/design/logo-packit.sketch
+-rw-r--r--   0        0        0   135444 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/hexsticker.png
+-rw-r--r--   0        0        0   132230 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo-dark.png
+-rw-r--r--   0        0        0    75002 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo-extended.jpg
+-rw-r--r--   0        0        0    48468 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo-extended.png
+-rw-r--r--   0        0        0    24881 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo-extended.svg
+-rw-r--r--   0        0        0   106567 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo-guideline.pdf
+-rw-r--r--   0        0        0    66141 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo-no-borders.jpg
+-rw-r--r--   0        0        0   143587 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo-no-borders.png
+-rw-r--r--   0        0        0    20683 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo-small.png
+-rw-r--r--   0        0        0    70268 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo-square-small-borders.jpg
+-rw-r--r--   0        0        0   150044 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo-square-small-borders.png
+-rw-r--r--   0        0        0    43972 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo-stg-square-bigger-borders.svg
+-rw-r--r--   0        0        0   107242 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo-stg-square-small-borders.png
+-rw-r--r--   0        0        0    43981 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo-stg-square-small-borders.svg
+-rw-r--r--   0        0        0    28826 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo-stg.png
+-rw-r--r--   0        0        0    24351 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo-stg.svg
+-rw-r--r--   0        0        0    18005 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo-text.jpg
+-rw-r--r--   0        0        0    14198 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo-text.png
+-rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo-text.svg
+-rw-r--r--   0        0        0   144552 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo-white.png
+-rw-r--r--   0        0        0   158074 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo.png
+-rw-r--r--   0        0        0    14697 2020-02-02 00:00:00.000000 packitos-0.96.0/design/export/logo.svg
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 packitos-0.96.0/files/install-requirements-git.yaml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 packitos-0.96.0/files/install-requirements-pip.yaml
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 packitos-0.96.0/files/install-requirements-rpms.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 packitos-0.96.0/files/local-tests-requirements.yaml
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 packitos-0.96.0/files/packit-testing-farm-prepare-session-recording.yaml
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 packitos-0.96.0/files/packit-testing-farm-prepare.yaml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 packitos-0.96.0/files/zuul-reverse-dep-packit-service.yaml
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 packitos-0.96.0/files/zuul-tests-session-recording.yaml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 packitos-0.96.0/files/zuul-tests.yaml
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 packitos-0.96.0/files/bash-completion/packit
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 packitos-0.96.0/files/tasks/build-rpm-deps.yaml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 packitos-0.96.0/files/tasks/centpkg.yaml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 packitos-0.96.0/files/tasks/generic-dnf-requirements.yaml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 packitos-0.96.0/files/tasks/install-packit-service.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 packitos-0.96.0/files/tasks/install-packit.yaml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 packitos-0.96.0/files/tasks/ogr.yaml
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 packitos-0.96.0/files/tasks/packit-service-requirements.yaml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 packitos-0.96.0/files/tasks/project-dir.yaml
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 packitos-0.96.0/files/tasks/python-compile-deps.yaml
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 packitos-0.96.0/files/tasks/requre.yaml
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 packitos-0.96.0/files/tasks/rpm-test-deps.yaml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 packitos-0.96.0/files/tasks/sandcastle.yaml
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 packitos-0.96.0/files/tasks/specfile.yaml
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/__init__.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/actions.py
+-rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/actions_handler.py
+-rw-r--r--   0        0        0    92130 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/api.py
+-rw-r--r--   0        0        0    24887 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/base_git.py
+-rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/command_handler.py
+-rw-r--r--   0        0        0     9167 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/constants.py
+-rw-r--r--   0        0        0    20419 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/copr_helper.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/dist_git_instance.py
+-rw-r--r--   0        0        0    26519 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/distgit.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/exceptions.py
+-rw-r--r--   0        0        0    40197 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/local_project.py
+-rw-r--r--   0        0        0    35127 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/patches.py
+-rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/pkgtool.py
+-rw-r--r--   0        0        0    29596 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/schema.py
+-rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/security.py
+-rw-r--r--   0        0        0    13547 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/source_git.py
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/status.py
+-rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/sync.py
+-rw-r--r--   0        0        0    54070 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/upstream.py
+-rw-r--r--   0        0        0    10496 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/vm_image_build.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/__init__.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/build.py
+-rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/create_update.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/dist_git.py
+-rw-r--r--   0        0        0    15635 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/dist_git_init.py
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/init.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/packit_base.py
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/prepare_sources.py
+-rw-r--r--   0        0        0     7011 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/propose_downstream.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/push_updates.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/source_git.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/source_git_init.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/source_git_status.py
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/srpm.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/status.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/sync_from_downstream.py
+-rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/types.py
+-rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/update_dist_git.py
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/update_source_git.py
+-rw-r--r--   0        0        0    13599 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/utils.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/validate_config.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/builds/__init__.py
+-rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/builds/copr_build.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/builds/in_image_builder.py
+-rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/builds/koji_build.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/builds/local_build.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/cli/builds/mock_build.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/config/__init__.py
+-rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/config/aliases.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/config/commands.py
+-rw-r--r--   0        0        0    24810 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/config/common_package_config.py
+-rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/config/config.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/config/job_config.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/config/notifications.py
+-rw-r--r--   0        0        0    19870 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/config/package_config.py
+-rw-r--r--   0        0        0     9005 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/config/package_config_validator.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/config/requirements.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/config/sources.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/data/__init__.py
+-rwxr-xr-x   0        0        0     3233 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/data/_packitpatch
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/utils/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/utils/bodhi.py
+-rw-r--r--   0        0        0    10759 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/utils/changelog_helper.py
+-rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/utils/commands.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/utils/decorators.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/utils/extensions.py
+-rw-r--r--   0        0        0    10373 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/utils/koji_helper.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/utils/logging.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/utils/lookaside.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/utils/monitoring.py
+-rw-r--r--   0        0        0    18617 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/utils/repo.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/utils/source_script.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/utils/upstream_version.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 packitos-0.96.0/packit/utils/versions.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 packitos-0.96.0/plans/README.md
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 packitos-0.96.0/plans/full.fmf
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 packitos-0.96.0/plans/git_reference.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 packitos-0.96.0/plans/main.fmf
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 packitos-0.96.0/plans/rpmlint.fmf
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 packitos-0.96.0/plans/session-recording.fmf
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 packitos-0.96.0/plans/smoke.fmf
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/__init__.py
+-rw-r--r--   0        0        0     7163 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/conftest.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/full.fmf
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/smoke.fmf
+-rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/smoke.sh
+-rw-r--r--   0        0        0    22298 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/spellbook.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/copr_config
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/cockpit-ostree/Makefile
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/cockpit-ostree/cockpit-ostree.spec.dg
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/cockpit-ostree/cockpit-ostree.spec.in
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/cockpit-ostree/packit.yaml
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/cronie/.cronie.metadata
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/cronie/.gitignore
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/cronie/SOURCES/cronie-1.5.2-context-role.patch
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/cronie/SOURCES/cronie-1.5.2-restart-on-failure.patch
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/cronie/SOURCES/fix-memory-leaks.patch
+-rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/cronie/SOURCES/fix-unsafe-code.patch
+-rw-r--r--   0        0        0    19523 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/cronie/SPECS/cronie.spec
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/dg-ogr/.packit.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/dg-ogr/README.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/dg-ogr/README.packit
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/dg-ogr/python-ogr.spec
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/dg-ogr/sources
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/dist_git/.packit.yaml
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/dist_git/beer.spec
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/dist_git_with_autochangelog/.packit.yaml
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/dist_git_with_autochangelog/beer.spec
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/edd/.packit.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/edd/LICENSE
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/edd/Makefile
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/edd/README.rst
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/edd/edd
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/edd/edd.spec
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/edd/docs/man.rst
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/empty_changelog/.packit.yaml
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/empty_changelog/beer.spec
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/no_version_tag_in_spec/.packit.yaml
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/no_version_tag_in_spec/beer.spec
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/no_version_tag_in_spec/source
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/osbuild/.packit.yaml
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/osbuild/__init__.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/osbuild/osbuild.spec
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/osbuild/setup.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/osbuild/sources/test
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/patches/previous/git-diff.patch
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/patches/previous/missing-diff-line.patch
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/patches/previous/unified-diff.patch
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/patches/previous/weird-identical.patch
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/patches/regenerated/git-diff.patch
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/patches/regenerated/missing-diff-line.patch
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/patches/regenerated/unified-diff.patch
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/patches/regenerated/weird-identical.patch
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/patches/rpms/hello/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/patches/rpms/hello/hello.spec
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/patches/src/hello/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/patches/src/hello/.distro/hello.spec
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/patches/src/hello/.distro/source-git.yaml
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/rpms/hello/0017-Patch-This..patch
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/rpms/hello/from-git.patch
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/rpms/hello/hello.spec
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/rpms/hello/sources
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/rpms/hello/turn-into-fedora.patch
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/snapd/.packit.yaml
+-rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/snapd/packaging/fedora/fix-spec
+-rwxr-xr-x   0        0        0     1866 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/snapd/packaging/fedora/pack-source
+-rw-r--r--   0        0        0    18386 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/snapd/packaging/fedora/snapd.spec
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/snapd/packaging/fedora/some-file-to-add
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/snapd/vendor/vendor.json
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/sourcegit/source_git/ignored_file.txt
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/sourcegit/source_git/.distro/beer.spec
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/sourcegit/source_git/.distro/source-git.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/sourcegit/upstream/big-source-file.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/spec_not_in_root/upstream/.packit.yaml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/spec_not_in_root/upstream/dir_with_spec/beer.spec
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/src/.gitignore
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/src/hello/Makefile
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/src/hello/README.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/src/hello/hello.rs
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/sync_files/a.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/sync_files/b.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/sync_files/c.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/sync_files/example_dir/d.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/sync_files/example_dir/e.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/sync_files/example_dir/f.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/upstream_git/.packit.yaml
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/upstream_git/beer.spec
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/upstream_git_macro_in_source/.packit.yaml
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/upstream_git_macro_in_source/beer.spec
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/upstream_git_weird_sources/.packit.yaml
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/upstream_git_weird_sources/beer.spec
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/upstream_git_with_multiple_sources/.packit.yaml
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/upstream_git_with_multiple_sources/beer.spec
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/.packit.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/AUDIT
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/BENCHMARKS
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/BUGS
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/COPYING
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/Changelog
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/FAQ
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/INSTALL
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/README
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/README.security
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/REWARD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/SIZE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/SPEED
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/TODO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/TUNING
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/vsftpd.8
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/vsftpd.conf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/vsftpd.conf.5
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/EXAMPLE/example
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/Fedora/vsftpd-generator
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/Fedora/vsftpd.ftpusers
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/Fedora/vsftpd.pam
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/Fedora/vsftpd.service
+-rw-r--r--   0        0        0    27817 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/Fedora/vsftpd.spec
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/Fedora/vsftpd.target
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/Fedora/vsftpd.user_list
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/Fedora/vsftpd.xinetd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/Fedora/vsftpd@.service
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/Fedora/vsftpd_conf_migrate.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/RedHat/vsftpd.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/data/vsftpd/SECURITY/security
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/functional/README.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/functional/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/functional/spellbook.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/functional/test_local_build.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/functional/test_prepare_sources.py
+-rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/functional/test_srpm.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/functional/test_validate_config.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/README.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/bodhi_latest_builds.py
+-rw-r--r--   0        0        0    42198 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/bodhi_status_updates.py
+-rw-r--r--   0        0        0    15059 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_actions.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_api.py
+-rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_base_git.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_build.py
+-rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_changelog_helper.py
+-rw-r--r--   0        0        0    21951 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_copr_build.py
+-rw-r--r--   0        0        0    15035 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_create_update.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_distgit.py
+-rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_get_api.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_init.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_local_project.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_pagure.py
+-rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_patches.py
+-rw-r--r--   0        0        0    19018 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_push_updates.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_security.py
+-rw-r--r--   0        0        0    24135 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_source_git.py
+-rw-r--r--   0        0        0     8032 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_source_git_init.py
+-rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_source_git_status.py
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_source_git_synch_push.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_source_git_update_source_git.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_spec.py
+-rw-r--r--   0        0        0    19938 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_update.py
+-rw-r--r--   0        0        0    20736 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_upstream.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_using_cockpit.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_using_examples.py
+-rw-r--r--   0        0        0     7837 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_validate_config.py
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/test_validate_synced_files.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/integration/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/conftest.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_actions.py
+-rw-r--r--   0        0        0    20023 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_api.py
+-rw-r--r--   0        0        0    34586 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_base_git.py
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_cli.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_cli_utils.py
+-rw-r--r--   0        0        0     5611 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_copr_helper.py
+-rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_dg.py
+-rw-r--r--   0        0        0     7735 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_dist_git_init.py
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_image_builder.py
+-rw-r--r--   0        0        0    11886 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_iterate_packages.py
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_koji_build.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_load_authentication.py
+-rw-r--r--   0        0        0    34254 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_local_project.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_login_with_kerberos.py
+-rw-r--r--   0        0        0     7693 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_patches.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_prepare_sources.py
+-rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_propose_downstream.py
+-rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_security.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_specfile.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_status.py
+-rw-r--r--   0        0        0     6146 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_sync.py
+-rw-r--r--   0        0        0    20147 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_upstream.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/test_utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/config/__init__.py
+-rw-r--r--   0        0        0    22698 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/config/test_config.py
+-rw-r--r--   0        0        0    14916 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/config/test_config_aliases.py
+-rw-r--r--   0        0        0    95205 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/config/test_package_config.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/utils/__init__.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/utils/test_changelog_helper.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/utils/test_commands.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/utils/test_decorators.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/utils/test_dist_git_instance.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/utils/test_exceptions.py
+-rw-r--r--   0        0        0     6195 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/utils/test_koji_helper.py
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/utils/test_lookaside.py
+-rw-r--r--   0        0        0    16223 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/utils/test_repo.py
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/utils/test_source_script.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/utils/test_upstream_version.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 packitos-0.96.0/tests/unit/utils/test_versions.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/README.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/__init__.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/main.fmf
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_api.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_base_git.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_image_builder.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_local_project.py
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_repository_cache.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_status.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/testbase.py
+-rw-r--r--   0        0        0   513530 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml
+-rw-r--r--   0        0        0    53824 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.packit-dist-git2k0adr0g_1.tar.xz
+-rw-r--r--   0        0        0  1387468 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.tmpg_51_3z9_1.tar.xz
+-rw-r--r--   0        0        0   162050 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.packit-dist-gitfnk035np_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+-rw-r--r--   0        0        0  1425896 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0    86697 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml
+-rw-r--r--   0        0        0    64940 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.tmp5bwaoc9m_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_base_git/ProposeUpdate.test_download_remote_sources_via_spec.yaml
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_bad_request.yaml
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_get_token.yaml
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_token_auto_refresh.yaml
+-rw-r--r--   0        0        0    34569 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr.yaml
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr_no_merge.yaml
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml.python-requre_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.clone2_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml.python-requre_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml.clone1_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+-rw-r--r--   0        0        0  2668265 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml.tmpgtdjxv_x_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0    43243 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml.packit-dist-gitzea090jp_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml.tmpv3zw6n9v_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0   155977 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml.packit-dist-gitl12hm88e_1.tar.xz -> ../test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml.tmpyqn3l5sr_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0   152944 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml.tmp9u1xyoyx_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0    40654 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_status/TestStatus.test_status.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_status/TestStatus.test_status.yaml.tmp620nfd0i_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0    70501 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 packitos-0.96.0/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml.tmpco60quxn_1.tar.xz -> ../test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 packitos-0.96.0/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 packitos-0.96.0/LICENSE
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 packitos-0.96.0/README.md
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 packitos-0.96.0/pyproject.toml
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 packitos-0.96.0/PKG-INFO
```

### Comparing `packitos-0.95.0/.packit.yaml` & `packitos-0.96.0/.packit.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/.pre-commit-config.yaml` & `packitos-0.96.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/.zuul.yaml` & `packitos-0.96.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/CHANGELOG.md` & `packitos-0.96.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# 0.96.0
+
+- Packit will now upload to lookaside cache sources that are not specified by URLs and are present in the dist-git repo during release sync. Additionally, all the actions ran during syncing release will provide the PACKIT_PROJECT_VERSION env var. (#2297)
+- We have fixed the syncing of ACLs during CentOS Stream release syncing. (#2298)
+
 # 0.95.0
 
 - `packit dist-git init` now allows specifying `--version-update-mask` option and also any arbitrary top-level configuration options. (#2288)
 - We have fixed Packit auto-referencing Upstream Release Monitoring bug for release syncing to CentOS Stream. (#2284)
 
 # 0.94.2
```

### Comparing `packitos-0.95.0/CONTRIBUTING.md` & `packitos-0.96.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/DCO` & `packitos-0.96.0/DCO`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/Makefile` & `packitos-0.96.0/Makefile`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit.spec` & `packitos-0.96.0/packit.spec`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 %if 0%{?el9}
 %bcond_with tests
 %else
 %bcond_without tests
 %endif
 
 Name:           packit
-Version:        0.95.0
+Version:        0.96.0
 Release:        1%{?dist}
 Summary:        A tool for integrating upstream projects with Fedora operating system
 
 License:        MIT
 URL:            https://github.com/packit/packit
 Source0:        %{pypi_source packitos}
 BuildArch:      noarch
@@ -73,14 +73,17 @@
 # Epel9 does not tag the license file in pyproject_files as a license. Manually install it in this case
 %if 0%{?el9}
 %license LICENSE
 %endif
 %doc README.md
 
 %changelog
+* Fri May 03 2024 Packit Team <hello@packit.dev> - 0.96.0-1
+- New upstream release 0.96.0
+
 * Sat Apr 20 2024 Packit Team <hello@packit.dev> - 0.95.0-1
 - New upstream release 0.95.0
 
 * Mon Apr 08 2024 Packit Team <hello@packit.dev> - 0.94.2-1
 - New upstream release 0.94.2
 
 * Mon Mar 25 2024 Packit Team <hello@packit.dev> - 0.94.1-1
```

### Comparing `packitos-0.95.0/.github/stale.yml` & `packitos-0.96.0/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/.github/workflows/build-and-push.yml` & `packitos-0.96.0/.github/workflows/build-and-push.yml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/.github/workflows/do_release.yml` & `packitos-0.96.0/.github/workflows/do_release.yml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/.github/workflows/prepare-release.yml` & `packitos-0.96.0/.github/workflows/prepare-release.yml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/.github/workflows/pypi-publish.yml` & `packitos-0.96.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/logo-packit.sketch` & `packitos-0.96.0/design/logo-packit.sketch`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/hexsticker.png` & `packitos-0.96.0/design/export/hexsticker.png`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo-dark.png` & `packitos-0.96.0/design/export/logo-dark.png`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo-extended.jpg` & `packitos-0.96.0/design/export/logo-extended.jpg`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo-extended.png` & `packitos-0.96.0/design/export/logo-extended.png`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo-extended.svg` & `packitos-0.96.0/design/export/logo-extended.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo-guideline.pdf` & `packitos-0.96.0/design/export/logo-guideline.pdf`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo-no-borders.jpg` & `packitos-0.96.0/design/export/logo-no-borders.jpg`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo-no-borders.png` & `packitos-0.96.0/design/export/logo-no-borders.png`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo-small.png` & `packitos-0.96.0/design/export/logo-small.png`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo-square-small-borders.jpg` & `packitos-0.96.0/design/export/logo-square-small-borders.jpg`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo-square-small-borders.png` & `packitos-0.96.0/design/export/logo-square-small-borders.png`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo-stg-square-bigger-borders.svg` & `packitos-0.96.0/design/export/logo-stg-square-bigger-borders.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo-stg-square-small-borders.png` & `packitos-0.96.0/design/export/logo-stg-square-small-borders.png`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo-stg-square-small-borders.svg` & `packitos-0.96.0/design/export/logo-stg-square-small-borders.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo-stg.png` & `packitos-0.96.0/design/export/logo-stg.png`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo-stg.svg` & `packitos-0.96.0/design/export/logo-stg.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo-text.jpg` & `packitos-0.96.0/design/export/logo-text.jpg`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo-text.png` & `packitos-0.96.0/design/export/logo-text.png`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo-text.svg` & `packitos-0.96.0/design/export/logo-text.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo-white.png` & `packitos-0.96.0/design/export/logo-white.png`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo.png` & `packitos-0.96.0/design/export/logo.png`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/design/export/logo.svg` & `packitos-0.96.0/design/export/logo.svg`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/files/local-tests-requirements.yaml` & `packitos-0.96.0/files/local-tests-requirements.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/files/zuul-reverse-dep-packit-service.yaml` & `packitos-0.96.0/files/zuul-reverse-dep-packit-service.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/files/zuul-tests-session-recording.yaml` & `packitos-0.96.0/files/zuul-tests-session-recording.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/files/tasks/packit-service-requirements.yaml` & `packitos-0.96.0/files/tasks/packit-service-requirements.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/files/tasks/rpm-test-deps.yaml` & `packitos-0.96.0/files/tasks/rpm-test-deps.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/actions.py` & `packitos-0.96.0/packit/actions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/api.py` & `packitos-0.96.0/packit/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,16 +248,15 @@
     def pkg_tool(self) -> str:
         """Returns the packaging tool. Prefers the package-level override."""
         if self.package_config and self.package_config.pkg_tool:
             return self.package_config.pkg_tool
 
         return self.config.pkg_tool
 
-    @property
-    def sync_release_env(self):
+    def sync_release_env(self, version: Optional[str] = None):
         if self.config.command_handler == RunCommandType.sandcastle:
             exec_dir = Path(self._get_sandcastle_exec_dir())
             # working dirs should be placed under
             # self.config.command_handler_working_dir
             # when running this code as a service
             downstream_suffix = Path(self.dg.local_project.working_dir).relative_to(
                 self.config.command_handler_work_dir,
@@ -274,14 +273,17 @@
                 ),
             }
         else:
             env = {
                 "PACKIT_DOWNSTREAM_REPO": str(self.dg.local_project.working_dir),
                 "PACKIT_UPSTREAM_REPO": str(self.up.local_project.working_dir),
             }
+        if version:
+            env["PACKIT_PROJECT_VERSION"] = version
+
         return env | self.up.package_config.get_package_names_as_env()
 
     def update_dist_git(
         self,
         version: Optional[str],
         upstream_ref: Optional[str],
         add_new_sources: bool,
@@ -352,28 +354,28 @@
         # the working directories of the repositories.
         for item in synced_files:
             item.resolve(
                 src_base=self.up.local_project.working_dir,
                 dest_base=self.dg.local_project.working_dir,
             )
 
-        if self.up.with_action(
+        if self.up.actions_handler.with_action(
             action=ActionName.prepare_files,
-            env=self.sync_release_env,
+            env=self.sync_release_env(version=version),
         ):
             synced_files = self._prepare_files_to_sync(
                 synced_files=synced_files,
                 full_version=version,
                 upstream_tag=upstream_tag,
                 resolved_bugs=resolved_bugs,
             )
         sync_files(synced_files)
-        if upstream_ref and self.up.with_action(
+        if upstream_ref and self.up.actions_handler.with_action(
             action=ActionName.create_patches,
-            env=self.sync_release_env,
+            env=self.sync_release_env(version=version),
         ):
             patches = self.up.create_patches(
                 upstream=upstream_ref,
                 destination=str(self.dg.absolute_specfile_dir),
             )
             # Undo identical patches, but don't remove them
             # from the list, so that they are added to the spec-file.
@@ -796,21 +798,29 @@
             "product": ["Fedora"],
             "component": [package_name],
             "bug_status": "NEW",
             # e.g. python-ogr-50.1 is available
             "summary": "is available",
             "creator": "Upstream Release Monitoring",
         }
+        logger.debug(
+            f"About to search for Bugzilla bugs with these parameters: {query}",
+        )
         try:
             bugs = bzapi.query(query)
         except Exception as ex:
             logger.error(f"There was an error when calling Bugzilla API: {ex!r}")
             return None
 
-        logger.debug(f"Bugzilla IDs found via Bugzilla API: {[bug.id for bug in bugs]}")
+        logger.debug(
+            f"Bugzilla IDs found via Bugzilla API: {[bug.id for bug in bugs]}",
+        )
+
+        if bugs:
+            logger.debug(f"About to find the bug matching version {version}")
 
         for bug in bugs:
             match = re.search(f"{package_name}-(.*?) is available", bug.summary)
             if match and match.group(1) == version:
                 logger.debug(f"Found matching bug with ID {bug.id}")
                 return f"rhbz#{bug.id}"
 
@@ -1029,30 +1039,33 @@
 
             if use_downstream_specfile:
                 logger.info(
                     "Using the downstream specfile instead of the upstream one.",
                 )
                 self.up.set_specfile(self.dg.specfile)
 
-            self.up.run_action(
+            self.up.actions_handler.run_action(
                 actions=ActionName.post_upstream_clone,
-                env=self.sync_release_env,
+                env=self.sync_release_env(version=version),
             )
 
             # compare versions here because users can mangle with specfile in
             # post_upstream_clone action
             spec_ver = self.up.get_specfile_version()
             if compare_versions(version, spec_ver) > 0:
                 logger.warning(f"Version {spec_ver!r} in spec file is outdated.")
 
             self.check_version_distance(version, spec_ver, dist_git_branch)
 
             self.dg.check_last_commit()
 
-            self.up.run_action(actions=ActionName.pre_sync, env=self.sync_release_env)
+            self.up.actions_handler.run_action(
+                actions=ActionName.pre_sync,
+                env=self.sync_release_env(version=version),
+            )
             if not use_downstream_specfile:
                 self.up.specfile.reload()
 
             if create_pr:
                 local_pr_branch = (
                     f"{version}-{dist_git_branch}-{local_pr_branch_suffix}"
                 )
@@ -1077,26 +1090,25 @@
                     user=self.config.fas_user,
                 )
                 if create_pr and add_pr_instructions
                 else ""
             )
 
             # Evaluate the commit title and message
-            commit_msg_action_output = self.up.get_output_from_action(
+            commit_msg_action_output = self.up.actions_handler.get_output_from_action(
                 ActionName.commit_message,
                 env={
-                    "PACKIT_PROJECT_VERSION": version,
                     "PACKIT_UPSTREAM_TAG": upstream_tag,
                     "PACKIT_UPSTREAM_COMMIT": self.up.local_project.commit_hexsha,
                     "PACKIT_DEBUG_DIVIDER": COMMIT_ACTION_DIVIDER.strip(),
                     "PACKIT_RESOLVED_BUGS": " ".join(resolved_bugs)
                     if resolved_bugs
                     else "",
                 }
-                | self.sync_release_env,
+                | self.sync_release_env(version),
             )
 
             commit_title, commit_description = get_commit_message_from_action(
                 output=commit_msg_action_output,
                 default_title=title or f"Update to {version} upstream release",
                 default_description=description
                 or self.get_default_commit_description(upstream_tag, resolved_bugs),
@@ -1487,44 +1499,29 @@
             force_new_sources: Download/upload the archive even if it's
                 name is already in the cache or in sources file.
                 Actually, fedpkg/centpkg won't upload it if archive with the same
                 name & hash is already there, so this might be useful only if
                 you want to upload archive with the same name but different hash.
             pkg_tool: Tool to upload sources.
         """
-
-        archives_to_upload = False
-        sources_file = self.dg.local_project.working_dir / "sources"
-
         # We need to download the sources beforehand! Previous solution was relying
         # on the HTTP index of the uploaded archives in the lookaside cache which
         # appears to be Fedora-only. Making the check distro-agnostic requires us
         # to use the `pyrpkg` which needs hash of the archive when doing the lookup,
         # therefore it needs the archive itself beforehand.
-        archives = self.dg.download_upstream_archives()
-
-        # Here, dist-git spec-file has already been updated from the upstream spec-file.
-        # => Any update done to the Source tags in upstream
-        # is already available in the dist-git spec-file.
-        for archive in archives:
-            archive_name = os.path.basename(archive)
-
-            archive_name_in_cache = self.dg.is_archive_in_lookaside_cache(
-                archive,
-            )
-            archive_name_in_sources_file = (
-                sources_file.is_file() and archive_name in sources_file.read_text()
-            )
+        upstream_archives = self.dg.download_upstream_archives()
+        # Check for existing local archives and upload those as well
+        local_archives = self.get_local_archives_to_upload()
 
-            if not archive_name_in_cache or not archive_name_in_sources_file:
-                archives_to_upload = True
-                # found one that needs uploading, no need to continue
-                break
+        archives = upstream_archives + local_archives
 
-        if not archives_to_upload and not force_new_sources:
+        if (
+            not self.should_archives_be_uploaded_to_lookaside(archives)
+            and not force_new_sources
+        ):
             return
 
         # There is at least one archive to upload,
         # because it is missing from lookaside, sources file, or both,
         # or because force_new_sources is set.
         self.init_kerberos_ticket()
         # Upload all of archives. If we uploaded only those that need uploading,
@@ -1533,14 +1530,47 @@
         # to uploading, and it replaces it entirely, losing the previous content
         self.dg.upload_to_lookaside_cache(
             archives=archives,
             pkg_tool=pkg_tool,
             offline=not self.package_config.upload_sources,
         )
 
+    def should_archives_be_uploaded_to_lookaside(self, archives: list[Path]) -> bool:
+        # Here, dist-git spec-file has already been updated from the upstream spec-file.
+        # => Any update done to the Source tags in upstream
+        # is already available in the dist-git spec-file.
+        sources_file = self.dg.local_project.working_dir / "sources"
+        for archive in archives:
+            archive_name = os.path.basename(archive)
+            archive_name_in_cache = self.dg.is_archive_in_lookaside_cache(
+                archive,
+            )
+            archive_name_in_sources_file = (
+                sources_file.is_file() and archive_name in sources_file.read_text()
+            )
+
+            if not archive_name_in_cache or not archive_name_in_sources_file:
+                return True
+
+        return False
+
+    def get_local_archives_to_upload(self) -> list[Path]:
+        local_archives = self.dg.local_archive_names
+        local_archives_to_upload = []
+        for local_archive in local_archives:
+            archive_path = self.dg.absolute_source_dir / local_archive
+            if not archive_path.exists():
+                logger.debug(
+                    f"Local archive {archive_path} doesn't exist. Skipping the handling of it.",
+                )
+                continue
+            local_archives_to_upload.append(archive_path)
+
+        return local_archives_to_upload
+
     def build(
         self,
         dist_git_branch: str,
         scratch: bool = False,
         nowait: bool = False,
         koji_target: Optional[str] = None,
         from_upstream: bool = False,
@@ -1646,15 +1676,15 @@
             update_release: whether to change Release in the spec-file
             result_dir: directory where the specfile directory content should be copied
             create_symlinks: whether symlinks should be created instead of copying the files
                 (currently when the archive is created outside the specfile dir, or in the future
                  if we will create symlinks in some other places)
             merged_ref: git ref in the upstream repo used to identify correct most recent tag
         """
-        self.up.run_action(
+        self.up.actions_handler.run_action(
             actions=ActionName.post_upstream_clone,
             env=self.up.package_config.get_package_names_as_env(),
         )
 
         if update_release is None:
             update_release = self.package_config.update_release
         try:
@@ -1756,15 +1786,15 @@
             rpm_dir: Path to the directory where the RPMs are meant to be placed.
             release_suffix: Release suffix that is used during modification of specfile.
             merged_ref: git ref in the upstream repo used to identify correct most recent tag
 
         Returns:
             List of paths to the built RPMs.
         """
-        self.up.run_action(
+        self.up.actions_handler.run_action(
             actions=ActionName.post_upstream_clone,
             env=self.up.package_config.get_package_names_as_env(),
         )
 
         try:
             self.up.prepare_upstream_for_srpm_creation(
                 upstream_ref=upstream_ref,
```

### Comparing `packitos-0.95.0/packit/base_git.py` & `packitos-0.96.0/packit/base_git.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # Copyright Contributors to the Packit project.
 # SPDX-License-Identifier: MIT
 
 import os
-import shlex
 from collections.abc import Iterable
 from importlib.metadata import version
 from logging import getLogger
 from pathlib import Path
-from typing import Callable, Optional
+from typing import Optional
 
 import git
 import requests
 import rpm
 from git import GitCommandError, PushInfo
 from ogr.abstract import AccessLevel, GitProject, PullRequest
+from ogr.services.pagure import PagureProject
 from specfile import Specfile
 from specfile.exceptions import (
     DuplicateSourceException,
     SourceNumberException,
     SpecfileException,
 )
 from specfile.macro_definitions import CommentOutStyle
 from specfile.sections import Section
 
-from packit.actions import ActionName
+from packit.actions_handler import ActionsHandler
 from packit.command_handler import RUN_COMMAND_HANDLER_MAPPING, CommandHandler
 from packit.config import Config, RunCommandType
 from packit.config.common_package_config import MultiplePackages
 from packit.constants import HTTP_REQUEST_TIMEOUT
 from packit.exceptions import PackitDownloadFailedException, PackitException
 from packit.local_project import LocalProject
 from packit.patches import PatchMetadata
@@ -56,14 +56,15 @@
         self.package_config = package_config
         self._specfile_path: Optional[Path] = None
         self._specfile: Optional[Specfile] = None
         self.allowed_gpg_keys: Optional[list[str]] = None
 
         self._handler_kls = None
         self._command_handler: Optional[CommandHandler] = None
+        self._actions_handler: Optional[ActionsHandler] = None
 
     @property
     def handler_kls(self):
         if self._handler_kls is None:
             logger.debug(f"Command handler: {self.config.command_handler}")
             self._handler_kls = RUN_COMMAND_HANDLER_MAPPING[self.config.command_handler]
         return self._handler_kls
@@ -74,14 +75,23 @@
             self._command_handler = self.handler_kls(
                 local_project=self.local_project,
                 config=self.config,
             )
         return self._command_handler
 
     @property
+    def actions_handler(self):
+        if not self._actions_handler:
+            self._actions_handler = ActionsHandler(
+                self.package_config,
+                self.command_handler,
+            )
+        return self._actions_handler
+
+    @property
     def repository_cache(self) -> Optional[RepositoryCache]:
         if self.config.repository_cache:
             return RepositoryCache(
                 cache_path=self.config.repository_cache,
                 add_new=self.config.add_repositories_to_repository_cache,
             )
         return None
@@ -214,156 +224,14 @@
             )
         self.local_project.git_repo.index.write()
 
         with commit_message_file(main_msg, msg, trailers) as commit_message:
             commit_args = ["-F", commit_message]
             self.local_project.git_repo.git.commit(*commit_args)
 
-    def run_action(
-        self,
-        actions: ActionName,
-        method: Optional[Callable] = None,
-        env: Optional[dict] = None,
-        *args,
-        **kwargs,
-    ):
-        """
-        Run the method in the self._with_action block.
-
-        Usage:
-
-        >   self._run_action(
-        >        action_name="sync", method=dg.sync_files, upstream_project=up.local_project
-        >   )
-        >   # If user provided custom command for the `sync`, it will be used.
-        >   # Otherwise, the method `dg.sync_files` will be used
-        >   # with parameter `upstream_project=up.local_project`
-        >
-        >   self._run_action(action_name="pre-sync")
-        >   # This will be used as an optional hook
-
-        :param actions: ActionName enum (Name of the action that can be overwritten
-                                                in the package_config.actions)
-        :param method: method to run if the action was not defined by user
-                    (if not specified, the action can be used for custom hooks)
-        :param args: args for the method
-        :param kwargs: kwargs for the method
-        """
-        if not method:
-            logger.debug(f"Running {actions} hook.")
-        if self.with_action(action=actions, env=env) and method:
-            method(*args, **kwargs)
-
-    def has_action(self, action: ActionName) -> bool:
-        """
-        Is the action defined in the config?
-        """
-        return action in self.package_config.actions
-
-    def get_commands_for_actions(self, action: ActionName) -> list[list[str]]:
-        """
-        Parse the following types of the structure and return list of commands in the form of list.
-
-        I)
-        action_name: "one cmd"
-
-        II)
-        action_name:
-          - "one cmd""
-
-        III)
-        action_name:
-          - ["one", "cmd"]
-
-
-        Returns [["one", "cmd"]] for all of them.
-
-        :param action: str or list[str] or list[list[str]]
-        :return: list[list[str]]
-        """
-        configured_action = self.package_config.actions[action]
-        if isinstance(configured_action, str):
-            configured_action = [configured_action]
-
-        if not isinstance(configured_action, list):
-            raise ValueError(
-                f"Expecting 'str' or 'list' as a command, got '{type(configured_action)}'. "
-                f"The value: {configured_action}",
-            )
-
-        parsed_commands = []
-        for cmd in configured_action:
-            if isinstance(cmd, str):
-                parsed_commands.append(shlex.split(cmd))
-            elif isinstance(cmd, list):
-                parsed_commands.append(cmd)
-            else:
-                raise ValueError(
-                    f"Expecting 'str' or 'list' as a command, got '{type(cmd)}'. "
-                    f"The value: {cmd}",
-                )
-        return parsed_commands
-
-    def with_action(self, action: ActionName, env: Optional[dict] = None) -> bool:
-        """
-        If the action is defined in the self.package_config.actions,
-        we run it and return False (so we can skip the if block)
-
-        If the action is not defined, return True.
-
-        Usage:
-
-        >   if self._with_action(action_name="patch"):
-        >       # Run default implementation
-        >
-        >   # Custom command was run if defined in the config
-
-        Context manager is currently not possible without ugly hacks:
-        https://stackoverflow.com/questions/12594148/skipping-execution-of-with-block
-        https://www.python.org/dev/peps/pep-0377/ (rejected)
-
-        :param action: ActionName enum (Name of the action that can be overwritten
-                                                in the package_config.actions)
-        :param env: dict with env vars to set for the command
-        :return: True, if the action is not overwritten, False when custom command was run
-        """
-        logger.debug(f"Running {action}.")
-        if action in self.package_config.actions:
-            commands_to_run = self.get_commands_for_actions(action)
-            logger.info(f"Using user-defined script for {action}: {commands_to_run}")
-            for cmd in commands_to_run:
-                self.command_handler.run_command(command=cmd, env=env, print_live=True)
-            return False
-        logger.debug(f"Running default implementation for {action}.")
-        return True
-
-    def get_output_from_action(
-        self,
-        action: ActionName,
-        env: Optional[dict] = None,
-    ) -> Optional[list[str]]:
-        """
-        Run self.actions[action] command(s) and return their outputs.
-        """
-        if action not in self.package_config.actions:
-            return None
-
-        commands_to_run = self.get_commands_for_actions(action)
-
-        logger.info(f"Using user-defined script for {action}: {commands_to_run}")
-        return [
-            self.command_handler.run_command(
-                cmd,
-                return_output=True,
-                env=env,
-                print_live=True,
-            ).stdout
-            for cmd in commands_to_run
-        ]
-
     def specfile_add_patches(
         self,
         patch_list: list[PatchMetadata],
         patch_id_digits: int = 4,
     ) -> None:
         """
         Add the given list of (patch_name, msg) to the specfile.
@@ -733,14 +601,20 @@
         for user in committers - fork_committers - fork_owners:
             logger.debug(f"Adding user {user}")
             try:
                 fork.add_user(user, AccessLevel.push)
             except Exception as ex:
                 logger.debug(f"It was not possible to add user {user}: {ex}")
 
+        if not isinstance(project, PagureProject):
+            logger.debug(
+                "Syncing of group ACLs is skipped for forges other than Pagure.",
+            )
+            return
+
         commit_groups = project.which_groups_can_merge_pr()
         fork_commit_groups = fork.which_groups_can_merge_pr()
         for group in fork_commit_groups - commit_groups:
             logger.debug(f"Removing group {group}")
             fork.remove_group(group)
         for group in commit_groups - fork_commit_groups:
             logger.debug(f"Adding group {group}")
```

### Comparing `packitos-0.95.0/packit/command_handler.py` & `packitos-0.96.0/packit/command_handler.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/constants.py` & `packitos-0.96.0/packit/constants.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/copr_helper.py` & `packitos-0.96.0/packit/copr_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/dist_git_instance.py` & `packitos-0.96.0/packit/dist_git_instance.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/distgit.py` & `packitos-0.96.0/packit/distgit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # Copyright Contributors to the Packit project.
 # SPDX-License-Identifier: MIT
 
 import logging
 import re
 import tempfile
 from collections.abc import Iterable, Sequence
+from functools import partial
 from pathlib import Path
 from typing import Optional, Union
 
 import cccolutils
 import git
 from bodhi.client.bindings import BodhiClientException
 from fedora.client import AuthError
+from lazy_object_proxy import Proxy
 from ogr.abstract import PullRequest
 from specfile.utils import NEVR
 
 from packit.base_git import PackitRepositoryBase
+from packit.command_handler import CommandHandler
 from packit.config import (
     Config,
     MultiplePackages,
     PackageConfig,
     get_local_package_config,
 )
 from packit.constants import EXISTING_BODHI_UPDATE_REGEX
@@ -157,14 +160,24 @@
             self._local_project.git_project = self.config.get_project(
                 url=self.package_config.dist_git_package_url,
             )
 
         return self._local_project
 
     @property
+    def command_handler(self) -> CommandHandler:
+        if self._command_handler is None:
+            self._command_handler = self.handler_kls(
+                # so that the local_project is evaluated only when needed
+                local_project=Proxy(partial(DistGit.local_project.__get__, self)),  # type: ignore
+                config=self.config,
+            )
+        return self._command_handler
+
+    @property
     def downstream_config(self) -> Optional[PackageConfig]:
         if not self._downstream_config:
             try:
                 self._downstream_config = get_local_package_config(
                     self.local_project.working_dir,
                     repo_name=self.local_project.repo_name,
                 )
@@ -336,28 +349,57 @@
 
         logger.info(f"PR created: {dist_git_pr.url}")
         return dist_git_pr
 
     @property
     def upstream_archive_names(self) -> list[str]:
         """
-        Files that are considered upstream and should be uploaded to lookaside.
+        Sources that are considered upstream and should be uploaded to lookaside.
         Currently that's the source identified by spec_source_id (Source0 by default)
         and all other sources specified as URLs in the spec file.
 
-        :return: names of the archives, e.g. ['sen-0.6.1.tar.gz']
+        Returns:
+             names of the archives, e.g. ['sen-0.6.1.tar.gz']
         """
         with self.specfile.sources() as sources:
             archive_names = [
                 s.expanded_filename
                 for s in sources
                 if (s.remote or s.number == self.package_config.spec_source_id_number)
                 and s.valid
             ]
-        logger.debug(f"Upstream archive names: {archive_names}")
+        logger.debug(
+            f"Remote sources or sources specified by spec_source_id (Source0 by default): "
+            f"{archive_names}",
+        )
+        return archive_names
+
+    @property
+    def local_archive_names(self) -> list[str]:
+        """
+        Sources that are considered local (are not specified by URL).
+        Source specified by spec_source_id is excluded as it is
+        handled as upstream archive in upstream_archive_names.
+
+        Returns:
+             names of the archives, e.g. ['sen-0.6.1.tar.gz']
+        """
+        with self.specfile.sources() as sources:
+            archive_names = [
+                s.expanded_filename
+                for s in sources
+                if (
+                    not s.remote
+                    and s.number != self.package_config.spec_source_id_number
+                )
+                and s.valid
+            ]
+        logger.debug(
+            f"Local sources (source specified by spec_source_id excluded): {archive_names}",
+        )
         return archive_names
 
     def download_upstream_archives(self) -> list[Path]:
         """
         Fetch archives for the current upstream release defined in dist-git's spec
 
         :return: list of path to the archives
```

### Comparing `packitos-0.95.0/packit/exceptions.py` & `packitos-0.96.0/packit/exceptions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/local_project.py` & `packitos-0.96.0/packit/local_project.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/patches.py` & `packitos-0.96.0/packit/patches.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/pkgtool.py` & `packitos-0.96.0/packit/pkgtool.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/schema.py` & `packitos-0.96.0/packit/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -434,14 +434,17 @@
 
     # Packaging tool used for interaction with lookaside cache
     pkg_tool = fields.String(missing=None)
     version_update_mask = fields.String(missing=None)
 
     parse_time_macros = fields.Dict(missing=None)
 
+    # sidetag group identifier for downstream Koji builds and Bodhi updates
+    sidetag_group = fields.String(missing=None)
+
     @staticmethod
     def spec_source_id_serialize(value: CommonPackageConfig):
         return value.spec_source_id
 
     @staticmethod
     def spec_source_id_fm(value: Union[str, int]):
         """
```

### Comparing `packitos-0.95.0/packit/security.py` & `packitos-0.96.0/packit/security.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/source_git.py` & `packitos-0.96.0/packit/source_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/status.py` & `packitos-0.96.0/packit/status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/sync.py` & `packitos-0.96.0/packit/sync.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/upstream.py` & `packitos-0.96.0/packit/upstream.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 import datetime
 import logging
 import os
 import re
 import shlex
 import shutil
 import tarfile
-from functools import reduce
+from functools import partial, reduce
 from pathlib import Path
 from typing import Optional, Union
 
 import git
+from lazy_object_proxy import Proxy
 
 from packit.actions import ActionName
 from packit.base_git import PackitRepositoryBase
+from packit.command_handler import CommandHandler
 from packit.config import Config
 from packit.config.common_package_config import MultiplePackages
 from packit.constants import DATETIME_FORMAT, DEFAULT_ARCHIVE_EXT
 from packit.exceptions import (
     PackitCommandFailedError,
     PackitException,
     PackitFailedToCreateRPMException,
@@ -99,14 +101,24 @@
             self._local_project.git_project = self.config.get_project(
                 url=self.package_config.upstream_project_url,
                 required=self._project_required,
             )
         return self._local_project
 
     @property
+    def command_handler(self) -> CommandHandler:
+        if self._command_handler is None:
+            self._command_handler = self.handler_kls(
+                # so that the local_project is evaluated only when needed
+                local_project=Proxy(partial(Upstream.local_project.__get__, self)),  # type: ignore
+                config=self.config,
+            )
+        return self._command_handler
+
+    @property
     def active_branch(self) -> str:
         return self.local_project.ref
 
     def push_to_fork(
         self,
         branch_name: str,
         force: bool = False,
@@ -253,15 +265,15 @@
 
         version = get_upstream_version(self.package_config.downstream_package_name)
         logger.info(f"Version in upstream registries is {version!r}.")
         return version
 
     def get_version_from_action(self) -> str:
         """provide version from action"""
-        action_output = self.get_output_from_action(
+        action_output = self.actions_handler.get_output_from_action(
             action=ActionName.get_current_version,
             env=self.package_config.get_package_names_as_env(),
         )
         return action_output[-1].strip() if action_output else None
 
     def get_version(self) -> str:
         """
@@ -636,15 +648,15 @@
     def create_patches_and_update_specfile(self, upstream_ref) -> None:
         """
         Create patches for the sourcegit and add them to the specfile.
 
         :param upstream_ref: the base git ref for the source git
         """
         env = self.package_config.get_package_names_as_env()
-        if self.with_action(action=ActionName.create_patches, env=env):
+        if self.actions_handler.with_action(action=ActionName.create_patches, env=env):
             patches = self.create_patches(
                 upstream=upstream_ref,
                 destination=str(self.absolute_specfile_dir),
             )
             self.specfile_add_patches(patches)
 
     def koji_build(
@@ -1146,15 +1158,18 @@
             # like when no release_suffix is given: so use "" instead.
             env["PACKIT_RPMSPEC_RELEASE"] = self.upstream.get_spec_release("")
             new_release = release_suffix.format(**env)
         else:
             new_release = self.upstream.get_spec_release(release_suffix)
         env = env | self.upstream.package_config.get_package_names_as_env()
 
-        if self.upstream.with_action(action=ActionName.fix_spec, env=env):
+        if self.upstream.actions_handler.with_action(
+            action=ActionName.fix_spec,
+            env=env,
+        ):
             self.upstream.fix_spec(
                 archive=archive,
                 version=self.current_version,
                 commit=current_commit,
                 update_release=update_release,
                 release=new_release,
             )
@@ -1237,16 +1252,16 @@
         logger.debug(f"Name + version = {dir_name}")
 
         env = {
             "PACKIT_PROJECT_VERSION": self.version,
             "PACKIT_PROJECT_NAME_VERSION": dir_name,
         }
         env = env | self.upstream.package_config.get_package_names_as_env()
-        if self.upstream.has_action(action=ActionName.create_archive):
-            outputs = self.upstream.get_output_from_action(
+        if self.upstream.actions_handler.has_action(action=ActionName.create_archive):
+            outputs = self.upstream.actions_handler.get_output_from_action(
                 action=ActionName.create_archive,
                 env=env,
             )
             if not outputs:
                 raise PackitException("No output from create-archive action.")
 
             archive_path = self._get_archive_path_from_output(outputs)
```

### Comparing `packitos-0.95.0/packit/vm_image_build.py` & `packitos-0.96.0/packit/vm_image_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/build.py` & `packitos-0.96.0/packit/cli/build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/create_update.py` & `packitos-0.96.0/packit/cli/create_update.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/dist_git_init.py` & `packitos-0.96.0/packit/cli/dist_git_init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/init.py` & `packitos-0.96.0/packit/cli/init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/packit_base.py` & `packitos-0.96.0/packit/cli/packit_base.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/prepare_sources.py` & `packitos-0.96.0/packit/cli/prepare_sources.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/propose_downstream.py` & `packitos-0.96.0/packit/cli/propose_downstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/push_updates.py` & `packitos-0.96.0/packit/cli/push_updates.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/source_git.py` & `packitos-0.96.0/packit/cli/source_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/source_git_init.py` & `packitos-0.96.0/packit/cli/source_git_init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/source_git_status.py` & `packitos-0.96.0/packit/cli/source_git_status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/srpm.py` & `packitos-0.96.0/packit/cli/srpm.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/status.py` & `packitos-0.96.0/packit/cli/status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/sync_from_downstream.py` & `packitos-0.96.0/packit/cli/sync_from_downstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/types.py` & `packitos-0.96.0/packit/cli/types.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/update_dist_git.py` & `packitos-0.96.0/packit/cli/update_dist_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/update_source_git.py` & `packitos-0.96.0/packit/cli/update_source_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/utils.py` & `packitos-0.96.0/packit/cli/utils.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/validate_config.py` & `packitos-0.96.0/packit/cli/validate_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/builds/copr_build.py` & `packitos-0.96.0/packit/cli/builds/copr_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/builds/in_image_builder.py` & `packitos-0.96.0/packit/cli/builds/in_image_builder.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/builds/koji_build.py` & `packitos-0.96.0/packit/cli/builds/koji_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/builds/local_build.py` & `packitos-0.96.0/packit/cli/builds/local_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/cli/builds/mock_build.py` & `packitos-0.96.0/packit/cli/builds/mock_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/config/__init__.py` & `packitos-0.96.0/packit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/config/aliases.py` & `packitos-0.96.0/packit/config/aliases.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/config/common_package_config.py` & `packitos-0.96.0/packit/config/common_package_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,14 +155,15 @@
         version_update_mask: String containing a reg exp. The old version contained in the
             specfile and the newly released version have both to match this reg exp
             otherwise Packit shall not sync the release downstream.
         parse_time_macros: Dict with macros to (un)define before parsing specfile.
             Keys are macro names and values are macro values. A value of None will undefine
             the corresponding macro.
         status_name_template: Template for configurable names for status checks.
+        sidetag_group: Sidetag group identifier for downstream Koji builds and Bodhi updates.
     """
 
     def __init__(
         self,
         config_file_path: Optional[str] = None,
         specfile_path: Optional[str] = None,
         synced_files: Optional[list[SyncFilesItem]] = None,
@@ -235,14 +236,15 @@
         upload_sources: bool = True,
         pkg_tool: Optional[str] = None,
         version_update_mask: Optional[str] = None,
         test_command: Optional[TestCommandConfig] = None,
         parse_time_macros: Optional[dict[str, str]] = None,
         require: Optional[RequirementsConfig] = None,
         status_name_template: Optional[str] = None,
+        sidetag_group: Optional[str] = None,
     ):
         self.config_file_path: Optional[str] = config_file_path
         self.specfile_path: Optional[str] = specfile_path
 
         self._files_to_sync: list[SyncFilesItem] = files_to_sync or []  # new option
         self._files_to_sync_used: bool = files_to_sync is not None
         self.synced_files: list[SyncFilesItem] = (
@@ -348,14 +350,16 @@
         self.follow_fedora_branching = follow_fedora_branching
         self.upload_sources = upload_sources
 
         self.pkg_tool = pkg_tool
 
         self.parse_time_macros = parse_time_macros or {}
 
+        self.sidetag_group = sidetag_group
+
     @property
     def dist_git_base_url(self) -> str:
         return self.dist_git_instance.url
 
     @property
     def dist_git_namespace(self) -> Optional[str]:
         return self.dist_git_instance.namespace
```

### Comparing `packitos-0.95.0/packit/config/config.py` & `packitos-0.96.0/packit/config/config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/config/job_config.py` & `packitos-0.96.0/packit/config/job_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/config/notifications.py` & `packitos-0.96.0/packit/config/notifications.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/config/package_config.py` & `packitos-0.96.0/packit/config/package_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/config/package_config_validator.py` & `packitos-0.96.0/packit/config/package_config_validator.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/config/requirements.py` & `packitos-0.96.0/packit/config/requirements.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/data/_packitpatch` & `packitos-0.96.0/packit/data/_packitpatch`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/utils/__init__.py` & `packitos-0.96.0/packit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/utils/bodhi.py` & `packitos-0.96.0/packit/utils/bodhi.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/utils/changelog_helper.py` & `packitos-0.96.0/packit/utils/changelog_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,18 @@
         resolved_bugs_str = " ".join(resolved_bugs) if resolved_bugs else ""
         env = self.package_config.get_package_names_as_env() | {
             "PACKIT_PROJECT_VERSION": version,
             "PACKIT_RESOLVED_BUGS": resolved_bugs_str,
             "PACKIT_PROJECT_UPSTREAM_TAG": upstream_tag or "",
             "PACKIT_PROJECT_PREVIOUS_VERSION": previous_version or "",
         }
-        messages = self.up.get_output_from_action(ActionName.changelog_entry, env=env)
+        messages = self.up.actions_handler.get_output_from_action(
+            ActionName.changelog_entry,
+            env=env,
+        )
         if not messages:
             return None
 
         return "\n".join(line.rstrip() for line in messages)
 
     @staticmethod
     def sanitize_entry(entry: str) -> str:
```

### Comparing `packitos-0.95.0/packit/utils/commands.py` & `packitos-0.96.0/packit/utils/commands.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/utils/decorators.py` & `packitos-0.96.0/packit/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/utils/extensions.py` & `packitos-0.96.0/packit/utils/extensions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/utils/koji_helper.py` & `packitos-0.96.0/packit/utils/koji_helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                 tag=tag,
                 inherit=True,
                 latest=True,
                 strict=True,
             )
         except Exception as e:
             logger.debug(
-                f"Failed to latest build of package {package} in tag {tag} from Koji: {e}",
+                f"Failed to get latest build of package {package} in tag {tag} from Koji: {e}",
             )
             return None
         if not builds:
             return None
         return builds[0]
 
     def get_latest_nvr_in_tag(self, package: str, tag: str) -> Optional[str]:
@@ -151,14 +151,103 @@
             logger.debug(f"Failed to get changelog of build {nvr} from Koji: {e}")
             return []
         for k, v in headers.items():
             if not isinstance(v, list):
                 headers[k] = [v]
         return list(zip(*[headers[h] for h in requested_headers]))
 
+    def get_tag_info(self, tag: str) -> Optional[dict]:
+        """
+        Gets tag information.
+
+        Args:
+            tag: Koji tag.
+
+        Returns:
+            Tag information or None if there is no such tag.
+        """
+        try:
+            info = self.session.getBuildConfig(tag)
+        except Exception as e:
+            logger.debug(f"Failed to get tag info of {tag} from Koji: {e}")
+            return None
+        return info
+
+    def create_sidetag(self, dist_git_branch: str) -> Optional[dict]:
+        """
+        Creates a new sidetag for the specified dist-git branch.
+
+        Attempts to log in if the underlying session is not authenticated.
+
+        Args:
+            dist_git_branch: dist-git branch name.
+
+        Returns:
+            New tag information or None if creation failed.
+        """
+        target_name = self.get_build_target(dist_git_branch)
+        try:
+            target = self.session.getBuildTarget(target_name)
+        except Exception as e:
+            logger.debug(f"Failed to get build target {target_name} from Koji: {e}")
+            return None
+        if not target:
+            logger.debug(f"Failed to get build target {target_name} from Koji")
+            return None
+        if not (build_tag := target.get("build_tag_name")):
+            logger.debug(f"Failed to get build tag from build target {target_name}")
+            return None
+        if not self.session.logged_in:
+            try:
+                self.session.gssapi_login()
+            except Exception as e:
+                logger.debug(f"Authentication failed: {e}")
+                return None
+        try:
+            info = self.session.createSideTag(build_tag)
+        except Exception as e:
+            logger.debug(f"Failed to create sidetag for {build_tag} in Koji: {e}")
+            return None
+        return info
+
+    def remove_sidetag(self, sidetag: str) -> None:
+        """
+        Removes the specified sidetag.
+
+        Attempts to log in if the underlying session is not authenticated.
+
+        Args:
+            sidetag: Sidetag name.
+        """
+        if not self.session.logged_in:
+            try:
+                self.session.gssapi_login()
+            except Exception as e:
+                logger.debug(f"Authentication failed: {e}")
+                return
+        try:
+            self.session.removeSideTag(sidetag)
+        except Exception as e:
+            logger.debug(f"Failed to remove sidetag {sidetag} in Koji: {e}")
+
+    @staticmethod
+    def get_build_target(dist_git_branch: str) -> str:
+        """
+        Gets a build target from a dist-git branch name.
+
+        Args:
+            dist_git_branch: dist-git branch name.
+
+        Returns:
+            Name of matching build target.
+        """
+        if dist_git_branch in ["rawhide", "main"]:
+            return "rawhide"
+        return f"{dist_git_branch}-candidate"
+
     @staticmethod
     def format_changelog(changelog: list[tuple[int, str, str]], since: int = 0) -> str:
         """
         Formats changelog entries since the specified timestamp.
 
         Args:
             changelog: Changelog as a list of entries in form of
```

### Comparing `packitos-0.95.0/packit/utils/logging.py` & `packitos-0.96.0/packit/utils/logging.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/utils/lookaside.py` & `packitos-0.96.0/packit/utils/lookaside.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/utils/monitoring.py` & `packitos-0.96.0/packit/utils/monitoring.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/utils/repo.py` & `packitos-0.96.0/packit/utils/repo.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/utils/source_script.py` & `packitos-0.96.0/packit/utils/source_script.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/utils/upstream_version.py` & `packitos-0.96.0/packit/utils/upstream_version.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/packit/utils/versions.py` & `packitos-0.96.0/packit/utils/versions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/plans/full.fmf` & `packitos-0.96.0/plans/full.fmf`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/plans/session-recording.fmf` & `packitos-0.96.0/plans/session-recording.fmf`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/conftest.py` & `packitos-0.96.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/full.fmf` & `packitos-0.96.0/tests/full.fmf`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/spellbook.py` & `packitos-0.96.0/tests/spellbook.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/cockpit-ostree/Makefile` & `packitos-0.96.0/tests/data/cockpit-ostree/Makefile`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/cockpit-ostree/cockpit-ostree.spec.dg` & `packitos-0.96.0/tests/data/cockpit-ostree/cockpit-ostree.spec.dg`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/cockpit-ostree/cockpit-ostree.spec.in` & `packitos-0.96.0/tests/data/cockpit-ostree/cockpit-ostree.spec.in`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/cronie/SOURCES/cronie-1.5.2-context-role.patch` & `packitos-0.96.0/tests/data/cronie/SOURCES/cronie-1.5.2-context-role.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/cronie/SOURCES/fix-memory-leaks.patch` & `packitos-0.96.0/tests/data/cronie/SOURCES/fix-memory-leaks.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/cronie/SOURCES/fix-unsafe-code.patch` & `packitos-0.96.0/tests/data/cronie/SOURCES/fix-unsafe-code.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/cronie/SPECS/cronie.spec` & `packitos-0.96.0/tests/data/cronie/SPECS/cronie.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/dg-ogr/.packit.yaml` & `packitos-0.96.0/tests/data/dg-ogr/.packit.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/dg-ogr/python-ogr.spec` & `packitos-0.96.0/tests/data/dg-ogr/python-ogr.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/edd/Makefile` & `packitos-0.96.0/tests/data/edd/Makefile`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/edd/edd.spec` & `packitos-0.96.0/tests/data/edd/edd.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/osbuild/osbuild.spec` & `packitos-0.96.0/tests/data/osbuild/osbuild.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/patches/previous/git-diff.patch` & `packitos-0.96.0/tests/data/patches/previous/git-diff.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/patches/previous/missing-diff-line.patch` & `packitos-0.96.0/tests/data/patches/previous/missing-diff-line.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/patches/previous/unified-diff.patch` & `packitos-0.96.0/tests/data/patches/previous/unified-diff.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/patches/previous/weird-identical.patch` & `packitos-0.96.0/tests/data/patches/previous/weird-identical.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/patches/regenerated/git-diff.patch` & `packitos-0.96.0/tests/data/patches/regenerated/git-diff.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/patches/regenerated/missing-diff-line.patch` & `packitos-0.96.0/tests/data/patches/regenerated/missing-diff-line.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/patches/regenerated/unified-diff.patch` & `packitos-0.96.0/tests/data/patches/regenerated/unified-diff.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/patches/regenerated/weird-identical.patch` & `packitos-0.96.0/tests/data/patches/regenerated/weird-identical.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/rpms/hello/0017-Patch-This..patch` & `packitos-0.96.0/tests/data/rpms/hello/0017-Patch-This..patch`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/rpms/hello/from-git.patch` & `packitos-0.96.0/tests/data/rpms/hello/from-git.patch`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/snapd/packaging/fedora/fix-spec` & `packitos-0.96.0/tests/data/snapd/packaging/fedora/fix-spec`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/snapd/packaging/fedora/pack-source` & `packitos-0.96.0/tests/data/snapd/packaging/fedora/pack-source`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/snapd/packaging/fedora/snapd.spec` & `packitos-0.96.0/tests/data/snapd/packaging/fedora/snapd.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/snapd/vendor/vendor.json` & `packitos-0.96.0/tests/data/snapd/vendor/vendor.json`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/sourcegit/source_git/.distro/beer.spec` & `packitos-0.96.0/tests/data/sourcegit/source_git/.distro/beer.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/upstream_git/beer.spec` & `packitos-0.96.0/tests/data/upstream_git/beer.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/upstream_git_macro_in_source/beer.spec` & `packitos-0.96.0/tests/data/upstream_git_macro_in_source/beer.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/data/vsftpd/Fedora/vsftpd.spec` & `packitos-0.96.0/tests/data/vsftpd/Fedora/vsftpd.spec`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/functional/spellbook.py` & `packitos-0.96.0/tests/functional/spellbook.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/functional/test_local_build.py` & `packitos-0.96.0/tests/functional/test_local_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/functional/test_prepare_sources.py` & `packitos-0.96.0/tests/functional/test_prepare_sources.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/functional/test_srpm.py` & `packitos-0.96.0/tests/functional/test_srpm.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/bodhi_latest_builds.py` & `packitos-0.96.0/tests/integration/bodhi_latest_builds.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/bodhi_status_updates.py` & `packitos-0.96.0/tests/integration/bodhi_status_updates.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/conftest.py` & `packitos-0.96.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_actions.py` & `packitos-0.96.0/tests/integration/test_actions.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     command,
     env_vars: dict,
     should_raise,
 ):
     _, upstream = upstream_instance
     upstream.package_config.actions = {action: command}
     try:
-        upstream.with_action(action, env=env_vars)
+        upstream.actions_handler.with_action(action, env=env_vars)
     except PackitException as ex:
         if should_raise:
             assert "Command " in str(ex)
             assert command.split(" ")[0] in str(ex)
         else:
             raise
 
@@ -52,15 +52,15 @@
     env_vars: dict,
     should_raise,
     expected_output: str,
 ):
     _, upstream = upstream_instance
     upstream.package_config.actions = {action: command}
     try:
-        out = upstream.get_output_from_action(action, env=env_vars)
+        out = upstream.actions_handler.get_output_from_action(action, env=env_vars)
     except PackitException as ex:
         if should_raise:
             assert "Command " in str(ex)
             assert command.split(" ")[0] in str(ex)
             return
         raise
     if expected_output:
```

### Comparing `packitos-0.95.0/tests/integration/test_api.py` & `packitos-0.96.0/tests/integration/test_api.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_base_git.py` & `packitos-0.96.0/tests/integration/test_base_git.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,17 @@
                 },
             ),
         ),
     )
 
     packit_repository_base.local_project = flexmock(working_dir=".")
 
-    result = packit_repository_base.get_output_from_action(ActionName.pre_sync)
+    result = packit_repository_base.actions_handler.get_output_from_action(
+        ActionName.pre_sync,
+    )
     assert result == expected_output
 
 
 @pytest.mark.skipif(
     not can_a_module_be_imported("sandcastle"),
     reason="sandcastle is not installed",
 )
@@ -64,15 +66,17 @@
     packit_repository_base.local_project = LocalProjectBuilder().build(
         working_dir="/tmp",
     )
 
     flexmock(Sandcastle).should_receive("run")
     flexmock(Sandcastle).should_receive("exec").and_return(echo_cmd)
     flexmock(Sandcastle).should_receive("delete_pod").and_return(None)
-    result = packit_repository_base.get_output_from_action(ActionName.pre_sync)
+    result = packit_repository_base.actions_handler.get_output_from_action(
+        ActionName.pre_sync,
+    )
     assert result[-1] == echo_cmd
 
 
 @pytest.mark.skip(
     reason="Skipping since we don't have an OpenShift cluster by default.",
 )
 def test_run_in_sandbox():
@@ -84,15 +88,17 @@
                     actions={ActionName.pre_sync: "ls -lha"},
                 ),
             },
         ),
     )
     packit_repository_base.config.actions_handler = "sandcastle"
 
-    result = packit_repository_base.get_output_from_action(ActionName.pre_sync)
+    result = packit_repository_base.actions_handler.get_output_from_action(
+        ActionName.pre_sync,
+    )
     assert "total 4.0K" in result
     assert "drwxr-xr-x. 1 root root" in result
 
 
 def test_base_push_bad(distgit_and_remote):
     distgit, _ = distgit_and_remote
```

### Comparing `packitos-0.95.0/tests/integration/test_build.py` & `packitos-0.96.0/tests/integration/test_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_changelog_helper.py` & `packitos-0.96.0/tests/integration/test_changelog_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,18 +199,22 @@
         "PACKIT_UPSTREAM_PACKAGE_NAME": "beerware",
         "PACKIT_DOWNSTREAM_PACKAGE_NAME": "beer",
         "PACKIT_PROJECT_VERSION": "0.1.0",
         "PACKIT_RESOLVED_BUGS": "rhbz#123 rhbz#124",
         "PACKIT_PROJECT_UPSTREAM_TAG": "0.1.0",
         "PACKIT_PROJECT_PREVIOUS_VERSION": "0.0.0",
     }
-    flexmock(upstream).should_receive("get_output_from_action").with_args(
+    flexmock(upstream.actions_handler).should_receive(
+        "get_output_from_action",
+    ).with_args(
         ActionName.changelog_entry,
         env=expected_env,
-    ).and_return("- entry").once()
+    ).and_return(
+        "- entry",
+    ).once()
 
     ChangelogHelper(upstream, downstream, package_config).update_dist_git(
         upstream_tag="0.1.0",
         full_version="0.1.0",
         resolved_bugs=["rhbz#123", "rhbz#124"],
     )
```

### Comparing `packitos-0.95.0/tests/integration/test_copr_build.py` & `packitos-0.96.0/tests/integration/test_copr_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_create_update.py` & `packitos-0.96.0/tests/integration/test_create_update.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_get_api.py` & `packitos-0.96.0/tests/integration/test_get_api.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_init.py` & `packitos-0.96.0/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_local_project.py` & `packitos-0.96.0/tests/integration/test_local_project.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_pagure.py` & `packitos-0.96.0/tests/integration/test_pagure.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_patches.py` & `packitos-0.96.0/tests/integration/test_patches.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_push_updates.py` & `packitos-0.96.0/tests/integration/test_push_updates.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_security.py` & `packitos-0.96.0/tests/integration/test_security.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_source_git.py` & `packitos-0.96.0/tests/integration/test_source_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_source_git_init.py` & `packitos-0.96.0/tests/integration/test_source_git_init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_source_git_status.py` & `packitos-0.96.0/tests/integration/test_source_git_status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_source_git_synch_push.py` & `packitos-0.96.0/tests/integration/test_source_git_synch_push.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_source_git_update_source_git.py` & `packitos-0.96.0/tests/integration/test_source_git_update_source_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_spec.py` & `packitos-0.96.0/tests/integration/test_spec.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_update.py` & `packitos-0.96.0/tests/integration/test_update.py`

 * *Files 7% similar despite different names*

```diff
@@ -242,14 +242,59 @@
     # assert that we have changelog entries for both versions
     with spec.sections() as sections:
         changelog = "\n".join(sections.changelog)
     assert "0.0.0" in changelog
     assert "0.1.0" in changelog
 
 
+def test_basic_local_update_with_adding_second_local_source(
+    cwd_upstream,
+    api_instance,
+    mock_remote_functionality_upstream,
+):
+    """basic propose-downstream test: mock remote API, use local upstream and dist-git"""
+    u, d, api = api_instance
+    mock_spec_download_remote_s(d, files_to_create=["the_source.tar.gz"])
+    flexmock(api).should_receive("init_kerberos_ticket").at_least().once()
+    with Specfile(u / "beer.spec", autosave=True).sources() as sources:
+        sources.append("the_source.tar.gz")
+    subprocess.check_call(["git", "add", "beer.spec"], cwd=u)
+    subprocess.check_call(
+        ["git", "commit", "-m", "Added new source to specfile"],
+        cwd=u,
+    )
+    subprocess.check_call(["git", "tag", "0.1.0", "-f"], cwd=u)
+
+    dist_git_first_source = d / TARBALL_NAME
+    dist_git_second_source = d / "the_source.tar.gz"
+    flexmock(api.dg).should_call("upload_to_lookaside_cache").with_args(
+        archives=[dist_git_first_source, dist_git_second_source],
+        pkg_tool="",
+        offline=False,
+    )
+
+    api.sync_release(dist_git_branch="main", version="0.1.0")
+
+    assert dist_git_first_source.is_file()
+    assert dist_git_second_source.is_file()
+    spec = Specfile(d / "beer.spec")
+    assert spec.expanded_version == "0.1.0"
+    with spec.sources() as sources:
+        newly_added_source = sources[1]
+        assert newly_added_source.expanded_location == "the_source.tar.gz"
+        assert newly_added_source.filename == "the_source.tar.gz"
+    assert spec.sources()
+    assert (d / "README.packit").is_file()
+    # assert that we have changelog entries for both versions
+    with spec.sections() as sections:
+        changelog = "\n".join(sections.changelog)
+    assert "0.0.0" in changelog
+    assert "0.1.0" in changelog
+
+
 def test_basic_local_update_with_removing_second_source(
     cwd_upstream,
     api_instance,
     mock_remote_functionality_upstream,
 ):
     """basic propose-downstream test: mock remote API, use local upstream and dist-git"""
     u, d, api = api_instance
```

### Comparing `packitos-0.95.0/tests/integration/test_upstream.py` & `packitos-0.96.0/tests/integration/test_upstream.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,15 +325,15 @@
     )
 
     flexmock(upstream.local_project).should_receive("commit_hexsha").and_return("4321")
     flexmock(upstream).should_receive("get_spec_release").with_args(
         release_suffix="",
     ).and_return("1.1234.main.0.1221")
 
-    flexmock(upstream).should_receive("with_action").with_args(
+    flexmock(upstream.actions_handler).should_receive("with_action").with_args(
         action=ActionName.fix_spec,
         env={
             "PACKIT_PROJECT_VERSION": "0.1.0",
             "PACKIT_RPMSPEC_RELEASE": "1.1234.main.0.1221",
             "PACKIT_PROJECT_COMMIT": "4321",
             "PACKIT_PROJECT_ARCHIVE": "archive.tar.gz",
             "PACKIT_PROJECT_BRANCH": "main",
```

### Comparing `packitos-0.95.0/tests/integration/test_using_cockpit.py` & `packitos-0.96.0/tests/integration/test_using_cockpit.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_using_examples.py` & `packitos-0.96.0/tests/integration/test_using_examples.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_validate_config.py` & `packitos-0.96.0/tests/integration/test_validate_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/integration/test_validate_synced_files.py` & `packitos-0.96.0/tests/integration/test_validate_synced_files.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/conftest.py` & `packitos-0.96.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/test_actions.py` & `packitos-0.96.0/tests/unit/test_actions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/test_api.py` & `packitos-0.96.0/tests/unit/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,21 +198,21 @@
     )
     api_mock.up.package_config.should_receive("get_package_names_as_env").and_return({})
     api_mock.should_receive("push_and_create_pr").and_return(flexmock())
     api_mock.sync_release(version="1.1", dist_git_branch="_")
 
 
 def test_sync_release_env(api_mock):
-    env = api_mock.sync_release_env
+    env = api_mock.sync_release_env()
     assert env == {
         "PACKIT_DOWNSTREAM_REPO": "/mock_dir/sandcastle/dist-git",
         "PACKIT_UPSTREAM_REPO": "/mock_dir/sandcastle/local-project",
     }
     api_mock.config.command_handler = RunCommandType.sandcastle
-    env = api_mock.sync_release_env
+    env = api_mock.sync_release_env()
     assert env == {
         "PACKIT_DOWNSTREAM_REPO": "/mock_dir/sandcastle/sandcastle-exec-dir/dist-git",
         "PACKIT_UPSTREAM_REPO": "/mock_dir/sandcastle/sandcastle-exec-dir/local-project",
     }
 
 
 @pytest.mark.parametrize(
```

### Comparing `packitos-0.95.0/tests/unit/test_base_git.py` & `packitos-0.96.0/tests/unit/test_base_git.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,27 +65,29 @@
             git_service=flexmock(),
         ),
     )
 
 
 @pytest.fixture()
 def packit_repository_base():
-    return PackitRepositoryBase(
+    repo_base = PackitRepositoryBase(
         config=Config(),
         package_config=PackageConfig(
             packages={
                 "package": CommonPackageConfig(
                     actions={
                         ActionName.pre_sync: "command --a",
                         ActionName.get_current_version: "command --b",
                     },
                 ),
             },
         ),
     )
+    repo_base.local_project = flexmock()
+    return repo_base
 
 
 @pytest.fixture()
 def packit_repository_base_more_actions():
     return PackitRepositoryBase(
         config=Config(),
         package_config=PackageConfig(
@@ -119,59 +121,67 @@
         ),
     )
     b.local_project = LocalProjectBuilder().build(working_dir=Path("/sandcastle"))
     return b
 
 
 def test_has_action_upstream(upstream_with_actions):
-    assert upstream_with_actions.has_action(ActionName.pre_sync)
-    assert not upstream_with_actions.has_action(ActionName.create_patches)
+    assert upstream_with_actions.actions_handler.has_action(ActionName.pre_sync)
+    assert not upstream_with_actions.actions_handler.has_action(
+        ActionName.create_patches,
+    )
 
 
 def test_has_action_distgit(distgit_with_actions):
-    assert distgit_with_actions.has_action(ActionName.pre_sync)
-    assert not distgit_with_actions.has_action(ActionName.create_patches)
+    assert distgit_with_actions.actions_handler.has_action(ActionName.pre_sync)
+    assert not distgit_with_actions.actions_handler.has_action(
+        ActionName.create_patches,
+    )
 
 
 def test_with_action_non_defined(packit_repository_base):
-    if packit_repository_base.with_action(action=ActionName.create_patches):
+    if packit_repository_base.actions_handler.with_action(
+        action=ActionName.create_patches,
+    ):
         # this is the style we are using that function
         return
 
     raise AssertionError()
 
 
 def test_with_action_defined(packit_repository_base):
     flexmock(commands).should_receive("run_command").once()
 
     packit_repository_base.local_project = flexmock(working_dir="my/working/dir")
 
-    if packit_repository_base.with_action(action=ActionName.pre_sync):
+    if packit_repository_base.actions_handler.with_action(action=ActionName.pre_sync):
         # this is the style we are using that function
         raise AssertionError()
 
 
 def test_with_action_working_dir(packit_repository_base):
     flexmock(LocalCommandHandler).should_receive("run_command").with_args(
         command=["command", "--a"],
         env=None,
         print_live=True,
     ).and_return("command --a").once()
 
     packit_repository_base.local_project = flexmock(working_dir="my/working/dir")
 
-    assert not packit_repository_base.with_action(action=ActionName.pre_sync)
+    assert not packit_repository_base.actions_handler.with_action(
+        action=ActionName.pre_sync,
+    )
 
 
 def test_run_action_hook_not_defined(packit_repository_base):
     flexmock(commands).should_receive("run_command").times(0)
 
     packit_repository_base.local_project = flexmock(working_dir="my/working/dir")
 
-    packit_repository_base.run_action(actions=ActionName.create_patches)
+    packit_repository_base.actions_handler.run_action(actions=ActionName.create_patches)
 
 
 def test_run_action_not_defined(packit_repository_base):
     flexmock(LocalCommandHandler).should_receive("run_command").times(0)
 
     packit_repository_base.local_project = flexmock(working_dir="my/working/dir")
 
@@ -179,15 +189,15 @@
         flexmock()
         .should_receive("action_function")
         .with_args("arg", kwarg="kwarg")
         .once()
         .mock()
         .action_function
     )
-    packit_repository_base.run_action(
+    packit_repository_base.actions_handler.run_action(
         ActionName.create_patches,
         action_method,
         {},
         "arg",
         kwarg="kwarg",
     )
 
@@ -206,15 +216,15 @@
         .should_receive("action_function")
         .with_args("arg", kwarg="kwarg")
         .times(0)
         .mock()
         .action_function
     )
 
-    packit_repository_base.run_action(
+    packit_repository_base.actions_handler.run_action(
         ActionName.pre_sync,
         action_method,
         {},
         "arg",
         "kwarg",
     )
 
@@ -247,21 +257,21 @@
                 "TEMP_DIR=$(mktemp --tmpdir -d anaconda-localization-XXXXXXXXXX)\n"
             )
         raise Exception("This command was not expected")
 
     flexmock(Sandcastle, exec=mocked_exec)
     flexmock(Sandcastle).should_receive("delete_pod").once().and_return(None)
     with caplog.at_level(logging.INFO, logger="packit"):
-        packit_repository_base_with_sandcastle_object.run_action(
+        packit_repository_base_with_sandcastle_object.actions_handler.run_action(
             ActionName.pre_sync,
             None,
             "arg1",
             "kwarg1",
         )
-        packit_repository_base_with_sandcastle_object.run_action(
+        packit_repository_base_with_sandcastle_object.actions_handler.run_action(
             ActionName.get_current_version,
             None,
             "arg2",
             "kwarg2",
         )
         # this is being called in PackitAPI.clean
         packit_repository_base_with_sandcastle_object.command_handler.clean()
@@ -302,28 +312,30 @@
         flexmock()
         .should_receive("action_function")
         .with_args("arg", kwarg="kwarg")
         .times(0)
         .mock()
         .action_function
     )
-    packit_repository_base_more_actions.run_action(
+    packit_repository_base_more_actions.actions_handler.run_action(
         ActionName.pre_sync,
         action_method,
         "arg",
         kwarg="kwarg",
     )
 
 
 def test_get_output_from_action_not_defined(packit_repository_base):
     flexmock(LocalCommandHandler).should_receive("run_command").times(0)
 
     packit_repository_base.local_project = flexmock(working_dir="my/working/dir")
 
-    result = packit_repository_base.get_output_from_action(ActionName.create_patches)
+    result = packit_repository_base.actions_handler.get_output_from_action(
+        ActionName.create_patches,
+    )
     assert result is None
 
 
 @pytest.mark.parametrize(
     "source, package_config, expected_urls, extra_source",
     [
         pytest.param(
```

### Comparing `packitos-0.95.0/tests/unit/test_cli.py` & `packitos-0.96.0/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/test_cli_utils.py` & `packitos-0.96.0/tests/unit/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/test_copr_helper.py` & `packitos-0.96.0/tests/unit/test_copr_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/test_dg.py` & `packitos-0.96.0/tests/unit/test_dg.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/test_dist_git_init.py` & `packitos-0.96.0/tests/unit/test_dist_git_init.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/test_image_builder.py` & `packitos-0.96.0/tests/unit/test_image_builder.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/test_iterate_packages.py` & `packitos-0.96.0/tests/unit/test_iterate_packages.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/test_koji_build.py` & `packitos-0.96.0/tests/unit/test_koji_build.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/test_load_authentication.py` & `packitos-0.96.0/tests/unit/test_load_authentication.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/test_local_project.py` & `packitos-0.96.0/tests/unit/test_local_project.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/test_login_with_kerberos.py` & `packitos-0.96.0/tests/unit/test_login_with_kerberos.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/test_patches.py` & `packitos-0.96.0/tests/unit/test_patches.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/test_prepare_sources.py` & `packitos-0.96.0/tests/unit/test_prepare_sources.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/test_propose_downstream.py` & `packitos-0.96.0/tests/unit/test_propose_downstream.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/test_security.py` & `packitos-0.96.0/tests/unit/test_security.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/test_specfile.py` & `packitos-0.96.0/tests/unit/test_specfile.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/test_status.py` & `packitos-0.96.0/tests/unit/test_status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/test_sync.py` & `packitos-0.96.0/tests/unit/test_sync.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/test_upstream.py` & `packitos-0.96.0/tests/unit/test_upstream.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from contextlib import suppress as does_not_raise
 
 import pytest
 from flexmock import flexmock
 
 import packit
 from packit.actions import ActionName
+from packit.actions_handler import ActionsHandler
 from packit.exceptions import PackitException
 from packit.upstream import Archive, SRPMBuilder, Upstream
 
 
 @pytest.fixture
 def upstream_pr_mock():
     return flexmock(url="test_pr_url")
@@ -93,15 +94,19 @@
         package_config=flexmock(
             actions={ActionName.create_archive: action_config},
             synced_files=flexmock(),
         ),
         config=flexmock(),
         local_project=flexmock(),
     )
-    assert ups.get_commands_for_actions(action=ActionName.create_archive) == result
+    ups._command_handler = flexmock()
+    assert (
+        ups.actions_handler.get_commands_for_actions(action=ActionName.create_archive)
+        == result
+    )
 
 
 @pytest.mark.parametrize(
     "action_output, version, expected_result",
     [
         pytest.param(
             ("some_action_output", "1.0.1"),
@@ -111,15 +116,17 @@
         ),
         pytest.param(None, "1.0.2", "1.0.2", id="tag_valid_version"),
         pytest.param(None, "1.0-3", "1.0.3", id="tag_version_with_dash"),
     ],
 )
 def test_get_current_version(action_output, version, expected_result, upstream_mock):
     flexmock(packit.upstream.os).should_receive("listdir").and_return("mocked")
-    upstream_mock.should_receive("get_output_from_action").and_return(action_output)
+    flexmock(ActionsHandler).should_receive("get_output_from_action").and_return(
+        action_output,
+    )
     upstream_mock.should_receive("get_last_tag").and_return("_mocked")
     upstream_mock.should_receive("get_version_from_tag").and_return(version)
     upstream_mock.package_config.should_receive("get_package_names_as_env").and_return(
         {},
     )
     assert upstream_mock.get_current_version() == expected_result
```

### Comparing `packitos-0.95.0/tests/unit/test_utils.py` & `packitos-0.96.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/config/test_config.py` & `packitos-0.96.0/tests/unit/config/test_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/config/test_config_aliases.py` & `packitos-0.96.0/tests/unit/config/test_config_aliases.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/config/test_package_config.py` & `packitos-0.96.0/tests/unit/config/test_package_config.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/utils/test_changelog_helper.py` & `packitos-0.96.0/tests/unit/utils/test_changelog_helper.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/utils/test_decorators.py` & `packitos-0.96.0/tests/unit/utils/test_decorators.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/utils/test_dist_git_instance.py` & `packitos-0.96.0/tests/unit/utils/test_dist_git_instance.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/utils/test_lookaside.py` & `packitos-0.96.0/tests/unit/utils/test_lookaside.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/utils/test_repo.py` & `packitos-0.96.0/tests/unit/utils/test_repo.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/utils/test_source_script.py` & `packitos-0.96.0/tests/unit/utils/test_source_script.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/utils/test_upstream_version.py` & `packitos-0.96.0/tests/unit/utils/test_upstream_version.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests/unit/utils/test_versions.py` & `packitos-0.96.0/tests/unit/utils/test_versions.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/README.md` & `packitos-0.96.0/tests_recording/README.md`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_api.py` & `packitos-0.96.0/tests_recording/test_api.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_base_git.py` & `packitos-0.96.0/tests_recording/test_base_git.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_image_builder.py` & `packitos-0.96.0/tests_recording/test_image_builder.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_local_project.py` & `packitos-0.96.0/tests_recording/test_local_project.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_repository_cache.py` & `packitos-0.96.0/tests_recording/test_repository_cache.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_status.py` & `packitos-0.96.0/tests_recording/test_status.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/testbase.py` & `packitos-0.96.0/tests_recording/testbase.py`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml` & `packitos-0.96.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.packit-dist-git2k0adr0g_1.tar.xz` & `packitos-0.96.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.packit-dist-git2k0adr0g_1.tar.xz`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.tmpg_51_3z9_1.tar.xz` & `packitos-0.96.0/tests_recording/test_data/test_api/ProposeUpdate.test_changelog_sync.yaml.tmpg_51_3z9_1.tar.xz`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml` & `packitos-0.96.0/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz` & `packitos-0.96.0/tests_recording/test_data/test_api/ProposeUpdate.test_comment_in_spec.yaml.tmplxw77ha6_1.tar.xz`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml` & `packitos-0.96.0/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz` & `packitos-0.96.0/tests_recording/test_data/test_api/ProposeUpdate.test_version_change_exception.yaml.packit-dist-git_44ibzyh_1.tar.xz`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_base_git/ProposeUpdate.test_download_remote_sources_via_spec.yaml` & `packitos-0.96.0/tests_recording/test_data/test_base_git/ProposeUpdate.test_download_remote_sources_via_spec.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_bad_request.yaml` & `packitos-0.96.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_bad_request.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_get_token.yaml` & `packitos-0.96.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_get_token.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_token_auto_refresh.yaml` & `packitos-0.96.0/tests_recording/test_data/test_image_builder/TestLocalProject.test_token_auto_refresh.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr.yaml` & `packitos-0.96.0/tests_recording/test_data/test_local_project/TestLocalProject.test_checkout_pr.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml` & `packitos-0.96.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_accept_str.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml` & `packitos-0.96.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_add_new_and_use_it.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml` & `packitos-0.96.0/tests_recording/test_data/test_repository_cache/RepositoryCacheTest.test_repository_cache_do_not_add_new_if_not_enabled.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml` & `packitos-0.96.0/tests_recording/test_data/test_status/TestStatus.test_copr_builds.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml` & `packitos-0.96.0/tests_recording/test_data/test_status/TestStatus.test_distgen_versions.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml` & `packitos-0.96.0/tests_recording/test_data/test_status/TestStatus.test_dowstream_pr.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml` & `packitos-0.96.0/tests_recording/test_data/test_status/TestStatus.test_koji_builds.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_status.yaml` & `packitos-0.96.0/tests_recording/test_data/test_status/TestStatus.test_status.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml` & `packitos-0.96.0/tests_recording/test_data/test_status/TestStatus.test_up_releases.yaml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/LICENSE` & `packitos-0.96.0/LICENSE`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/README.md` & `packitos-0.96.0/README.md`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/pyproject.toml` & `packitos-0.96.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `packitos-0.95.0/PKG-INFO` & `packitos-0.96.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: packitos
-Version: 0.95.0
+Version: 0.96.0
 Summary: A set of tools to integrate upstream open source projects into Fedora operating system.
 Project-URL: Homepage, https://github.com/packit/packit
 Author-email: Red Hat <user-cont-team@redhat.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: dist-git,fedora,git,packaging,rpm
 Classifier: Development Status :: 4 - Beta
```

