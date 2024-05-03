# Comparing `tmp/sbcli_dev-2.5.1.zip` & `tmp/sbcli_dev-2.5.2.zip`

## zipinfo {}

```diff
@@ -1,148 +1,148 @@
-Zip file size: 213790 bytes, number of entries: 146
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 11:13 sbcli_dev-2.5.1/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 11:13 sbcli_dev-2.5.1/sbcli_dev.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/
--rw-r--r--  2.0 unx     2269 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/setup.py
--rw-r--r--  2.0 unx     1068 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/README.md
--rw-r--r--  2.0 unx      148 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/env_var
--rw-r--r--  2.0 unx       84 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/pyproject.toml
--rw-r--r--  2.0 unx       38 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/setup.cfg
--rw-r--r--  2.0 unx     1489 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/PKG-INFO
--rw-r--r--  2.0 unx    78197 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx      357 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_cli/main.py
--rw-r--r--  2.0 unx        1 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/sbcli_dev.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     5191 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/sbcli_dev.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       49 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/sbcli_dev.egg-info/top_level.txt
--rw-r--r--  2.0 unx     1489 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/sbcli_dev.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       73 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/sbcli_dev.egg-info/requires.txt
--rw-r--r--  2.0 unx       55 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/sbcli_dev.egg-info/entry_points.txt
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/controllers/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/models/
--rw-r--r--  2.0 unx    66195 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx     1472 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/constants.py
--rw-r--r--  2.0 unx     3153 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     3444 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx      279 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx      938 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx     3193 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/snode_client.py
--rw-r--r--  2.0 unx     8189 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     7640 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/utils.py
--rw-r--r--  2.0 unx    24165 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx     5112 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx    21493 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     7504 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx     2189 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx     3203 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx     5462 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx      229 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx     5268 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx      173 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     2410 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx     5140 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx     7439 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     2423 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     4118 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx      837 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     3003 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2671 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx     6577 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/services/storage_node_monitor.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/alerting/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/dashboards/
--rw-r--r--  2.0 unx      930 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx      152 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/set_db_config.sh
--rw-r--r--  2.0 unx     1163 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx     4977 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx       54 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/db_config_single.sh
--rw-r--r--  2.0 unx     5305 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx     4470 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
--rw-r--r--  2.0 unx      453 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx     1782 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx      311 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx      118 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx      360 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/datasource.yml
--rw-r--r--  2.0 unx       43 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx     1420 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx      311 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/prometheus.yml
--rwxr-xr-x  2.0 unx      657 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/apply_dashboard.sh
--rw-r--r--  2.0 unx    25433 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/alerting/alert_rules.yaml
--rw-r--r--  2.0 unx     1889 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/alerting/alert_resources.yaml.j2
--rw-r--r--  2.0 unx   106705 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/dashboards/devices.json
--rw-r--r--  2.0 unx   799409 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/dashboards/node-exporter.json
--rw-r--r--  2.0 unx    99758 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/dashboards/nodes.json
--rw-r--r--  2.0 unx    99707 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/dashboards/lvols.json
--rw-r--r--  2.0 unx    99862 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/dashboards/cluster.json
--rw-r--r--  2.0 unx    99707 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/scripts/dashboards/pools.json
--rw-r--r--  2.0 unx    13877 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx     1120 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx     3191 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx     1521 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx     1630 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx    10557 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1568 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx    10375 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/controllers/pool_controller.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx     1900 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx    22847 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx     1122 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx    47339 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx    11294 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx      695 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx     1500 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx      806 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     4846 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx     2579 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx      917 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx      736 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx     1602 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx     1228 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx     1020 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/models/port_stat.py
--rw-r--r--  2.0 unx     3696 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     4242 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     2565 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx     3766 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     2094 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_core/models/nvme_device.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/templates/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/blueprints/
--rw-r--r--  2.0 unx      725 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx     5098 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx      703 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx     1263 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/app.py
--rw-r--r--  2.0 unx     1638 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx      717 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx     2513 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx      507 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx      322 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/static/tst.py
--rw-r--r--  2.0 unx      434 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx      827 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx     1302 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      463 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx      417 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx     2876 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/templates/deploy_spdk.yaml.j2
--rw-r--r--  2.0 unx     5547 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx     4795 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx     5317 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx     9573 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx     8547 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx    11244 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx    12198 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx      975 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     6326 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx     7846 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     2940 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     5274 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     3103 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx     6206 b- defN 24-May-03 11:13 sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_pool.py
-146 files, 1926597 bytes uncompressed, 187206 bytes compressed:  90.3%
+Zip file size: 213410 bytes, number of entries: 146
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 12:39 sbcli_dev-2.5.2/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 12:39 sbcli_dev-2.5.2/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 12:39 sbcli_dev-2.5.2/sbcli_dev.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 12:39 sbcli_dev-2.5.2/simplyblock_core/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 12:39 sbcli_dev-2.5.2/simplyblock_web/
+-rw-r--r--  2.0 unx     2269 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/setup.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/README.md
+-rw-r--r--  2.0 unx      148 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/env_var
+-rw-r--r--  2.0 unx       84 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/pyproject.toml
+-rw-r--r--  2.0 unx       38 b- defN 24-May-03 12:39 sbcli_dev-2.5.2/setup.cfg
+-rw-r--r--  2.0 unx     1489 b- defN 24-May-03 12:39 sbcli_dev-2.5.2/PKG-INFO
+-rw-r--r--  2.0 unx    77735 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx      357 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_cli/main.py
+-rw-r--r--  2.0 unx        1 b- defN 24-May-03 12:39 sbcli_dev-2.5.2/sbcli_dev.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     5188 b- defN 24-May-03 12:39 sbcli_dev-2.5.2/sbcli_dev.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       49 b- defN 24-May-03 12:39 sbcli_dev-2.5.2/sbcli_dev.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     1489 b- defN 24-May-03 12:39 sbcli_dev-2.5.2/sbcli_dev.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       73 b- defN 24-May-03 12:39 sbcli_dev-2.5.2/sbcli_dev.egg-info/requires.txt
+-rw-r--r--  2.0 unx       55 b- defN 24-May-03 12:39 sbcli_dev-2.5.2/sbcli_dev.egg-info/entry_points.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 12:39 sbcli_dev-2.5.2/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 12:39 sbcli_dev-2.5.2/simplyblock_core/scripts/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 12:39 sbcli_dev-2.5.2/simplyblock_core/controllers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 12:39 sbcli_dev-2.5.2/simplyblock_core/models/
+-rw-r--r--  2.0 unx    66179 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx     1518 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx     3153 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx      279 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx      938 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/snode_client.py
+-rw-r--r--  2.0 unx     8189 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     7640 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx    23423 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx    21493 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     7479 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx     5462 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx      229 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx     5268 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx      173 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     2410 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx     5140 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx     7439 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     2423 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     4118 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx      837 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     3003 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx     6577 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/services/storage_node_monitor.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 12:39 sbcli_dev-2.5.2/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 12:39 sbcli_dev-2.5.2/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx      930 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx      152 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/set_db_config.sh
+-rw-r--r--  2.0 unx     1163 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx     5333 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx       54 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/db_config_single.sh
+-rw-r--r--  2.0 unx     5305 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx     4470 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+-rw-r--r--  2.0 unx      453 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx     1782 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx      311 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx      118 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx      360 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx       43 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx     1420 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx      311 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/prometheus.yml
+-rwxr-xr-x  2.0 unx      657 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx    25433 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx     1856 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx   106705 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx   799409 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/dashboards/node-exporter.json
+-rw-r--r--  2.0 unx    99758 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx    99862 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/scripts/dashboards/pools.json
+-rw-r--r--  2.0 unx    13877 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx     3191 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx     1630 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx    10557 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx    10375 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/controllers/pool_controller.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx    22847 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx    47339 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx    11294 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx      695 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx      806 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx      917 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx      736 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/models/port_stat.py
+-rw-r--r--  2.0 unx     3696 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     2071 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_core/models/nvme_device.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 12:39 sbcli_dev-2.5.2/simplyblock_web/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 12:39 sbcli_dev-2.5.2/simplyblock_web/templates/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-03 12:39 sbcli_dev-2.5.2/simplyblock_web/blueprints/
+-rw-r--r--  2.0 unx      725 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx     5098 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx      703 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx     1263 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/app.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx      717 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx     2513 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx      507 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx      322 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/static/tst.py
+-rw-r--r--  2.0 unx      434 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx      827 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx     1302 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      463 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx      417 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx     2876 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/templates/deploy_spdk.yaml.j2
+-rw-r--r--  2.0 unx     5547 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx     4795 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx     5317 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx     9573 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx     8547 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx    12198 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx      975 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     6326 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx     7846 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     5274 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx     6206 b- defN 24-May-03 12:38 sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_pool.py
+146 files, 1925695 bytes uncompressed, 186832 bytes compressed:  90.3%
```

