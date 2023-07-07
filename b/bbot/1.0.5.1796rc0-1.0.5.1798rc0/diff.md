# Comparing `tmp/bbot-1.0.5.1796rc0.tar.gz` & `tmp/bbot-1.0.5.1798rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbot-1.0.5.1796rc0.tar", max compression
+gzip compressed data, was "bbot-1.0.5.1798rc0.tar", max compression
```

## Comparing `bbot-1.0.5.1796rc0.tar` & `bbot-1.0.5.1798rc0.tar`

### file list

```diff
@@ -1,277 +1,277 @@
--rw-r--r--   0        0        0    32473 2023-07-04 16:56:57.081548 bbot-1.0.5.1796rc0/LICENSE
--rw-r--r--   0        0        0    51778 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/README.md
--rw-r--r--   0        0        0      211 2023-07-04 16:57:22.769815 bbot-1.0.5.1796rc0/bbot/__init__.py
--rw-r--r--   0        0        0       25 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/agent/__init__.py
--rw-r--r--   0        0        0     7527 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/agent/agent.py
--rw-r--r--   0        0        0      450 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/agent/messages.py
--rwxr-xr-x   0        0        0    14606 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/cli.py
--rw-r--r--   0        0        0       93 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/__init__.py
--rw-r--r--   0        0        0     3171 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/configurator/__init__.py
--rw-r--r--   0        0        0     8720 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/configurator/args.py
--rw-r--r--   0        0        0     5150 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/configurator/environ.py
--rw-r--r--   0        0        0     1170 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/configurator/files.py
--rw-r--r--   0        0        0      574 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/errors.py
--rw-r--r--   0        0        0      104 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/event/__init__.py
--rw-r--r--   0        0        0    31058 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/event/base.py
--rw-r--r--   0        0        0     1496 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/event/helpers.py
--rw-r--r--   0        0        0       61 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/helpers/__init__.py
--rw-r--r--   0        0        0     1993 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/helpers/async_helpers.py
--rw-r--r--   0        0        0     3475 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/helpers/cache.py
--rw-r--r--   0        0        0     1394 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/helpers/cloud/__init__.py
--rw-r--r--   0        0        0      565 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/helpers/cloud/aws.py
--rw-r--r--   0        0        0      716 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/helpers/cloud/azure.py
--rw-r--r--   0        0        0     4006 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/helpers/cloud/base.py
--rw-r--r--   0        0        0      297 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/helpers/cloud/digitalocean.py
--rw-r--r--   0        0        0      271 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/helpers/cloud/firebase.py
--rw-r--r--   0        0        0      352 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/helpers/cloud/gcp.py
--rw-r--r--   0        0        0     5022 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/helpers/command.py
--rw-r--r--   0        0        0       37 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/helpers/depsinstaller/__init__.py
--rw-r--r--   0        0        0    14159 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/helpers/depsinstaller/installer.py
--rw-r--r--   0        0        0       87 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
--rw-r--r--   0        0        0     9234 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/helpers/diff.py
--rw-r--r--   0        0        0    27284 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/helpers/dns.py
--rw-r--r--   0        0        0     3104 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/helpers/files.py
--rw-r--r--   0        0        0     4373 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/helpers/helper.py
--rw-r--r--   0        0        0     5687 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/helpers/interactsh.py
--rw-r--r--   0        0        0     1408 2023-07-04 16:56:57.085548 bbot-1.0.5.1796rc0/bbot/core/helpers/logger.py
--rw-r--r--   0        0        0    32311 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/core/helpers/misc.py
--rw-r--r--   0        0        0    14831 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/core/helpers/modules.py
--rw-r--r--   0        0        0     9603 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/core/helpers/names_generator.py
--rw-r--r--   0        0        0     2578 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/core/helpers/ntlm.py
--rw-r--r--   0        0        0      795 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/core/helpers/punycode.py
--rw-r--r--   0        0        0     1548 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/core/helpers/ratelimiter.py
--rw-r--r--   0        0        0     1929 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/core/helpers/regexes.py
--rw-r--r--   0        0        0     4153 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/core/helpers/url.py
--rw-r--r--   0        0        0     3192 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/core/helpers/validators.py
--rw-r--r--   0        0        0    13229 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/core/helpers/web.py
--rw-r--r--   0        0        0    11137 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/core/helpers/wordcloud.py
--rw-r--r--   0        0        0       99 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/core/logger/__init__.py
--rw-r--r--   0        0        0     8300 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/core/logger/logger.py
--rw-r--r--   0        0        0     2091 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/db/neo4j.py
--rw-r--r--   0        0        0     3786 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/defaults.yml
--rw-r--r--   0        0        0      396 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/__init__.py
--rw-r--r--   0        0        0     1395 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/anubisdb.py
--rw-r--r--   0        0        0     3491 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/azure_tenant.py
--rw-r--r--   0        0        0     2600 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/badsecrets.py
--rw-r--r--   0        0        0    25482 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/base.py
--rw-r--r--   0        0        0     2257 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/bevigil.py
--rw-r--r--   0        0        0     1263 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/binaryedge.py
--rw-r--r--   0        0        0     5461 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/bucket_aws.py
--rw-r--r--   0        0        0     1004 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/bucket_azure.py
--rw-r--r--   0        0        0      758 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/bucket_digitalocean.py
--rw-r--r--   0        0        0     1102 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/bucket_firebase.py
--rw-r--r--   0        0        0     2119 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/bucket_gcp.py
--rw-r--r--   0        0        0     4760 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/builtwith.py
--rw-r--r--   0        0        0     5125 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/bypass403.py
--rw-r--r--   0        0        0     1140 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/c99.py
--rw-r--r--   0        0        0     2636 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/censys.py
--rw-r--r--   0        0        0      764 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/certspotter.py
--rw-r--r--   0        0        0      680 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/columbus.py
--rw-r--r--   0        0        0     5520 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/crobat.py
--rw-r--r--   0        0        0     1184 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/crt.py
--rw-r--r--   0        0        0    13670 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/deadly/ffuf.py
--rw-r--r--   0        0        0    15857 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/deadly/nuclei.py
--rw-r--r--   0        0        0     5227 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/deadly/vhost.py
--rw-r--r--   0        0        0     2539 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/dnscommonsrv.py
--rw-r--r--   0        0        0     2929 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/dnsdumpster.py
--rw-r--r--   0        0        0     2976 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/dnszonetransfer.py
--rw-r--r--   0        0        0      743 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/emailformat.py
--rw-r--r--   0        0        0    11304 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/ffuf_shortnames.py
--rw-r--r--   0        0        0     2176 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/fingerprintx.py
--rw-r--r--   0        0        0     1159 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/fullhunt.py
--rw-r--r--   0        0        0     7776 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/generic_ssrf.py
--rw-r--r--   0        0        0     1307 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/git.py
--rw-r--r--   0        0        0     2939 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/github.py
--rw-r--r--   0        0        0    10065 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/gowitness.py
--rw-r--r--   0        0        0      807 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/hackertarget.py
--rw-r--r--   0        0        0     7437 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/host_header.py
--rw-r--r--   0        0        0     5749 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/httpx.py
--rw-r--r--   0        0        0     7754 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/hunt.py
--rw-r--r--   0        0        0     2032 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/hunterio.py
--rw-r--r--   0        0        0     9552 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/iis_shortnames.py
--rw-r--r--   0        0        0        0 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/internal/__init__.py
--rw-r--r--   0        0        0      304 2023-07-04 16:56:57.089548 bbot-1.0.5.1796rc0/bbot/modules/internal/aggregate.py
--rw-r--r--   0        0        0      578 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/internal/base.py
--rw-r--r--   0        0        0    16933 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/internal/excavate.py
--rw-r--r--   0        0        0     5124 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/internal/speculate.py
--rw-r--r--   0        0        0     1292 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/ipneighbor.py
--rw-r--r--   0        0        0     2128 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/ipstack.py
--rw-r--r--   0        0        0     1496 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/leakix.py
--rw-r--r--   0        0        0    11285 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/masscan.py
--rw-r--r--   0        0        0    15167 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/massdns.py
--rw-r--r--   0        0        0     4269 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/naabu.py
--rw-r--r--   0        0        0     5248 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/nmap.py
--rw-r--r--   0        0        0     4993 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/ntlm.py
--rw-r--r--   0        0        0      728 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/otx.py
--rw-r--r--   0        0        0        0 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/output/__init__.py
--rw-r--r--   0        0        0    11391 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/output/asset_inventory.py
--rw-r--r--   0        0        0     1623 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/output/base.py
--rw-r--r--   0        0        0     2579 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/output/csv.py
--rw-r--r--   0        0        0     1944 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/output/http.py
--rw-r--r--   0        0        0     1820 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/output/human.py
--rw-r--r--   0        0        0     1031 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/output/json.py
--rw-r--r--   0        0        0     1420 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/output/neo4j.py
--rw-r--r--   0        0        0      210 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/output/python.py
--rw-r--r--   0        0        0     3627 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/output/web_report.py
--rw-r--r--   0        0        0     2079 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/output/websocket.py
--rw-r--r--   0        0        0     1426 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/paramminer_cookies.py
--rw-r--r--   0        0        0     1493 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/paramminer_getparams.py
--rw-r--r--   0        0        0     5331 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/paramminer_headers.py
--rw-r--r--   0        0        0     1571 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/passivetotal.py
--rw-r--r--   0        0        0     1380 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/pgp.py
--rw-r--r--   0        0        0      786 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/rapiddns.py
--rw-r--r--   0        0        0     1602 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/report/affiliates.py
--rw-r--r--   0        0        0     8302 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/report/asn.py
--rw-r--r--   0        0        0      105 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/report/base.py
--rw-r--r--   0        0        0      782 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/riddler.py
--rw-r--r--   0        0        0     2273 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/robots.py
--rw-r--r--   0        0        0     2768 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/secretsdb.py
--rw-r--r--   0        0        0     1153 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/securitytrails.py
--rw-r--r--   0        0        0     1290 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/shodan_dns.py
--rw-r--r--   0        0        0     1466 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/skymem.py
--rw-r--r--   0        0        0     1744 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/smuggler.py
--rw-r--r--   0        0        0     1539 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/social.py
--rw-r--r--   0        0        0     7882 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/sslcert.py
--rw-r--r--   0        0        0     6110 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/subdomain_hijack.py
--rw-r--r--   0        0        0      507 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/sublist3r.py
--rw-r--r--   0        0        0    11359 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/telerik.py
--rw-r--r--   0        0        0      644 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/threatminer.py
--rw-r--r--   0        0        0     3843 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/url_manipulation.py
--rw-r--r--   0        0        0     2866 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/urlscan.py
--rw-r--r--   0        0        0     2554 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/viewdns.py
--rw-r--r--   0        0        0     1555 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/virustotal.py
--rw-r--r--   0        0        0     1711 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/wafw00f.py
--rw-r--r--   0        0        0     1245 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/wappalyzer.py
--rw-r--r--   0        0        0     2291 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/wayback.py
--rw-r--r--   0        0        0     2295 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/modules/zoomeye.py
--rw-r--r--   0        0        0       29 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/scanner/__init__.py
--rw-r--r--   0        0        0      793 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/scanner/dispatcher.py
--rw-r--r--   0        0        0    24694 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/scanner/manager.py
--rw-r--r--   0        0        0    27042 2023-07-04 16:56:57.093548 bbot-1.0.5.1796rc0/bbot/scanner/scanner.py
--rw-r--r--   0        0        0     3225 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/scanner/stats.py
--rw-r--r--   0        0        0     4044 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/scanner/target.py
--rw-r--r--   0        0        0        0 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/__init__.py
--rw-r--r--   0        0        0    10812 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/bbot_fixtures.py
--rw-r--r--   0        0        0     2668 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/conftest.py
--rwxr-xr-x   0        0        0      607 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/run_tests.sh
--rw-r--r--   0        0        0     1086 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test.conf
--rw-r--r--   0        0        0      322 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_output.json
--rw-r--r--   0        0        0        0 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_1/__init__.py
--rw-r--r--   0        0        0     1445 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_1/test__module__tests.py
--rw-r--r--   0        0        0     5153 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_agent.py
--rw-r--r--   0        0        0     6435 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_cli.py
--rw-r--r--   0        0        0      965 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_cloud_helpers.py
--rw-r--r--   0        0        0     4943 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_command.py
--rw-r--r--   0        0        0      495 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_config.py
--rw-r--r--   0        0        0      722 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_depsinstaller.py
--rw-r--r--   0        0        0     6082 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_dns.py
--rw-r--r--   0        0        0    15109 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_events.py
--rw-r--r--   0        0        0      702 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_files.py
--rw-r--r--   0        0        0    24751 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_helpers.py
--rw-r--r--   0        0        0     7959 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_manager.py
--rw-r--r--   0        0        0     7688 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_modules_basic.py
--rw-r--r--   0        0        0     1694 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_python_api.py
--rw-r--r--   0        0        0     2664 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_scan.py
--rw-r--r--   0        0        0      706 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_scope.py
--rw-r--r--   0        0        0     2148 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_target.py
--rw-r--r--   0        0        0     6570 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_web.py
--rw-r--r--   0        0        0        0 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/__init__.py
--rw-r--r--   0        0        0     4850 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/base.py
--rw-r--r--   0        0        0      346 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
--rw-r--r--   0        0        0      313 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
--rw-r--r--   0        0        0      546 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
--rw-r--r--   0        0        0    10606 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
--rw-r--r--   0        0        0     1886 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
--rw-r--r--   0        0        0     1949 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
--rw-r--r--   0        0        0     4779 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
--rw-r--r--   0        0        0     1045 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
--rw-r--r--   0        0        0     1101 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
--rw-r--r--   0        0        0     3882 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py
--rw-r--r--   0        0        0      546 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
--rw-r--r--   0        0        0      901 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
--rw-r--r--   0        0        0      502 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
--rw-r--r--   0        0        0     1088 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py
--rw-r--r--   0        0        0     5051 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
--rw-r--r--   0        0        0     2069 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
--rw-r--r--   0        0        0      982 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
--rw-r--r--   0        0        0     1770 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
--rw-r--r--   0        0        0      636 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
--rw-r--r--   0        0        0      555 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
--rw-r--r--   0        0        0      762 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
--rw-r--r--   0        0        0      717 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
--rw-r--r--   0        0        0      273 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
--rw-r--r--   0        0        0      972 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
--rw-r--r--   0        0        0    59749 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
--rw-r--r--   0        0        0     1794 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py
--rw-r--r--   0        0        0      461 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
--rw-r--r--   0        0        0     7339 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
--rw-r--r--   0        0        0     1964 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
--rw-r--r--   0        0        0     7669 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
--rw-r--r--   0        0        0      445 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
--rw-r--r--   0        0        0     1946 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
--rw-r--r--   0        0        0     2040 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
--rw-r--r--   0        0        0     1726 2023-07-04 16:56:57.097549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_git.py
--rw-r--r--   0        0        0     8204 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_github.py
--rw-r--r--   0        0        0     1752 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
--rw-r--r--   0        0        0      609 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
--rw-r--r--   0        0        0     2702 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
--rw-r--r--   0        0        0      706 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_http.py
--rw-r--r--   0        0        0     1572 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
--rw-r--r--   0        0        0      249 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_human.py
--rw-r--r--   0        0        0      665 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
--rw-r--r--   0        0        0     4086 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
--rw-r--r--   0        0        0     2600 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
--rw-r--r--   0        0        0     1297 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
--rw-r--r--   0        0        0     2900 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
--rw-r--r--   0        0        0      474 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_json.py
--rw-r--r--   0        0        0      987 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
--rw-r--r--   0        0        0     1945 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
--rw-r--r--   0        0        0      698 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
--rw-r--r--   0        0        0      419 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_naabu.py
--rw-r--r--   0        0        0      659 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
--rw-r--r--   0        0        0      337 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
--rw-r--r--   0        0        0     1116 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
--rw-r--r--   0        0        0     4708 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
--rw-r--r--   0        0        0     1160 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
--rw-r--r--   0        0        0     1614 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
--rw-r--r--   0        0        0     1596 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
--rw-r--r--   0        0        0     1673 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
--rw-r--r--   0        0        0      961 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
--rw-r--r--   0        0        0     1609 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
--rw-r--r--   0        0        0      184 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_python.py
--rw-r--r--   0        0        0      750 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
--rw-r--r--   0        0        0      747 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
--rw-r--r--   0        0        0     1564 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
--rw-r--r--   0        0        0      888 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
--rw-r--r--   0        0        0      758 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
--rw-r--r--   0        0        0      717 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
--rw-r--r--   0        0        0     2321 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
--rw-r--r--   0        0        0     2426 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
--rw-r--r--   0        0        0      588 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_social.py
--rw-r--r--   0        0        0     1004 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
--rw-r--r--   0        0        0      318 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
--rw-r--r--   0        0        0     1925 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py
--rw-r--r--   0        0        0      611 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
--rw-r--r--   0        0        0     5562 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
--rw-r--r--   0        0        0      489 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
--rw-r--r--   0        0        0     1144 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
--rw-r--r--   0        0        0     2902 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
--rw-r--r--   0        0        0     2874 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
--rw-r--r--   0        0        0    15239 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
--rw-r--r--   0        0        0     3401 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
--rw-r--r--   0        0        0      563 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
--rw-r--r--   0        0        0      936 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
--rw-r--r--   0        0        0      548 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
--rw-r--r--   0        0        0     2370 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
--rw-r--r--   0        0        0     1009 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
--rw-r--r--   0        0        0     1984 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
--rw-r--r--   0        0        0     1948 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/testsslcert.pem
--rw-r--r--   0        0        0     3268 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/test/testsslkey.pem
--rw-r--r--   0        0        0      476 2023-07-04 16:56:57.101549 bbot-1.0.5.1796rc0/bbot/wordlists/devops_mutations.txt
--rw-r--r--   0        0        0   959424 2023-07-04 16:56:57.109549 bbot-1.0.5.1796rc0/bbot/wordlists/ffuf_shortname_candidates.txt
--rw-r--r--   0        0        0    32226 2023-07-04 16:56:57.109549 bbot-1.0.5.1796rc0/bbot/wordlists/nameservers.txt
--rw-r--r--   0        0        0     6068 2023-07-04 16:56:57.109549 bbot-1.0.5.1796rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
--rw-r--r--   0        0        0   570241 2023-07-04 16:56:57.109549 bbot-1.0.5.1796rc0/bbot/wordlists/wordninja_dns.txt.gz
--rw-r--r--   0        0        0     1537 2023-07-04 16:57:22.769815 bbot-1.0.5.1796rc0/pyproject.toml
--rw-r--r--   0        0        0    53180 1970-01-01 00:00:00.000000 bbot-1.0.5.1796rc0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/LICENSE
+-rw-r--r--   0        0        0    51778 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/README.md
+-rw-r--r--   0        0        0      211 2023-07-07 14:08:15.024347 bbot-1.0.5.1798rc0/bbot/__init__.py
+-rw-r--r--   0        0        0       25 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/agent/__init__.py
+-rw-r--r--   0        0        0     7527 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/agent/agent.py
+-rw-r--r--   0        0        0      450 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/agent/messages.py
+-rwxr-xr-x   0        0        0    14606 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/cli.py
+-rw-r--r--   0        0        0       93 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/__init__.py
+-rw-r--r--   0        0        0     3171 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/configurator/__init__.py
+-rw-r--r--   0        0        0     8720 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/configurator/args.py
+-rw-r--r--   0        0        0     5150 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/configurator/environ.py
+-rw-r--r--   0        0        0     1170 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/configurator/files.py
+-rw-r--r--   0        0        0      574 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/errors.py
+-rw-r--r--   0        0        0      104 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/event/__init__.py
+-rw-r--r--   0        0        0    31058 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/event/base.py
+-rw-r--r--   0        0        0     1496 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/event/helpers.py
+-rw-r--r--   0        0        0       61 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/helpers/__init__.py
+-rw-r--r--   0        0        0     1993 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/helpers/async_helpers.py
+-rw-r--r--   0        0        0     3475 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/helpers/cache.py
+-rw-r--r--   0        0        0     1394 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/helpers/cloud/__init__.py
+-rw-r--r--   0        0        0      565 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/helpers/cloud/aws.py
+-rw-r--r--   0        0        0      716 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/helpers/cloud/azure.py
+-rw-r--r--   0        0        0     4006 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/helpers/cloud/base.py
+-rw-r--r--   0        0        0      297 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/helpers/cloud/digitalocean.py
+-rw-r--r--   0        0        0      271 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/helpers/cloud/firebase.py
+-rw-r--r--   0        0        0      352 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/helpers/cloud/gcp.py
+-rw-r--r--   0        0        0     5022 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/helpers/command.py
+-rw-r--r--   0        0        0       37 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/helpers/depsinstaller/__init__.py
+-rw-r--r--   0        0        0    14159 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/helpers/depsinstaller/installer.py
+-rw-r--r--   0        0        0       87 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
+-rw-r--r--   0        0        0     9234 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/helpers/diff.py
+-rw-r--r--   0        0        0    27284 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/helpers/dns.py
+-rw-r--r--   0        0        0     3104 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/helpers/files.py
+-rw-r--r--   0        0        0     4373 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/helpers/helper.py
+-rw-r--r--   0        0        0     5687 2023-07-07 14:07:38.156145 bbot-1.0.5.1798rc0/bbot/core/helpers/interactsh.py
+-rw-r--r--   0        0        0     1408 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/core/helpers/logger.py
+-rw-r--r--   0        0        0    32311 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/core/helpers/misc.py
+-rw-r--r--   0        0        0    14831 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/core/helpers/modules.py
+-rw-r--r--   0        0        0     9603 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/core/helpers/names_generator.py
+-rw-r--r--   0        0        0     2578 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/core/helpers/ntlm.py
+-rw-r--r--   0        0        0      795 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/core/helpers/punycode.py
+-rw-r--r--   0        0        0     1548 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/core/helpers/ratelimiter.py
+-rw-r--r--   0        0        0     1929 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/core/helpers/regexes.py
+-rw-r--r--   0        0        0     4153 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/core/helpers/url.py
+-rw-r--r--   0        0        0     3192 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/core/helpers/validators.py
+-rw-r--r--   0        0        0    13229 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/core/helpers/web.py
+-rw-r--r--   0        0        0    11137 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/core/helpers/wordcloud.py
+-rw-r--r--   0        0        0       99 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/core/logger/__init__.py
+-rw-r--r--   0        0        0     8300 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/core/logger/logger.py
+-rw-r--r--   0        0        0     2091 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/db/neo4j.py
+-rw-r--r--   0        0        0     3786 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/defaults.yml
+-rw-r--r--   0        0        0      396 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/__init__.py
+-rw-r--r--   0        0        0     1395 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/anubisdb.py
+-rw-r--r--   0        0        0     3491 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/azure_tenant.py
+-rw-r--r--   0        0        0     2600 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/badsecrets.py
+-rw-r--r--   0        0        0    25482 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/base.py
+-rw-r--r--   0        0        0     2257 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/bevigil.py
+-rw-r--r--   0        0        0     1263 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/binaryedge.py
+-rw-r--r--   0        0        0     5461 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/bucket_aws.py
+-rw-r--r--   0        0        0     1004 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/bucket_azure.py
+-rw-r--r--   0        0        0      758 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/bucket_digitalocean.py
+-rw-r--r--   0        0        0     1102 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/bucket_firebase.py
+-rw-r--r--   0        0        0     2119 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/bucket_gcp.py
+-rw-r--r--   0        0        0     4760 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/builtwith.py
+-rw-r--r--   0        0        0     5125 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/bypass403.py
+-rw-r--r--   0        0        0     1140 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/c99.py
+-rw-r--r--   0        0        0     2636 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/censys.py
+-rw-r--r--   0        0        0      764 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/certspotter.py
+-rw-r--r--   0        0        0      680 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/columbus.py
+-rw-r--r--   0        0        0     5520 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/crobat.py
+-rw-r--r--   0        0        0     1184 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/crt.py
+-rw-r--r--   0        0        0    13670 2023-07-07 14:07:38.160145 bbot-1.0.5.1798rc0/bbot/modules/deadly/ffuf.py
+-rw-r--r--   0        0        0    15857 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/deadly/nuclei.py
+-rw-r--r--   0        0        0     5227 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/deadly/vhost.py
+-rw-r--r--   0        0        0     2539 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/dnscommonsrv.py
+-rw-r--r--   0        0        0     2929 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/dnsdumpster.py
+-rw-r--r--   0        0        0     2976 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/dnszonetransfer.py
+-rw-r--r--   0        0        0      743 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/emailformat.py
+-rw-r--r--   0        0        0    11304 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/ffuf_shortnames.py
+-rw-r--r--   0        0        0     2176 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/fingerprintx.py
+-rw-r--r--   0        0        0     1159 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/fullhunt.py
+-rw-r--r--   0        0        0     7776 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/generic_ssrf.py
+-rw-r--r--   0        0        0     1307 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/git.py
+-rw-r--r--   0        0        0     2939 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/github.py
+-rw-r--r--   0        0        0    10065 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/gowitness.py
+-rw-r--r--   0        0        0      807 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/hackertarget.py
+-rw-r--r--   0        0        0     7437 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/host_header.py
+-rw-r--r--   0        0        0     5749 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/httpx.py
+-rw-r--r--   0        0        0     7754 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/hunt.py
+-rw-r--r--   0        0        0     2032 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/hunterio.py
+-rw-r--r--   0        0        0     9552 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/iis_shortnames.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/internal/__init__.py
+-rw-r--r--   0        0        0      304 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/internal/aggregate.py
+-rw-r--r--   0        0        0      578 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/internal/base.py
+-rw-r--r--   0        0        0    16933 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/internal/excavate.py
+-rw-r--r--   0        0        0     5124 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/internal/speculate.py
+-rw-r--r--   0        0        0     1292 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/ipneighbor.py
+-rw-r--r--   0        0        0     2128 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/ipstack.py
+-rw-r--r--   0        0        0     1496 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/leakix.py
+-rw-r--r--   0        0        0    11285 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/masscan.py
+-rw-r--r--   0        0        0    15167 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/massdns.py
+-rw-r--r--   0        0        0     4269 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/naabu.py
+-rw-r--r--   0        0        0     5248 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/nmap.py
+-rw-r--r--   0        0        0     4993 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/ntlm.py
+-rw-r--r--   0        0        0      728 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/otx.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/output/__init__.py
+-rw-r--r--   0        0        0    11391 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/output/asset_inventory.py
+-rw-r--r--   0        0        0     1623 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/output/base.py
+-rw-r--r--   0        0        0     2579 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/output/csv.py
+-rw-r--r--   0        0        0     1944 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/output/http.py
+-rw-r--r--   0        0        0     1820 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/output/human.py
+-rw-r--r--   0        0        0     1031 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/output/json.py
+-rw-r--r--   0        0        0     1420 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/output/neo4j.py
+-rw-r--r--   0        0        0      210 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/output/python.py
+-rw-r--r--   0        0        0     3627 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/output/web_report.py
+-rw-r--r--   0        0        0     2079 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/output/websocket.py
+-rw-r--r--   0        0        0     1426 2023-07-07 14:07:38.164145 bbot-1.0.5.1798rc0/bbot/modules/paramminer_cookies.py
+-rw-r--r--   0        0        0     1493 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/paramminer_getparams.py
+-rw-r--r--   0        0        0     5331 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/paramminer_headers.py
+-rw-r--r--   0        0        0     1571 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/passivetotal.py
+-rw-r--r--   0        0        0     1380 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/pgp.py
+-rw-r--r--   0        0        0      786 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/rapiddns.py
+-rw-r--r--   0        0        0     1602 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/report/affiliates.py
+-rw-r--r--   0        0        0     8302 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/report/asn.py
+-rw-r--r--   0        0        0      105 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/report/base.py
+-rw-r--r--   0        0        0      782 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/riddler.py
+-rw-r--r--   0        0        0     2273 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/robots.py
+-rw-r--r--   0        0        0     2768 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/secretsdb.py
+-rw-r--r--   0        0        0     1153 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/securitytrails.py
+-rw-r--r--   0        0        0     1290 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/shodan_dns.py
+-rw-r--r--   0        0        0     1466 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/skymem.py
+-rw-r--r--   0        0        0     1744 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/smuggler.py
+-rw-r--r--   0        0        0     1539 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/social.py
+-rw-r--r--   0        0        0     7882 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/sslcert.py
+-rw-r--r--   0        0        0     6110 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/subdomain_hijack.py
+-rw-r--r--   0        0        0      507 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/sublist3r.py
+-rw-r--r--   0        0        0    11359 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/telerik.py
+-rw-r--r--   0        0        0      644 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/threatminer.py
+-rw-r--r--   0        0        0     3843 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/url_manipulation.py
+-rw-r--r--   0        0        0     2866 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/urlscan.py
+-rw-r--r--   0        0        0     2554 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/viewdns.py
+-rw-r--r--   0        0        0     1555 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/virustotal.py
+-rw-r--r--   0        0        0     1711 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/wafw00f.py
+-rw-r--r--   0        0        0     1245 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/wappalyzer.py
+-rw-r--r--   0        0        0     2291 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/wayback.py
+-rw-r--r--   0        0        0     2295 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/modules/zoomeye.py
+-rw-r--r--   0        0        0       29 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/scanner/__init__.py
+-rw-r--r--   0        0        0      793 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/scanner/dispatcher.py
+-rw-r--r--   0        0        0    24694 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/scanner/manager.py
+-rw-r--r--   0        0        0    27042 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/scanner/scanner.py
+-rw-r--r--   0        0        0     3225 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/scanner/stats.py
+-rw-r--r--   0        0        0     4044 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/scanner/target.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/test/__init__.py
+-rw-r--r--   0        0        0    10812 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/test/bbot_fixtures.py
+-rw-r--r--   0        0        0     2668 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/test/conftest.py
+-rwxr-xr-x   0        0        0      607 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/test/run_tests.sh
+-rw-r--r--   0        0        0     1086 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/test/test.conf
+-rw-r--r--   0        0        0      322 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/test/test_output.json
+-rw-r--r--   0        0        0        0 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/test/test_step_1/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/test/test_step_1/test__module__tests.py
+-rw-r--r--   0        0        0     5153 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_agent.py
+-rw-r--r--   0        0        0     6435 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_cli.py
+-rw-r--r--   0        0        0      965 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_cloud_helpers.py
+-rw-r--r--   0        0        0     4943 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_command.py
+-rw-r--r--   0        0        0      495 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_config.py
+-rw-r--r--   0        0        0      722 2023-07-07 14:07:38.168145 bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_depsinstaller.py
+-rw-r--r--   0        0        0     6082 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_dns.py
+-rw-r--r--   0        0        0    15109 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_events.py
+-rw-r--r--   0        0        0      702 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_files.py
+-rw-r--r--   0        0        0    24751 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_helpers.py
+-rw-r--r--   0        0        0     7959 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_manager.py
+-rw-r--r--   0        0        0     7688 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_modules_basic.py
+-rw-r--r--   0        0        0     1694 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_python_api.py
+-rw-r--r--   0        0        0     2664 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_scan.py
+-rw-r--r--   0        0        0      706 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_scope.py
+-rw-r--r--   0        0        0     2148 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_target.py
+-rw-r--r--   0        0        0     6867 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_web.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/__init__.py
+-rw-r--r--   0        0        0     4850 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/base.py
+-rw-r--r--   0        0        0      346 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
+-rw-r--r--   0        0        0      313 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
+-rw-r--r--   0        0        0      546 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
+-rw-r--r--   0        0        0    10606 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
+-rw-r--r--   0        0        0     1886 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
+-rw-r--r--   0        0        0     1949 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
+-rw-r--r--   0        0        0     4779 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
+-rw-r--r--   0        0        0     1045 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
+-rw-r--r--   0        0        0     1101 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
+-rw-r--r--   0        0        0     3882 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py
+-rw-r--r--   0        0        0      546 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
+-rw-r--r--   0        0        0      901 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
+-rw-r--r--   0        0        0      502 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
+-rw-r--r--   0        0        0     1088 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py
+-rw-r--r--   0        0        0     5051 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
+-rw-r--r--   0        0        0     2069 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
+-rw-r--r--   0        0        0      982 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
+-rw-r--r--   0        0        0     1770 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
+-rw-r--r--   0        0        0      636 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
+-rw-r--r--   0        0        0      555 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
+-rw-r--r--   0        0        0      762 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
+-rw-r--r--   0        0        0      717 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
+-rw-r--r--   0        0        0      273 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
+-rw-r--r--   0        0        0      972 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
+-rw-r--r--   0        0        0    59749 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
+-rw-r--r--   0        0        0     1794 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py
+-rw-r--r--   0        0        0      461 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
+-rw-r--r--   0        0        0     7339 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
+-rw-r--r--   0        0        0     1964 2023-07-07 14:07:38.172145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
+-rw-r--r--   0        0        0     7669 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
+-rw-r--r--   0        0        0      445 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
+-rw-r--r--   0        0        0     1946 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
+-rw-r--r--   0        0        0     2040 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
+-rw-r--r--   0        0        0     1726 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_git.py
+-rw-r--r--   0        0        0     8204 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_github.py
+-rw-r--r--   0        0        0     1752 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
+-rw-r--r--   0        0        0      609 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
+-rw-r--r--   0        0        0     2702 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
+-rw-r--r--   0        0        0      706 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_http.py
+-rw-r--r--   0        0        0     1572 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
+-rw-r--r--   0        0        0      249 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_human.py
+-rw-r--r--   0        0        0      665 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
+-rw-r--r--   0        0        0     4086 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
+-rw-r--r--   0        0        0     2600 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
+-rw-r--r--   0        0        0     1297 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
+-rw-r--r--   0        0        0     2900 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
+-rw-r--r--   0        0        0      474 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_json.py
+-rw-r--r--   0        0        0      987 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
+-rw-r--r--   0        0        0     1945 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
+-rw-r--r--   0        0        0      698 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
+-rw-r--r--   0        0        0      419 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_naabu.py
+-rw-r--r--   0        0        0      659 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
+-rw-r--r--   0        0        0      337 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
+-rw-r--r--   0        0        0     1116 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
+-rw-r--r--   0        0        0     4708 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
+-rw-r--r--   0        0        0     1160 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
+-rw-r--r--   0        0        0     1614 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
+-rw-r--r--   0        0        0     1596 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
+-rw-r--r--   0        0        0     1673 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
+-rw-r--r--   0        0        0      961 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
+-rw-r--r--   0        0        0     1609 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
+-rw-r--r--   0        0        0      184 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_python.py
+-rw-r--r--   0        0        0      750 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
+-rw-r--r--   0        0        0      747 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
+-rw-r--r--   0        0        0     1564 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
+-rw-r--r--   0        0        0      888 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
+-rw-r--r--   0        0        0      758 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
+-rw-r--r--   0        0        0      717 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
+-rw-r--r--   0        0        0     2321 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
+-rw-r--r--   0        0        0     2426 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
+-rw-r--r--   0        0        0      588 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_social.py
+-rw-r--r--   0        0        0     1004 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
+-rw-r--r--   0        0        0      318 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
+-rw-r--r--   0        0        0     1925 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py
+-rw-r--r--   0        0        0      611 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
+-rw-r--r--   0        0        0     5562 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
+-rw-r--r--   0        0        0      489 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
+-rw-r--r--   0        0        0     1144 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
+-rw-r--r--   0        0        0     2902 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
+-rw-r--r--   0        0        0     2874 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
+-rw-r--r--   0        0        0    15239 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
+-rw-r--r--   0        0        0     3401 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
+-rw-r--r--   0        0        0      563 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
+-rw-r--r--   0        0        0      936 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
+-rw-r--r--   0        0        0      548 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
+-rw-r--r--   0        0        0     2370 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
+-rw-r--r--   0        0        0     1009 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
+-rw-r--r--   0        0        0     1984 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
+-rw-r--r--   0        0        0     1948 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/testsslcert.pem
+-rw-r--r--   0        0        0     3268 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/test/testsslkey.pem
+-rw-r--r--   0        0        0      476 2023-07-07 14:07:38.176145 bbot-1.0.5.1798rc0/bbot/wordlists/devops_mutations.txt
+-rw-r--r--   0        0        0   959424 2023-07-07 14:07:38.184145 bbot-1.0.5.1798rc0/bbot/wordlists/ffuf_shortname_candidates.txt
+-rw-r--r--   0        0        0    32226 2023-07-07 14:07:38.184145 bbot-1.0.5.1798rc0/bbot/wordlists/nameservers.txt
+-rw-r--r--   0        0        0     6068 2023-07-07 14:07:38.184145 bbot-1.0.5.1798rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
+-rw-r--r--   0        0        0   570241 2023-07-07 14:07:38.184145 bbot-1.0.5.1798rc0/bbot/wordlists/wordninja_dns.txt.gz
+-rw-r--r--   0        0        0     1537 2023-07-07 14:08:15.020347 bbot-1.0.5.1798rc0/pyproject.toml
+-rw-r--r--   0        0        0    53180 1970-01-01 00:00:00.000000 bbot-1.0.5.1798rc0/PKG-INFO
```

### Comparing `bbot-1.0.5.1796rc0/LICENSE` & `bbot-1.0.5.1798rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/README.md` & `bbot-1.0.5.1798rc0/README.md`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/agent/agent.py` & `bbot-1.0.5.1798rc0/bbot/agent/agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/cli.py` & `bbot-1.0.5.1798rc0/bbot/cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/configurator/__init__.py` & `bbot-1.0.5.1798rc0/bbot/core/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/configurator/args.py` & `bbot-1.0.5.1798rc0/bbot/core/configurator/args.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/configurator/environ.py` & `bbot-1.0.5.1798rc0/bbot/core/configurator/environ.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/configurator/files.py` & `bbot-1.0.5.1798rc0/bbot/core/configurator/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/errors.py` & `bbot-1.0.5.1798rc0/bbot/core/errors.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/event/base.py` & `bbot-1.0.5.1798rc0/bbot/core/event/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/event/helpers.py` & `bbot-1.0.5.1798rc0/bbot/core/event/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/async_helpers.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/async_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/cache.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/cloud/__init__.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/cloud/aws.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/cloud/azure.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/cloud/base.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/cloud/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/command.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/depsinstaller/installer.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/depsinstaller/installer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/diff.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/dns.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/files.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/helper.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/interactsh.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/interactsh.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/logger.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/misc.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/modules.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/modules.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/names_generator.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/names_generator.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/ntlm.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/punycode.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/punycode.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/ratelimiter.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/regexes.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/url.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/url.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/validators.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/web.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         """
         Downloads file, returns full path of filename
         If download failed, returns None
 
         Caching supported via "cache_hrs"
         """
         success = False
-        filename = kwargs.get("filename", self.parent_helper.cache_filename(url))
+        filename = kwargs.pop("filename", self.parent_helper.cache_filename(url))
         cache_hrs = float(kwargs.pop("cache_hrs", -1))
         log.debug(f"Downloading file from {url} with cache_hrs={cache_hrs}")
         if cache_hrs > 0 and self.parent_helper.is_cached(url):
             log.debug(f"{url} is cached at {self.parent_helper.cache_filename(url)}")
             success = True
         else:
             # kwargs["raise_error"] = True
```

