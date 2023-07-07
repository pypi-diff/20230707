# Comparing `tmp/talos_install-0.2.0.dev368.tar.gz` & `tmp/talos_install-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talos_install-0.2.0.dev368.tar", last modified: Sat Jul  1 08:45:36 2023, max compression
+gzip compressed data, was "talos_install-0.2.1.tar", last modified: Fri Jul  7 16:44:50 2023, max compression
```

## Comparing `talos_install-0.2.0.dev368.tar` & `talos_install-0.2.1.tar`

### file list

```diff
@@ -1,225 +1,225 @@
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.948916 talos_install-0.2.0.dev368/
--rw-rw-r--   0 installer  (3002) installer  (3002)      347 2023-07-01 08:45:36.000000 talos_install-0.2.0.dev368/AUTHORS
--rw-rw-r--   0 installer  (3002) installer  (3002)    13162 2023-07-01 08:45:36.000000 talos_install-0.2.0.dev368/ChangeLog
--rw-rw-r--   0 installer  (3002) installer  (3002)     4233 2023-07-01 08:45:36.949916 talos_install-0.2.0.dev368/PKG-INFO
--rw-rw-r--   0 installer  (3002) installer  (3002)     3573 2023-06-30 16:33:53.000000 talos_install-0.2.0.dev368/README.md
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.920916 talos_install-0.2.0.dev368/ansible/
--rw-rw-r--   0 installer  (3002) installer  (3002)      334 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/ansible.cfg
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.920916 talos_install-0.2.0.dev368/ansible/group_vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)      672 2023-06-30 15:05:58.000000 talos_install-0.2.0.dev368/ansible/group_vars/all.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.917916 talos_install-0.2.0.dev368/ansible/roles/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.905916 talos_install-0.2.0.dev368/ansible/roles/cli/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.920916 talos_install-0.2.0.dev368/ansible/roles/cli/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/cli/files/FOUNDMEDEVKEY
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.921916 talos_install-0.2.0.dev368/ansible/roles/cli/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/cli/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.922916 talos_install-0.2.0.dev368/ansible/roles/cli/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1197 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/cli/tasks/clone.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1512 2023-06-16 10:28:42.000000 talos_install-0.2.0.dev368/ansible/roles/cli/tasks/env.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      301 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/cli/tasks/logrotate.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      467 2023-06-30 16:15:20.000000 talos_install-0.2.0.dev368/ansible/roles/cli/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     2692 2023-06-30 15:05:58.000000 talos_install-0.2.0.dev368/ansible/roles/cli/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1675 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/cli/tasks/web.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.924916 talos_install-0.2.0.dev368/ansible/roles/cli/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3814 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev368/ansible/roles/cli/templates/agent.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      453 2023-06-30 15:05:58.000000 talos_install-0.2.0.dev368/ansible/roles/cli/templates/app.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      772 2023-06-30 15:05:58.000000 talos_install-0.2.0.dev368/ansible/roles/cli/templates/cli.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     2433 2023-06-30 15:05:58.000000 talos_install-0.2.0.dev368/ansible/roles/cli/templates/env_talos.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1381 2023-06-16 10:28:42.000000 talos_install-0.2.0.dev368/ansible/roles/cli/templates/globals.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1711 2023-06-16 12:33:23.000000 talos_install-0.2.0.dev368/ansible/roles/cli/templates/my-httpd.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      379 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/cli/templates/passwords.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      506 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/cli/templates/talos-logrotate.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1088 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/cli/templates/talos.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)       22 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/cli/templates/talospass.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.906916 talos_install-0.2.0.dev368/ansible/roles/common/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.924916 talos_install-0.2.0.dev368/ansible/roles/common/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       59 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/common/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.925916 talos_install-0.2.0.dev368/ansible/roles/common/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      360 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/common/tasks/install_extra_pkgs.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      155 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/common/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      818 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/common/tasks/misc.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.906916 talos_install-0.2.0.dev368/ansible/roles/gather_facts/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.925916 talos_install-0.2.0.dev368/ansible/roles/gather_facts/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      495 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/gather_facts/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.926916 talos_install-0.2.0.dev368/ansible/roles/gather_facts/vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)      949 2023-06-29 13:29:49.000000 talos_install-0.2.0.dev368/ansible/roles/gather_facts/vars/RedHat.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      948 2023-06-29 13:29:49.000000 talos_install-0.2.0.dev368/ansible/roles/gather_facts/vars/Rocky.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.907916 talos_install-0.2.0.dev368/ansible/roles/install_ansible/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.906916 talos_install-0.2.0.dev368/ansible/roles/install_ansible/files/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.926916 talos_install-0.2.0.dev368/ansible/roles/install_ansible/files/inventory_plugins/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3333 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.926916 talos_install-0.2.0.dev368/ansible/roles/install_ansible/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_ansible/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.927916 talos_install-0.2.0.dev368/ansible/roles/install_ansible/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1764 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_ansible/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.927916 talos_install-0.2.0.dev368/ansible/roles/install_ansible/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)      512 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_ansible/templates/ansible.cfg.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.907916 talos_install-0.2.0.dev368/ansible/roles/install_certificates/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.927916 talos_install-0.2.0.dev368/ansible/roles/install_certificates/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_certificates/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.927916 talos_install-0.2.0.dev368/ansible/roles/install_certificates/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      689 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_certificates/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.908916 talos_install-0.2.0.dev368/ansible/roles/install_docker/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.928916 talos_install-0.2.0.dev368/ansible/roles/install_docker/handlers/
--rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_docker/handlers/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.928916 talos_install-0.2.0.dev368/ansible/roles/install_docker/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_docker/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.928916 talos_install-0.2.0.dev368/ansible/roles/install_docker/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1526 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_docker/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.929916 talos_install-0.2.0.dev368/ansible/roles/install_docker/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)      183 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_docker/templates/daemon.json.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1919 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_docker/templates/docker-ce.repo.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.909916 talos_install-0.2.0.dev368/ansible/roles/install_python/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.929916 talos_install-0.2.0.dev368/ansible/roles/install_python/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      590 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_python/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.929916 talos_install-0.2.0.dev368/ansible/roles/install_python/vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_python/vars/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.913916 talos_install-0.2.0.dev368/ansible/roles/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.929916 talos_install-0.2.0.dev368/ansible/roles/nagios/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      253 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.910916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.909916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.929916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/etc/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.930916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/etc/nagios/conf.d/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/etc/nagios/conf.d/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.930916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/etc/nagios/monitor/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/etc/nagios/monitor/.ID
--rw-rw-r--   0 installer  (3002) installer  (3002)      499 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/etc/nagios/resource.cfg
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.912916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.930916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.910916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/apache2/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.930916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1615 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf
--rw-rw-r--   0 installer  (3002) installer  (3002)      245 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/rsyslog.conf
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.911916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.931916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/apache/
--rw-rw-r--   0 installer  (3002) installer  (3002)      140 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/apache/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.931916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/nagios/
--rw-rw-r--   0 installer  (3002) installer  (3002)      835 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/nagios/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.931916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/postfix/
--rw-rw-r--   0 installer  (3002) installer  (3002)      752 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/postfix/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.931916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/
--rw-rw-r--   0 installer  (3002) installer  (3002)       51 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.912916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.911916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.931916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/etc/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.932916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.933916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/images/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13613 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png
--rw-rw-r--   0 installer  (3002) installer  (3002)    13958 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png
--rw-rw-r--   0 installer  (3002) installer  (3002)     1614 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php
--rw-rw-r--   0 installer  (3002) installer  (3002)     1585 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html
--rw-rw-r--   0 installer  (3002) installer  (3002)     5972 2023-06-16 10:28:42.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.933916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-footer.ssi
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-header.ssi
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.934916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/
--rw-rw-r--   0 installer  (3002) installer  (3002)     9882 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css
--rw-rw-r--   0 installer  (3002) installer  (3002)     7391 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.912916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagiosgraph/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.934916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)      950 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.912916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/usr/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.913916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/usr/local/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.934916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/usr/local/bin/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1147 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.935916 talos_install-0.2.0.dev368/ansible/roles/nagios/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      748 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/tasks/build.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      349 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1070 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1098 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/tasks/run.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.936916 talos_install-0.2.0.dev368/ansible/roles/nagios/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)    14403 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/templates/Dockerfile.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)    11609 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/templates/cgi.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     3808 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/templates/contacts.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     2765 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/templates/localhost.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      116 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/templates/nagios.conf.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.915916 talos_install-0.2.0.dev368/ansible/roles/opendcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.936916 talos_install-0.2.0.dev368/ansible/roles/opendcim/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      263 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.938916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1167 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/apache2.conf
--rw-rw-r--   0 installer  (3002) installer  (3002)      106 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/apache2.sh
--rw-rw-r--   0 installer  (3002) installer  (3002)    60057 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/default.sql
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.913916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.914916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/etc/opendcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.938916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/etc/opendcim/drawings/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.938916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/etc/opendcim/pictures/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png
--rw-rw-r--   0 installer  (3002) installer  (3002)      233 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/mysqld.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.914916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.914916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.914916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.938916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.939916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/css/
--rw-rw-r--   0 installer  (3002) installer  (3002)    53198 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php
--rw-rw-r--   0 installer  (3002) installer  (3002)    20094 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.939916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/images/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png
--rw-rw-r--   0 installer  (3002) installer  (3002)    38561 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php
--rw-rw-r--   0 installer  (3002) installer  (3002)     1350 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/pre-conf.sh
--rw-rw-r--   0 installer  (3002) installer  (3002)     1114 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/startup.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.940916 talos_install-0.2.0.dev368/ansible/roles/opendcim/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)        4 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.940916 talos_install-0.2.0.dev368/ansible/roles/opendcim/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1052 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/tasks/build.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      353 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      725 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1131 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/tasks/run.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.941916 talos_install-0.2.0.dev368/ansible/roles/opendcim/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3023 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/templates/Dockerfile.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      635 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/templates/first-run.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      157 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/templates/opendcim.conf.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.915916 talos_install-0.2.0.dev368/ansible/roles/os_tune/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.941916 talos_install-0.2.0.dev368/ansible/roles/os_tune/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1403 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/os_tune/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.916916 talos_install-0.2.0.dev368/ansible/roles/talos_users/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.942916 talos_install-0.2.0.dev368/ansible/roles/talos_users/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)       75 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/talos_users/files/talos
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.942916 talos_install-0.2.0.dev368/ansible/roles/talos_users/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/talos_users/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.942916 talos_install-0.2.0.dev368/ansible/roles/talos_users/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      634 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev368/ansible/roles/talos_users/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.917916 talos_install-0.2.0.dev368/ansible/roles/uninstall/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.942916 talos_install-0.2.0.dev368/ansible/roles/uninstall/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)       89 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/uninstall/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.943916 talos_install-0.2.0.dev368/ansible/roles/uninstall/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/uninstall/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.943916 talos_install-0.2.0.dev368/ansible/roles/uninstall/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      656 2023-06-30 15:05:58.000000 talos_install-0.2.0.dev368/ansible/roles/uninstall/tasks/cli.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      315 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/uninstall/tasks/docker.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      176 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/uninstall/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      339 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/uninstall/tasks/user.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.944916 talos_install-0.2.0.dev368/ansible/roles/wiki/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.944916 talos_install-0.2.0.dev368/ansible/roles/wiki/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      572 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev368/ansible/roles/wiki/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.944916 talos_install-0.2.0.dev368/ansible/roles/wiki/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/wiki/meta/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/wiki/requirements.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.945916 talos_install-0.2.0.dev368/ansible/roles/wiki/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      542 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/wiki/tasks/compose.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      161 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev368/ansible/roles/wiki/tasks/init.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      325 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev368/ansible/roles/wiki/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      240 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/wiki/tasks/misc.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.946916 talos_install-0.2.0.dev368/ansible/roles/wiki/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1275 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev368/ansible/roles/wiki/templates/docker-compose.yml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      327 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/wiki/templates/wiki.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      436 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/wiki/templates/wikidump.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1844 2023-06-30 16:15:20.000000 talos_install-0.2.0.dev368/ansible/site.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.947916 talos_install-0.2.0.dev368/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)      311 2023-06-16 10:28:42.000000 talos_install-0.2.0.dev368/etc/example_globals.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1090 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/etc/example_talos.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)       46 2023-04-16 16:14:10.000000 talos_install-0.2.0.dev368/etc/inventory
--rw-rw-r--   0 installer  (3002) installer  (3002)     1188 2023-07-01 08:45:36.956916 talos_install-0.2.0.dev368/setup.cfg
--rw-rw-r--   0 installer  (3002) installer  (3002)      321 2023-06-15 16:56:29.000000 talos_install-0.2.0.dev368/setup.py
--rwxrwxr-x   0 installer  (3002) installer  (3002)    10898 2023-06-30 16:33:24.000000 talos_install-0.2.0.dev368/talos_install
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.948916 talos_install-0.2.0.dev368/talos_install.egg-info/
--rw-rw-r--   0 installer  (3002) installer  (3002)     4233 2023-07-01 08:45:36.000000 talos_install-0.2.0.dev368/talos_install.egg-info/PKG-INFO
--rw-rw-r--   0 installer  (3002) installer  (3002)     5634 2023-07-01 08:45:36.000000 talos_install-0.2.0.dev368/talos_install.egg-info/SOURCES.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-07-01 08:45:36.000000 talos_install-0.2.0.dev368/talos_install.egg-info/dependency_links.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-06-15 16:56:45.000000 talos_install-0.2.0.dev368/talos_install.egg-info/not-zip-safe
--rw-rw-r--   0 installer  (3002) installer  (3002)       47 2023-07-01 08:45:36.000000 talos_install-0.2.0.dev368/talos_install.egg-info/pbr.json
--rw-rw-r--   0 installer  (3002) installer  (3002)       94 2023-07-01 08:45:36.000000 talos_install-0.2.0.dev368/talos_install.egg-info/requires.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-07-01 08:45:36.000000 talos_install-0.2.0.dev368/talos_install.egg-info/top_level.txt
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.716694 talos_install-0.2.1/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      347 2023-07-07 16:44:50.000000 talos_install-0.2.1/AUTHORS
+-rw-rw-r--   0 installer  (3002) installer  (3002)    14160 2023-07-07 16:44:50.000000 talos_install-0.2.1/ChangeLog
+-rw-rw-r--   0 installer  (3002) installer  (3002)     4825 2023-07-07 16:44:50.716694 talos_install-0.2.1/PKG-INFO
+-rw-rw-r--   0 installer  (3002) installer  (3002)     4172 2023-07-04 12:06:47.000000 talos_install-0.2.1/README.md
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.688694 talos_install-0.2.1/ansible/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      334 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/ansible.cfg
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.689694 talos_install-0.2.1/ansible/group_vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      603 2023-07-07 16:42:14.000000 talos_install-0.2.1/ansible/group_vars/all.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.685694 talos_install-0.2.1/ansible/roles/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.674694 talos_install-0.2.1/ansible/roles/cli/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.689694 talos_install-0.2.1/ansible/roles/cli/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/cli/files/FOUNDMEDEVKEY
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.689694 talos_install-0.2.1/ansible/roles/cli/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/cli/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.690694 talos_install-0.2.1/ansible/roles/cli/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1197 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/cli/tasks/clone.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1512 2023-06-16 10:28:42.000000 talos_install-0.2.1/ansible/roles/cli/tasks/env.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      301 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/cli/tasks/logrotate.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      434 2023-07-02 09:06:27.000000 talos_install-0.2.1/ansible/roles/cli/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2692 2023-07-02 09:06:27.000000 talos_install-0.2.1/ansible/roles/cli/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1675 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/cli/tasks/web.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.693694 talos_install-0.2.1/ansible/roles/cli/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3814 2023-06-15 16:34:43.000000 talos_install-0.2.1/ansible/roles/cli/templates/agent.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      418 2023-07-04 12:06:47.000000 talos_install-0.2.1/ansible/roles/cli/templates/app.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      745 2023-07-04 12:06:47.000000 talos_install-0.2.1/ansible/roles/cli/templates/cli.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2388 2023-07-04 12:06:47.000000 talos_install-0.2.1/ansible/roles/cli/templates/env_talos.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1381 2023-06-16 10:28:42.000000 talos_install-0.2.1/ansible/roles/cli/templates/globals.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1711 2023-06-16 12:33:23.000000 talos_install-0.2.1/ansible/roles/cli/templates/my-httpd.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      379 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/cli/templates/passwords.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      506 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/cli/templates/talos-logrotate.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1088 2023-07-07 16:42:43.000000 talos_install-0.2.1/ansible/roles/cli/templates/talos.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)       22 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/cli/templates/talospass.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.675694 talos_install-0.2.1/ansible/roles/common/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.693694 talos_install-0.2.1/ansible/roles/common/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       59 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/common/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.694694 talos_install-0.2.1/ansible/roles/common/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      360 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/common/tasks/install_extra_pkgs.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      155 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/common/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      818 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/common/tasks/misc.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.675694 talos_install-0.2.1/ansible/roles/gather_facts/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.694694 talos_install-0.2.1/ansible/roles/gather_facts/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      495 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/gather_facts/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.694694 talos_install-0.2.1/ansible/roles/gather_facts/vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      949 2023-06-29 13:29:49.000000 talos_install-0.2.1/ansible/roles/gather_facts/vars/RedHat.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      948 2023-06-29 13:29:49.000000 talos_install-0.2.1/ansible/roles/gather_facts/vars/Rocky.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.676694 talos_install-0.2.1/ansible/roles/install_ansible/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.675694 talos_install-0.2.1/ansible/roles/install_ansible/files/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.694694 talos_install-0.2.1/ansible/roles/install_ansible/files/inventory_plugins/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3333 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.695694 talos_install-0.2.1/ansible/roles/install_ansible/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_ansible/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.695694 talos_install-0.2.1/ansible/roles/install_ansible/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1764 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_ansible/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.695694 talos_install-0.2.1/ansible/roles/install_ansible/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      512 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_ansible/templates/ansible.cfg.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.676694 talos_install-0.2.1/ansible/roles/install_certificates/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.695694 talos_install-0.2.1/ansible/roles/install_certificates/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_certificates/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.696694 talos_install-0.2.1/ansible/roles/install_certificates/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      689 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_certificates/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.677694 talos_install-0.2.1/ansible/roles/install_docker/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.696694 talos_install-0.2.1/ansible/roles/install_docker/handlers/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_docker/handlers/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.696694 talos_install-0.2.1/ansible/roles/install_docker/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_docker/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.696694 talos_install-0.2.1/ansible/roles/install_docker/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1526 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_docker/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.697694 talos_install-0.2.1/ansible/roles/install_docker/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      183 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_docker/templates/daemon.json.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1919 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_docker/templates/docker-ce.repo.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.677694 talos_install-0.2.1/ansible/roles/install_python/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.697694 talos_install-0.2.1/ansible/roles/install_python/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      590 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_python/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.697694 talos_install-0.2.1/ansible/roles/install_python/vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_python/vars/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.682694 talos_install-0.2.1/ansible/roles/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.697694 talos_install-0.2.1/ansible/roles/nagios/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      253 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.679694 talos_install-0.2.1/ansible/roles/nagios/files/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.678694 talos_install-0.2.1/ansible/roles/nagios/files/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.698694 talos_install-0.2.1/ansible/roles/nagios/files/etc/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.698694 talos_install-0.2.1/ansible/roles/nagios/files/etc/nagios/conf.d/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/etc/nagios/conf.d/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.698694 talos_install-0.2.1/ansible/roles/nagios/files/etc/nagios/monitor/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/etc/nagios/monitor/.ID
+-rw-rw-r--   0 installer  (3002) installer  (3002)      499 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/etc/nagios/resource.cfg
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.681694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.698694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.679694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/apache2/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.698694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1615 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf
+-rw-rw-r--   0 installer  (3002) installer  (3002)      245 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/rsyslog.conf
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.680694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.699694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/apache/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      140 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/apache/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.699694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/nagios/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      835 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/nagios/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.699694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/postfix/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      752 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/postfix/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.699694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       51 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.681694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.680694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.699694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/etc/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.700694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.701694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/images/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13613 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13958 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1614 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1585 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html
+-rw-rw-r--   0 installer  (3002) installer  (3002)     5972 2023-06-16 10:28:42.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.701694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-footer.ssi
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-header.ssi
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.701694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     9882 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css
+-rw-rw-r--   0 installer  (3002) installer  (3002)     7391 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.681694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagiosgraph/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.702694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      950 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.681694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/usr/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.681694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/usr/local/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.702694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/usr/local/bin/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1147 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.703694 talos_install-0.2.1/ansible/roles/nagios/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      748 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/tasks/build.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      349 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1070 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1098 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/tasks/run.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.704694 talos_install-0.2.1/ansible/roles/nagios/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    14403 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/templates/Dockerfile.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)    11609 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/templates/cgi.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3808 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/templates/contacts.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2765 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/templates/localhost.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      116 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/templates/nagios.conf.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.684694 talos_install-0.2.1/ansible/roles/opendcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.704694 talos_install-0.2.1/ansible/roles/opendcim/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      295 2023-07-04 12:06:47.000000 talos_install-0.2.1/ansible/roles/opendcim/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.706694 talos_install-0.2.1/ansible/roles/opendcim/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1167 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/apache2.conf
+-rw-rw-r--   0 installer  (3002) installer  (3002)      106 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/apache2.sh
+-rw-rw-r--   0 installer  (3002) installer  (3002)    60057 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/default.sql
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.682694 talos_install-0.2.1/ansible/roles/opendcim/files/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.683694 talos_install-0.2.1/ansible/roles/opendcim/files/etc/opendcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.706694 talos_install-0.2.1/ansible/roles/opendcim/files/etc/opendcim/drawings/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.706694 talos_install-0.2.1/ansible/roles/opendcim/files/etc/opendcim/pictures/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)      233 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/mysqld.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.683694 talos_install-0.2.1/ansible/roles/opendcim/files/overlay/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.683694 talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.683694 talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.706694 talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.707694 talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/css/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    53198 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)    20094 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.707694 talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/images/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)    38561 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1350 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/pre-conf.sh
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1114 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/startup.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.707694 talos_install-0.2.1/ansible/roles/opendcim/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        4 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.708694 talos_install-0.2.1/ansible/roles/opendcim/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1052 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/tasks/build.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      353 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      725 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1131 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/tasks/run.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.709694 talos_install-0.2.1/ansible/roles/opendcim/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3023 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/templates/Dockerfile.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      712 2023-07-04 12:06:47.000000 talos_install-0.2.1/ansible/roles/opendcim/templates/first-run.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      168 2023-07-04 12:06:47.000000 talos_install-0.2.1/ansible/roles/opendcim/templates/opendcim.conf.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.684694 talos_install-0.2.1/ansible/roles/os_tune/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.709694 talos_install-0.2.1/ansible/roles/os_tune/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1403 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/os_tune/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.685694 talos_install-0.2.1/ansible/roles/talos_users/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.709694 talos_install-0.2.1/ansible/roles/talos_users/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       75 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/talos_users/files/talos
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.710694 talos_install-0.2.1/ansible/roles/talos_users/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/talos_users/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.710694 talos_install-0.2.1/ansible/roles/talos_users/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      634 2023-06-15 16:34:43.000000 talos_install-0.2.1/ansible/roles/talos_users/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.685694 talos_install-0.2.1/ansible/roles/uninstall/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.710694 talos_install-0.2.1/ansible/roles/uninstall/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       89 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/uninstall/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.710694 talos_install-0.2.1/ansible/roles/uninstall/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/uninstall/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.711694 talos_install-0.2.1/ansible/roles/uninstall/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      656 2023-07-02 09:06:27.000000 talos_install-0.2.1/ansible/roles/uninstall/tasks/cli.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      315 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/uninstall/tasks/docker.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      176 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/uninstall/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      339 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/uninstall/tasks/user.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.711694 talos_install-0.2.1/ansible/roles/wiki/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.712694 talos_install-0.2.1/ansible/roles/wiki/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      572 2023-06-15 16:34:43.000000 talos_install-0.2.1/ansible/roles/wiki/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.712694 talos_install-0.2.1/ansible/roles/wiki/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/wiki/meta/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/wiki/requirements.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.713694 talos_install-0.2.1/ansible/roles/wiki/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      542 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/wiki/tasks/compose.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      161 2023-06-15 16:34:43.000000 talos_install-0.2.1/ansible/roles/wiki/tasks/init.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      325 2023-06-15 16:34:43.000000 talos_install-0.2.1/ansible/roles/wiki/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      240 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/wiki/tasks/misc.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.713694 talos_install-0.2.1/ansible/roles/wiki/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1275 2023-06-15 16:34:43.000000 talos_install-0.2.1/ansible/roles/wiki/templates/docker-compose.yml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      327 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/wiki/templates/wiki.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      436 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/wiki/templates/wikidump.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1844 2023-07-02 09:06:27.000000 talos_install-0.2.1/ansible/site.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.714694 talos_install-0.2.1/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      311 2023-07-02 09:06:27.000000 talos_install-0.2.1/etc/example_globals.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1090 2023-07-02 09:06:27.000000 talos_install-0.2.1/etc/example_talos.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)       46 2023-04-16 16:14:10.000000 talos_install-0.2.1/etc/inventory
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1188 2023-07-07 16:44:50.722694 talos_install-0.2.1/setup.cfg
+-rw-rw-r--   0 installer  (3002) installer  (3002)      321 2023-06-15 16:56:29.000000 talos_install-0.2.1/setup.py
+-rwxrwxr-x   0 installer  (3002) installer  (3002)    10898 2023-07-02 09:06:27.000000 talos_install-0.2.1/talos_install
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.716694 talos_install-0.2.1/talos_install.egg-info/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     4825 2023-07-07 16:44:50.000000 talos_install-0.2.1/talos_install.egg-info/PKG-INFO
+-rw-rw-r--   0 installer  (3002) installer  (3002)     5634 2023-07-07 16:44:50.000000 talos_install-0.2.1/talos_install.egg-info/SOURCES.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-07-07 16:44:50.000000 talos_install-0.2.1/talos_install.egg-info/dependency_links.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-06-15 16:56:45.000000 talos_install-0.2.1/talos_install.egg-info/not-zip-safe
+-rw-rw-r--   0 installer  (3002) installer  (3002)       47 2023-07-07 16:44:50.000000 talos_install-0.2.1/talos_install.egg-info/pbr.json
+-rw-rw-r--   0 installer  (3002) installer  (3002)       94 2023-07-07 16:44:50.000000 talos_install-0.2.1/talos_install.egg-info/requires.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-07-07 16:44:50.000000 talos_install-0.2.1/talos_install.egg-info/top_level.txt
```

### Comparing `talos_install-0.2.0.dev368/ChangeLog` & `talos_install-0.2.1/ChangeLog`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,50 @@
 CHANGES
 =======
 
+* Release 0.2.1
+* fix SSH-o batchmode=yes
+* fix SSH checks for key:ok-host:no
+* fix SSH checks
+*  fix check config
+*  fix check config
+* Skip for unecessary run
+* Skip for unecessary run
+* Fix documentation
+* exclude no ssh available from Dsicovery (22 port)
+* exclude no ssh available from Dsicovery (22 port)
+* exclude BMC from Dsicovery (623 & 5900 port)
+* Fix ssh target completion and messages
+* Fix ssh target mode
+* Fix ssh target mode
+* Fix ssh target mode
+* Fix ssh target mode
+* Fix ssh ping check
+* Fix ssh ping check
+* Fix ssh exit check
+* Fix ssh output
+* Fix Library
+* Fix Library
+* Add SSH check
+* Fix talos-check config
+* Fix talos-check config
+* Fix talos-check config
+* Add talos-check config
+* Add talos-check config
+* Add talos-check
+* Fix follow
+* Fix talos-check config
+* Fix talos-check config
+* Fix talos-check config
+* Add talos-check config
+* Add talos-check config
+* Add talos-check
+* add config file check on update
+* add config file check on update
+* add compatible PB
 *  Add Update in talos\_install to update Env config
 *  add import role (install) and sync PB
 * Fix paths
 * Fix psw query after moving system
 * Fix psw query after moving system
 *  review wikiDB
 * Fix output option show
```