## zipnote {}

```diff
@@ -1,439 +1,439 @@
-Filename: sbcli_dev-2.5.1/
+Filename: sbcli_dev-2.5.2/
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_cli/
+Filename: sbcli_dev-2.5.2/simplyblock_cli/
 Comment: 
 
-Filename: sbcli_dev-2.5.1/sbcli_dev.egg-info/
+Filename: sbcli_dev-2.5.2/sbcli_dev.egg-info/
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/
+Filename: sbcli_dev-2.5.2/simplyblock_core/
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/
+Filename: sbcli_dev-2.5.2/simplyblock_web/
 Comment: 
 
-Filename: sbcli_dev-2.5.1/setup.py
+Filename: sbcli_dev-2.5.2/setup.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/README.md
+Filename: sbcli_dev-2.5.2/README.md
 Comment: 
 
-Filename: sbcli_dev-2.5.1/env_var
+Filename: sbcli_dev-2.5.2/env_var
 Comment: 
 
-Filename: sbcli_dev-2.5.1/pyproject.toml
+Filename: sbcli_dev-2.5.2/pyproject.toml
 Comment: 
 
-Filename: sbcli_dev-2.5.1/setup.cfg
+Filename: sbcli_dev-2.5.2/setup.cfg
 Comment: 
 
-Filename: sbcli_dev-2.5.1/PKG-INFO
+Filename: sbcli_dev-2.5.2/PKG-INFO
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_cli/cli.py
+Filename: sbcli_dev-2.5.2/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_cli/main.py
+Filename: sbcli_dev-2.5.2/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/sbcli_dev.egg-info/dependency_links.txt
+Filename: sbcli_dev-2.5.2/sbcli_dev.egg-info/dependency_links.txt
 Comment: 
 
-Filename: sbcli_dev-2.5.1/sbcli_dev.egg-info/SOURCES.txt
+Filename: sbcli_dev-2.5.2/sbcli_dev.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli_dev-2.5.1/sbcli_dev.egg-info/top_level.txt
+Filename: sbcli_dev-2.5.2/sbcli_dev.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli_dev-2.5.1/sbcli_dev.egg-info/PKG-INFO
+Filename: sbcli_dev-2.5.2/sbcli_dev.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli_dev-2.5.1/sbcli_dev.egg-info/requires.txt
+Filename: sbcli_dev-2.5.2/sbcli_dev.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli_dev-2.5.1/sbcli_dev.egg-info/entry_points.txt
+Filename: sbcli_dev-2.5.2/sbcli_dev.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/services/
+Filename: sbcli_dev-2.5.2/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/controllers/
+Filename: sbcli_dev-2.5.2/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/models/
+Filename: sbcli_dev-2.5.2/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/storage_node_ops.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/constants.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/cnode_client.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/shell_utils.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/pci_utils.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/__init__.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/snode_client.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/kv_store.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/utils.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/cluster_ops.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/compute_node_ops.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/rpc_client.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/distr_controller.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/services/health_check_service.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/services/service_template.service
+Filename: sbcli_dev-2.5.2/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/services/remove_service.sh
+Filename: sbcli_dev-2.5.2/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/services/log_agg_service.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/services/device_monitor.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/services/__init__.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/services/install_service.sh
+Filename: sbcli_dev-2.5.2/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/services/cap_monitor.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/alerting/
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/dashboards/
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/__init__.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/datasource.yml
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/prometheus.yml
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/apply_dashboard.sh
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/alerting/alert_rules.yaml
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/alerting/alert_resources.yaml.j2
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/dashboards/devices.json
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/dashboards/node-exporter.json
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/dashboards/node-exporter.json
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/dashboards/nodes.json
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/dashboards/lvols.json
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/dashboards/cluster.json
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/scripts/dashboards/pools.json
+Filename: sbcli_dev-2.5.2/simplyblock_core/scripts/dashboards/pools.json
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/controllers/device_controller.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/controllers/events_controller.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/controllers/storage_events.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/controllers/device_events.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/controllers/__init__.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/controllers/health_controller.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/controllers/pool_events.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/models/events.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/models/iface.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/models/base_model.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/models/lvol_model.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/models/lvol_model.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/models/compute_node.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/models/snapshot.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/models/pool.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/models/global_settings.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/models/port_stat.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/models/storage_node.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/models/__init__.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/models/stats.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/models/cluster.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/models/mgmt_node.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/models/caching_node.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_core/models/nvme_device.py
+Filename: sbcli_dev-2.5.2/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/static/
+Filename: sbcli_dev-2.5.2/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/templates/
+Filename: sbcli_dev-2.5.2/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/blueprints/
+Filename: sbcli_dev-2.5.2/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/node_utils.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/snode_app.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/app.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/auth_middleware.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/__init__.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/caching_node_app.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/utils.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/node_webapp.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli_dev-2.5.2/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/static/tst.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/static/is_up.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/static/delete.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/static/deploy.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli_dev-2.5.2/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/static/rpac.yaml
+Filename: sbcli_dev-2.5.2/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/static/list_deps.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli_dev-2.5.2/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/blueprints/csi.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/blueprints/__init__.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli_dev-2.5.1/setup.py` & `sbcli_dev-2.5.2/setup.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/README.md` & `sbcli_dev-2.5.2/README.md`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/PKG-INFO` & `sbcli_dev-2.5.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 2.5.1
+Version: 2.5.2
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_dev-2.5.1/simplyblock_cli/cli.py` & `sbcli_dev-2.5.2/simplyblock_cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,22 +306,18 @@
         sub_command.add_argument("--cap-crit", help='Capacity critical level in percent, default=90',
                                  type=int, required=False, dest="cap_crit")
         sub_command.add_argument("--prov-cap-warn", help='Capacity warning level in percent, default=180',
                                  type=int, required=False, dest="prov_cap_warn")
         sub_command.add_argument("--prov-cap-crit", help='Capacity critical level in percent, default=190',
                                  type=int, required=False, dest="prov_cap_crit")
         sub_command.add_argument("--ifname", help='Management interface name, default: eth0')