### Comparing `bbot-1.0.5.1796rc0/bbot/core/helpers/wordcloud.py` & `bbot-1.0.5.1798rc0/bbot/core/helpers/wordcloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/core/logger/logger.py` & `bbot-1.0.5.1798rc0/bbot/core/logger/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/db/neo4j.py` & `bbot-1.0.5.1798rc0/bbot/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/defaults.yml` & `bbot-1.0.5.1798rc0/bbot/defaults.yml`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/anubisdb.py` & `bbot-1.0.5.1798rc0/bbot/modules/anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/azure_tenant.py` & `bbot-1.0.5.1798rc0/bbot/modules/azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/badsecrets.py` & `bbot-1.0.5.1798rc0/bbot/modules/badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/base.py` & `bbot-1.0.5.1798rc0/bbot/modules/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/bevigil.py` & `bbot-1.0.5.1798rc0/bbot/modules/bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/binaryedge.py` & `bbot-1.0.5.1798rc0/bbot/modules/binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/bucket_aws.py` & `bbot-1.0.5.1798rc0/bbot/modules/bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/bucket_azure.py` & `bbot-1.0.5.1798rc0/bbot/modules/bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/bucket_digitalocean.py` & `bbot-1.0.5.1798rc0/bbot/modules/bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/bucket_firebase.py` & `bbot-1.0.5.1798rc0/bbot/modules/bucket_firebase.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/bucket_gcp.py` & `bbot-1.0.5.1798rc0/bbot/modules/bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/builtwith.py` & `bbot-1.0.5.1798rc0/bbot/modules/builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/bypass403.py` & `bbot-1.0.5.1798rc0/bbot/modules/bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/c99.py` & `bbot-1.0.5.1798rc0/bbot/modules/c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/censys.py` & `bbot-1.0.5.1798rc0/bbot/modules/censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/certspotter.py` & `bbot-1.0.5.1798rc0/bbot/modules/certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/columbus.py` & `bbot-1.0.5.1798rc0/bbot/modules/columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/crobat.py` & `bbot-1.0.5.1798rc0/bbot/modules/crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/crt.py` & `bbot-1.0.5.1798rc0/bbot/modules/crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/deadly/ffuf.py` & `bbot-1.0.5.1798rc0/bbot/modules/deadly/ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/deadly/nuclei.py` & `bbot-1.0.5.1798rc0/bbot/modules/deadly/nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/deadly/vhost.py` & `bbot-1.0.5.1798rc0/bbot/modules/deadly/vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/dnscommonsrv.py` & `bbot-1.0.5.1798rc0/bbot/modules/dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/dnsdumpster.py` & `bbot-1.0.5.1798rc0/bbot/modules/dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/dnszonetransfer.py` & `bbot-1.0.5.1798rc0/bbot/modules/dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/emailformat.py` & `bbot-1.0.5.1798rc0/bbot/modules/emailformat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/ffuf_shortnames.py` & `bbot-1.0.5.1798rc0/bbot/modules/ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/fingerprintx.py` & `bbot-1.0.5.1798rc0/bbot/modules/fingerprintx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/fullhunt.py` & `bbot-1.0.5.1798rc0/bbot/modules/fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/generic_ssrf.py` & `bbot-1.0.5.1798rc0/bbot/modules/generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/git.py` & `bbot-1.0.5.1798rc0/bbot/modules/git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/github.py` & `bbot-1.0.5.1798rc0/bbot/modules/github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/gowitness.py` & `bbot-1.0.5.1798rc0/bbot/modules/gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/hackertarget.py` & `bbot-1.0.5.1798rc0/bbot/modules/hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/host_header.py` & `bbot-1.0.5.1798rc0/bbot/modules/host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/httpx.py` & `bbot-1.0.5.1798rc0/bbot/modules/httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/hunt.py` & `bbot-1.0.5.1798rc0/bbot/modules/hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/hunterio.py` & `bbot-1.0.5.1798rc0/bbot/modules/hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/iis_shortnames.py` & `bbot-1.0.5.1798rc0/bbot/modules/iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/internal/base.py` & `bbot-1.0.5.1798rc0/bbot/modules/internal/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/internal/excavate.py` & `bbot-1.0.5.1798rc0/bbot/modules/internal/excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/internal/speculate.py` & `bbot-1.0.5.1798rc0/bbot/modules/internal/speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/ipneighbor.py` & `bbot-1.0.5.1798rc0/bbot/modules/ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/ipstack.py` & `bbot-1.0.5.1798rc0/bbot/modules/ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/leakix.py` & `bbot-1.0.5.1798rc0/bbot/modules/leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/masscan.py` & `bbot-1.0.5.1798rc0/bbot/modules/masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/massdns.py` & `bbot-1.0.5.1798rc0/bbot/modules/massdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/naabu.py` & `bbot-1.0.5.1798rc0/bbot/modules/naabu.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/nmap.py` & `bbot-1.0.5.1798rc0/bbot/modules/nmap.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/ntlm.py` & `bbot-1.0.5.1798rc0/bbot/modules/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/otx.py` & `bbot-1.0.5.1798rc0/bbot/modules/otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/output/asset_inventory.py` & `bbot-1.0.5.1798rc0/bbot/modules/output/asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/output/base.py` & `bbot-1.0.5.1798rc0/bbot/modules/output/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/output/csv.py` & `bbot-1.0.5.1798rc0/bbot/modules/output/csv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/output/http.py` & `bbot-1.0.5.1798rc0/bbot/modules/output/http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/output/human.py` & `bbot-1.0.5.1798rc0/bbot/modules/output/human.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/output/json.py` & `bbot-1.0.5.1798rc0/bbot/modules/output/json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/output/neo4j.py` & `bbot-1.0.5.1798rc0/bbot/modules/output/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/output/web_report.py` & `bbot-1.0.5.1798rc0/bbot/modules/output/web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/output/websocket.py` & `bbot-1.0.5.1798rc0/bbot/modules/output/websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/paramminer_cookies.py` & `bbot-1.0.5.1798rc0/bbot/modules/paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/paramminer_getparams.py` & `bbot-1.0.5.1798rc0/bbot/modules/paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/paramminer_headers.py` & `bbot-1.0.5.1798rc0/bbot/modules/paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/passivetotal.py` & `bbot-1.0.5.1798rc0/bbot/modules/passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/pgp.py` & `bbot-1.0.5.1798rc0/bbot/modules/pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/rapiddns.py` & `bbot-1.0.5.1798rc0/bbot/modules/rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/report/affiliates.py` & `bbot-1.0.5.1798rc0/bbot/modules/report/affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/report/asn.py` & `bbot-1.0.5.1798rc0/bbot/modules/report/asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/riddler.py` & `bbot-1.0.5.1798rc0/bbot/modules/riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/robots.py` & `bbot-1.0.5.1798rc0/bbot/modules/robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/secretsdb.py` & `bbot-1.0.5.1798rc0/bbot/modules/secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/securitytrails.py` & `bbot-1.0.5.1798rc0/bbot/modules/securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/shodan_dns.py` & `bbot-1.0.5.1798rc0/bbot/modules/shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/skymem.py` & `bbot-1.0.5.1798rc0/bbot/modules/skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/smuggler.py` & `bbot-1.0.5.1798rc0/bbot/modules/smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/social.py` & `bbot-1.0.5.1798rc0/bbot/modules/social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/sslcert.py` & `bbot-1.0.5.1798rc0/bbot/modules/sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/subdomain_hijack.py` & `bbot-1.0.5.1798rc0/bbot/modules/subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/telerik.py` & `bbot-1.0.5.1798rc0/bbot/modules/telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/threatminer.py` & `bbot-1.0.5.1798rc0/bbot/modules/threatminer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/url_manipulation.py` & `bbot-1.0.5.1798rc0/bbot/modules/url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/urlscan.py` & `bbot-1.0.5.1798rc0/bbot/modules/urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/viewdns.py` & `bbot-1.0.5.1798rc0/bbot/modules/viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/virustotal.py` & `bbot-1.0.5.1798rc0/bbot/modules/virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/wafw00f.py` & `bbot-1.0.5.1798rc0/bbot/modules/wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/wappalyzer.py` & `bbot-1.0.5.1798rc0/bbot/modules/wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/wayback.py` & `bbot-1.0.5.1798rc0/bbot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/modules/zoomeye.py` & `bbot-1.0.5.1798rc0/bbot/modules/zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/scanner/dispatcher.py` & `bbot-1.0.5.1798rc0/bbot/scanner/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/scanner/manager.py` & `bbot-1.0.5.1798rc0/bbot/scanner/manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/scanner/scanner.py` & `bbot-1.0.5.1798rc0/bbot/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/scanner/stats.py` & `bbot-1.0.5.1798rc0/bbot/scanner/stats.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/scanner/target.py` & `bbot-1.0.5.1798rc0/bbot/scanner/target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/bbot_fixtures.py` & `bbot-1.0.5.1798rc0/bbot/test/bbot_fixtures.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/conftest.py` & `bbot-1.0.5.1798rc0/bbot/test/conftest.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/run_tests.sh` & `bbot-1.0.5.1798rc0/bbot/test/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test.conf` & `bbot-1.0.5.1798rc0/bbot/test/test.conf`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_1/test__module__tests.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_1/test__module__tests.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_agent.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_cli.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_cloud_helpers.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_command.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_depsinstaller.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_depsinstaller.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_dns.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_events.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_events.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_files.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_helpers.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_manager.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_modules_basic.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_modules_basic.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_python_api.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_python_api.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_scan.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_scan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_scope.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_scope.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_target.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_1/test_web.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_1/test_web.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,21 @@
     download_content = "test_http_helpers_download_yep"
     bbot_httpserver.expect_request(uri=path).respond_with_data(download_content)
     filename = await scan1.helpers.download(url)
     assert Path(str(filename)).is_file()
     assert scan1.helpers.is_cached(url)
     with open(filename) as f:
         assert f.read() == download_content