### Comparing `talos_install-0.2.0.dev368/PKG-INFO` & `talos_install-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talos_install
-Version: 0.2.0.dev368
+Version: 0.2.1
 Summary: E4 CLI Manager
 Home-page: https://www.e4company.com/
 Author: "Marco Cicala"
 Author-email: marco.cicala@e4company.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
@@ -105,14 +105,24 @@
 
 ```bash
 talos_install deploy
 ```
 
 A list of change will be shown for user approval. Use `-y` to confirm automatically.
 
+### Run update
+
+Generally speaking, the update process is done with `talos-config update`; if something goes wrong during backward compatibilty process (like an update from a very old build), should be necessary to run `talos_install update` (as install user) to fix environment. Be aware about unecessary `talos_install update` and always check configuration files first (talos.yaml and global.yaml in your HOME directory).
+
+```bash
+talos_install update
+```
+
+A list of change will be shown for user approval. Use `-y` to confirm automatically.
+
 ## Post installation
 
 Then need to validate configuration.
 First access as talos user:
 
 ```bash
 sudo su - talos
@@ -137,21 +147,27 @@
 ```bash
 talos-config init
 ```
 
 Check Key Pairs with Talos-cli (needed for update only)
 
 ```bash
-talos-config git_keys
+talos-check git_keys
+```
+
+Check System status
+
+```bash
+talos-check status
 ```
 
-Check Overall status
+Check Version status
 
 ```bash