-        sub_command.add_argument("--log-del-interval", help='graylog deletion interval, default: 24h',
-                                 dest='log_del_interval', default='24h')
+        sub_command.add_argument("--log-del-interval", help='graylog deletion interval, default: 7d',
+                                 dest='log_del_interval', default='7d')
         sub_command.add_argument("--metrics-retention-period", help='retention period for prometheus metrics, default: 7d',
                                  dest='metrics_retention_period', default='7d')
-        sub_command.add_argument("--slack-webhook", help='the slack webhook url to be used for alerting',
-                                 dest='slack_webhook', default='')
-        sub_command.add_argument("--grafana-endpoint", help='the endpoint url for grafana',
-                                 dest='grafana_endpoint', default='')
 
         # show cluster list
         sub_command = self.add_sub_command(subparser, 'list', 'Show clusters list')
 
         # # join cluster
         # sub_command = self.add_sub_command(subparser, 'join', 'join cluster')
         # sub_command.add_argument("cluster_ip", help='the cluster IP address')
@@ -1351,22 +1347,20 @@
         cap_warn = args.cap_warn
         cap_crit = args.cap_crit
         prov_cap_warn = args.prov_cap_warn
         prov_cap_crit = args.prov_cap_crit
         ifname = args.ifname
         log_del_interval = args.log_del_interval
         metrics_retention_period = args.metrics_retention_period