+    filename = Path("/tmp/bbot_download_test_file")
+    filename.unlink(missing_ok=True)
+    filename2 = await scan1.helpers.download(url, filename=filename)
+    assert filename2 == filename
+    assert filename2.is_file()
+    with open(filename2) as f:
+        assert f.read() == download_content
     # 404
     path = "/test_http_helpers_download_404"
     url = bbot_httpserver.url_for(path)
     download_content = "404"
     bbot_httpserver.expect_request(uri=path).respond_with_data(download_content, status=404)
     filename = await scan1.helpers.download(url)
     assert filename is None
```

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/base.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_asn.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_c99.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_censys.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_crt.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_git.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_github.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_http.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_otx.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_robots.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_social.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py` & `bbot-1.0.5.1798rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/testsslcert.pem` & `bbot-1.0.5.1798rc0/bbot/test/testsslcert.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/test/testsslkey.pem` & `bbot-1.0.5.1798rc0/bbot/test/testsslkey.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/wordlists/ffuf_shortname_candidates.txt` & `bbot-1.0.5.1798rc0/bbot/wordlists/ffuf_shortname_candidates.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/wordlists/nameservers.txt` & `bbot-1.0.5.1798rc0/bbot/wordlists/nameservers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt` & `bbot-1.0.5.1798rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/bbot/wordlists/wordninja_dns.txt.gz` & `bbot-1.0.5.1798rc0/bbot/wordlists/wordninja_dns.txt.gz`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1796rc0/pyproject.toml` & `bbot-1.0.5.1798rc0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbot"
-version = "v1.0.5.1796rc"
+version = "v1.0.5.1798rc"
 description = "OSINT automation for hackers."
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 readme = "README.md"
 repository = "https://github.com/blacklanternsecurity/bbot"
 homepage = "https://github.com/blacklanternsecurity/bbot"
```

### Comparing `bbot-1.0.5.1796rc0/PKG-INFO` & `bbot-1.0.5.1798rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbot
-Version: 1.0.5.1796rc0
+Version: 1.0.5.1798rc0
 Summary: OSINT automation for hackers.
 Home-page: https://github.com/blacklanternsecurity/bbot
 License: GPL-3.0
 Author: TheTechromancer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