-talos-config check
+talos-check version
 ```
 
 ## Known Issue
 
 ansible-core requires the locale have UTF-8 encoding since 2.14.0
 
 Excerpt from the 2.14.0 release notes1
```

### Comparing `talos_install-0.2.0.dev368/README.md` & `talos_install-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -87,14 +87,24 @@
 
 ```bash
 talos_install deploy
 ```
 
 A list of change will be shown for user approval. Use `-y` to confirm automatically.
 
+### Run update
+
+Generally speaking, the update process is done with `talos-config update`; if something goes wrong during backward compatibilty process (like an update from a very old build), should be necessary to run `talos_install update` (as install user) to fix environment. Be aware about unecessary `talos_install update` and always check configuration files first (talos.yaml and global.yaml in your HOME directory).
+
+```bash
+talos_install update
+```
+
+A list of change will be shown for user approval. Use `-y` to confirm automatically.
+
 ## Post installation
 
 Then need to validate configuration.
 First access as talos user:
 
 ```bash
 sudo su - talos
@@ -119,21 +129,27 @@
 ```bash
 talos-config init
 ```
 
 Check Key Pairs with Talos-cli (needed for update only)
 
 ```bash
-talos-config git_keys
+talos-check git_keys
+```
+
+Check System status
+
+```bash
+talos-check status
 ```
 
-Check Overall status
+Check Version status
 
 ```bash