-        slack_webhook = args.slack_webhook
-        grafana_endpoint = args.grafana_endpoint
 
         # TODO: Validate the inputs
         return cluster_ops.create_cluster(
             blk_size, page_size_in_blocks, ha_type, tls,
             auth_hosts_only, CLI_PASS, model_ids, cap_warn, cap_crit, prov_cap_warn, prov_cap_crit,
-            ifname, log_del_interval, metrics_retention_period, slack_webhook, grafana_endpoint)
+            ifname, log_del_interval, metrics_retention_period)
 
     def cluster_join(self, args):
         cluster_id = args.cluster_id
         cluster_ip = args.cluster_ip
         role = args.role
         ifname = args.ifname
         data_nics = args.data_nics
```

## Comparing `sbcli_dev-2.5.1/sbcli_dev.egg-info/SOURCES.txt` & `sbcli_dev-2.5.2/sbcli_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 simplyblock_core/scripts/docker-compose-swarm.yml
 simplyblock_core/scripts/haproxy.cfg
 simplyblock_core/scripts/install_deps.sh
 simplyblock_core/scripts/prometheus.yml
 simplyblock_core/scripts/run_ssh.sh
 simplyblock_core/scripts/set_db_config.sh
 simplyblock_core/scripts/stack_deploy_wait.sh
-simplyblock_core/scripts/alerting/alert_resources.yaml.j2
+simplyblock_core/scripts/alerting/alert_resources.yaml
 simplyblock_core/scripts/alerting/alert_rules.yaml
 simplyblock_core/scripts/dashboards/cluster.json
 simplyblock_core/scripts/dashboards/devices.json
 simplyblock_core/scripts/dashboards/lvols.json
 simplyblock_core/scripts/dashboards/node-exporter.json
 simplyblock_core/scripts/dashboards/nodes.json
 simplyblock_core/scripts/dashboards/pools.json
```

## Comparing `sbcli_dev-2.5.1/sbcli_dev.egg-info/PKG-INFO` & `sbcli_dev-2.5.2/sbcli_dev.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 2.5.1
+Version: 2.5.2
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_dev-2.5.1/simplyblock_core/storage_node_ops.py` & `sbcli_dev-2.5.2/simplyblock_core/storage_node_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1031,14 +1031,29 @@
             else:
                 node.remote_devices.append(dev)
             count += 1
         node.write_to_db(kv_store)
         logger.info(f"connected to devices count: {count}")
         time.sleep(3)
 
+    logger.info("Sending cluster map")
+    ret = distr_controller.send_cluster_map_to_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map"
+    time.sleep(3)
+
+    for lvol_id in snode.lvols:
+        lvol = lvol_controller.recreate_lvol(lvol_id, snode)
+        if not lvol:
+            logger.error(f"Failed to create LVol: {lvol_id}")
+            return False
+        lvol.status = lvol.STATUS_ONLINE
+        lvol.io_error = False
+        lvol.write_to_db(db_controller.kv_store)
+
     logger.info("Setting node status to Online")
     old_status = snode.status
     snode.status = StorageNode.STATUS_ONLINE
     snode.write_to_db(kv_store)
     storage_events.snode_status_change(snode, snode.status, old_status)
 
     logger.info("Sending node event update")
@@ -1047,29 +1062,14 @@
     logger.info("Sending devices event updates")
     for dev in snode.nvme_devices:
         if dev.status != NVMeDevice.STATUS_ONLINE:
             logger.debug(f"Device is not online: {dev.get_id()}, status: {dev.status}")
             continue
         distr_controller.send_dev_status_event(dev.cluster_device_order, NVMeDevice.STATUS_ONLINE)
 
-    logger.info("Sending cluster map to current node")
-    ret = distr_controller.send_cluster_map_to_node(snode)
-    if not ret:
-        return False, "Failed to send cluster map"
-    time.sleep(3)
-
-    for lvol_id in snode.lvols:
-        lvol = lvol_controller.recreate_lvol(lvol_id, snode)
-        if not lvol:
-            logger.error(f"Failed to create LVol: {lvol_id}")
-            return False
-        lvol.status = lvol.STATUS_ONLINE
-        lvol.io_error = False
-        lvol.write_to_db(db_controller.kv_store)
-
     logger.info("Done")
     return "Success"
 
 
 def list_storage_nodes(kv_store, is_json):
     db_controller = DBController(kv_store)
     nodes = db_controller.get_storage_nodes()
```

## Comparing `sbcli_dev-2.5.1/simplyblock_core/constants.py` & `sbcli_dev-2.5.2/simplyblock_core/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,12 +47,14 @@
 # To use 75% of hugepages to calculate ssd size to use for the ocf bdev
 CACHING_NODE_MEMORY_FACTOR = 0.75
 
 HEALTH_CHECK_INTERVAL_SEC = 60
 
 GRAYLOG_CHECK_INTERVAL_SEC = 60
 
-SIMPLY_BLOCK_DOCKER_IMAGE = "simplyblock/simplyblock:dev"
+FDB_CHECK_INTERVAL_SEC = 60
+
+SIMPLY_BLOCK_DOCKER_IMAGE = "simplyblock/simplyblock:cleanup_foundationdb"
 SIMPLY_BLOCK_SPDK_CORE_IMAGE = "simplyblock/spdk-core:latest"
 SIMPLY_BLOCK_SPDK_ULTRA_IMAGE = "simplyblock/spdk:main-latest"
 
 GELF_PORT = 12201
```

## Comparing `sbcli_dev-2.5.1/simplyblock_core/mgmt_node_ops.py` & `sbcli_dev-2.5.2/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/cnode_client.py` & `sbcli_dev-2.5.2/simplyblock_core/cnode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/pci_utils.py` & `sbcli_dev-2.5.2/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/snode_client.py` & `sbcli_dev-2.5.2/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/kv_store.py` & `sbcli_dev-2.5.2/simplyblock_core/kv_store.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/utils.py` & `sbcli_dev-2.5.2/simplyblock_core/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/cluster_ops.py` & `sbcli_dev-2.5.2/simplyblock_core/cluster_ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,23 @@
 import math
 import os
 import time
 import uuid
 
 import docker
 import requests
-from jinja2 import Environment, FileSystemLoader
 
 from simplyblock_core import utils, scripts, constants, mgmt_node_ops, storage_node_ops, shell_utils
 from simplyblock_core.controllers import cluster_events, device_controller
 from simplyblock_core.kv_store import DBController
 from simplyblock_core.models.cluster import Cluster
 from simplyblock_core.models.nvme_device import NVMeDevice
 from simplyblock_core.models.storage_node import StorageNode
 
 logger = logging.getLogger()