-talos-config check
+talos-check version
 ```
 
 ## Known Issue
 
 ansible-core requires the locale have UTF-8 encoding since 2.14.0
 
 Excerpt from the 2.14.0 release notes1
```

### Comparing `talos_install-0.2.0.dev368/ansible/roles/cli/tasks/clone.yaml` & `talos_install-0.2.1/ansible/roles/cli/tasks/clone.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/cli/tasks/env.yaml` & `talos_install-0.2.1/ansible/roles/cli/tasks/env.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/cli/tasks/misc.yaml` & `talos_install-0.2.1/ansible/roles/cli/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/cli/tasks/web.yaml` & `talos_install-0.2.1/ansible/roles/cli/tasks/web.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/cli/templates/agent.sh.j2` & `talos_install-0.2.1/ansible/roles/cli/templates/agent.sh.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/cli/templates/cli.conf.j2` & `talos_install-0.2.1/ansible/roles/cli/templates/cli.conf.j2`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 app.name:              {{ app.name }}
 app.cli_version:       {{ app.cli_version }}
 app.cli_repo:          {{ app.cli_repo }}
-app.data_repo:         {{ app.data_repo }}
 app.dir:               {{ app.dir }}
 app.clidir:            {{ app.clidir }}
 app.datadir:           {{ app.datadir }}
 app.etcdir:            {{ app.etcdir }}
 app.webdir:            {{ app.webdir }}
 app.logdir:            {{ app.logdir }}
+app.nexus_repo:        {{ app.nexus_repo }}
 customer.name:         {{ customer.name }}
-customer.domain:         {{ customer.domain }}
-nexus_repository:      {{ app.nexus_repo }}
-data_repository:       {{ app.data_repo }}
-master.user:      {{ master.user }}
-master.uid:       {{ master.uid }}
-master.password:  {{ master.password }}
-master.mail:      {{ master.mail }}
+customer.domain:       {{ customer.domain }}
+master.user:           {{ master.user }}
+master.uid:            {{ master.uid }}
+master.password:       {{ master.password }}
+master.home:           {{ master.home }}
+master.mail:           {{ master.mail }}
 mgm_password:          {{ mgm_password }}
```

### Comparing `talos_install-0.2.0.dev368/ansible/roles/cli/templates/env_talos.j2` & `talos_install-0.2.1/ansible/roles/cli/templates/env_talos.j2`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 export ANSIBLE_PATH="$TALOS_ETC_PATH/ansible"
 export ANSIBLE_CONFIG="$TALOS_ETC_PATH/ansible/ansible.cfg"
 export ANSIBLE_INVENTORY="$ANSIBLE_PATH/inventory/hosts-cli"
 export ANSIBLE_PB_PATH="$ANSIBLE_PATH/playbook"
 
 # REPOS
 export NEXUS_REPOSITORY="{{ app.nexus_repo }}"
-export DATA_REPOSITORY="{{ app.data_repo }}"
 
 # DATA
 export GREEN='\033[0;32m'
 export BLUE='\033[0;34m'
 export RED='\033[1;31m'
 export REDBAND='\033[41;1;37m'
 export YELLOW='\033[0;33m'
```