-TOP_DIR = os.path.dirname(os.path.dirname(os.path.realpath(__file__)))
 
 
 def _add_graylog_input(cluster_ip, password):
     url = f"http://{cluster_ip}:9000/api/system/inputs"
     payload = json.dumps({
         "title": "spdk log input",
         "type": "org.graylog2.inputs.gelf.udp.GELFUDPInput",
@@ -45,17 +43,15 @@
     session.auth = ("admin", password)
     response = session.request("POST", url, headers=headers, data=payload)
     logger.debug(response.text)
     return response.status_code == 201
 
 def create_cluster(blk_size, page_size_in_blocks, ha_type, tls,
                    auth_hosts_only, cli_pass, model_ids,
-                   cap_warn, cap_crit, prov_cap_warn, prov_cap_crit,
-                   ifname, log_del_interval, metrics_retention_period, slack_webhook,
-                   grafana_endpoint):
+                   cap_warn, cap_crit, prov_cap_warn, prov_cap_crit, ifname, log_del_interval, metrics_retention_period):
     logger.info("Installing dependencies...")
     ret = scripts.install_deps()
     logger.info("Installing dependencies > Done")
 
     if not ifname:
         ifname = "eth0"
 
@@ -106,27 +102,14 @@
     if cap_crit and cap_crit > 0:
         c.cap_crit = cap_crit
     if prov_cap_warn and prov_cap_warn > 0:
         c.prov_cap_warn = prov_cap_warn
     if prov_cap_crit and prov_cap_crit > 0:
         c.prov_cap_crit = prov_cap_crit
 
-    alerts_template_folder = os.path.join(TOP_DIR, "simplyblock_core/scripts/alerting/")
-
-    env = Environment(loader=FileSystemLoader(alerts_template_folder), trim_blocks=True, lstrip_blocks=True)
-    alert_resources_file = "alert_resources.yaml"
-    template = env.get_template(f'{alert_resources_file}.j2')
-    values = {
-        'SLACK_WEBHOOK': slack_webhook,
-        'GRAFANA_ENDPOINT': grafana_endpoint,
-    }
-
-    with open(os.path.join(alerts_template_folder, alert_resources_file), 'w') as file:
-        file.write(template.render(values))
-
     logger.info("Deploying swarm stack ...")
     ret = scripts.deploy_stack(cli_pass, DEV_IP, constants.SIMPLY_BLOCK_DOCKER_IMAGE, c.secret, c.uuid, log_del_interval, metrics_retention_period)
     logger.info("Deploying swarm stack > Done")
 
     logger.info("Configuring DB...")
     out = scripts.set_db_config_single()
     logger.info("Configuring DB > Done")
@@ -705,7 +688,8 @@
         if node.status == StorageNode.STATUS_ONLINE:
             storage_node_ops.shutdown_storage_node(node.get_id(), force=True)
             time.sleep(3)
         storage_node_ops.restart_storage_node(node.get_id())
 
     logger.info("Done")
     return True
+
```

## Comparing `sbcli_dev-2.5.1/simplyblock_core/compute_node_ops.py` & `sbcli_dev-2.5.2/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/rpc_client.py` & `sbcli_dev-2.5.2/simplyblock_core/rpc_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/distr_controller.py` & `sbcli_dev-2.5.2/simplyblock_core/distr_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     map_prob = []
     for snode in snodes:
         dev_map = {}
         dev_w_map = []
         node_w = 0
         for i, dev in enumerate(snode.nvme_devices):
             logger.debug(f"Device: {dev.get_id()}, status: {dev.status}")
-            if dev.status in [NVMeDevice.STATUS_JM, NVMeDevice.STATUS_NEW]:
+            if dev.status == NVMeDevice.STATUS_JM:
                 continue
 
             dev_w = int(dev.size/(1024*1024*1024)) or 1
             node_w += dev_w
             name = None
             if snode.get_id() == target_node.get_id():
                 name = dev.alceml_bdev
```

## Comparing `sbcli_dev-2.5.1/simplyblock_core/services/lvol_monitor.py` & `sbcli_dev-2.5.2/simplyblock_core/services/lvol_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/services/caching_node_monitor.py` & `sbcli_dev-2.5.2/simplyblock_core/services/caching_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/services/health_check_service.py` & `sbcli_dev-2.5.2/simplyblock_core/services/health_check_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/services/lvol_stat_collector.py` & `sbcli_dev-2.5.2/simplyblock_core/services/lvol_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/services/log_agg_service.py` & `sbcli_dev-2.5.2/simplyblock_core/services/log_agg_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/services/distr_event_collector.py` & `sbcli_dev-2.5.2/simplyblock_core/services/distr_event_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli_dev-2.5.2/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/services/port_stat_collector.py` & `sbcli_dev-2.5.2/simplyblock_core/services/port_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/services/device_monitor.py` & `sbcli_dev-2.5.2/simplyblock_core/services/device_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/services/__init__.py` & `sbcli_dev-2.5.2/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/services/install_service.sh` & `sbcli_dev-2.5.2/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli_dev-2.5.2/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/services/cap_monitor.py` & `sbcli_dev-2.5.2/simplyblock_core/services/cap_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/services/storage_node_monitor.py` & `sbcli_dev-2.5.2/simplyblock_core/services/storage_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/scripts/deploy_stack.sh` & `sbcli_dev-2.5.2/simplyblock_core/scripts/deploy_stack.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/scripts/haproxy.cfg` & `sbcli_dev-2.5.2/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli_dev-2.5.2/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,26 @@
     deploy:
       placement:
         constraints: [node.role == manager]
     volumes:
       - "/etc/foundationdb:/etc/foundationdb"
     networks:
       - hostnet
-
+  CleanupFDB:
+    image: $SIMPLYBLOCK_DOCKER_IMAGE
+    environment:
+      LOG_DELETION_INTERVAL: "${LOG_DELETION_INTERVAL}"
+    command: "python simplyblock_core/workers/cleanup_foundationdb.py"
+    deploy:
+      placement:
+        constraints: [node.role == manager]
+    volumes:
+      - "/etc/foundationdb:/etc/foundationdb"
+    networks:
+      - hostnet
 volumes:
   os_data:
 
 networks:
   hostnet:
     external: true
     name: host
```

## Comparing `sbcli_dev-2.5.1/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli_dev-2.5.2/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml` & `sbcli_dev-2.5.2/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/scripts/__init__.py` & `sbcli_dev-2.5.2/simplyblock_core/scripts/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/scripts/install_deps.sh` & `sbcli_dev-2.5.2/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/scripts/apply_dashboard.sh` & `sbcli_dev-2.5.2/simplyblock_core/scripts/apply_dashboard.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/scripts/alerting/alert_rules.yaml` & `sbcli_dev-2.5.2/simplyblock_core/scripts/alerting/alert_rules.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/scripts/alerting/alert_resources.yaml.j2` & `sbcli_dev-2.5.2/simplyblock_core/scripts/alerting/alert_resources.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -11,23 +11,20 @@
   - orgId: 1
     name: grafana-alerts
     receivers:
       - uid: grafana
         type: slack
         settings:
           username: grafana_bot
-          url: '{{ SLACK_WEBHOOK }}'
+          url: 'https://hooks.slack.com/services/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'
           title: |
-            {% raw %}
             {{ template "slack.title" . }}
           text: |
             {{ template "slack.message" . }}
-            {% endraw %}
 
-{% raw %}
 templates:
   - orgId: 1
     name: slack.title
     template: |-
       {{ define "slack.title" -}}
       [{{ .Status | toUpper }}{{ if eq .Status "firing" }}:{{ .Alerts.Firing | len }}{{ end }}] Grafana Alerting Notification
       {{- end -}}
@@ -37,17 +34,15 @@
       {{ define "slack.print_alert" -}}
       *Alert*: {{ .Labels.alertname }}
       {{ if .Annotations -}}
       *Summary*: {{ .Annotations.summary}}
       *Description*: {{ .Annotations.description }}
       {{ end -}}
       *Log message*: {{ index .Labels "message" }}
-      {% endraw %}
-      *Explore logs:* {{ GRAFANA_ENDPOINT }}
-      {% raw %}
+      *Explore logs:* https://grafanaURL.com/explore?orgId=1
       {{ if .DashboardURL -}}
       *Go to dashboard:* {{ .DashboardURL }}
       {{- end }}
       {{ if .PanelURL -}}
       *Go to panel:* {{ .PanelURL }}
       {{- end }}
 
@@ -66,8 +61,7 @@
       {{ len .Alerts.Firing }} firing alert(s):
       {{ range .Alerts.Firing }}
       {{ template "slack.print_alert" . }}
       {{ end -}}
       {{ end }}
 
       {{- end }}
-      {% endraw %}
```

## Comparing `sbcli_dev-2.5.1/simplyblock_core/scripts/dashboards/devices.json` & `sbcli_dev-2.5.2/simplyblock_core/scripts/dashboards/devices.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/scripts/dashboards/node-exporter.json` & `sbcli_dev-2.5.2/simplyblock_core/scripts/dashboards/node-exporter.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/scripts/dashboards/nodes.json` & `sbcli_dev-2.5.2/simplyblock_core/scripts/dashboards/nodes.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/scripts/dashboards/lvols.json` & `sbcli_dev-2.5.2/simplyblock_core/scripts/dashboards/lvols.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/scripts/dashboards/cluster.json` & `sbcli_dev-2.5.2/simplyblock_core/scripts/dashboards/cluster.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/scripts/dashboards/pools.json` & `sbcli_dev-2.5.2/simplyblock_core/scripts/dashboards/pools.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/controllers/device_controller.py` & `sbcli_dev-2.5.2/simplyblock_core/controllers/device_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/controllers/mgmt_events.py` & `sbcli_dev-2.5.2/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/controllers/events_controller.py` & `sbcli_dev-2.5.2/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/controllers/storage_events.py` & `sbcli_dev-2.5.2/simplyblock_core/controllers/storage_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/controllers/lvol_events.py` & `sbcli_dev-2.5.2/simplyblock_core/controllers/lvol_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/controllers/snapshot_controller.py` & `sbcli_dev-2.5.2/simplyblock_core/controllers/snapshot_controller.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -133,22 +133,22 @@
     # creating RPCClient instance
     rpc_client = RPCClient(
         snode.mgmt_ip,
         snode.rpc_port,
         snode.rpc_username,
         snode.rpc_password)
 
-    ret = rpc_client.ultra21_lvol_dismount(snap.snap_bdev)
+    ret = rpc_client.bdev_distrib_delete(snap.base_bdev)
     if not ret:
-        logger.error(f"Failed to delete BDev {snap.snap_bdev}")
+        logger.error(f"Failed to delete BDev {snap.base_bdev}")
         return False
 
-    ret = rpc_client.bdev_distrib_delete(snap.base_bdev)
+    ret = rpc_client.ultra21_lvol_dismount(snap.snap_bdev)
     if not ret:
-        logger.error(f"Failed to delete BDev {snap.base_bdev}")
+        logger.error(f"Failed to delete BDev {snap.snap_bdev}")
         return False
 
     snap.remove(db_controller.kv_store)
 
     base_lvol = db_controller.get_lvol_by_id(snap.lvol.get_id())
     if base_lvol.deleted is True:
         lvol_controller.delete_lvol(base_lvol.get_id())
```

## Comparing `sbcli_dev-2.5.1/simplyblock_core/controllers/device_events.py` & `sbcli_dev-2.5.2/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/controllers/pool_controller.py` & `sbcli_dev-2.5.2/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/controllers/cluster_events.py` & `sbcli_dev-2.5.2/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/controllers/caching_node_controller.py` & `sbcli_dev-2.5.2/simplyblock_core/controllers/caching_node_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/controllers/snapshot_events.py` & `sbcli_dev-2.5.2/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/controllers/lvol_controller.py` & `sbcli_dev-2.5.2/simplyblock_core/controllers/lvol_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/controllers/health_controller.py` & `sbcli_dev-2.5.2/simplyblock_core/controllers/health_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/controllers/pool_events.py` & `sbcli_dev-2.5.2/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/models/events.py` & `sbcli_dev-2.5.2/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/models/iface.py` & `sbcli_dev-2.5.2/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/models/base_model.py` & `sbcli_dev-2.5.2/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/models/lvol_model.py` & `sbcli_dev-2.5.2/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/models/compute_node.py` & `sbcli_dev-2.5.2/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/models/snapshot.py` & `sbcli_dev-2.5.2/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/models/pool.py` & `sbcli_dev-2.5.2/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/models/global_settings.py` & `sbcli_dev-2.5.2/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/models/port_stat.py` & `sbcli_dev-2.5.2/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/models/storage_node.py` & `sbcli_dev-2.5.2/simplyblock_core/models/storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/models/stats.py` & `sbcli_dev-2.5.2/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/models/cluster.py` & `sbcli_dev-2.5.2/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/models/mgmt_node.py` & `sbcli_dev-2.5.2/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/models/caching_node.py` & `sbcli_dev-2.5.2/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_core/models/nvme_device.py` & `sbcli_dev-2.5.2/simplyblock_core/models/nvme_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from simplyblock_core.models.base_model import BaseModel
 
 
 class NVMeDevice(BaseModel):
 
     STATUS_JM = "JM_DEV"
 
-    STATUS_NEW = "new"
     STATUS_ONLINE = 'online'
     STATUS_UNAVAILABLE = 'unavailable'
     STATUS_REMOVED = 'removed'
     STATUS_FAILED = 'failed'
     STATUS_READONLY = 'read_only'
 
     attributes = {
```

## Comparing `sbcli_dev-2.5.1/simplyblock_web/caching_node_app_k8s.py` & `sbcli_dev-2.5.2/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/node_utils.py` & `sbcli_dev-2.5.2/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/snode_app.py` & `sbcli_dev-2.5.2/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/app.py` & `sbcli_dev-2.5.2/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/auth_middleware.py` & `sbcli_dev-2.5.2/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/caching_node_app.py` & `sbcli_dev-2.5.2/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/utils.py` & `sbcli_dev-2.5.2/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/node_webapp.py` & `sbcli_dev-2.5.2/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/static/delete.py` & `sbcli_dev-2.5.2/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/static/deploy.py` & `sbcli_dev-2.5.2/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/static/deploy_spdk.yaml` & `sbcli_dev-2.5.2/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli_dev-2.5.2/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli_dev-2.5.2/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli_dev-2.5.2/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/blueprints/snode_ops.py` & `sbcli_dev-2.5.2/simplyblock_web/blueprints/snode_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/blueprints/csi.py` & `sbcli_dev-2.5.2/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli_dev-2.5.2/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli_dev-2.5.2/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_device.py` & `sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/blueprints/node_api_basic.py` & `sbcli_dev-2.5.2/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.1/simplyblock_web/blueprints/web_api_pool.py` & `sbcli_dev-2.5.2/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