### Comparing `talos_install-0.2.0.dev368/ansible/roles/cli/templates/globals.yaml.j2` & `talos_install-0.2.1/ansible/roles/cli/templates/globals.yaml.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/cli/templates/my-httpd.conf.j2` & `talos_install-0.2.1/ansible/roles/cli/templates/my-httpd.conf.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/cli/templates/talos.conf.j2` & `talos_install-0.2.1/ansible/roles/cli/templates/talos.conf.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/common/tasks/misc.yaml` & `talos_install-0.2.1/ansible/roles/common/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/gather_facts/vars/RedHat.yaml` & `talos_install-0.2.1/ansible/roles/gather_facts/vars/RedHat.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/gather_facts/vars/Rocky.yaml` & `talos_install-0.2.1/ansible/roles/gather_facts/vars/Rocky.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py` & `talos_install-0.2.1/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/install_ansible/tasks/main.yaml` & `talos_install-0.2.1/ansible/roles/install_ansible/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/install_ansible/templates/ansible.cfg.j2` & `talos_install-0.2.1/ansible/roles/install_ansible/templates/ansible.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/install_certificates/tasks/main.yaml` & `talos_install-0.2.1/ansible/roles/install_certificates/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/install_docker/tasks/main.yaml` & `talos_install-0.2.1/ansible/roles/install_docker/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/install_docker/templates/docker-ce.repo.j2` & `talos_install-0.2.1/ansible/roles/install_docker/templates/docker-ce.repo.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/install_python/tasks/main.yaml` & `talos_install-0.2.1/ansible/roles/install_python/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf` & `talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/nagios/run` & `talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/nagios/run`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/postfix/run` & `talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/postfix/run`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png` & `talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png` & `talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php` & `talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html` & `talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php` & `talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css` & `talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css` & `talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh` & `talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios` & `talos_install-0.2.1/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/nagios/tasks/build.yaml` & `talos_install-0.2.1/ansible/roles/nagios/tasks/build.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/nagios/tasks/misc.yaml` & `talos_install-0.2.1/ansible/roles/nagios/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/nagios/tasks/run.yaml` & `talos_install-0.2.1/ansible/roles/nagios/tasks/run.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/nagios/templates/Dockerfile.j2` & `talos_install-0.2.1/ansible/roles/nagios/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/nagios/templates/cgi.cfg.j2` & `talos_install-0.2.1/ansible/roles/nagios/templates/cgi.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/nagios/templates/contacts.cfg.j2` & `talos_install-0.2.1/ansible/roles/nagios/templates/contacts.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/nagios/templates/localhost.cfg.j2` & `talos_install-0.2.1/ansible/roles/nagios/templates/localhost.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/opendcim/files/apache2.conf` & `talos_install-0.2.1/ansible/roles/opendcim/files/apache2.conf`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/opendcim/files/default.sql` & `talos_install-0.2.1/ansible/roles/opendcim/files/default.sql`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png` & `talos_install-0.2.1/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png` & `talos_install-0.2.1/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php` & `talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css` & `talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png` & `talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php` & `talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/opendcim/files/pre-conf.sh` & `talos_install-0.2.1/ansible/roles/opendcim/files/pre-conf.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/opendcim/files/startup.sh` & `talos_install-0.2.1/ansible/roles/opendcim/files/startup.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/opendcim/tasks/build.yaml` & `talos_install-0.2.1/ansible/roles/opendcim/tasks/build.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/opendcim/tasks/misc.yaml` & `talos_install-0.2.1/ansible/roles/opendcim/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/opendcim/tasks/run.yaml` & `talos_install-0.2.1/ansible/roles/opendcim/tasks/run.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/opendcim/templates/Dockerfile.j2` & `talos_install-0.2.1/ansible/roles/opendcim/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/opendcim/templates/first-run.sh.j2` & `talos_install-0.2.1/ansible/roles/opendcim/templates/first-run.sh.j2`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/bin/bash
 
 sed -i "s@CUSTOMERNAME@{{ customer.name }}@g" /root/default.sql
 
 /etc/init.d/mysql start
-mysqladmin -u root password '{{ mgm_password }}'
-mysqladmin -u root -p'{{ mgm_password }}' reload
-mysqladmin -u root -p'{{ mgm_password }}' create dcim
-echo "CREATE USER 'dcim'@'localhost' IDENTIFIED BY 'dcim'; " | mysql -uroot -p'{{ mgm_password }}'
-echo "GRANT ALL ON dcim.* TO dcim@localhost IDENTIFIED BY 'dcim'; flush privileges; " | mysql -uroot -p'{{ mgm_password }}'
-echo "SET GLOBAL sql_mode = '';" | mysql -u root -p'{{ mgm_password }}'
-mysql -u root -p'{{ mgm_password }}' dcim < /root/default.sql
+mysqladmin -u root password '{{ opendcim.mysql_password }}'
+mysqladmin -u root -p'{{ opendcim.mysql_password }}' reload
+mysqladmin -u root -p'{{ opendcim.mysql_password }}' create dcim
+echo "CREATE USER 'dcim'@'localhost' IDENTIFIED BY 'dcim'; " | mysql -uroot -p'{{ opendcim.mysql_password }}'
+echo "GRANT ALL ON dcim.* TO dcim@localhost IDENTIFIED BY 'dcim'; flush privileges; " | mysql -uroot -p'{{ opendcim.mysql_password }}'
+echo "SET GLOBAL sql_mode = '';" | mysql -u root -p'{{ opendcim.mysql_password }}'
+mysql -u root -p'{{ opendcim.mysql_password }}' dcim < /root/default.sql
 rm -f /root/default.sql
```

### Comparing `talos_install-0.2.0.dev368/ansible/roles/os_tune/tasks/main.yaml` & `talos_install-0.2.1/ansible/roles/os_tune/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/talos_users/tasks/main.yaml` & `talos_install-0.2.1/ansible/roles/talos_users/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/uninstall/tasks/cli.yaml` & `talos_install-0.2.1/ansible/roles/uninstall/tasks/cli.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/wiki/defaults/main.yaml` & `talos_install-0.2.1/ansible/roles/wiki/defaults/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/wiki/tasks/compose.yaml` & `talos_install-0.2.1/ansible/roles/wiki/tasks/compose.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/roles/wiki/templates/docker-compose.yml.j2` & `talos_install-0.2.1/ansible/roles/wiki/templates/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/ansible/site.yaml` & `talos_install-0.2.1/ansible/site.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/etc/example_talos.yaml` & `talos_install-0.2.1/etc/example_talos.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/setup.cfg` & `talos_install-0.2.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = talos_install
-version = 0.2.0
+version = 0.2.1
 summary = E4 CLI Manager
 description_file = 
 	README.md
 author = "Marco Cicala"
 author_email = marco.cicala@e4company.com
 home_page = https://www.e4company.com/
 license = GNU General Public License v3 (GPLv3)
```

### Comparing `talos_install-0.2.0.dev368/talos_install` & `talos_install-0.2.1/talos_install`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev368/talos_install.egg-info/PKG-INFO` & `talos_install-0.2.1/talos_install.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talos-install
-Version: 0.2.0.dev368
+Version: 0.2.1
 Summary: E4 CLI Manager
 Home-page: https://www.e4company.com/
 Author: "Marco Cicala"
 Author-email: marco.cicala@e4company.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
@@ -105,14 +105,24 @@
 
 ```bash
 talos_install deploy
 ```
 
 A list of change will be shown for user approval. Use `-y` to confirm automatically.
 
+### Run update
+
+Generally speaking, the update process is done with `talos-config update`; if something goes wrong during backward compatibilty process (like an update from a very old build), should be necessary to run `talos_install update` (as install user) to fix environment. Be aware about unecessary `talos_install update` and always check configuration files first (talos.yaml and global.yaml in your HOME directory).
+
+```bash
+talos_install update
+```
+
+A list of change will be shown for user approval. Use `-y` to confirm automatically.
+
 ## Post installation
 
 Then need to validate configuration.
 First access as talos user:
 
 ```bash
 sudo su - talos
@@ -137,21 +147,27 @@
 ```bash
 talos-config init
 ```
 
 Check Key Pairs with Talos-cli (needed for update only)
 
 ```bash
-talos-config git_keys
+talos-check git_keys
+```
+
+Check System status
+
+```bash
+talos-check status
 ```
 
-Check Overall status
+Check Version status
 
 ```bash
-talos-config check
+talos-check version
 ```
 
 ## Known Issue
 
 ansible-core requires the locale have UTF-8 encoding since 2.14.0
 
 Excerpt from the 2.14.0 release notes1
```

### Comparing `talos_install-0.2.0.dev368/talos_install.egg-info/SOURCES.txt` & `talos_install-0.2.1/talos_install.egg-info/SOURCES.txt`

 * *Files identical despite different names*

