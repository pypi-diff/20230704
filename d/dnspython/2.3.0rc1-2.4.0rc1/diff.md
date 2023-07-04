# Comparing `tmp/dnspython-2.3.0rc1.tar.gz` & `tmp/dnspython-2.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnspython-2.3.0rc1.tar", max compression
+gzip compressed data, was "dnspython-2.4.0rc1.tar", max compression
```

## Comparing `dnspython-2.3.0rc1.tar` & `dnspython-2.4.0rc1.tar`

### file list

```diff
@@ -1,229 +1,239 @@
--rw-r--r--   0        0        0     1526 2022-12-27 19:43:15.409990 dnspython-2.3.0rc1/LICENSE
--rw-r--r--   0        0        0     3698 2022-12-27 19:43:27.611558 dnspython-2.3.0rc1/README.md
--rw-r--r--   0        0        0     1645 2022-12-27 19:43:15.410817 dnspython-2.3.0rc1/dns/__init__.py
--rw-r--r--   0        0        0     2002 2022-12-27 19:43:15.411058 dnspython-2.3.0rc1/dns/_asyncbackend.py
--rw-r--r--   0        0        0     4928 2022-12-27 19:43:15.411327 dnspython-2.3.0rc1/dns/_asyncio_backend.py
--rw-r--r--   0        0        0     3561 2022-12-27 19:43:15.411534 dnspython-2.3.0rc1/dns/_curio_backend.py
--rw-r--r--   0        0        0     2460 2022-12-27 19:43:15.411805 dnspython-2.3.0rc1/dns/_immutable_ctx.py
--rw-r--r--   0        0        0     3923 2022-12-27 19:43:15.411991 dnspython-2.3.0rc1/dns/_trio_backend.py
--rw-r--r--   0        0        0     2948 2022-12-27 19:43:15.412145 dnspython-2.3.0rc1/dns/asyncbackend.py
--rw-r--r--   0        0        0    25273 2022-12-27 19:43:15.412486 dnspython-2.3.0rc1/dns/asyncquery.py
--rw-r--r--   0        0        0    10490 2022-12-27 19:43:15.412793 dnspython-2.3.0rc1/dns/asyncresolver.py
--rw-r--r--   0        0        0    43181 2022-12-27 19:43:15.413045 dnspython-2.3.0rc1/dns/dnssec.py
--rw-r--r--   0        0        0     1799 2022-12-27 19:43:15.413311 dnspython-2.3.0rc1/dns/dnssectypes.py
--rw-r--r--   0        0        0     3978 2022-12-27 19:43:15.413486 dnspython-2.3.0rc1/dns/e164.py
--rw-r--r--   0        0        0    14021 2022-12-27 19:43:15.413646 dnspython-2.3.0rc1/dns/edns.py
--rw-r--r--   0        0        0     4244 2022-12-27 19:43:15.413921 dnspython-2.3.0rc1/dns/entropy.py
--rw-r--r--   0        0        0     3243 2022-12-27 19:43:15.414181 dnspython-2.3.0rc1/dns/enum.py
--rw-r--r--   0        0        0     5583 2022-12-27 19:43:15.414451 dnspython-2.3.0rc1/dns/exception.py
--rw-r--r--   0        0        0     2751 2022-12-27 19:43:15.414584 dnspython-2.3.0rc1/dns/flags.py
--rw-r--r--   0        0        0     2148 2022-12-27 19:43:15.414744 dnspython-2.3.0rc1/dns/grange.py
--rw-r--r--   0        0        0     1837 2022-12-27 19:43:15.414921 dnspython-2.3.0rc1/dns/immutable.py
--rw-r--r--   0        0        0     5021 2022-12-27 19:43:15.415090 dnspython-2.3.0rc1/dns/inet.py
--rw-r--r--   0        0        0     2065 2022-12-27 19:43:15.415239 dnspython-2.3.0rc1/dns/ipv4.py
--rw-r--r--   0        0        0     6193 2022-12-27 19:43:15.415413 dnspython-2.3.0rc1/dns/ipv6.py
--rw-r--r--   0        0        0    61832 2022-12-27 19:43:15.415746 dnspython-2.3.0rc1/dns/message.py
--rw-r--r--   0        0        0    34426 2022-12-27 19:43:15.416175 dnspython-2.3.0rc1/dns/name.py
--rw-r--r--   0        0        0     4000 2022-12-27 19:43:15.416421 dnspython-2.3.0rc1/dns/namedict.py
--rw-r--r--   0        0        0    12666 2022-12-27 19:43:15.416729 dnspython-2.3.0rc1/dns/node.py
--rw-r--r--   0        0        0     2730 2022-12-27 19:43:15.416873 dnspython-2.3.0rc1/dns/opcode.py
--rw-r--r--   0        0        0        0 2022-12-27 19:43:15.416904 dnspython-2.3.0rc1/dns/py.typed
--rw-r--r--   0        0        0    49641 2022-12-27 19:43:15.417180 dnspython-2.3.0rc1/dns/query.py
--rw-r--r--   0        0        0     2162 2022-12-27 19:43:15.417417 dnspython-2.3.0rc1/dns/quic/__init__.py
--rw-r--r--   0        0        0     7249 2022-12-27 19:43:15.417695 dnspython-2.3.0rc1/dns/quic/_asyncio.py
--rw-r--r--   0        0        0     5402 2022-12-27 19:43:15.417866 dnspython-2.3.0rc1/dns/quic/_common.py
--rw-r--r--   0        0        0     7179 2022-12-27 19:43:15.418135 dnspython-2.3.0rc1/dns/quic/_sync.py
--rw-r--r--   0        0        0     5932 2022-12-27 19:43:15.418314 dnspython-2.3.0rc1/dns/quic/_trio.py
--rw-r--r--   0        0        0     4156 2022-12-27 19:43:15.418470 dnspython-2.3.0rc1/dns/rcode.py
--rw-r--r--   0        0        0    29766 2022-12-27 19:43:15.418843 dnspython-2.3.0rc1/dns/rdata.py
--rw-r--r--   0        0        0     2984 2022-12-27 19:43:15.418984 dnspython-2.3.0rc1/dns/rdataclass.py
--rw-r--r--   0        0        0    17066 2022-12-27 19:43:15.419292 dnspython-2.3.0rc1/dns/rdataset.py
--rw-r--r--   0        0        0     7339 2022-12-27 19:43:15.419461 dnspython-2.3.0rc1/dns/rdatatype.py
--rw-r--r--   0        0        0     1662 2022-12-27 19:43:15.419643 dnspython-2.3.0rc1/dns/rdtypes/ANY/AFSDB.py
--rw-r--r--   0        0        0     3382 2022-12-27 19:43:15.419817 dnspython-2.3.0rc1/dns/rdtypes/ANY/AMTRELAY.py
--rw-r--r--   0        0        0     1025 2022-12-27 19:43:15.419900 dnspython-2.3.0rc1/dns/rdtypes/ANY/AVC.py
--rw-r--r--   0        0        0     2512 2022-12-27 19:43:15.420070 dnspython-2.3.0rc1/dns/rdtypes/ANY/CAA.py
--rw-r--r--   0        0        0     1226 2022-12-27 19:43:15.420225 dnspython-2.3.0rc1/dns/rdtypes/ANY/CDNSKEY.py
--rw-r--r--   0        0        0     1164 2022-12-27 19:43:15.420300 dnspython-2.3.0rc1/dns/rdtypes/ANY/CDS.py
--rw-r--r--   0        0        0     3534 2022-12-27 19:43:15.420458 dnspython-2.3.0rc1/dns/rdtypes/ANY/CERT.py
--rw-r--r--   0        0        0     1207 2022-12-27 19:43:15.420525 dnspython-2.3.0rc1/dns/rdtypes/ANY/CNAME.py
--rw-r--r--   0        0        0     2440 2022-12-27 19:43:15.420684 dnspython-2.3.0rc1/dns/rdtypes/ANY/CSYNC.py
--rw-r--r--   0        0        0      987 2022-12-27 19:43:15.420765 dnspython-2.3.0rc1/dns/rdtypes/ANY/DLV.py
--rw-r--r--   0        0        0     1151 2022-12-27 19:43:15.420828 dnspython-2.3.0rc1/dns/rdtypes/ANY/DNAME.py
--rw-r--r--   0        0        0     1224 2022-12-27 19:43:15.421003 dnspython-2.3.0rc1/dns/rdtypes/ANY/DNSKEY.py
--rw-r--r--   0        0        0      996 2022-12-27 19:43:15.421088 dnspython-2.3.0rc1/dns/rdtypes/ANY/DS.py
--rw-r--r--   0        0        0     1152 2022-12-27 19:43:15.421176 dnspython-2.3.0rc1/dns/rdtypes/ANY/EUI48.py
--rw-r--r--   0        0        0     1162 2022-12-27 19:43:15.421450 dnspython-2.3.0rc1/dns/rdtypes/ANY/EUI64.py
--rw-r--r--   0        0        0     4434 2022-12-27 19:43:15.421615 dnspython-2.3.0rc1/dns/rdtypes/ANY/GPOS.py
--rw-r--r--   0        0        0     2250 2022-12-27 19:43:15.421765 dnspython-2.3.0rc1/dns/rdtypes/ANY/HINFO.py
--rw-r--r--   0        0        0     3229 2022-12-27 19:43:15.421915 dnspython-2.3.0rc1/dns/rdtypes/ANY/HIP.py
--rw-r--r--   0        0        0     2714 2022-12-27 19:43:15.422058 dnspython-2.3.0rc1/dns/rdtypes/ANY/ISDN.py
--rw-r--r--   0        0        0     1287 2022-12-27 19:43:15.422207 dnspython-2.3.0rc1/dns/rdtypes/ANY/L32.py
--rw-r--r--   0        0        0     1593 2022-12-27 19:43:15.422352 dnspython-2.3.0rc1/dns/rdtypes/ANY/L64.py
--rw-r--r--   0        0        0    12028 2022-12-27 19:43:15.422522 dnspython-2.3.0rc1/dns/rdtypes/ANY/LOC.py
--rw-r--r--   0        0        0     1339 2022-12-27 19:43:15.422662 dnspython-2.3.0rc1/dns/rdtypes/ANY/LP.py
--rw-r--r--   0        0        0      996 2022-12-27 19:43:15.422718 dnspython-2.3.0rc1/dns/rdtypes/ANY/MX.py
--rw-r--r--   0        0        0     1545 2022-12-27 19:43:15.422868 dnspython-2.3.0rc1/dns/rdtypes/ANY/NID.py
--rw-r--r--   0        0        0     1042 2022-12-27 19:43:15.422946 dnspython-2.3.0rc1/dns/rdtypes/ANY/NINFO.py
--rw-r--r--   0        0        0      996 2022-12-27 19:43:15.422994 dnspython-2.3.0rc1/dns/rdtypes/ANY/NS.py
--rw-r--r--   0        0        0     2476 2022-12-27 19:43:15.423111 dnspython-2.3.0rc1/dns/rdtypes/ANY/NSEC.py
--rw-r--r--   0        0        0     3957 2022-12-27 19:43:15.423227 dnspython-2.3.0rc1/dns/rdtypes/ANY/NSEC3.py
--rw-r--r--   0        0        0     2636 2022-12-27 19:43:15.423349 dnspython-2.3.0rc1/dns/rdtypes/ANY/NSEC3PARAM.py
--rw-r--r--   0        0        0     1852 2022-12-27 19:43:15.423466 dnspython-2.3.0rc1/dns/rdtypes/ANY/OPENPGPKEY.py
--rw-r--r--   0        0        0     2563 2022-12-27 19:43:15.423587 dnspython-2.3.0rc1/dns/rdtypes/ANY/OPT.py
--rw-r--r--   0        0        0      998 2022-12-27 19:43:15.423644 dnspython-2.3.0rc1/dns/rdtypes/ANY/PTR.py
--rw-r--r--   0        0        0     2185 2022-12-27 19:43:15.423759 dnspython-2.3.0rc1/dns/rdtypes/ANY/RP.py
--rw-r--r--   0        0        0     4924 2022-12-27 19:43:15.423883 dnspython-2.3.0rc1/dns/rdtypes/ANY/RRSIG.py
--rw-r--r--   0        0        0     1014 2022-12-27 19:43:15.423930 dnspython-2.3.0rc1/dns/rdtypes/ANY/RT.py
--rw-r--r--   0        0        0      222 2022-12-27 19:43:15.423975 dnspython-2.3.0rc1/dns/rdtypes/ANY/SMIMEA.py
--rw-r--r--   0        0        0     3146 2022-12-27 19:43:15.424090 dnspython-2.3.0rc1/dns/rdtypes/ANY/SOA.py
--rw-r--r--   0        0        0     1023 2022-12-27 19:43:15.424156 dnspython-2.3.0rc1/dns/rdtypes/ANY/SPF.py
--rw-r--r--   0        0        0     2531 2022-12-27 19:43:15.424280 dnspython-2.3.0rc1/dns/rdtypes/ANY/SSHFP.py
--rw-r--r--   0        0        0     4932 2022-12-27 19:43:15.424407 dnspython-2.3.0rc1/dns/rdtypes/ANY/TKEY.py
--rw-r--r--   0        0        0      219 2022-12-27 19:43:15.424496 dnspython-2.3.0rc1/dns/rdtypes/ANY/TLSA.py
--rw-r--r--   0        0        0     4751 2022-12-27 19:43:15.424647 dnspython-2.3.0rc1/dns/rdtypes/ANY/TSIG.py
--rw-r--r--   0        0        0     1001 2022-12-27 19:43:15.424698 dnspython-2.3.0rc1/dns/rdtypes/ANY/TXT.py
--rw-r--r--   0        0        0     2922 2022-12-27 19:43:15.424840 dnspython-2.3.0rc1/dns/rdtypes/ANY/URI.py
--rw-r--r--   0        0        0     1945 2022-12-27 19:43:15.424955 dnspython-2.3.0rc1/dns/rdtypes/ANY/X25.py
--rw-r--r--   0        0        0     2394 2022-12-27 19:43:15.425082 dnspython-2.3.0rc1/dns/rdtypes/ANY/ZONEMD.py
--rw-r--r--   0        0        0     1497 2022-12-27 19:43:15.425223 dnspython-2.3.0rc1/dns/rdtypes/ANY/__init__.py
--rw-r--r--   0        0        0     2217 2022-12-27 19:43:15.425390 dnspython-2.3.0rc1/dns/rdtypes/CH/A.py
--rw-r--r--   0        0        0      923 2022-12-27 19:43:15.425508 dnspython-2.3.0rc1/dns/rdtypes/CH/__init__.py
--rw-r--r--   0        0        0     1815 2022-12-27 19:43:15.425676 dnspython-2.3.0rc1/dns/rdtypes/IN/A.py
--rw-r--r--   0        0        0     1821 2022-12-27 19:43:15.425819 dnspython-2.3.0rc1/dns/rdtypes/IN/AAAA.py
--rw-r--r--   0        0        0     5100 2022-12-27 19:43:15.425972 dnspython-2.3.0rc1/dns/rdtypes/IN/APL.py
--rw-r--r--   0        0        0     1857 2022-12-27 19:43:15.426114 dnspython-2.3.0rc1/dns/rdtypes/IN/DHCID.py
--rw-r--r--   0        0        0      220 2022-12-27 19:43:15.426257 dnspython-2.3.0rc1/dns/rdtypes/IN/HTTPS.py
--rw-r--r--   0        0        0     3291 2022-12-27 19:43:15.426392 dnspython-2.3.0rc1/dns/rdtypes/IN/IPSECKEY.py
--rw-r--r--   0        0        0     1014 2022-12-27 19:43:15.426447 dnspython-2.3.0rc1/dns/rdtypes/IN/KX.py
--rw-r--r--   0        0        0     3751 2022-12-27 19:43:15.426582 dnspython-2.3.0rc1/dns/rdtypes/IN/NAPTR.py
--rw-r--r--   0        0        0     2166 2022-12-27 19:43:15.426710 dnspython-2.3.0rc1/dns/rdtypes/IN/NSAP.py
--rw-r--r--   0        0        0     1016 2022-12-27 19:43:15.426759 dnspython-2.3.0rc1/dns/rdtypes/IN/NSAP_PTR.py
--rw-r--r--   0        0        0     2757 2022-12-27 19:43:15.426880 dnspython-2.3.0rc1/dns/rdtypes/IN/PX.py
--rw-r--r--   0        0        0     2770 2022-12-27 19:43:15.427027 dnspython-2.3.0rc1/dns/rdtypes/IN/SRV.py
--rw-r--r--   0        0        0      218 2022-12-27 19:43:15.427163 dnspython-2.3.0rc1/dns/rdtypes/IN/SVCB.py
--rw-r--r--   0        0        0     3653 2022-12-27 19:43:15.427302 dnspython-2.3.0rc1/dns/rdtypes/IN/WKS.py
--rw-r--r--   0        0        0     1083 2022-12-27 19:43:15.427435 dnspython-2.3.0rc1/dns/rdtypes/IN/__init__.py
--rw-r--r--   0        0        0     1073 2022-12-27 19:43:15.427576 dnspython-2.3.0rc1/dns/rdtypes/__init__.py
--rw-r--r--   0        0        0     2851 2022-12-27 19:43:15.427689 dnspython-2.3.0rc1/dns/rdtypes/dnskeybase.py
--rw-r--r--   0        0        0     3397 2022-12-27 19:43:15.427811 dnspython-2.3.0rc1/dns/rdtypes/dsbase.py
--rw-r--r--   0        0        0     2631 2022-12-27 19:43:15.427925 dnspython-2.3.0rc1/dns/rdtypes/euibase.py
--rw-r--r--   0        0        0     3199 2022-12-27 19:43:15.428046 dnspython-2.3.0rc1/dns/rdtypes/mxbase.py
--rw-r--r--   0        0        0     2325 2022-12-27 19:43:15.428181 dnspython-2.3.0rc1/dns/rdtypes/nsbase.py
--rw-r--r--   0        0        0    16936 2022-12-27 19:43:15.428447 dnspython-2.3.0rc1/dns/rdtypes/svcbbase.py
--rw-r--r--   0        0        0     2597 2022-12-27 19:43:15.428588 dnspython-2.3.0rc1/dns/rdtypes/tlsabase.py
--rw-r--r--   0        0        0     3631 2022-12-27 19:43:15.428714 dnspython-2.3.0rc1/dns/rdtypes/txtbase.py
--rw-r--r--   0        0        0     8745 2022-12-27 19:43:15.428857 dnspython-2.3.0rc1/dns/rdtypes/util.py
--rw-r--r--   0        0        0    10674 2022-12-27 19:43:15.429113 dnspython-2.3.0rc1/dns/renderer.py
--rw-r--r--   0        0        0    63405 2022-12-27 19:43:15.429391 dnspython-2.3.0rc1/dns/resolver.py
--rw-r--r--   0        0        0     3828 2022-12-27 19:43:15.429531 dnspython-2.3.0rc1/dns/reversename.py
--rw-r--r--   0        0        0     9184 2022-12-27 19:43:15.429775 dnspython-2.3.0rc1/dns/rrset.py
--rw-r--r--   0        0        0     3606 2022-12-27 19:43:15.429905 dnspython-2.3.0rc1/dns/serial.py
--rw-r--r--   0        0        0     9089 2022-12-27 19:43:15.430037 dnspython-2.3.0rc1/dns/set.py
--rw-r--r--   0        0        0    23584 2022-12-27 19:43:15.430294 dnspython-2.3.0rc1/dns/tokenizer.py
--rw-r--r--   0        0        0    21629 2022-12-27 19:43:15.430580 dnspython-2.3.0rc1/dns/transaction.py
--rw-r--r--   0        0        0    11457 2022-12-27 19:43:15.430842 dnspython-2.3.0rc1/dns/tsig.py
--rw-r--r--   0        0        0     2638 2022-12-27 19:43:15.430975 dnspython-2.3.0rc1/dns/tsigkeyring.py
--rw-r--r--   0        0        0     2979 2022-12-27 19:43:15.431100 dnspython-2.3.0rc1/dns/ttl.py
--rw-r--r--   0        0        0    12252 2022-12-27 19:43:15.431217 dnspython-2.3.0rc1/dns/update.py
--rw-r--r--   0        0        0     1926 2022-12-27 19:43:27.612189 dnspython-2.3.0rc1/dns/version.py
--rw-r--r--   0        0        0    11776 2022-12-27 19:43:15.431524 dnspython-2.3.0rc1/dns/versioned.py
--rw-r--r--   0        0        0     9057 2022-12-27 19:43:15.431734 dnspython-2.3.0rc1/dns/win32util.py
--rw-r--r--   0        0        0     2831 2022-12-27 19:43:15.431854 dnspython-2.3.0rc1/dns/wire.py
--rw-r--r--   0        0        0    13273 2022-12-27 19:43:15.432077 dnspython-2.3.0rc1/dns/xfr.py
--rw-r--r--   0        0        0    51058 2022-12-27 19:43:15.432413 dnspython-2.3.0rc1/dns/zone.py
--rw-r--r--   0        0        0    27484 2022-12-27 19:43:15.432688 dnspython-2.3.0rc1/dns/zonefile.py
--rw-r--r--   0        0        0      690 2022-12-27 19:43:15.432788 dnspython-2.3.0rc1/dns/zonetypes.py
--rw-r--r--   0        0        0      703 2022-12-27 19:43:15.437628 dnspython-2.3.0rc1/examples/async_dns.py
--rwxr-xr-x   0        0        0     1194 2022-12-27 19:43:15.437749 dnspython-2.3.0rc1/examples/ddns.py
--rwxr-xr-x   0        0        0     3007 2022-12-27 19:43:15.437870 dnspython-2.3.0rc1/examples/doh-json.py
--rwxr-xr-x   0        0        0     1186 2022-12-27 19:43:15.437979 dnspython-2.3.0rc1/examples/doh.py
--rw-r--r--   0        0        0     3143 2022-12-27 19:43:15.438117 dnspython-2.3.0rc1/examples/doq.py
--rwxr-xr-x   0        0        0      115 2022-12-27 19:43:15.438218 dnspython-2.3.0rc1/examples/e164.py
--rwxr-xr-x   0        0        0      427 2022-12-27 19:43:15.438327 dnspython-2.3.0rc1/examples/ecs.py
--rwxr-xr-x   0        0        0     1741 2022-12-27 19:43:15.438444 dnspython-2.3.0rc1/examples/edns.py
--rw-r--r--   0        0        0     1534 2022-12-27 19:43:15.438609 dnspython-2.3.0rc1/examples/edns_resolver.py
--rwxr-xr-x   0        0        0      189 2022-12-27 19:43:15.438759 dnspython-2.3.0rc1/examples/mx.py
--rwxr-xr-x   0        0        0      356 2022-12-27 19:43:15.438891 dnspython-2.3.0rc1/examples/name.py
--rw-r--r--   0        0        0     1270 2022-12-27 19:43:15.439020 dnspython-2.3.0rc1/examples/query_specific.py
--rw-r--r--   0        0        0     1022 2022-12-27 19:43:15.439164 dnspython-2.3.0rc1/examples/receive_notify.py
--rwxr-xr-x   0        0        0     1391 2022-12-27 19:43:15.439299 dnspython-2.3.0rc1/examples/reverse.py
--rwxr-xr-x   0        0        0      140 2022-12-27 19:43:15.439413 dnspython-2.3.0rc1/examples/reverse_name.py
--rwxr-xr-x   0        0        0      340 2022-12-27 19:43:15.439530 dnspython-2.3.0rc1/examples/xfr.py
--rwxr-xr-x   0        0        0    12173 2022-12-27 19:43:15.439684 dnspython-2.3.0rc1/examples/zonediff.py
--rw-r--r--   0        0        0     2342 2022-12-27 19:43:27.612674 dnspython-2.3.0rc1/pyproject.toml
--rw-r--r--   0        0        0     2041 2022-12-27 19:43:27.612883 dnspython-2.3.0rc1/setup.cfg
--rw-r--r--   0        0        0        0 2022-12-27 19:43:15.440576 dnspython-2.3.0rc1/tests/__init__.py
--rw-r--r--   0        0        0    12844 2022-12-27 19:43:15.440821 dnspython-2.3.0rc1/tests/example
--rw-r--r--   0        0        0    10967 2022-12-27 19:43:15.440907 dnspython-2.3.0rc1/tests/example1.good
--rw-r--r--   0        0        0    12647 2022-12-27 19:43:15.440981 dnspython-2.3.0rc1/tests/example2.good
--rw-r--r--   0        0        0    10967 2022-12-27 19:43:15.441027 dnspython-2.3.0rc1/tests/example3.good
--rw-r--r--   0        0        0    10984 2022-12-27 19:43:15.441072 dnspython-2.3.0rc1/tests/example4.good
--rw-r--r--   0        0        0     8696 2022-12-27 19:43:15.441299 dnspython-2.3.0rc1/tests/keys.py
--rw-r--r--   0        0        0       91 2022-12-27 19:43:15.441419 dnspython-2.3.0rc1/tests/md_module.py
--rw-r--r--   0        0        0      223 2022-12-27 19:43:15.441475 dnspython-2.3.0rc1/tests/mx-2-0.pickle
--rw-r--r--   0        0        0    11832 2022-12-27 19:43:15.441726 dnspython-2.3.0rc1/tests/nanonameserver.py
--rw-r--r--   0        0        0     4143 2022-12-27 19:43:15.441928 dnspython-2.3.0rc1/tests/nanoquic.py
--rw-r--r--   0        0        0      140 2022-12-27 19:43:15.441978 dnspython-2.3.0rc1/tests/query
--rw-r--r--   0        0        0      111 2022-12-27 19:43:15.442089 dnspython-2.3.0rc1/tests/stxt_module.py
--rw-r--r--   0        0        0     4573 2022-12-27 19:43:15.442145 dnspython-2.3.0rc1/tests/svcb_test_vectors.generic
--rw-r--r--   0        0        0     1157 2022-12-27 19:43:15.442195 dnspython-2.3.0rc1/tests/svcb_test_vectors.text
--rw-r--r--   0        0        0    21140 2022-12-27 19:43:15.442349 dnspython-2.3.0rc1/tests/test_address.py
--rw-r--r--   0        0        0    22089 2022-12-27 19:43:15.442591 dnspython-2.3.0rc1/tests/test_async.py
--rw-r--r--   0        0        0     3752 2022-12-27 19:43:15.442730 dnspython-2.3.0rc1/tests/test_bugs.py
--rw-r--r--   0        0        0     1295 2022-12-27 19:43:15.442849 dnspython-2.3.0rc1/tests/test_constants.py
--rw-r--r--   0        0        0    44250 2022-12-27 19:43:15.443161 dnspython-2.3.0rc1/tests/test_dnssec.py
--rw-r--r--   0        0        0    10148 2022-12-27 19:43:15.443368 dnspython-2.3.0rc1/tests/test_doh.py
--rw-r--r--   0        0        0     1401 2022-12-27 19:43:15.443556 dnspython-2.3.0rc1/tests/test_doq.py
--rw-r--r--   0        0        0     8926 2022-12-27 19:43:15.443690 dnspython-2.3.0rc1/tests/test_edns.py
--rw-r--r--   0        0        0     1977 2022-12-27 19:43:15.443813 dnspython-2.3.0rc1/tests/test_entropy.py
--rw-r--r--   0        0        0     2192 2022-12-27 19:43:15.443934 dnspython-2.3.0rc1/tests/test_exceptions.py
--rw-r--r--   0        0        0     2914 2022-12-27 19:43:15.444052 dnspython-2.3.0rc1/tests/test_flags.py
--rw-r--r--   0        0        0    24372 2022-12-27 19:43:15.444203 dnspython-2.3.0rc1/tests/test_generate.py
--rw-r--r--   0        0        0     3055 2022-12-27 19:43:15.444334 dnspython-2.3.0rc1/tests/test_grange.py
--rw-r--r--   0        0        0     4386 2022-12-27 19:43:15.444469 dnspython-2.3.0rc1/tests/test_immutable.py
--rw-r--r--   0        0        0    27357 2022-12-27 19:43:15.444727 dnspython-2.3.0rc1/tests/test_message.py
--rw-r--r--   0        0        0    37873 2022-12-27 19:43:15.444990 dnspython-2.3.0rc1/tests/test_name.py
--rw-r--r--   0        0        0     5625 2022-12-27 19:43:15.445140 dnspython-2.3.0rc1/tests/test_namedict.py
--rw-r--r--   0        0        0     1907 2022-12-27 19:43:15.445279 dnspython-2.3.0rc1/tests/test_nsec3.py
--rw-r--r--   0        0        0     3686 2022-12-27 19:43:15.445426 dnspython-2.3.0rc1/tests/test_nsec3_hash.py
--rw-r--r--   0        0        0    10878 2022-12-27 19:43:15.445586 dnspython-2.3.0rc1/tests/test_ntoaaton.py
--rw-r--r--   0        0        0     4037 2022-12-27 19:43:15.445713 dnspython-2.3.0rc1/tests/test_processing_order.py
--rw-r--r--   0        0        0    23516 2022-12-27 19:43:15.445960 dnspython-2.3.0rc1/tests/test_query.py
--rw-r--r--   0        0        0    43527 2022-12-27 19:43:15.446282 dnspython-2.3.0rc1/tests/test_rdata.py
--rw-r--r--   0        0        0     6136 2022-12-27 19:43:15.446437 dnspython-2.3.0rc1/tests/test_rdataset.py
--rw-r--r--   0        0        0     4308 2022-12-27 19:43:15.446593 dnspython-2.3.0rc1/tests/test_rdtypeandclass.py
--rw-r--r--   0        0        0     1696 2022-12-27 19:43:15.446736 dnspython-2.3.0rc1/tests/test_rdtypeanydnskey.py
--rw-r--r--   0        0        0     7283 2022-12-27 19:43:15.446886 dnspython-2.3.0rc1/tests/test_rdtypeanyeui.py
--rw-r--r--   0        0        0     3437 2022-12-27 19:43:15.447041 dnspython-2.3.0rc1/tests/test_rdtypeanyloc.py
--rw-r--r--   0        0        0     4309 2022-12-27 19:43:15.447198 dnspython-2.3.0rc1/tests/test_rdtypeanytkey.py
--rw-r--r--   0        0        0     3972 2022-12-27 19:43:15.447425 dnspython-2.3.0rc1/tests/test_renderer.py
--rw-r--r--   0        0        0    21490 2022-12-27 19:43:15.447587 dnspython-2.3.0rc1/tests/test_resolution.py
--rw-r--r--   0        0        0    42427 2022-12-27 19:43:15.447886 dnspython-2.3.0rc1/tests/test_resolver.py
--rw-r--r--   0        0        0     8942 2022-12-27 19:43:15.448102 dnspython-2.3.0rc1/tests/test_resolver_override.py
--rw-r--r--   0        0        0     8220 2022-12-27 19:43:15.448231 dnspython-2.3.0rc1/tests/test_rrset.py
--rw-r--r--   0        0        0     3920 2022-12-27 19:43:15.448425 dnspython-2.3.0rc1/tests/test_rrset_reader.py
--rw-r--r--   0        0        0     3776 2022-12-27 19:43:15.448555 dnspython-2.3.0rc1/tests/test_serial.py
--rw-r--r--   0        0        0     8872 2022-12-27 19:43:15.448680 dnspython-2.3.0rc1/tests/test_set.py
--rw-r--r--   0        0        0    14173 2022-12-27 19:43:15.448824 dnspython-2.3.0rc1/tests/test_svcb.py
--rw-r--r--   0        0        0    13465 2022-12-27 19:43:15.448953 dnspython-2.3.0rc1/tests/test_tokenizer.py
--rw-r--r--   0        0        0    21789 2022-12-27 19:43:15.449181 dnspython-2.3.0rc1/tests/test_transaction.py
--rw-r--r--   0        0        0    12773 2022-12-27 19:43:15.449412 dnspython-2.3.0rc1/tests/test_tsig.py
--rw-r--r--   0        0        0     2072 2022-12-27 19:43:15.449544 dnspython-2.3.0rc1/tests/test_tsigkeyring.py
--rw-r--r--   0        0        0     1120 2022-12-27 19:43:15.449671 dnspython-2.3.0rc1/tests/test_ttl.py
--rw-r--r--   0        0        0    11423 2022-12-27 19:43:15.449814 dnspython-2.3.0rc1/tests/test_update.py
--rw-r--r--   0        0        0     3308 2022-12-27 19:43:15.449957 dnspython-2.3.0rc1/tests/test_wire.py
--rw-r--r--   0        0        0    21909 2022-12-27 19:43:15.450198 dnspython-2.3.0rc1/tests/test_xfr.py
--rw-r--r--   0        0        0    44797 2022-12-27 19:43:15.450529 dnspython-2.3.0rc1/tests/test_zone.py
--rw-r--r--   0        0        0     9119 2022-12-27 19:43:15.450680 dnspython-2.3.0rc1/tests/test_zonedigest.py
--rw-r--r--   0        0        0     1204 2022-12-27 19:43:15.450840 dnspython-2.3.0rc1/tests/tls/ca.crt
--rw-r--r--   0        0        0      119 2022-12-27 19:43:15.450958 dnspython-2.3.0rc1/tests/tls/private.pem
--rw-r--r--   0        0        0     2095 2022-12-27 19:43:15.451093 dnspython-2.3.0rc1/tests/tls/public.crt
--rw-r--r--   0        0        0      101 2022-12-27 19:43:15.451212 dnspython-2.3.0rc1/tests/ttxt_module.py
--rw-r--r--   0        0        0      372 2022-12-27 19:43:15.451364 dnspython-2.3.0rc1/tests/utest.py
--rw-r--r--   0        0        0     4215 2022-12-27 19:43:15.451593 dnspython-2.3.0rc1/tests/util.py
--rwxr-xr-x   0        0        0     3126 2022-12-27 19:43:15.451704 dnspython-2.3.0rc1/util/constants-tool
--rw-r--r--   0        0        0      437 2022-12-27 19:43:15.451861 dnspython-2.3.0rc1/util/generate-mx-pickle.py
--rw-r--r--   0        0        0      358 2022-12-27 19:43:15.452109 dnspython-2.3.0rc1/util/generate-rdatatype-doc.py
--rw-r--r--   0        0        0     4816 1970-01-01 00:00:00.000000 dnspython-2.3.0rc1/setup.py
--rw-r--r--   0        0        0     5319 1970-01-01 00:00:00.000000 dnspython-2.3.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1526 2023-07-04 20:25:17.555883 dnspython-2.4.0rc1/LICENSE
+-rw-r--r--   0        0        0     3602 2023-07-04 20:25:17.556125 dnspython-2.4.0rc1/README.md
+-rw-r--r--   0        0        0     1663 2023-07-04 20:25:17.556391 dnspython-2.4.0rc1/dns/__init__.py
+-rw-r--r--   0        0        0     2275 2023-07-04 20:25:17.556483 dnspython-2.4.0rc1/dns/_asyncbackend.py
+-rw-r--r--   0        0        0     8664 2023-07-04 20:25:17.556600 dnspython-2.4.0rc1/dns/_asyncio_backend.py
+-rw-r--r--   0        0        0     5247 2023-07-04 20:25:17.556701 dnspython-2.4.0rc1/dns/_ddr.py
+-rw-r--r--   0        0        0     2459 2023-07-04 20:25:17.556790 dnspython-2.4.0rc1/dns/_immutable_ctx.py
+-rw-r--r--   0        0        0     7838 2023-07-04 20:25:17.556896 dnspython-2.4.0rc1/dns/_trio_backend.py
+-rw-r--r--   0        0        0     2794 2023-07-04 20:25:17.556987 dnspython-2.4.0rc1/dns/asyncbackend.py
+-rw-r--r--   0        0        0    25994 2023-07-04 20:25:17.557140 dnspython-2.4.0rc1/dns/asyncquery.py
+-rw-r--r--   0        0        0    17852 2023-07-04 20:25:17.557283 dnspython-2.4.0rc1/dns/asyncresolver.py
+-rw-r--r--   0        0        0    40543 2023-07-04 20:25:17.557492 dnspython-2.4.0rc1/dns/dnssec.py
+-rw-r--r--   0        0        0     3978 2023-07-04 20:25:17.557633 dnspython-2.4.0rc1/dns/dnssecalgs/__init__.py
+-rw-r--r--   0        0        0     2446 2023-07-04 20:25:17.557734 dnspython-2.4.0rc1/dns/dnssecalgs/base.py
+-rw-r--r--   0        0        0     2425 2023-07-04 20:25:17.557827 dnspython-2.4.0rc1/dns/dnssecalgs/cryptography.py
+-rw-r--r--   0        0        0     3497 2023-07-04 20:25:17.557918 dnspython-2.4.0rc1/dns/dnssecalgs/dsa.py
+-rw-r--r--   0        0        0     3016 2023-07-04 20:25:17.558010 dnspython-2.4.0rc1/dns/dnssecalgs/ecdsa.py
+-rw-r--r--   0        0        0     1914 2023-07-04 20:25:17.558097 dnspython-2.4.0rc1/dns/dnssecalgs/eddsa.py
+-rw-r--r--   0        0        0     3555 2023-07-04 20:25:17.558185 dnspython-2.4.0rc1/dns/dnssecalgs/rsa.py
+-rw-r--r--   0        0        0     1799 2023-07-04 20:25:17.558277 dnspython-2.4.0rc1/dns/dnssectypes.py
+-rw-r--r--   0        0        0     3978 2023-07-04 20:25:17.558375 dnspython-2.4.0rc1/dns/e164.py
+-rw-r--r--   0        0        0    14004 2023-07-04 20:25:17.558517 dnspython-2.4.0rc1/dns/edns.py
+-rw-r--r--   0        0        0     4242 2023-07-04 20:25:17.558637 dnspython-2.4.0rc1/dns/entropy.py
+-rw-r--r--   0        0        0     3691 2023-07-04 20:25:17.558728 dnspython-2.4.0rc1/dns/enum.py
+-rw-r--r--   0        0        0     5957 2023-07-04 20:25:17.558828 dnspython-2.4.0rc1/dns/exception.py
+-rw-r--r--   0        0        0     2750 2023-07-04 20:25:17.558931 dnspython-2.4.0rc1/dns/flags.py
+-rw-r--r--   0        0        0     2148 2023-07-04 20:25:17.559029 dnspython-2.4.0rc1/dns/grange.py
+-rw-r--r--   0        0        0     1836 2023-07-04 20:25:17.559146 dnspython-2.4.0rc1/dns/immutable.py
+-rw-r--r--   0        0        0     5278 2023-07-04 20:25:17.559247 dnspython-2.4.0rc1/dns/inet.py
+-rw-r--r--   0        0        0     2064 2023-07-04 20:25:17.559340 dnspython-2.4.0rc1/dns/ipv4.py
+-rw-r--r--   0        0        0     6192 2023-07-04 20:25:17.559438 dnspython-2.4.0rc1/dns/ipv6.py
+-rw-r--r--   0        0        0    63161 2023-07-04 20:25:17.559712 dnspython-2.4.0rc1/dns/message.py
+-rw-r--r--   0        0        0    34424 2023-07-04 20:25:17.559936 dnspython-2.4.0rc1/dns/name.py
+-rw-r--r--   0        0        0     4000 2023-07-04 20:25:17.560047 dnspython-2.4.0rc1/dns/namedict.py
+-rw-r--r--   0        0        0     9096 2023-07-04 20:25:17.560149 dnspython-2.4.0rc1/dns/nameserver.py
+-rw-r--r--   0        0        0    12664 2023-07-04 20:25:17.560268 dnspython-2.4.0rc1/dns/node.py
+-rw-r--r--   0        0        0     2730 2023-07-04 20:25:17.560373 dnspython-2.4.0rc1/dns/opcode.py
+-rw-r--r--   0        0        0        0 2023-07-04 20:25:17.560394 dnspython-2.4.0rc1/dns/py.typed
+-rw-r--r--   0        0        0    51760 2023-07-04 20:25:17.560625 dnspython-2.4.0rc1/dns/query.py
+-rw-r--r--   0        0        0     2163 2023-07-04 20:25:17.560743 dnspython-2.4.0rc1/dns/quic/__init__.py
+-rw-r--r--   0        0        0     7534 2023-07-04 20:25:17.560862 dnspython-2.4.0rc1/dns/quic/_asyncio.py
+-rw-r--r--   0        0        0     5460 2023-07-04 20:25:17.560957 dnspython-2.4.0rc1/dns/quic/_common.py
+-rw-r--r--   0        0        0     7608 2023-07-04 20:25:17.561070 dnspython-2.4.0rc1/dns/quic/_sync.py
+-rw-r--r--   0        0        0     6255 2023-07-04 20:25:17.561176 dnspython-2.4.0rc1/dns/quic/_trio.py
+-rw-r--r--   0        0        0     4156 2023-07-04 20:25:17.561280 dnspython-2.4.0rc1/dns/rcode.py
+-rw-r--r--   0        0        0    29557 2023-07-04 20:25:17.561459 dnspython-2.4.0rc1/dns/rdata.py
+-rw-r--r--   0        0        0     2984 2023-07-04 20:25:17.561566 dnspython-2.4.0rc1/dns/rdataclass.py
+-rw-r--r--   0        0        0    17049 2023-07-04 20:25:17.561718 dnspython-2.4.0rc1/dns/rdataset.py
+-rw-r--r--   0        0        0     7339 2023-07-04 20:25:17.561851 dnspython-2.4.0rc1/dns/rdatatype.py
+-rw-r--r--   0        0        0     1662 2023-07-04 20:25:17.562039 dnspython-2.4.0rc1/dns/rdtypes/ANY/AFSDB.py
+-rw-r--r--   0        0        0     3382 2023-07-04 20:25:17.562157 dnspython-2.4.0rc1/dns/rdtypes/ANY/AMTRELAY.py
+-rw-r--r--   0        0        0     1025 2023-07-04 20:25:17.562275 dnspython-2.4.0rc1/dns/rdtypes/ANY/AVC.py
+-rw-r--r--   0        0        0     2512 2023-07-04 20:25:17.562393 dnspython-2.4.0rc1/dns/rdtypes/ANY/CAA.py
+-rw-r--r--   0        0        0     1226 2023-07-04 20:25:17.562492 dnspython-2.4.0rc1/dns/rdtypes/ANY/CDNSKEY.py
+-rw-r--r--   0        0        0     1164 2023-07-04 20:25:17.562586 dnspython-2.4.0rc1/dns/rdtypes/ANY/CDS.py
+-rw-r--r--   0        0        0     3534 2023-07-04 20:25:17.562698 dnspython-2.4.0rc1/dns/rdtypes/ANY/CERT.py
+-rw-r--r--   0        0        0     1207 2023-07-04 20:25:17.562833 dnspython-2.4.0rc1/dns/rdtypes/ANY/CNAME.py
+-rw-r--r--   0        0        0     2440 2023-07-04 20:25:17.562955 dnspython-2.4.0rc1/dns/rdtypes/ANY/CSYNC.py
+-rw-r--r--   0        0        0      987 2023-07-04 20:25:17.563082 dnspython-2.4.0rc1/dns/rdtypes/ANY/DLV.py
+-rw-r--r--   0        0        0     1151 2023-07-04 20:25:17.563200 dnspython-2.4.0rc1/dns/rdtypes/ANY/DNAME.py
+-rw-r--r--   0        0        0     1224 2023-07-04 20:25:17.563311 dnspython-2.4.0rc1/dns/rdtypes/ANY/DNSKEY.py
+-rw-r--r--   0        0        0      996 2023-07-04 20:25:17.563418 dnspython-2.4.0rc1/dns/rdtypes/ANY/DS.py
+-rw-r--r--   0        0        0     1152 2023-07-04 20:25:17.563504 dnspython-2.4.0rc1/dns/rdtypes/ANY/EUI48.py
+-rw-r--r--   0        0        0     1162 2023-07-04 20:25:17.563611 dnspython-2.4.0rc1/dns/rdtypes/ANY/EUI64.py
+-rw-r--r--   0        0        0     4434 2023-07-04 20:25:17.563722 dnspython-2.4.0rc1/dns/rdtypes/ANY/GPOS.py
+-rw-r--r--   0        0        0     2250 2023-07-04 20:25:17.563835 dnspython-2.4.0rc1/dns/rdtypes/ANY/HINFO.py
+-rw-r--r--   0        0        0     3229 2023-07-04 20:25:17.563955 dnspython-2.4.0rc1/dns/rdtypes/ANY/HIP.py
+-rw-r--r--   0        0        0     2714 2023-07-04 20:25:17.564091 dnspython-2.4.0rc1/dns/rdtypes/ANY/ISDN.py
+-rw-r--r--   0        0        0     1287 2023-07-04 20:25:17.564211 dnspython-2.4.0rc1/dns/rdtypes/ANY/L32.py
+-rw-r--r--   0        0        0     1593 2023-07-04 20:25:17.564324 dnspython-2.4.0rc1/dns/rdtypes/ANY/L64.py
+-rw-r--r--   0        0        0    12025 2023-07-04 20:25:17.564452 dnspython-2.4.0rc1/dns/rdtypes/ANY/LOC.py
+-rw-r--r--   0        0        0     1339 2023-07-04 20:25:17.564550 dnspython-2.4.0rc1/dns/rdtypes/ANY/LP.py
+-rw-r--r--   0        0        0      996 2023-07-04 20:25:17.564656 dnspython-2.4.0rc1/dns/rdtypes/ANY/MX.py
+-rw-r--r--   0        0        0     1545 2023-07-04 20:25:17.564763 dnspython-2.4.0rc1/dns/rdtypes/ANY/NID.py
+-rw-r--r--   0        0        0     1042 2023-07-04 20:25:17.564866 dnspython-2.4.0rc1/dns/rdtypes/ANY/NINFO.py
+-rw-r--r--   0        0        0      996 2023-07-04 20:25:17.564973 dnspython-2.4.0rc1/dns/rdtypes/ANY/NS.py
+-rw-r--r--   0        0        0     2476 2023-07-04 20:25:17.565080 dnspython-2.4.0rc1/dns/rdtypes/ANY/NSEC.py
+-rw-r--r--   0        0        0     4152 2023-07-04 20:25:17.565199 dnspython-2.4.0rc1/dns/rdtypes/ANY/NSEC3.py
+-rw-r--r--   0        0        0     2636 2023-07-04 20:25:17.565309 dnspython-2.4.0rc1/dns/rdtypes/ANY/NSEC3PARAM.py
+-rw-r--r--   0        0        0     1852 2023-07-04 20:25:17.565419 dnspython-2.4.0rc1/dns/rdtypes/ANY/OPENPGPKEY.py
+-rw-r--r--   0        0        0     2562 2023-07-04 20:25:17.565534 dnspython-2.4.0rc1/dns/rdtypes/ANY/OPT.py
+-rw-r--r--   0        0        0      998 2023-07-04 20:25:17.565640 dnspython-2.4.0rc1/dns/rdtypes/ANY/PTR.py
+-rw-r--r--   0        0        0     2185 2023-07-04 20:25:17.565751 dnspython-2.4.0rc1/dns/rdtypes/ANY/RP.py
+-rw-r--r--   0        0        0     4924 2023-07-04 20:25:17.565873 dnspython-2.4.0rc1/dns/rdtypes/ANY/RRSIG.py
+-rw-r--r--   0        0        0     1014 2023-07-04 20:25:17.565986 dnspython-2.4.0rc1/dns/rdtypes/ANY/RT.py
+-rw-r--r--   0        0        0      222 2023-07-04 20:25:17.566041 dnspython-2.4.0rc1/dns/rdtypes/ANY/SMIMEA.py
+-rw-r--r--   0        0        0     3146 2023-07-04 20:25:17.566152 dnspython-2.4.0rc1/dns/rdtypes/ANY/SOA.py
+-rw-r--r--   0        0        0     1023 2023-07-04 20:25:17.566254 dnspython-2.4.0rc1/dns/rdtypes/ANY/SPF.py
+-rw-r--r--   0        0        0     2531 2023-07-04 20:25:17.566363 dnspython-2.4.0rc1/dns/rdtypes/ANY/SSHFP.py
+-rw-r--r--   0        0        0     4932 2023-07-04 20:25:17.566488 dnspython-2.4.0rc1/dns/rdtypes/ANY/TKEY.py
+-rw-r--r--   0        0        0      219 2023-07-04 20:25:17.566589 dnspython-2.4.0rc1/dns/rdtypes/ANY/TLSA.py
+-rw-r--r--   0        0        0     4751 2023-07-04 20:25:17.566722 dnspython-2.4.0rc1/dns/rdtypes/ANY/TSIG.py
+-rw-r--r--   0        0        0     1001 2023-07-04 20:25:17.566839 dnspython-2.4.0rc1/dns/rdtypes/ANY/TXT.py
+-rw-r--r--   0        0        0     2922 2023-07-04 20:25:17.566954 dnspython-2.4.0rc1/dns/rdtypes/ANY/URI.py
+-rw-r--r--   0        0        0     1945 2023-07-04 20:25:17.567073 dnspython-2.4.0rc1/dns/rdtypes/ANY/X25.py
+-rw-r--r--   0        0        0     2394 2023-07-04 20:25:17.567194 dnspython-2.4.0rc1/dns/rdtypes/ANY/ZONEMD.py
+-rw-r--r--   0        0        0     1497 2023-07-04 20:25:17.567301 dnspython-2.4.0rc1/dns/rdtypes/ANY/__init__.py
+-rw-r--r--   0        0        0     2217 2023-07-04 20:25:17.567452 dnspython-2.4.0rc1/dns/rdtypes/CH/A.py
+-rw-r--r--   0        0        0      923 2023-07-04 20:25:17.567576 dnspython-2.4.0rc1/dns/rdtypes/CH/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-04 20:25:17.567726 dnspython-2.4.0rc1/dns/rdtypes/IN/A.py
+-rw-r--r--   0        0        0     1821 2023-07-04 20:25:17.567850 dnspython-2.4.0rc1/dns/rdtypes/IN/AAAA.py
+-rw-r--r--   0        0        0     5099 2023-07-04 20:25:17.567982 dnspython-2.4.0rc1/dns/rdtypes/IN/APL.py
+-rw-r--r--   0        0        0     1857 2023-07-04 20:25:17.568096 dnspython-2.4.0rc1/dns/rdtypes/IN/DHCID.py
+-rw-r--r--   0        0        0      220 2023-07-04 20:25:17.568206 dnspython-2.4.0rc1/dns/rdtypes/IN/HTTPS.py
+-rw-r--r--   0        0        0     3291 2023-07-04 20:25:17.568324 dnspython-2.4.0rc1/dns/rdtypes/IN/IPSECKEY.py
+-rw-r--r--   0        0        0     1014 2023-07-04 20:25:17.568415 dnspython-2.4.0rc1/dns/rdtypes/IN/KX.py
+-rw-r--r--   0        0        0     3751 2023-07-04 20:25:17.568541 dnspython-2.4.0rc1/dns/rdtypes/IN/NAPTR.py
+-rw-r--r--   0        0        0     2166 2023-07-04 20:25:17.568668 dnspython-2.4.0rc1/dns/rdtypes/IN/NSAP.py
+-rw-r--r--   0        0        0     1016 2023-07-04 20:25:17.568778 dnspython-2.4.0rc1/dns/rdtypes/IN/NSAP_PTR.py
+-rw-r--r--   0        0        0     2757 2023-07-04 20:25:17.568879 dnspython-2.4.0rc1/dns/rdtypes/IN/PX.py
+-rw-r--r--   0        0        0     2770 2023-07-04 20:25:17.568984 dnspython-2.4.0rc1/dns/rdtypes/IN/SRV.py
+-rw-r--r--   0        0        0      218 2023-07-04 20:25:17.569089 dnspython-2.4.0rc1/dns/rdtypes/IN/SVCB.py
+-rw-r--r--   0        0        0     3653 2023-07-04 20:25:17.569205 dnspython-2.4.0rc1/dns/rdtypes/IN/WKS.py
+-rw-r--r--   0        0        0     1083 2023-07-04 20:25:17.569312 dnspython-2.4.0rc1/dns/rdtypes/IN/__init__.py
+-rw-r--r--   0        0        0     1073 2023-07-04 20:25:17.569420 dnspython-2.4.0rc1/dns/rdtypes/__init__.py
+-rw-r--r--   0        0        0     2857 2023-07-04 20:25:17.569527 dnspython-2.4.0rc1/dns/rdtypes/dnskeybase.py
+-rw-r--r--   0        0        0     3428 2023-07-04 20:25:17.569634 dnspython-2.4.0rc1/dns/rdtypes/dsbase.py
+-rw-r--r--   0        0        0     2631 2023-07-04 20:25:17.569734 dnspython-2.4.0rc1/dns/rdtypes/euibase.py
+-rw-r--r--   0        0        0     3199 2023-07-04 20:25:17.569836 dnspython-2.4.0rc1/dns/rdtypes/mxbase.py
+-rw-r--r--   0        0        0     2325 2023-07-04 20:25:17.569936 dnspython-2.4.0rc1/dns/rdtypes/nsbase.py
+-rw-r--r--   0        0        0    16952 2023-07-04 20:25:17.570083 dnspython-2.4.0rc1/dns/rdtypes/svcbbase.py
+-rw-r--r--   0        0        0     2597 2023-07-04 20:25:17.570192 dnspython-2.4.0rc1/dns/rdtypes/tlsabase.py
+-rw-r--r--   0        0        0     3630 2023-07-04 20:25:17.570305 dnspython-2.4.0rc1/dns/rdtypes/txtbase.py
+-rw-r--r--   0        0        0     9003 2023-07-04 20:25:17.570427 dnspython-2.4.0rc1/dns/rdtypes/util.py
+-rw-r--r--   0        0        0    10673 2023-07-04 20:25:17.570554 dnspython-2.4.0rc1/dns/renderer.py
+-rw-r--r--   0        0        0    73514 2023-07-04 20:25:17.570871 dnspython-2.4.0rc1/dns/resolver.py
+-rw-r--r--   0        0        0     3828 2023-07-04 20:25:17.570982 dnspython-2.4.0rc1/dns/reversename.py
+-rw-r--r--   0        0        0     9168 2023-07-04 20:25:17.571090 dnspython-2.4.0rc1/dns/rrset.py
+-rw-r--r--   0        0        0     3606 2023-07-04 20:25:17.571184 dnspython-2.4.0rc1/dns/serial.py
+-rw-r--r--   0        0        0     9089 2023-07-04 20:25:17.571296 dnspython-2.4.0rc1/dns/set.py
+-rw-r--r--   0        0        0    23583 2023-07-04 20:25:17.571448 dnspython-2.4.0rc1/dns/tokenizer.py
+-rw-r--r--   0        0        0    22660 2023-07-04 20:25:17.571593 dnspython-2.4.0rc1/dns/transaction.py
+-rw-r--r--   0        0        0    11422 2023-07-04 20:25:17.571716 dnspython-2.4.0rc1/dns/tsig.py
+-rw-r--r--   0        0        0     2633 2023-07-04 20:25:17.571812 dnspython-2.4.0rc1/dns/tsigkeyring.py
+-rw-r--r--   0        0        0     2979 2023-07-04 20:25:17.571905 dnspython-2.4.0rc1/dns/ttl.py
+-rw-r--r--   0        0        0    12243 2023-07-04 20:25:17.572013 dnspython-2.4.0rc1/dns/update.py
+-rw-r--r--   0        0        0     1926 2023-07-04 20:25:17.572101 dnspython-2.4.0rc1/dns/version.py
+-rw-r--r--   0        0        0    11765 2023-07-04 20:25:17.572210 dnspython-2.4.0rc1/dns/versioned.py
+-rw-r--r--   0        0        0     9057 2023-07-04 20:25:17.572313 dnspython-2.4.0rc1/dns/win32util.py
+-rw-r--r--   0        0        0     2830 2023-07-04 20:25:17.572408 dnspython-2.4.0rc1/dns/wire.py
+-rw-r--r--   0        0        0    13273 2023-07-04 20:25:17.572527 dnspython-2.4.0rc1/dns/xfr.py
+-rw-r--r--   0        0        0    51093 2023-07-04 20:25:17.572741 dnspython-2.4.0rc1/dns/zone.py
+-rw-r--r--   0        0        0    27930 2023-07-04 20:25:17.572907 dnspython-2.4.0rc1/dns/zonefile.py
+-rw-r--r--   0        0        0      690 2023-07-04 20:25:17.573002 dnspython-2.4.0rc1/dns/zonetypes.py
+-rw-r--r--   0        0        0      874 2023-07-04 20:25:17.576936 dnspython-2.4.0rc1/examples/async_dns.py
+-rwxr-xr-x   0        0        0     1194 2023-07-04 20:25:17.577026 dnspython-2.4.0rc1/examples/ddns.py
+-rw-r--r--   0        0        0      950 2023-07-04 20:25:17.577121 dnspython-2.4.0rc1/examples/ddr.py
+-rwxr-xr-x   0        0        0     3001 2023-07-04 20:25:17.577215 dnspython-2.4.0rc1/examples/doh-json.py
+-rwxr-xr-x   0        0        0      534 2023-07-04 20:25:17.577298 dnspython-2.4.0rc1/examples/doh.py
+-rw-r--r--   0        0        0     3143 2023-07-04 20:25:17.577395 dnspython-2.4.0rc1/examples/doq.py
+-rwxr-xr-x   0        0        0      115 2023-07-04 20:25:17.577473 dnspython-2.4.0rc1/examples/e164.py
+-rwxr-xr-x   0        0        0      427 2023-07-04 20:25:17.577562 dnspython-2.4.0rc1/examples/ecs.py
+-rwxr-xr-x   0        0        0     1739 2023-07-04 20:25:17.577656 dnspython-2.4.0rc1/examples/edns.py
+-rw-r--r--   0        0        0     1532 2023-07-04 20:25:17.577756 dnspython-2.4.0rc1/examples/edns_resolver.py
+-rwxr-xr-x   0        0        0      189 2023-07-04 20:25:17.577853 dnspython-2.4.0rc1/examples/mx.py
+-rwxr-xr-x   0        0        0      356 2023-07-04 20:25:17.577945 dnspython-2.4.0rc1/examples/name.py
+-rw-r--r--   0        0        0     1655 2023-07-04 20:25:17.578033 dnspython-2.4.0rc1/examples/query_specific.py
+-rw-r--r--   0        0        0     1022 2023-07-04 20:25:17.578118 dnspython-2.4.0rc1/examples/receive_notify.py
+-rwxr-xr-x   0        0        0     1389 2023-07-04 20:25:17.578204 dnspython-2.4.0rc1/examples/reverse.py
+-rwxr-xr-x   0        0        0      140 2023-07-04 20:25:17.578290 dnspython-2.4.0rc1/examples/reverse_name.py
+-rwxr-xr-x   0        0        0      340 2023-07-04 20:25:17.578377 dnspython-2.4.0rc1/examples/xfr.py
+-rwxr-xr-x   0        0        0    12173 2023-07-04 20:25:17.578484 dnspython-2.4.0rc1/examples/zonediff.py
+-rw-r--r--   0        0        0     2202 2023-07-04 20:25:17.578733 dnspython-2.4.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1970 2023-07-04 20:25:17.578869 dnspython-2.4.0rc1/setup.cfg
+-rw-r--r--   0        0        0        0 2023-07-04 20:25:17.579110 dnspython-2.4.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0    12881 2023-07-04 20:25:17.579239 dnspython-2.4.0rc1/tests/example
+-rw-r--r--   0        0        0    11010 2023-07-04 20:25:17.579352 dnspython-2.4.0rc1/tests/example1.good
+-rw-r--r--   0        0        0    12699 2023-07-04 20:25:17.579470 dnspython-2.4.0rc1/tests/example2.good
+-rw-r--r--   0        0        0    11010 2023-07-04 20:25:17.579582 dnspython-2.4.0rc1/tests/example3.good
+-rw-r--r--   0        0        0    11027 2023-07-04 20:25:17.579702 dnspython-2.4.0rc1/tests/example4.good
+-rw-r--r--   0        0        0     8696 2023-07-04 20:25:17.579816 dnspython-2.4.0rc1/tests/keys.py
+-rw-r--r--   0        0        0       91 2023-07-04 20:25:17.579893 dnspython-2.4.0rc1/tests/md_module.py
+-rw-r--r--   0        0        0      223 2023-07-04 20:25:17.579936 dnspython-2.4.0rc1/tests/mx-2-0.pickle
+-rw-r--r--   0        0        0    11832 2023-07-04 20:25:17.580050 dnspython-2.4.0rc1/tests/nanonameserver.py
+-rw-r--r--   0        0        0     4246 2023-07-04 20:25:17.580145 dnspython-2.4.0rc1/tests/nanoquic.py
+-rw-r--r--   0        0        0      140 2023-07-04 20:25:17.580189 dnspython-2.4.0rc1/tests/query
+-rw-r--r--   0        0        0      111 2023-07-04 20:25:17.580274 dnspython-2.4.0rc1/tests/stxt_module.py
+-rw-r--r--   0        0        0     4573 2023-07-04 20:25:17.580325 dnspython-2.4.0rc1/tests/svcb_test_vectors.generic
+-rw-r--r--   0        0        0     1157 2023-07-04 20:25:17.580371 dnspython-2.4.0rc1/tests/svcb_test_vectors.text
+-rw-r--r--   0        0        0    21140 2023-07-04 20:25:17.580497 dnspython-2.4.0rc1/tests/test_address.py
+-rw-r--r--   0        0        0    23340 2023-07-04 20:25:17.580646 dnspython-2.4.0rc1/tests/test_async.py
+-rw-r--r--   0        0        0     3752 2023-07-04 20:25:17.580757 dnspython-2.4.0rc1/tests/test_bugs.py
+-rw-r--r--   0        0        0     1295 2023-07-04 20:25:17.580847 dnspython-2.4.0rc1/tests/test_constants.py
+-rw-r--r--   0        0        0     1258 2023-07-04 20:25:17.580940 dnspython-2.4.0rc1/tests/test_ddr.py
+-rw-r--r--   0        0        0    50033 2023-07-04 20:25:17.581161 dnspython-2.4.0rc1/tests/test_dnssec.py
+-rw-r--r--   0        0        0    10264 2023-07-04 20:25:17.581285 dnspython-2.4.0rc1/tests/test_dnssecalgs.py
+-rw-r--r--   0        0        0     6976 2023-07-04 20:25:17.581400 dnspython-2.4.0rc1/tests/test_doh.py
+-rw-r--r--   0        0        0     1401 2023-07-04 20:25:17.581489 dnspython-2.4.0rc1/tests/test_doq.py
+-rw-r--r--   0        0        0     8926 2023-07-04 20:25:17.581597 dnspython-2.4.0rc1/tests/test_edns.py
+-rw-r--r--   0        0        0     1977 2023-07-04 20:25:17.581693 dnspython-2.4.0rc1/tests/test_entropy.py
+-rw-r--r--   0        0        0     2192 2023-07-04 20:25:17.581783 dnspython-2.4.0rc1/tests/test_exceptions.py
+-rw-r--r--   0        0        0     2914 2023-07-04 20:25:17.581875 dnspython-2.4.0rc1/tests/test_flags.py
+-rw-r--r--   0        0        0    24372 2023-07-04 20:25:17.581994 dnspython-2.4.0rc1/tests/test_generate.py
+-rw-r--r--   0        0        0     3055 2023-07-04 20:25:17.582093 dnspython-2.4.0rc1/tests/test_grange.py
+-rw-r--r--   0        0        0     4384 2023-07-04 20:25:17.582189 dnspython-2.4.0rc1/tests/test_immutable.py
+-rw-r--r--   0        0        0    27696 2023-07-04 20:25:17.582354 dnspython-2.4.0rc1/tests/test_message.py
+-rw-r--r--   0        0        0    37873 2023-07-04 20:25:17.582541 dnspython-2.4.0rc1/tests/test_name.py
+-rw-r--r--   0        0        0     5625 2023-07-04 20:25:17.582643 dnspython-2.4.0rc1/tests/test_namedict.py
+-rw-r--r--   0        0        0     1907 2023-07-04 20:25:17.582730 dnspython-2.4.0rc1/tests/test_nsec3.py
+-rw-r--r--   0        0        0     3685 2023-07-04 20:25:17.582820 dnspython-2.4.0rc1/tests/test_nsec3_hash.py
+-rw-r--r--   0        0        0    10872 2023-07-04 20:25:17.582933 dnspython-2.4.0rc1/tests/test_ntoaaton.py
+-rw-r--r--   0        0        0     4037 2023-07-04 20:25:17.583042 dnspython-2.4.0rc1/tests/test_processing_order.py
+-rw-r--r--   0        0        0    23514 2023-07-04 20:25:17.583177 dnspython-2.4.0rc1/tests/test_query.py
+-rw-r--r--   0        0        0    43483 2023-07-04 20:25:17.583386 dnspython-2.4.0rc1/tests/test_rdata.py
+-rw-r--r--   0        0        0     6136 2023-07-04 20:25:17.583494 dnspython-2.4.0rc1/tests/test_rdataset.py
+-rw-r--r--   0        0        0     4307 2023-07-04 20:25:17.583593 dnspython-2.4.0rc1/tests/test_rdtypeandclass.py
+-rw-r--r--   0        0        0     1696 2023-07-04 20:25:17.583681 dnspython-2.4.0rc1/tests/test_rdtypeanydnskey.py
+-rw-r--r--   0        0        0     7283 2023-07-04 20:25:17.583782 dnspython-2.4.0rc1/tests/test_rdtypeanyeui.py
+-rw-r--r--   0        0        0     3437 2023-07-04 20:25:17.583873 dnspython-2.4.0rc1/tests/test_rdtypeanyloc.py
+-rw-r--r--   0        0        0     4309 2023-07-04 20:25:17.583966 dnspython-2.4.0rc1/tests/test_rdtypeanytkey.py
+-rw-r--r--   0        0        0     3972 2023-07-04 20:25:17.584071 dnspython-2.4.0rc1/tests/test_renderer.py
+-rw-r--r--   0        0        0    21664 2023-07-04 20:25:17.584211 dnspython-2.4.0rc1/tests/test_resolution.py
+-rw-r--r--   0        0        0    45216 2023-07-04 20:25:17.584418 dnspython-2.4.0rc1/tests/test_resolver.py
+-rw-r--r--   0        0        0     8942 2023-07-04 20:25:17.584540 dnspython-2.4.0rc1/tests/test_resolver_override.py
+-rw-r--r--   0        0        0     8220 2023-07-04 20:25:17.584665 dnspython-2.4.0rc1/tests/test_rrset.py
+-rw-r--r--   0        0        0     3920 2023-07-04 20:25:17.584771 dnspython-2.4.0rc1/tests/test_rrset_reader.py
+-rw-r--r--   0        0        0     3776 2023-07-04 20:25:17.584870 dnspython-2.4.0rc1/tests/test_serial.py
+-rw-r--r--   0        0        0     8872 2023-07-04 20:25:17.584980 dnspython-2.4.0rc1/tests/test_set.py
+-rw-r--r--   0        0        0    14173 2023-07-04 20:25:17.585109 dnspython-2.4.0rc1/tests/test_svcb.py
+-rw-r--r--   0        0        0    13465 2023-07-04 20:25:17.585229 dnspython-2.4.0rc1/tests/test_tokenizer.py
+-rw-r--r--   0        0        0    22137 2023-07-04 20:25:17.585383 dnspython-2.4.0rc1/tests/test_transaction.py
+-rw-r--r--   0        0        0    12773 2023-07-04 20:25:17.585516 dnspython-2.4.0rc1/tests/test_tsig.py
+-rw-r--r--   0        0        0     2072 2023-07-04 20:25:17.585610 dnspython-2.4.0rc1/tests/test_tsigkeyring.py
+-rw-r--r--   0        0        0     1120 2023-07-04 20:25:17.585695 dnspython-2.4.0rc1/tests/test_ttl.py
+-rw-r--r--   0        0        0    11423 2023-07-04 20:25:17.585807 dnspython-2.4.0rc1/tests/test_update.py
+-rw-r--r--   0        0        0     3308 2023-07-04 20:25:17.585909 dnspython-2.4.0rc1/tests/test_wire.py
+-rw-r--r--   0        0        0    21524 2023-07-04 20:25:17.586053 dnspython-2.4.0rc1/tests/test_xfr.py
+-rw-r--r--   0        0        0    45309 2023-07-04 20:25:17.586257 dnspython-2.4.0rc1/tests/test_zone.py
+-rw-r--r--   0        0        0     9119 2023-07-04 20:25:17.586372 dnspython-2.4.0rc1/tests/test_zonedigest.py
+-rw-r--r--   0        0        0     1204 2023-07-04 20:25:17.586501 dnspython-2.4.0rc1/tests/tls/ca.crt
+-rw-r--r--   0        0        0      119 2023-07-04 20:25:17.586584 dnspython-2.4.0rc1/tests/tls/private.pem
+-rw-r--r--   0        0        0     2095 2023-07-04 20:25:17.586681 dnspython-2.4.0rc1/tests/tls/public.crt
+-rw-r--r--   0        0        0      101 2023-07-04 20:25:17.586769 dnspython-2.4.0rc1/tests/ttxt_module.py
+-rw-r--r--   0        0        0      372 2023-07-04 20:25:17.586854 dnspython-2.4.0rc1/tests/utest.py
+-rw-r--r--   0        0        0     4215 2023-07-04 20:25:17.586962 dnspython-2.4.0rc1/tests/util.py
+-rwxr-xr-x   0        0        0     3126 2023-07-04 20:25:17.587063 dnspython-2.4.0rc1/util/constants-tool
+-rw-r--r--   0        0        0      437 2023-07-04 20:25:17.587148 dnspython-2.4.0rc1/util/generate-mx-pickle.py
+-rw-r--r--   0        0        0      358 2023-07-04 20:25:17.587242 dnspython-2.4.0rc1/util/generate-rdatatype-doc.py
+-rw-r--r--   0        0        0     4952 1970-01-01 00:00:00.000000 dnspython-2.4.0rc1/PKG-INFO
```

### Comparing `dnspython-2.3.0rc1/LICENSE` & `dnspython-2.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/README.md` & `dnspython-2.4.0rc1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # dnspython
 
 [![Build Status](https://github.com/rthalley/dnspython/actions/workflows/python-package.yml/badge.svg)](https://github.com/rthalley/dnspython/actions/)
 [![Documentation Status](https://readthedocs.org/projects/dnspython/badge/?version=latest)](https://dnspython.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/dnspython.svg)](https://badge.fury.io/py/dnspython)
 [![License: ISC](https://img.shields.io/badge/License-ISC-brightgreen.svg)](https://opensource.org/licenses/ISC)
 [![Coverage](https://codecov.io/github/rthalley/dnspython/coverage.svg?branch=master)](https://codecov.io/github/rthalley/dnspython)
-[![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/rthalley/dnspython)](https://lgtm.com/projects/g/rthalley/dnspython/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## INTRODUCTION
 
 dnspython is a DNS toolkit for Python. It supports almost all record types. It
 can be used for queries, zone transfers, and dynamic updates. It supports TSIG
 authenticated messages and EDNS0.
@@ -27,26 +26,34 @@
 `socket.gethostbyname()`.
 
 dnspython originated at Nominum where it was developed
 to facilitate the testing of DNS software.
 
 ## ABOUT THIS RELEASE
 
-This is dnspython 2.3.0rc1.
+This is dnspython 2.4.0rc1.
 Please read
 [What's New](https://dnspython.readthedocs.io/en/latest/whatsnew.html) for
 information about the changes in this release.
 
 ## INSTALLATION
 
 * Many distributions have dnspython packaged for you, so you should
   check there first.
-* If you have pip installed, you can do `pip install dnspython`
-* If not just download the source file and unzip it, then run
-  `sudo python setup.py install`
+* To use a wheel downloaded from PyPi, run:
+
+    pip install dnspython
+
+* To install from the source code, go into the top-level of the source code
+  and run:
+
+    pip install --upgrade pip build
+    python -m build
+    pip install dist/*.whl
+
 * To install the latest from the master branch, run `pip install git+https://github.com/rthalley/dnspython.git`
 
 Dnspython's default installation does not depend on any modules other than
 those in the Python standard library.  To use some features, additional modules
 must be installed.  For convenience, pip options are defined for the
 requirements.
 
@@ -59,29 +66,26 @@
 If you want to use internationalized domain names (IDNA)
 functionality, you must run
 `pip install dnspython[idna]`
 
 If you want to use the Trio asynchronous I/O package, run
 `pip install dnspython[trio]`.
 
-If you want to use the Curio asynchronous I/O package, run
-`pip install dnspython[curio]`.
-
 If you want to use WMI on Windows to determine the active DNS settings
 instead of the default registry scanning method, run
 `pip install dnspython[wmi]`.
 
 If you want to try the experimental DNS-over-QUIC code, run
 `pip install dnspython[doq]`.
 
 Note that you can install any combination of the above, e.g.:
 `pip install dnspython[doh,dnssec,idna]`
 
 ### Notices
 
 Python 2.x support ended with the release of 1.16.0.  Dnspython 2.0.0 through
-2.2.x support Python 3.6 and later.  As of dnspython 2.3.0, the minimum
-supported Python version will be 3.7.  We plan to align future support with the
-lifetime of the Python 3 versions.
+2.2.x support Python 3.6 and later.  For dnspython 2.3.x, the minimum
+supported Python version is 3.7, and for 2.4.x the minimum supported verison is 3.8.
+We plan to align future support with the lifetime of the Python 3 versions.
 
 Documentation has moved to
 [dnspython.readthedocs.io](https://dnspython.readthedocs.io).
```

### Comparing `dnspython-2.3.0rc1/dns/__init__.py` & `dnspython-2.4.0rc1/dns/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 """dnspython DNS toolkit"""
 
 __all__ = [
     "asyncbackend",
     "asyncquery",
     "asyncresolver",
     "dnssec",
+    "dnssecalgs",
     "dnssectypes",
     "e164",
     "edns",
     "entropy",
     "exception",
     "flags",
     "immutable",
```

### Comparing `dnspython-2.3.0rc1/dns/_asyncbackend.py` & `dnspython-2.4.0rc1/dns/_asyncbackend.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 
     async def getpeername(self):
         raise NotImplementedError
 
     async def getsockname(self):
         raise NotImplementedError
 
+    async def getpeercert(self, timeout):
+        raise NotImplementedError
+
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
 
 
@@ -57,14 +60,19 @@
     async def sendall(self, what, timeout):
         raise NotImplementedError
 
     async def recv(self, size, timeout):
         raise NotImplementedError
 
 
+class NullTransport:
+    async def connect_tcp(self, host, port, timeout, local_address):
+        raise NotImplementedError
+
+
 class Backend:  # pragma: no cover
     def name(self):
         return "unknown"
 
     async def make_socket(
         self,
         af,
@@ -79,7 +87,10 @@
         raise NotImplementedError
 
     def datagram_connection_required(self):
         return False
 
     async def sleep(self, interval):
         raise NotImplementedError
+
+    def get_transport_class(self):
+        raise NotImplementedError
```

### Comparing `dnspython-2.3.0rc1/dns/_immutable_ctx.py` & `dnspython-2.4.0rc1/dns/_immutable_ctx.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # This implementation of the immutable decorator requires python >=
 # 3.7, and is significantly more storage efficient when making classes
 # with slots immutable.  It's also faster.
 
 import contextvars
 import inspect
 
-
 _in__init__ = contextvars.ContextVar("_immutable_in__init__", default=False)
 
 
 class _Immutable:
     """Immutable mixin class"""
 
     # We set slots to the empty list to say "we don't have any attributes".
```

### Comparing `dnspython-2.3.0rc1/dns/asyncbackend.py` & `dnspython-2.4.0rc1/dns/asyncbackend.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # Copyright (C) Dnspython Contributors, see LICENSE for text of ISC license
 
 from typing import Dict
 
 import dns.exception
 
 # pylint: disable=unused-import
-
-from dns._asyncbackend import (
-    Socket,
+from dns._asyncbackend import (  # noqa: F401  lgtm[py/unused-import]
+    Backend,
     DatagramSocket,
+    Socket,
     StreamSocket,
-    Backend,
-)  # noqa: F401  lgtm[py/unused-import]
+)
 
 # pylint: enable=unused-import
 
 _default_backend = None
 
 _backends: Dict[str, Backend] = {}
 
@@ -26,31 +25,27 @@
 class AsyncLibraryNotFoundError(dns.exception.DNSException):
     pass
 
 
 def get_backend(name: str) -> Backend:
     """Get the specified asynchronous backend.
 
-    *name*, a ``str``, the name of the backend.  Currently the "trio",
-    "curio", and "asyncio" backends are available.
+    *name*, a ``str``, the name of the backend.  Currently the "trio"
+    and "asyncio" backends are available.
 
     Raises NotImplementError if an unknown backend name is specified.
     """
     # pylint: disable=import-outside-toplevel,redefined-outer-name
     backend = _backends.get(name)
     if backend:
         return backend
     if name == "trio":
         import dns._trio_backend
 
         backend = dns._trio_backend.Backend()
-    elif name == "curio":
-        import dns._curio_backend
-
-        backend = dns._curio_backend.Backend()
     elif name == "asyncio":
         import dns._asyncio_backend
 
         backend = dns._asyncio_backend.Backend()
     else:
         raise NotImplementedError(f"unimplemented async backend {name}")
     _backends[name] = backend
@@ -69,17 +64,15 @@
         if _no_sniffio:
             raise ImportError
         import sniffio
 
         try:
             return sniffio.current_async_library()
         except sniffio.AsyncLibraryNotFoundError:
-            raise AsyncLibraryNotFoundError(
-                "sniffio cannot determine " + "async library"
-            )
+            raise AsyncLibraryNotFoundError("sniffio cannot determine async library")
     except ImportError:
         import asyncio
 
         try:
             asyncio.get_running_loop()
             return "asyncio"
         except RuntimeError:
```

### Comparing `dnspython-2.3.0rc1/dns/asyncquery.py` & `dnspython-2.4.0rc1/dns/asyncquery.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,47 +13,45 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """Talk to a DNS server."""
 
-from typing import Any, Dict, Optional, Tuple, Union
-
 import base64
 import contextlib
 import socket
 import struct
 import time
+from typing import Any, Dict, Optional, Tuple, Union
 
 import dns.asyncbackend
 import dns.exception
 import dns.inet
-import dns.name
 import dns.message
+import dns.name
 import dns.quic
 import dns.rcode
 import dns.rdataclass
 import dns.rdatatype
 import dns.transaction
-
 from dns._asyncbackend import NullContext
 from dns.query import (
-    _compute_times,
-    _matches_destination,
     BadResponse,
-    ssl,
-    UDPMode,
-    _have_httpx,
-    _have_http2,
     NoDOH,
     NoDOQ,
+    UDPMode,
+    _compute_times,
+    _have_http2,
+    _matches_destination,
+    have_doh,
+    ssl,
 )
 
-if _have_httpx:
+if have_doh:
     import httpx
 
 # for brevity
 _lltuple = dns.inet.low_level_address_tuple
 
 
 def _source_tuple(af, address, port):
@@ -491,46 +489,66 @@
     source_port: int = 0,  # pylint: disable=W0613
     one_rr_per_rrset: bool = False,
     ignore_trailing: bool = False,
     client: Optional["httpx.AsyncClient"] = None,
     path: str = "/dns-query",
     post: bool = True,
     verify: Union[bool, str] = True,
+    bootstrap_address: Optional[str] = None,
+    resolver: Optional["dns.asyncresolver.Resolver"] = None,
+    family: Optional[int] = socket.AF_UNSPEC,
 ) -> dns.message.Message:
     """Return the response obtained after sending a query via DNS-over-HTTPS.
 
     *client*, a ``httpx.AsyncClient``.  If provided, the client to use for
     the query.
 
     Unlike the other dnspython async functions, a backend cannot be provided
     in this function because httpx always auto-detects the async backend.
 
     See :py:func:`dns.query.https()` for the documentation of the other
     parameters, exceptions, and return type of this method.
     """
 
-    if not _have_httpx:
-        raise NoDOH("httpx is not available.")  # pragma: no cover
+    if not have_doh:
+        raise NoDOH  # pragma: no cover
+    if client and not isinstance(client, httpx.AsyncClient):
+        raise ValueError("session parameter must be an httpx.AsyncClient")
 
     wire = q.to_wire()
     try:
         af = dns.inet.af_for_address(where)
     except ValueError:
         af = None
     transport = None
     headers = {"accept": "application/dns-message"}
-    if af is not None:
+    if af is not None and dns.inet.is_address(where):
         if af == socket.AF_INET:
             url = "https://{}:{}{}".format(where, port, path)
         elif af == socket.AF_INET6:
             url = "https://[{}]:{}{}".format(where, port, path)
     else:
         url = where
-    if source is not None:
-        transport = httpx.AsyncHTTPTransport(local_address=source[0])
+
+    backend = dns.asyncbackend.get_default_backend()
+
+    if source is None:
+        local_address = None
+        local_port = 0
+    else:
+        local_address = source
+        local_port = source_port
+    transport = backend.get_transport_class()(
+        local_address=local_address,
+        verify=verify,
+        local_port=local_port,
+        bootstrap_address=bootstrap_address,
+        resolver=resolver,
+        family=family,
+    )
 
     if client:
         cm: contextlib.AbstractAsyncContextManager = NullContext(client)
     else:
         cm = httpx.AsyncClient(
             http1=True, http2=_have_http2, verify=verify, transport=transport
         )
@@ -686,14 +704,15 @@
     source: Optional[str] = None,
     source_port: int = 0,
     one_rr_per_rrset: bool = False,
     ignore_trailing: bool = False,
     connection: Optional[dns.quic.AsyncQuicConnection] = None,
     verify: Union[bool, str] = True,
     backend: Optional[dns.asyncbackend.Backend] = None,
+    server_hostname: Optional[str] = None,
 ) -> dns.message.Message:
     """Return the response obtained after sending an asynchronous query via
     DNS-over-QUIC.
 
     *backend*, a ``dns.asyncbackend.Backend``, or ``None``.  If ``None``,
     the default, then dnspython will use the default backend.
 
@@ -711,15 +730,17 @@
         cfactory = dns.quic.null_factory
         mfactory = dns.quic.null_factory
         the_connection = connection
     else:
         (cfactory, mfactory) = dns.quic.factories_for_backend(backend)
 
     async with cfactory() as context:
-        async with mfactory(context, verify_mode=verify) as the_manager:
+        async with mfactory(
+            context, verify_mode=verify, server_name=server_hostname
+        ) as the_manager:
             if not connection:
                 the_connection = the_manager.connect(where, port, source, source_port)
             start = time.time()
             stream = await the_connection.make_stream()
             async with stream:
                 await stream.send(wire, True)
                 wire = await stream.receive(timeout)
```

### Comparing `dnspython-2.3.0rc1/dns/dnssec.py` & `dnspython-2.4.0rc1/dns/dnssec.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,71 +13,68 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """Common DNSSEC-related functions and constants."""
 
-from typing import Any, cast, Dict, List, Optional, Set, Tuple, Union
 
+import base64
+import contextlib
+import functools
 import hashlib
-import math
 import struct
 import time
-import base64
 from datetime import datetime
-
-from dns.dnssectypes import Algorithm, DSDigest, NSEC3Hash
+from typing import Callable, Dict, List, Optional, Set, Tuple, Union, cast
 
 import dns.exception
 import dns.name
 import dns.node
-import dns.rdataset
 import dns.rdata
-import dns.rdatatype
 import dns.rdataclass
+import dns.rdataset
+import dns.rdatatype
 import dns.rrset
+import dns.transaction
+import dns.zone
+from dns.dnssectypes import Algorithm, DSDigest, NSEC3Hash
+from dns.exception import (  # pylint: disable=W0611
+    AlgorithmKeyMismatch,
+    DeniedByPolicy,
+    UnsupportedAlgorithm,
+    ValidationFailure,
+)
 from dns.rdtypes.ANY.CDNSKEY import CDNSKEY
 from dns.rdtypes.ANY.CDS import CDS
 from dns.rdtypes.ANY.DNSKEY import DNSKEY
 from dns.rdtypes.ANY.DS import DS
+from dns.rdtypes.ANY.NSEC import NSEC, Bitmap
+from dns.rdtypes.ANY.NSEC3PARAM import NSEC3PARAM
 from dns.rdtypes.ANY.RRSIG import RRSIG, sigtime_to_posixtime
 from dns.rdtypes.dnskeybase import Flag
 
-
-class UnsupportedAlgorithm(dns.exception.DNSException):
-    """The DNSSEC algorithm is not supported."""
-
-
-class AlgorithmKeyMismatch(UnsupportedAlgorithm):
-    """The DNSSEC algorithm is not supported for the given key type."""
-
-
-class ValidationFailure(dns.exception.DNSException):
-    """The DNSSEC signature is invalid."""
-
-
-class DeniedByPolicy(dns.exception.DNSException):
-    """Denied by DNSSEC policy."""
-
-
 PublicKey = Union[
+    "GenericPublicKey",
     "rsa.RSAPublicKey",
     "ec.EllipticCurvePublicKey",
     "ed25519.Ed25519PublicKey",
     "ed448.Ed448PublicKey",
 ]
 
 PrivateKey = Union[
+    "GenericPrivateKey",
     "rsa.RSAPrivateKey",
     "ec.EllipticCurvePrivateKey",
     "ed25519.Ed25519PrivateKey",
     "ed448.Ed448PrivateKey",
 ]
 
+RRsetSigner = Callable[[dns.transaction.Transaction, dns.rrset.RRset], None]
+
 
 def algorithm_from_text(text: str) -> Algorithm:
     """Convert text into a DNSSEC algorithm value.
 
     *text*, a ``str``, the text to convert to into an algorithm value.
 
     Returns an ``int``.
@@ -308,205 +305,30 @@
     return [
         cast(DNSKEY, rd)
         for rd in rdataset
         if rd.algorithm == rrsig.algorithm and key_id(rd) == rrsig.key_tag
     ]
 
 
-def _is_rsa(algorithm: int) -> bool:
-    return algorithm in (
-        Algorithm.RSAMD5,
-        Algorithm.RSASHA1,
-        Algorithm.RSASHA1NSEC3SHA1,
-        Algorithm.RSASHA256,
-        Algorithm.RSASHA512,
-    )
-
-
-def _is_dsa(algorithm: int) -> bool:
-    return algorithm in (Algorithm.DSA, Algorithm.DSANSEC3SHA1)
-
-
-def _is_ecdsa(algorithm: int) -> bool:
-    return algorithm in (Algorithm.ECDSAP256SHA256, Algorithm.ECDSAP384SHA384)
-
-
-def _is_eddsa(algorithm: int) -> bool:
-    return algorithm in (Algorithm.ED25519, Algorithm.ED448)
-
-
-def _is_gost(algorithm: int) -> bool:
-    return algorithm == Algorithm.ECCGOST
-
-
-def _is_md5(algorithm: int) -> bool:
-    return algorithm == Algorithm.RSAMD5
-
-
-def _is_sha1(algorithm: int) -> bool:
-    return algorithm in (
-        Algorithm.DSA,
-        Algorithm.RSASHA1,
-        Algorithm.DSANSEC3SHA1,
-        Algorithm.RSASHA1NSEC3SHA1,
-    )
-
-
-def _is_sha256(algorithm: int) -> bool:
-    return algorithm in (Algorithm.RSASHA256, Algorithm.ECDSAP256SHA256)
-
-
-def _is_sha384(algorithm: int) -> bool:
-    return algorithm == Algorithm.ECDSAP384SHA384
-
-
-def _is_sha512(algorithm: int) -> bool:
-    return algorithm == Algorithm.RSASHA512
-
-
-def _ensure_algorithm_key_combination(algorithm: int, key: PublicKey) -> None:
-    """Ensure algorithm is valid for key type, throwing an exception on
-    mismatch."""
-    if isinstance(key, rsa.RSAPublicKey):
-        if _is_rsa(algorithm):
-            return
-        raise AlgorithmKeyMismatch('algorithm "%s" not valid for RSA key' % algorithm)
-    if isinstance(key, dsa.DSAPublicKey):
-        if _is_dsa(algorithm):
-            return
-        raise AlgorithmKeyMismatch('algorithm "%s" not valid for DSA key' % algorithm)
-    if isinstance(key, ec.EllipticCurvePublicKey):
-        if _is_ecdsa(algorithm):
-            return
-        raise AlgorithmKeyMismatch('algorithm "%s" not valid for ECDSA key' % algorithm)
-    if isinstance(key, ed25519.Ed25519PublicKey):
-        if algorithm == Algorithm.ED25519:
-            return
-        raise AlgorithmKeyMismatch(
-            'algorithm "%s" not valid for ED25519 key' % algorithm
-        )
-    if isinstance(key, ed448.Ed448PublicKey):
-        if algorithm == Algorithm.ED448:
-            return
-        raise AlgorithmKeyMismatch('algorithm "%s" not valid for ED448 key' % algorithm)
-
-    raise TypeError("unsupported key type")
-
-
-def _make_hash(algorithm: int) -> Any:
-    if _is_md5(algorithm):
-        return hashes.MD5()
-    if _is_sha1(algorithm):
-        return hashes.SHA1()
-    if _is_sha256(algorithm):
-        return hashes.SHA256()
-    if _is_sha384(algorithm):
-        return hashes.SHA384()
-    if _is_sha512(algorithm):
-        return hashes.SHA512()
-    if algorithm == Algorithm.ED25519:
-        return hashes.SHA512()
-    if algorithm == Algorithm.ED448:
-        return hashes.SHAKE256(114)
-
-    raise ValidationFailure("unknown hash for algorithm %u" % algorithm)
-
-
-def _bytes_to_long(b: bytes) -> int:
-    return int.from_bytes(b, "big")
-
-
 def _get_rrname_rdataset(
     rrset: Union[dns.rrset.RRset, Tuple[dns.name.Name, dns.rdataset.Rdataset]],
 ) -> Tuple[dns.name.Name, dns.rdataset.Rdataset]:
     if isinstance(rrset, tuple):
         return rrset[0], rrset[1]
     else:
         return rrset.name, rrset
 
 
-def _validate_signature(sig: bytes, data: bytes, key: DNSKEY, chosen_hash: Any) -> None:
-    keyptr: bytes
-    if _is_rsa(key.algorithm):
-        # we ignore because mypy is confused and thinks key.key is a str for unknown
-        # reasons.
-        keyptr = key.key
-        (bytes_,) = struct.unpack("!B", keyptr[0:1])
-        keyptr = keyptr[1:]
-        if bytes_ == 0:
-            (bytes_,) = struct.unpack("!H", keyptr[0:2])
-            keyptr = keyptr[2:]
-        rsa_e = keyptr[0:bytes_]
-        rsa_n = keyptr[bytes_:]
-        try:
-            rsa_public_key = rsa.RSAPublicNumbers(
-                _bytes_to_long(rsa_e), _bytes_to_long(rsa_n)
-            ).public_key(default_backend())
-        except ValueError:
-            raise ValidationFailure("invalid public key")
-        rsa_public_key.verify(sig, data, padding.PKCS1v15(), chosen_hash)
-    elif _is_dsa(key.algorithm):
-        keyptr = key.key
-        (t,) = struct.unpack("!B", keyptr[0:1])
-        keyptr = keyptr[1:]
-        octets = 64 + t * 8
-        dsa_q = keyptr[0:20]
-        keyptr = keyptr[20:]
-        dsa_p = keyptr[0:octets]
-        keyptr = keyptr[octets:]
-        dsa_g = keyptr[0:octets]
-        keyptr = keyptr[octets:]
-        dsa_y = keyptr[0:octets]
-        try:
-            dsa_public_key = dsa.DSAPublicNumbers(  # type: ignore
-                _bytes_to_long(dsa_y),
-                dsa.DSAParameterNumbers(
-                    _bytes_to_long(dsa_p), _bytes_to_long(dsa_q), _bytes_to_long(dsa_g)
-                ),
-            ).public_key(default_backend())
-        except ValueError:
-            raise ValidationFailure("invalid public key")
-        dsa_public_key.verify(sig, data, chosen_hash)
-    elif _is_ecdsa(key.algorithm):
-        keyptr = key.key
-        curve: Any
-        if key.algorithm == Algorithm.ECDSAP256SHA256:
-            curve = ec.SECP256R1()
-            octets = 32
-        else:
-            curve = ec.SECP384R1()
-            octets = 48
-        ecdsa_x = keyptr[0:octets]
-        ecdsa_y = keyptr[octets : octets * 2]
-        try:
-            ecdsa_public_key = ec.EllipticCurvePublicNumbers(
-                curve=curve, x=_bytes_to_long(ecdsa_x), y=_bytes_to_long(ecdsa_y)
-            ).public_key(default_backend())
-        except ValueError:
-            raise ValidationFailure("invalid public key")
-        ecdsa_public_key.verify(sig, data, ec.ECDSA(chosen_hash))
-    elif _is_eddsa(key.algorithm):
-        keyptr = key.key
-        loader: Any
-        if key.algorithm == Algorithm.ED25519:
-            loader = ed25519.Ed25519PublicKey
-        else:
-            loader = ed448.Ed448PublicKey
-        try:
-            eddsa_public_key = loader.from_public_bytes(keyptr)
-        except ValueError:
-            raise ValidationFailure("invalid public key")
-        eddsa_public_key.verify(sig, data)
-    elif _is_gost(key.algorithm):
-        raise UnsupportedAlgorithm(
-            'algorithm "%s" not supported by dnspython'
-            % algorithm_to_text(key.algorithm)
-        )
-    else:
-        raise ValidationFailure("unknown algorithm %u" % key.algorithm)
+def _validate_signature(sig: bytes, data: bytes, key: DNSKEY) -> None:
+    public_cls = get_algorithm_cls_from_dnskey(key).public_cls
+    try:
+        public_key = public_cls.from_dnskey(key)
+    except ValueError:
+        raise ValidationFailure("invalid public key")
+    public_key.verify(sig, data)
 
 
 def _validate_rrsig(
     rrset: Union[dns.rrset.RRset, Tuple[dns.name.Name, dns.rdataset.Rdataset]],
     rrsig: RRSIG,
     keys: Dict[dns.name.Name, Union[dns.node.Node, dns.rdataset.Rdataset]],
     origin: Optional[dns.name.Name] = None,
@@ -555,37 +377,21 @@
     if now is None:
         now = time.time()
     if rrsig.expiration < now:
         raise ValidationFailure("expired")
     if rrsig.inception > now:
         raise ValidationFailure("not yet valid")
 
-    if _is_dsa(rrsig.algorithm):
-        sig_r = rrsig.signature[1:21]
-        sig_s = rrsig.signature[21:]
-        sig = utils.encode_dss_signature(_bytes_to_long(sig_r), _bytes_to_long(sig_s))
-    elif _is_ecdsa(rrsig.algorithm):
-        if rrsig.algorithm == Algorithm.ECDSAP256SHA256:
-            octets = 32
-        else:
-            octets = 48
-        sig_r = rrsig.signature[0:octets]
-        sig_s = rrsig.signature[octets:]
-        sig = utils.encode_dss_signature(_bytes_to_long(sig_r), _bytes_to_long(sig_s))
-    else:
-        sig = rrsig.signature
-
     data = _make_rrsig_signature_data(rrset, rrsig, origin)
-    chosen_hash = _make_hash(rrsig.algorithm)
 
     for candidate_key in candidate_keys:
         if not policy.ok_to_validate(candidate_key):
             continue
         try:
-            _validate_signature(sig, data, candidate_key, chosen_hash)
+            _validate_signature(rrsig.signature, data, candidate_key)
             return
         except (InvalidSignature, ValidationFailure):
             # this happens on an individual validation failure
             continue
     # nothing verified -- raise failure:
     raise ValidationFailure("verify failure")
 
@@ -669,14 +475,15 @@
     signer: dns.name.Name,
     dnskey: DNSKEY,
     inception: Optional[Union[datetime, str, int, float]] = None,
     expiration: Optional[Union[datetime, str, int, float]] = None,
     lifetime: Optional[int] = None,
     verify: bool = False,
     policy: Optional[Policy] = None,
+    origin: Optional[dns.name.Name] = None,
 ) -> RRSIG:
     """Sign RRset using private key.
 
     *rrset*, the RRset to validate.  This can be a
     ``dns.rrset.RRset`` or a (``dns.name.Name``, ``dns.rdataset.Rdataset``)
     tuple.
 
@@ -704,14 +511,18 @@
 
     *verify*, a ``bool``.  If set to ``True``, the signer will verify signatures
     after they are created; the default is ``False``.
 
     *policy*, a ``dns.dnssec.Policy`` or ``None``.  If ``None``, the default policy,
     ``dns.dnssec.default_policy`` is used; this policy defaults to that of RFC 8624.
 
+    *origin*, a ``dns.name.Name`` or ``None``.  If ``None``, the default, then all
+    names in the rrset (including its owner name) must be absolute; otherwise the
+    specified origin will be used to make names absolute when signing.
+
     Raises ``DeniedByPolicy`` if the signature is denied by policy.
     """
 
     if policy is None:
         policy = default_policy
     if not policy.ok_to_sign(dnskey):
         raise DeniedByPolicy
@@ -735,85 +546,50 @@
     if expiration is not None:
         rrsig_expiration = to_timestamp(expiration)
     elif lifetime is not None:
         rrsig_expiration = int(time.time()) + lifetime
     else:
         raise ValueError("expiration or lifetime must be specified")
 
+    # Derelativize now because we need a correct labels length for the
+    # rrsig_template.
+    if origin is not None:
+        rrname = rrname.derelativize(origin)
+    labels = len(rrname) - 1
+
+    # Adjust labels appropriately for wildcards.
+    if rrname.is_wild():
+        labels -= 1
+
     rrsig_template = RRSIG(
         rdclass=rdclass,
         rdtype=dns.rdatatype.RRSIG,
         type_covered=rdtype,
         algorithm=dnskey.algorithm,
-        labels=len(rrname) - 1,
+        labels=labels,
         original_ttl=original_ttl,
         expiration=rrsig_expiration,
         inception=rrsig_inception,
         key_tag=key_id(dnskey),
         signer=signer,
         signature=b"",
     )
 
-    data = dns.dnssec._make_rrsig_signature_data(rrset, rrsig_template)
-    chosen_hash = _make_hash(rrsig_template.algorithm)
-    signature = None
-
-    if isinstance(private_key, rsa.RSAPrivateKey):
-        if not _is_rsa(dnskey.algorithm):
-            raise ValueError("Invalid DNSKEY algorithm for RSA key")
-        signature = private_key.sign(data, padding.PKCS1v15(), chosen_hash)
-        if verify:
-            private_key.public_key().verify(
-                signature, data, padding.PKCS1v15(), chosen_hash
-            )
-    elif isinstance(private_key, dsa.DSAPrivateKey):
-        if not _is_dsa(dnskey.algorithm):
-            raise ValueError("Invalid DNSKEY algorithm for DSA key")
-        public_dsa_key = private_key.public_key()
-        if public_dsa_key.key_size > 1024:
-            raise ValueError("DSA key size overflow")
-        der_signature = private_key.sign(data, chosen_hash)
-        if verify:
-            public_dsa_key.verify(der_signature, data, chosen_hash)
-        dsa_r, dsa_s = utils.decode_dss_signature(der_signature)
-        dsa_t = (public_dsa_key.key_size // 8 - 64) // 8
-        octets = 20
-        signature = (
-            struct.pack("!B", dsa_t)
-            + int.to_bytes(dsa_r, length=octets, byteorder="big")
-            + int.to_bytes(dsa_s, length=octets, byteorder="big")
-        )
-    elif isinstance(private_key, ec.EllipticCurvePrivateKey):
-        if not _is_ecdsa(dnskey.algorithm):
-            raise ValueError("Invalid DNSKEY algorithm for EC key")
-        der_signature = private_key.sign(data, ec.ECDSA(chosen_hash))
-        if verify:
-            private_key.public_key().verify(der_signature, data, ec.ECDSA(chosen_hash))
-        if dnskey.algorithm == Algorithm.ECDSAP256SHA256:
-            octets = 32
-        else:
-            octets = 48
-        dsa_r, dsa_s = utils.decode_dss_signature(der_signature)
-        signature = int.to_bytes(dsa_r, length=octets, byteorder="big") + int.to_bytes(
-            dsa_s, length=octets, byteorder="big"
-        )
-    elif isinstance(private_key, ed25519.Ed25519PrivateKey):
-        if dnskey.algorithm != Algorithm.ED25519:
-            raise ValueError("Invalid DNSKEY algorithm for ED25519 key")
-        signature = private_key.sign(data)
-        if verify:
-            private_key.public_key().verify(signature, data)
-    elif isinstance(private_key, ed448.Ed448PrivateKey):
-        if dnskey.algorithm != Algorithm.ED448:
-            raise ValueError("Invalid DNSKEY algorithm for ED448 key")
-        signature = private_key.sign(data)
-        if verify:
-            private_key.public_key().verify(signature, data)
+    data = dns.dnssec._make_rrsig_signature_data(rrset, rrsig_template, origin)
+
+    if isinstance(private_key, GenericPrivateKey):
+        signing_key = private_key
     else:
-        raise TypeError("Unsupported key algorithm")
+        try:
+            private_cls = get_algorithm_cls_from_dnskey(dnskey)
+            signing_key = private_cls(key=private_key)
+        except UnsupportedAlgorithm:
+            raise TypeError("Unsupported key algorithm")
+
+    signature = signing_key.sign(data, verify)
 
     return cast(RRSIG, rrsig_template.replace(signature=signature))
 
 
 def _make_rrsig_signature_data(
     rrset: Union[dns.rrset.RRset, Tuple[dns.name.Name, dns.rdataset.Rdataset]],
     rrsig: RRSIG,
@@ -854,17 +630,20 @@
 
     # Derelativize the name before considering labels.
     if not rrname.is_absolute():
         if origin is None:
             raise ValidationFailure("relative RR name without an origin specified")
         rrname = rrname.derelativize(origin)
 
-    if len(rrname) - 1 < rrsig.labels:
+    name_len = len(rrname)
+    if rrname.is_wild() and rrsig.labels != name_len - 2:
+        raise ValidationFailure("wild owner name has wrong label length")
+    if name_len - 1 < rrsig.labels:
         raise ValidationFailure("owner name longer than RRSIG labels")
-    elif rrsig.labels < len(rrname) - 1:
+    elif rrsig.labels < name_len - 1:
         suffix = rrname.split(rrsig.labels + 1)[1]
         rrname = dns.name.from_text("*", suffix)
     rrnamebuf = rrname.to_digestable()
     rrfixed = struct.pack("!HHI", rdataset.rdtype, rdataset.rdclass, rrsig.original_ttl)
     rdatas = [rdata.to_digestable(origin) for rdata in rdataset]
     for rdata in sorted(rdatas):
         data += rrnamebuf
@@ -880,17 +659,16 @@
     public_key: PublicKey,
     algorithm: Union[int, str],
     flags: int = Flag.ZONE,
     protocol: int = 3,
 ) -> DNSKEY:
     """Convert a public key to DNSKEY Rdata
 
-    *public_key*, the public key to convert, a
-    ``cryptography.hazmat.primitives.asymmetric`` public key class applicable
-    for DNSSEC.
+    *public_key*, a ``PublicKey`` (``GenericPublicKey`` or
+    ``cryptography.hazmat.primitives.asymmetric``) to convert.
 
     *algorithm*, a ``str`` or ``int`` specifying the DNSKEY algorithm.
 
     *flags*: DNSKEY flags field as an integer.
 
     *protocol*: DNSKEY protocol field as an integer.
 
@@ -898,80 +676,21 @@
     unsupported, ``TypeError`` if the key type is unsupported,
     `UnsupportedAlgorithm` if the algorithm is unknown and
     `AlgorithmKeyMismatch` if the algorithm does not match the key type.
 
     Return DNSKEY ``Rdata``.
     """
 
-    def encode_rsa_public_key(public_key: "rsa.RSAPublicKey") -> bytes:
-        """Encode a public key per RFC 3110, section 2."""
-        pn = public_key.public_numbers()
-        _exp_len = math.ceil(int.bit_length(pn.e) / 8)
-        exp = int.to_bytes(pn.e, length=_exp_len, byteorder="big")
-        if _exp_len > 255:
-            exp_header = b"\0" + struct.pack("!H", _exp_len)
-        else:
-            exp_header = struct.pack("!B", _exp_len)
-        if pn.n.bit_length() < 512 or pn.n.bit_length() > 4096:
-            raise ValueError("unsupported RSA key length")
-        return exp_header + exp + pn.n.to_bytes((pn.n.bit_length() + 7) // 8, "big")
-
-    def encode_dsa_public_key(public_key: "dsa.DSAPublicKey") -> bytes:
-        """Encode a public key per RFC 2536, section 2."""
-        pn = public_key.public_numbers()
-        dsa_t = (public_key.key_size // 8 - 64) // 8
-        if dsa_t > 8:
-            raise ValueError("unsupported DSA key size")
-        octets = 64 + dsa_t * 8
-        res = struct.pack("!B", dsa_t)
-        res += pn.parameter_numbers.q.to_bytes(20, "big")
-        res += pn.parameter_numbers.p.to_bytes(octets, "big")
-        res += pn.parameter_numbers.g.to_bytes(octets, "big")
-        res += pn.y.to_bytes(octets, "big")
-        return res
-
-    def encode_ecdsa_public_key(public_key: "ec.EllipticCurvePublicKey") -> bytes:
-        """Encode a public key per RFC 6605, section 4."""
-        pn = public_key.public_numbers()
-        if isinstance(public_key.curve, ec.SECP256R1):
-            return pn.x.to_bytes(32, "big") + pn.y.to_bytes(32, "big")
-        elif isinstance(public_key.curve, ec.SECP384R1):
-            return pn.x.to_bytes(48, "big") + pn.y.to_bytes(48, "big")
-        else:
-            raise ValueError("unsupported ECDSA curve")
-
-    the_algorithm = Algorithm.make(algorithm)
+    algorithm = Algorithm.make(algorithm)
 
-    _ensure_algorithm_key_combination(the_algorithm, public_key)
-
-    if isinstance(public_key, rsa.RSAPublicKey):
-        key_bytes = encode_rsa_public_key(public_key)
-    elif isinstance(public_key, dsa.DSAPublicKey):
-        key_bytes = encode_dsa_public_key(public_key)
-    elif isinstance(public_key, ec.EllipticCurvePublicKey):
-        key_bytes = encode_ecdsa_public_key(public_key)
-    elif isinstance(public_key, ed25519.Ed25519PublicKey):
-        key_bytes = public_key.public_bytes(
-            encoding=serialization.Encoding.Raw, format=serialization.PublicFormat.Raw
-        )
-    elif isinstance(public_key, ed448.Ed448PublicKey):
-        key_bytes = public_key.public_bytes(
-            encoding=serialization.Encoding.Raw, format=serialization.PublicFormat.Raw
-        )
+    if isinstance(public_key, GenericPublicKey):
+        return public_key.to_dnskey(flags=flags, protocol=protocol)
     else:
-        raise TypeError("unsupported key algorithm")
-
-    return DNSKEY(
-        rdclass=dns.rdataclass.IN,
-        rdtype=dns.rdatatype.DNSKEY,
-        flags=flags,
-        protocol=protocol,
-        algorithm=the_algorithm,
-        key=key_bytes,
-    )
+        public_cls = get_algorithm_cls(algorithm).public_cls
+        return public_cls(key=public_key).to_dnskey(flags=flags, protocol=protocol)
 
 
 def _make_cdnskey(
     public_key: PublicKey,
     algorithm: Union[int, str],
     flags: int = Flag.ZONE,
     protocol: int = 3,
@@ -1212,31 +931,260 @@
                 algorithm=rdata.algorithm,
                 key=rdata.key,
             )
         )
     return dns.rdataset.from_rdata_list(rdataset.ttl, res)
 
 
+def default_rrset_signer(
+    txn: dns.transaction.Transaction,
+    rrset: dns.rrset.RRset,
+    signer: dns.name.Name,
+    ksks: List[Tuple[PrivateKey, DNSKEY]],
+    zsks: List[Tuple[PrivateKey, DNSKEY]],
+    inception: Optional[Union[datetime, str, int, float]] = None,
+    expiration: Optional[Union[datetime, str, int, float]] = None,
+    lifetime: Optional[int] = None,
+    policy: Optional[Policy] = None,
+    origin: Optional[dns.name.Name] = None,
+) -> None:
+    """Default RRset signer"""
+
+    if rrset.rdtype in set(
+        [
+            dns.rdatatype.RdataType.DNSKEY,
+            dns.rdatatype.RdataType.CDS,
+            dns.rdatatype.RdataType.CDNSKEY,
+        ]
+    ):
+        keys = ksks
+    else:
+        keys = zsks
+
+    for private_key, dnskey in keys:
+        rrsig = dns.dnssec.sign(
+            rrset=rrset,
+            private_key=private_key,
+            dnskey=dnskey,
+            inception=inception,
+            expiration=expiration,
+            lifetime=lifetime,
+            signer=signer,
+            policy=policy,
+            origin=origin,
+        )
+        txn.add(rrset.name, rrset.ttl, rrsig)
+
+
+def sign_zone(
+    zone: dns.zone.Zone,
+    txn: Optional[dns.transaction.Transaction] = None,
+    keys: Optional[List[Tuple[PrivateKey, DNSKEY]]] = None,
+    add_dnskey: bool = True,
+    dnskey_ttl: Optional[int] = None,
+    inception: Optional[Union[datetime, str, int, float]] = None,
+    expiration: Optional[Union[datetime, str, int, float]] = None,
+    lifetime: Optional[int] = None,
+    nsec3: Optional[NSEC3PARAM] = None,
+    rrset_signer: Optional[RRsetSigner] = None,
+    policy: Optional[Policy] = None,
+) -> None:
+    """Sign zone.
+
+    *zone*, a ``dns.zone.Zone``, the zone to sign.
+
+    *txn*, a ``dns.transaction.Transaction``, an optional transaction to use for
+    signing.
+
+    *keys*, a list of (``PrivateKey``, ``DNSKEY``) tuples, to use for signing. KSK/ZSK
+    roles are assigned automatically if the SEP flag is used, otherwise all RRsets are
+    signed by all keys.
+
+    *add_dnskey*, a ``bool``.  If ``True``, the default, all specified DNSKEYs are
+    automatically added to the zone on signing.
+
+    *dnskey_ttl*, a``int``, specifies the TTL for DNSKEY RRs. If not specified the TTL
+    of the existing DNSKEY RRset used or the TTL of the SOA RRset.
+
+    *inception*, a ``datetime``, ``str``, ``int``, ``float`` or ``None``, the signature
+    inception time.  If ``None``, the current time is used.  If a ``str``, the format is
+    "YYYYMMDDHHMMSS" or alternatively the number of seconds since the UNIX epoch in text
+    form; this is the same the RRSIG rdata's text form. Values of type `int` or `float`
+    are interpreted as seconds since the UNIX epoch.
+
+    *expiration*, a ``datetime``, ``str``, ``int``, ``float`` or ``None``, the signature
+    expiration time.  If ``None``, the expiration time will be the inception time plus
+    the value of the *lifetime* parameter.  See the description of *inception* above for
+    how the various parameter types are interpreted.
+
+    *lifetime*, an ``int`` or ``None``, the signature lifetime in seconds.  This
+    parameter is only meaningful if *expiration* is ``None``.
+
+    *nsec3*, a ``NSEC3PARAM`` Rdata, configures signing using NSEC3. Not yet
+    implemented.
+
+    *rrset_signer*, a ``Callable``, an optional function for signing RRsets. The
+    function requires two arguments: transaction and RRset. If the not specified,
+    ``dns.dnssec.default_rrset_signer`` will be used.
+
+    Returns ``None``.
+    """
+
+    ksks = []
+    zsks = []
+
+    # if we have both KSKs and ZSKs, split by SEP flag. if not, sign all
+    # records with all keys
+    if keys:
+        for key in keys:
+            if key[1].flags & Flag.SEP:
+                ksks.append(key)
+            else:
+                zsks.append(key)
+        if not ksks:
+            ksks = keys
+        if not zsks:
+            zsks = keys
+    else:
+        keys = []
+
+    if txn:
+        cm: contextlib.AbstractContextManager = contextlib.nullcontext(txn)
+    else:
+        cm = zone.writer()
+
+    with cm as _txn:
+        if add_dnskey:
+            if dnskey_ttl is None:
+                dnskey = _txn.get(zone.origin, dns.rdatatype.DNSKEY)
+                if dnskey:
+                    dnskey_ttl = dnskey.ttl
+                else:
+                    soa = _txn.get(zone.origin, dns.rdatatype.SOA)
+                    dnskey_ttl = soa.ttl
+            for _, dnskey in keys:
+                _txn.add(zone.origin, dnskey_ttl, dnskey)
+
+        if nsec3:
+            raise NotImplementedError("Signing with NSEC3 not yet implemented")
+        else:
+            _rrset_signer = rrset_signer or functools.partial(
+                default_rrset_signer,
+                signer=zone.origin,
+                ksks=ksks,
+                zsks=zsks,
+                inception=inception,
+                expiration=expiration,
+                lifetime=lifetime,
+                policy=policy,
+                origin=zone.origin,
+            )
+            return _sign_zone_nsec(zone, _txn, _rrset_signer)
+
+
+def _sign_zone_nsec(
+    zone: dns.zone.Zone,
+    txn: dns.transaction.Transaction,
+    rrset_signer: Optional[RRsetSigner] = None,
+) -> None:
+    """NSEC zone signer"""
+
+    def _txn_add_nsec(
+        txn: dns.transaction.Transaction,
+        name: dns.name.Name,
+        next_secure: Optional[dns.name.Name],
+        rdclass: dns.rdataclass.RdataClass,
+        ttl: int,
+        rrset_signer: Optional[RRsetSigner] = None,
+    ) -> None:
+        """NSEC zone signer helper"""
+        mandatory_types = set(
+            [dns.rdatatype.RdataType.RRSIG, dns.rdatatype.RdataType.NSEC]
+        )
+        node = txn.get_node(name)
+        if node and next_secure:
+            types = (
+                set([rdataset.rdtype for rdataset in node.rdatasets]) | mandatory_types
+            )
+            windows = Bitmap.from_rdtypes(list(types))
+            rrset = dns.rrset.from_rdata(
+                name,
+                ttl,
+                NSEC(
+                    rdclass=rdclass,
+                    rdtype=dns.rdatatype.RdataType.NSEC,
+                    next=next_secure,
+                    windows=windows,
+                ),
+            )
+            txn.add(rrset)
+            if rrset_signer:
+                rrset_signer(txn, rrset)
+
+    rrsig_ttl = zone.get_soa().minimum
+    delegation = None
+    last_secure = None
+
+    for name in sorted(txn.iterate_names()):
+        if delegation and name.is_subdomain(delegation):
+            # names below delegations are not secure
+            continue
+        elif txn.get(name, dns.rdatatype.NS) and name != zone.origin:
+            # inside delegation
+            delegation = name
+        else:
+            # outside delegation
+            delegation = None
+
+        if rrset_signer:
+            node = txn.get_node(name)
+            if node:
+                for rdataset in node.rdatasets:
+                    if rdataset.rdtype == dns.rdatatype.RRSIG:
+                        # do not sign RRSIGs
+                        continue
+                    elif delegation and rdataset.rdtype != dns.rdatatype.DS:
+                        # do not sign delegations except DS records
+                        continue
+                    else:
+                        rrset = dns.rrset.from_rdata(name, rdataset.ttl, *rdataset)
+                        rrset_signer(txn, rrset)
+
+        # We need "is not None" as the empty name is False because its length is 0.
+        if last_secure is not None:
+            _txn_add_nsec(txn, last_secure, name, zone.rdclass, rrsig_ttl, rrset_signer)
+        last_secure = name
+
+    if last_secure:
+        _txn_add_nsec(
+            txn, last_secure, zone.origin, zone.rdclass, rrsig_ttl, rrset_signer
+        )
+
+
 def _need_pyca(*args, **kwargs):
     raise ImportError(
-        "DNSSEC validation requires " + "python cryptography"
+        "DNSSEC validation requires python cryptography"
     )  # pragma: no cover
 
 
 try:
     from cryptography.exceptions import InvalidSignature
-    from cryptography.hazmat.backends import default_backend
-    from cryptography.hazmat.primitives import hashes, serialization
-    from cryptography.hazmat.primitives.asymmetric import padding
-    from cryptography.hazmat.primitives.asymmetric import utils
-    from cryptography.hazmat.primitives.asymmetric import dsa
-    from cryptography.hazmat.primitives.asymmetric import ec
-    from cryptography.hazmat.primitives.asymmetric import ed25519
-    from cryptography.hazmat.primitives.asymmetric import ed448
-    from cryptography.hazmat.primitives.asymmetric import rsa
+    from cryptography.hazmat.primitives.asymmetric import dsa  # pylint: disable=W0611
+    from cryptography.hazmat.primitives.asymmetric import ec  # pylint: disable=W0611
+    from cryptography.hazmat.primitives.asymmetric import ed448  # pylint: disable=W0611
+    from cryptography.hazmat.primitives.asymmetric import rsa  # pylint: disable=W0611
+    from cryptography.hazmat.primitives.asymmetric import (  # pylint: disable=W0611
+        ed25519,
+    )
+
+    from dns.dnssecalgs import (  # pylint: disable=C0412
+        get_algorithm_cls,
+        get_algorithm_cls_from_dnskey,
+    )
+    from dns.dnssecalgs.base import GenericPrivateKey, GenericPublicKey
 except ImportError:  # pragma: no cover
     validate = _need_pyca
     validate_rrsig = _need_pyca
     sign = _need_pyca
     make_dnskey = _need_pyca
     make_cdnskey = _need_pyca
     _have_pyca = False
```

### Comparing `dnspython-2.3.0rc1/dns/dnssectypes.py` & `dnspython-2.4.0rc1/dns/dnssectypes.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/e164.py` & `dnspython-2.4.0rc1/dns/e164.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/edns.py` & `dnspython-2.4.0rc1/dns/edns.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,19 +13,18 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """EDNS Options"""
 
-from typing import Any, Dict, Optional, Union
-
 import math
 import socket
 import struct
+from typing import Any, Dict, Optional, Union
 
 import dns.enum
 import dns.inet
 import dns.rdata
 import dns.wire
 
 
@@ -376,25 +375,25 @@
         else:
             return value
 
     @classmethod
     def from_wire_parser(
         cls, otype: Union[OptionType, str], parser: "dns.wire.Parser"
     ) -> Option:
-        the_code = EDECode.make(parser.get_uint16())
+        code = EDECode.make(parser.get_uint16())
         text = parser.get_remaining()
 
         if text:
             if text[-1] == 0:  # text MAY be null-terminated
                 text = text[:-1]
             btext = text.decode("utf8")
         else:
             btext = None
 
-        return cls(the_code, btext)
+        return cls(code, btext)
 
 
 _type_to_class: Dict[OptionType, Any] = {
     OptionType.ECS: ECSOption,
     OptionType.EDE: EDEOption,
 }
 
@@ -420,16 +419,16 @@
     *otype*, an ``int``, is the option type.
 
     *parser*, a ``dns.wire.Parser``, the parser, which should be
     restricted to the option length.
 
     Returns an instance of a subclass of ``dns.edns.Option``.
     """
-    the_otype = OptionType.make(otype)
-    cls = get_option_class(the_otype)
+    otype = OptionType.make(otype)
+    cls = get_option_class(otype)
     return cls.from_wire_parser(otype, parser)
 
 
 def option_from_wire(
     otype: Union[OptionType, str], wire: bytes, current: int, olen: int
 ) -> Option:
     """Build an EDNS option object from wire format.
```

### Comparing `dnspython-2.3.0rc1/dns/entropy.py` & `dnspython-2.4.0rc1/dns/entropy.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,25 +11,23 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-from typing import Any, Optional
-
-import os
 import hashlib
+import os
 import random
 import threading
 import time
+from typing import Any, Optional
 
 
 class EntropyPool:
-
     # This is an entropy pool for Python implementations that do not
     # have a working SystemRandom.  I'm not sure there are any, but
     # leaving this code doesn't hurt anything as the library code
     # is used if present.
 
     def __init__(self, seed: Optional[bytes] = None):
         self.pool_index = 0
```

### Comparing `dnspython-2.3.0rc1/dns/enum.py` & `dnspython-2.4.0rc1/dns/enum.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,26 +12,39 @@
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 import enum
+from typing import Type, TypeVar, Union
+
+TIntEnum = TypeVar("TIntEnum", bound="IntEnum")
 
 
 class IntEnum(enum.IntEnum):
     @classmethod
+    def _missing_(cls, value):
+        cls._check_value(value)
+        val = int.__new__(cls, value)
+        val._name_ = cls._extra_to_text(value, None) or f"{cls._prefix()}{value}"
+        val._value_ = value
+        return val
+
+    @classmethod
     def _check_value(cls, value):
         max = cls._maximum()
+        if not isinstance(value, int):
+            raise TypeError
         if value < 0 or value > max:
             name = cls._short_name()
-            raise ValueError(f"{name} must be between >= 0 and <= {max}")
+            raise ValueError(f"{name} must be an int between >= 0 and <= {max}")
 
     @classmethod
-    def from_text(cls, text):
+    def from_text(cls: Type[TIntEnum], text: str) -> TIntEnum:
         text = text.upper()
         try:
             return cls[text]
         except KeyError:
             pass
         value = cls._extra_from_text(text)
         if value:
@@ -43,27 +56,27 @@
             try:
                 return cls(value)
             except ValueError:
                 return value
         raise cls._unknown_exception_class()
 
     @classmethod
-    def to_text(cls, value):
+    def to_text(cls: Type[TIntEnum], value: int) -> str:
         cls._check_value(value)
         try:
             text = cls(value).name
         except ValueError:
             text = None
         text = cls._extra_to_text(value, text)
         if text is None:
             text = f"{cls._prefix()}{value}"
         return text
 
     @classmethod
-    def make(cls, value):
+    def make(cls: Type[TIntEnum], value: Union[int, str]) -> TIntEnum:
         """Convert text or a value into an enumerated type, if possible.
 
         *value*, the ``int`` or ``str`` to convert.
 
         Raises a class-specific exception if a ``str`` is provided that
         cannot be converted.
 
@@ -72,18 +85,15 @@
         Returns an enumeration from the calling class corresponding to the
         value, if one is defined, or an ``int`` otherwise.
         """
 
         if isinstance(value, str):
             return cls.from_text(value)
         cls._check_value(value)
-        try:
-            return cls(value)
-        except ValueError:
-            return value
+        return cls(value)
 
     @classmethod
     def _maximum(cls):
         raise NotImplementedError  # pragma: no cover
 
     @classmethod
     def _short_name(cls):
```

### Comparing `dnspython-2.3.0rc1/dns/exception.py` & `dnspython-2.4.0rc1/dns/exception.py`

 * *Files 12% similar despite different names*

```diff
@@ -136,14 +136,30 @@
 
     # We do this as otherwise mypy complains about unexpected keyword argument
     # idna_exception
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
+class UnsupportedAlgorithm(DNSException):
+    """The DNSSEC algorithm is not supported."""
+
+
+class AlgorithmKeyMismatch(UnsupportedAlgorithm):
+    """The DNSSEC algorithm is not supported for the given key type."""
+
+
+class ValidationFailure(DNSException):
+    """The DNSSEC signature is invalid."""
+
+
+class DeniedByPolicy(DNSException):
+    """Denied by DNSSEC policy."""
+
+
 class ExceptionWrapper:
     def __init__(self, exception_class):
         self.exception_class = exception_class
 
     def __enter__(self):
         return self
```

### Comparing `dnspython-2.3.0rc1/dns/flags.py` & `dnspython-2.4.0rc1/dns/flags.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,16 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """DNS Message Flags."""
 
-from typing import Any
-
 import enum
+from typing import Any
 
 # Standard DNS flags
 
 
 class Flag(enum.IntFlag):
     #: Query Response
     QR = 0x8000
```

### Comparing `dnspython-2.3.0rc1/dns/grange.py` & `dnspython-2.4.0rc1/dns/grange.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/immutable.py` & `dnspython-2.4.0rc1/dns/immutable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright (C) Dnspython Contributors, see LICENSE for text of ISC license
 
-from typing import Any
-
 import collections.abc
+from typing import Any
 
 from dns._immutable_ctx import immutable
 
 
 @immutable
 class Dict(collections.abc.Mapping):  # lgtm[py/missing-equals]
     def __init__(self, dictionary: Any, no_copy: bool = False):
```

### Comparing `dnspython-2.3.0rc1/dns/inet.py` & `dnspython-2.4.0rc1/dns/inet.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,22 +13,20 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """Generic Internet address helper functions."""
 
-from typing import Any, Optional, Tuple
-
 import socket
+from typing import Any, Optional, Tuple
 
 import dns.ipv4
 import dns.ipv6
 
-
 # We assume that AF_INET and AF_INET6 are always defined.  We keep
 # these here for the benefit of any old code (unlikely though that
 # is!).
 AF_INET = socket.AF_INET
 AF_INET6 = socket.AF_INET6
 
 
@@ -167,7 +165,16 @@
             return (addrpart, port, 0, socket.if_nametoindex(scope))
         except AttributeError:  # pragma: no cover  (we can't really test this)
             ai_flags = socket.AI_NUMERICHOST
             ((*_, tup), *_) = socket.getaddrinfo(address, port, flags=ai_flags)
             return tup
     else:
         raise NotImplementedError(f"unknown address family {af}")
+
+
+def any_for_af(af):
+    """Return the 'any' address for the specified address family."""
+    if af == socket.AF_INET:
+        return "0.0.0.0"
+    elif af == socket.AF_INET6:
+        return "::"
+    raise NotImplementedError(f"unknown address family {af}")
```

### Comparing `dnspython-2.3.0rc1/dns/ipv4.py` & `dnspython-2.4.0rc1/dns/ipv4.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,16 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """IPv4 helper functions."""
 
-from typing import Union
-
 import struct
+from typing import Union
 
 import dns.exception
 
 
 def inet_ntoa(address: bytes) -> str:
     """Convert an IPv4 address in binary form to text form.
```

### Comparing `dnspython-2.3.0rc1/dns/ipv6.py` & `dnspython-2.4.0rc1/dns/ipv6.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,17 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """IPv6 helper functions."""
 
-from typing import List, Union
-
-import re
 import binascii
+import re
+from typing import List, Union
 
 import dns.exception
 import dns.ipv4
 
 _leading_zero = re.compile(r"0+([0-9a-f]+)")
```

### Comparing `dnspython-2.3.0rc1/dns/message.py` & `dnspython-2.4.0rc1/dns/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,38 +13,37 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """DNS Messages"""
 
-from typing import Any, Dict, List, Optional, Tuple, Union
-
 import contextlib
 import io
 import time
+from typing import Any, Dict, List, Optional, Tuple, Union
 
-import dns.wire
 import dns.edns
+import dns.entropy
 import dns.enum
 import dns.exception
 import dns.flags
 import dns.name
 import dns.opcode
-import dns.entropy
 import dns.rcode
 import dns.rdata
 import dns.rdataclass
 import dns.rdatatype
-import dns.rrset
-import dns.renderer
-import dns.ttl
-import dns.tsig
 import dns.rdtypes.ANY.OPT
 import dns.rdtypes.ANY.TSIG
+import dns.renderer
+import dns.rrset
+import dns.tsig
+import dns.ttl
+import dns.wire
 
 
 class ShortHeader(dns.exception.FormError):
     """The DNS packet passed to from_wire() is too short."""
 
 
 class TrailingJunk(dns.exception.FormError):
@@ -131,15 +130,15 @@
     dns.name.Name,
     dns.rdataclass.RdataClass,
     dns.rdatatype.RdataType,
     Optional[dns.rdatatype.RdataType],
     Optional[dns.rdataclass.RdataClass],
 ]
 IndexType = Dict[IndexKeyType, dns.rrset.RRset]
-SectionType = Union[int, List[dns.rrset.RRset]]
+SectionType = Union[int, str, List[dns.rrset.RRset]]
 
 
 class Message:
     """A DNS message."""
 
     _section_enum = MessageSection
 
@@ -227,15 +226,15 @@
         if self.edns >= 0:
             s.write("edns %s\n" % self.edns)
             if self.ednsflags != 0:
                 s.write("eflags %s\n" % dns.flags.edns_to_text(self.ednsflags))
             s.write("payload %d\n" % self.payload)
         for opt in self.options:
             s.write("option %s\n" % opt.to_text())
-        for (name, which) in self._section_enum.__members__.items():
+        for name, which in self._section_enum.__members__.items():
             s.write(f";{name}\n")
             for rrset in self.section_from_number(which):
                 s.write(rrset.to_text(origin, relativize, **kw))
                 s.write("\n")
         #
         # We strip off the final \n so the caller can print the result without
         # doing weird things to get around eccentricities in Python print
@@ -344,122 +343,151 @@
         name: dns.name.Name,
         rdclass: dns.rdataclass.RdataClass,
         rdtype: dns.rdatatype.RdataType,
         covers: dns.rdatatype.RdataType = dns.rdatatype.NONE,
         deleting: Optional[dns.rdataclass.RdataClass] = None,
         create: bool = False,
         force_unique: bool = False,
+        idna_codec: Optional[dns.name.IDNACodec] = None,
     ) -> dns.rrset.RRset:
         """Find the RRset with the given attributes in the specified section.
 
-        *section*, an ``int`` section number, or one of the section
-        attributes of this message.  This specifies the
+        *section*, an ``int`` section number, a ``str`` section name, or one of
+        the section attributes of this message.  This specifies the
         the section of the message to search.  For example::
 
             my_message.find_rrset(my_message.answer, name, rdclass, rdtype)
             my_message.find_rrset(dns.message.ANSWER, name, rdclass, rdtype)
+            my_message.find_rrset("ANSWER", name, rdclass, rdtype)
 
-        *name*, a ``dns.name.Name``, the name of the RRset.
+        *name*, a ``dns.name.Name`` or ``str``, the name of the RRset.
 
-        *rdclass*, an ``int``, the class of the RRset.
+        *rdclass*, an ``int`` or ``str``, the class of the RRset.
 
-        *rdtype*, an ``int``, the type of the RRset.
+        *rdtype*, an ``int`` or ``str``, the type of the RRset.
 
-        *covers*, an ``int`` or ``None``, the covers value of the RRset.
-        The default is ``None``.
+        *covers*, an ``int`` or ``str``, the covers value of the RRset.
+        The default is ``dns.rdatatype.NONE``.
 
-        *deleting*, an ``int`` or ``None``, the deleting value of the RRset.
-        The default is ``None``.
+        *deleting*, an ``int``, ``str``, or ``None``, the deleting value of the
+        RRset.  The default is ``None``.
 
         *create*, a ``bool``.  If ``True``, create the RRset if it is not found.
         The created RRset is appended to *section*.
 
         *force_unique*, a ``bool``.  If ``True`` and *create* is also ``True``,
         create a new RRset regardless of whether a matching RRset exists
         already.  The default is ``False``.  This is useful when creating
         DDNS Update messages, as order matters for them.
 
+        *idna_codec*, a ``dns.name.IDNACodec``, specifies the IDNA
+        encoder/decoder.  If ``None``, the default IDNA 2003 encoder/decoder
+        is used.
+
         Raises ``KeyError`` if the RRset was not found and create was
         ``False``.
 
         Returns a ``dns.rrset.RRset object``.
         """
 
         if isinstance(section, int):
             section_number = section
-            the_section = self.section_from_number(section_number)
+            section = self.section_from_number(section_number)
+        elif isinstance(section, str):
+            section_number = MessageSection.from_text(section)
+            section = self.section_from_number(section_number)
         else:
             section_number = self.section_number(section)
-            the_section = section
+        if isinstance(name, str):
+            name = dns.name.from_text(name, idna_codec=idna_codec)
+        rdtype = dns.rdatatype.RdataType.make(rdtype)
+        rdclass = dns.rdataclass.RdataClass.make(rdclass)
+        covers = dns.rdatatype.RdataType.make(covers)
+        if deleting is not None:
+            deleting = dns.rdataclass.RdataClass.make(deleting)
         key = (section_number, name, rdclass, rdtype, covers, deleting)
         if not force_unique:
             if self.index is not None:
                 rrset = self.index.get(key)
                 if rrset is not None:
                     return rrset
             else:
-                for rrset in the_section:
+                for rrset in section:
                     if rrset.full_match(name, rdclass, rdtype, covers, deleting):
                         return rrset
         if not create:
             raise KeyError
         rrset = dns.rrset.RRset(name, rdclass, rdtype, covers, deleting)
-        the_section.append(rrset)
+        section.append(rrset)
         if self.index is not None:
             self.index[key] = rrset
         return rrset
 
     def get_rrset(
         self,
         section: SectionType,
         name: dns.name.Name,
         rdclass: dns.rdataclass.RdataClass,
         rdtype: dns.rdatatype.RdataType,
         covers: dns.rdatatype.RdataType = dns.rdatatype.NONE,
         deleting: Optional[dns.rdataclass.RdataClass] = None,
         create: bool = False,
         force_unique: bool = False,
+        idna_codec: Optional[dns.name.IDNACodec] = None,
     ) -> Optional[dns.rrset.RRset]:
         """Get the RRset with the given attributes in the specified section.
 
         If the RRset is not found, None is returned.
 
-        *section*, an ``int`` section number, or one of the section
-        attributes of this message.  This specifies the
+        *section*, an ``int`` section number, a ``str`` section name, or one of
+        the section attributes of this message.  This specifies the
         the section of the message to search.  For example::
 
             my_message.get_rrset(my_message.answer, name, rdclass, rdtype)
             my_message.get_rrset(dns.message.ANSWER, name, rdclass, rdtype)
+            my_message.get_rrset("ANSWER", name, rdclass, rdtype)
 
-        *name*, a ``dns.name.Name``, the name of the RRset.
+        *name*, a ``dns.name.Name`` or ``str``, the name of the RRset.
 
-        *rdclass*, an ``int``, the class of the RRset.
+        *rdclass*, an ``int`` or ``str``, the class of the RRset.
 
-        *rdtype*, an ``int``, the type of the RRset.
+        *rdtype*, an ``int`` or ``str``, the type of the RRset.
 
-        *covers*, an ``int`` or ``None``, the covers value of the RRset.
-        The default is ``None``.
+        *covers*, an ``int`` or ``str``, the covers value of the RRset.
+        The default is ``dns.rdatatype.NONE``.
 
-        *deleting*, an ``int`` or ``None``, the deleting value of the RRset.
-        The default is ``None``.
+        *deleting*, an ``int``, ``str``, or ``None``, the deleting value of the
+        RRset.  The default is ``None``.
 
         *create*, a ``bool``.  If ``True``, create the RRset if it is not found.
         The created RRset is appended to *section*.
 
         *force_unique*, a ``bool``.  If ``True`` and *create* is also ``True``,
         create a new RRset regardless of whether a matching RRset exists
         already.  The default is ``False``.  This is useful when creating
         DDNS Update messages, as order matters for them.
 
+        *idna_codec*, a ``dns.name.IDNACodec``, specifies the IDNA
+        encoder/decoder.  If ``None``, the default IDNA 2003 encoder/decoder
+        is used.
+
         Returns a ``dns.rrset.RRset object`` or ``None``.
         """
 
         try:
             rrset = self.find_rrset(
-                section, name, rdclass, rdtype, covers, deleting, create, force_unique
+                section,
+                name,
+                rdclass,
+                rdtype,
+                covers,
+                deleting,
+                create,
+                force_unique,
+                idna_codec,
             )
         except KeyError:
             rrset = None
         return rrset
 
     def _compute_opt_reserve(self) -> int:
         """Compute the size required for the OPT RR, padding excluded"""
@@ -1704,21 +1732,19 @@
     message.
 
     Returns a ``dns.message.QueryMessage``
     """
 
     if isinstance(qname, str):
         qname = dns.name.from_text(qname, idna_codec=idna_codec)
-    the_rdtype = dns.rdatatype.RdataType.make(rdtype)
-    the_rdclass = dns.rdataclass.RdataClass.make(rdclass)
+    rdtype = dns.rdatatype.RdataType.make(rdtype)
+    rdclass = dns.rdataclass.RdataClass.make(rdclass)
     m = QueryMessage(id=id)
     m.flags = dns.flags.Flag(flags)
-    m.find_rrset(
-        m.question, qname, the_rdclass, the_rdtype, create=True, force_unique=True
-    )
+    m.find_rrset(m.question, qname, rdclass, rdtype, create=True, force_unique=True)
     # only pass keywords on to use_edns if they have been set to a
     # non-None value.  Setting a field will turn EDNS on if it hasn't
     # been configured.
     kwargs: Dict[str, Any] = {}
     if ednsflags is not None:
         kwargs["ednsflags"] = ednsflags
     if payload is not None:
```

### Comparing `dnspython-2.3.0rc1/dns/name.py` & `dnspython-2.4.0rc1/dns/name.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,33 +14,30 @@
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """DNS Names.
 """
 
-from typing import Any, Dict, Iterable, Optional, Tuple, Union
-
 import copy
-import struct
-
 import encodings.idna  # type: ignore
+import struct
+from typing import Any, Dict, Iterable, Optional, Tuple, Union
 
 try:
     import idna  # type: ignore
 
     have_idna_2008 = True
 except ImportError:  # pragma: no cover
     have_idna_2008 = False
 
 import dns.enum
-import dns.wire
 import dns.exception
 import dns.immutable
-
+import dns.wire
 
 CompressType = Dict["Name", int]
 
 
 class NameRelation(dns.enum.IntEnum):
     """Name relation result from fullcompare()."""
 
@@ -234,15 +231,15 @@
         allow_pure_ascii: bool = False,
         strict_decode: bool = False,
     ):
         """Initialize the IDNA 2008 encoder/decoder.
 
         *uts_46* is a ``bool``.  If True, apply Unicode IDNA
         compatibility processing as described in Unicode Technical
-        Standard #46 (http://unicode.org/reports/tr46/).
+        Standard #46 (https://unicode.org/reports/tr46/).
         If False, do not apply the mapping.  The default is False.
 
         *transitional* is a ``bool``: If True, use the
         "transitional" mode described in Unicode Technical Standard
         #46.  The default is False.
 
         *allow_pure_ascii* is a ``bool``.  If True, then a label which
```

### Comparing `dnspython-2.3.0rc1/dns/namedict.py` & `dnspython-2.4.0rc1/dns/namedict.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/node.py` & `dnspython-2.4.0rc1/dns/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,27 +13,25 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """DNS nodes.  A node is a set of rdatasets."""
 
-from typing import Any, Dict, Optional
-
 import enum
 import io
+from typing import Any, Dict, Optional
 
 import dns.immutable
 import dns.name
 import dns.rdataclass
 import dns.rdataset
 import dns.rdatatype
-import dns.rrset
 import dns.renderer
-
+import dns.rrset
 
 _cname_types = {
     dns.rdatatype.CNAME,
 }
 
 # "neutral" types can coexist with a CNAME and thus are not "other data"
 _neutral_types = {
```

### Comparing `dnspython-2.3.0rc1/dns/opcode.py` & `dnspython-2.4.0rc1/dns/opcode.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/query.py` & `dnspython-2.4.0rc1/dns/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,65 +13,151 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """Talk to a DNS server."""
 
-from typing import Any, Dict, Optional, Tuple, Union
-
 import base64
 import contextlib
 import enum
 import errno
 import os
 import selectors
 import socket
 import struct
 import time
-import urllib.parse
+from typing import Any, Dict, Optional, Tuple, Union
 
 import dns.exception
 import dns.inet
-import dns.name
 import dns.message
+import dns.name
 import dns.quic
 import dns.rcode
 import dns.rdataclass
 import dns.rdatatype
 import dns.serial
 import dns.transaction
 import dns.tsig
 import dns.xfr
 
-try:
-    import requests
-    from requests_toolbelt.adapters.source import SourceAddressAdapter
-    from requests_toolbelt.adapters.host_header_ssl import HostHeaderSSLAdapter
 
-    _have_requests = True
-except ImportError:  # pragma: no cover
-    _have_requests = False
+def _remaining(expiration):
+    if expiration is None:
+        return None
+    timeout = expiration - time.time()
+    if timeout <= 0.0:
+        raise dns.exception.Timeout
+    return timeout
+
+
+def _expiration_for_this_attempt(timeout, expiration):
+    if expiration is None:
+        return None
+    return min(time.time() + timeout, expiration)
+
 
 _have_httpx = False
 _have_http2 = False
 try:
     import httpx
 
     _have_httpx = True
     try:
         # See if http2 support is available.
         with httpx.Client(http2=True):
             _have_http2 = True
     except Exception:
         pass
+
+    import httpcore
+    import httpcore.backends.base
+    import httpcore.backends.sync
+
+    class _NetworkBackend(httpcore.backends.base.NetworkBackend):
+        def __init__(self, resolver, local_port, bootstrap_address, family):
+            super().__init__()
+            self._local_port = local_port
+            self._resolver = resolver
+            self._bootstrap_address = bootstrap_address
+            self._family = family
+
+        def connect_tcp(
+            self, host, port, timeout, local_address, socket_options=None
+        ):  # pylint: disable=signature-differs
+            addresses = []
+            _, expiration = _compute_times(timeout)
+            if dns.inet.is_address(host):
+                addresses.append(host)
+            elif self._bootstrap_address is not None:
+                addresses.append(self._bootstrap_address)
+            else:
+                timeout = _remaining(expiration)
+                family = self._family
+                if local_address:
+                    family = dns.inet.af_for_address(local_address)
+                answers = self._resolver.resolve_name(
+                    host, family=family, lifetime=timeout
+                )
+                addresses = answers.addresses()
+            for address in addresses:
+                af = dns.inet.af_for_address(address)
+                if local_address is not None or self._local_port != 0:
+                    source = dns.inet.low_level_address_tuple(
+                        (local_address, self._local_port), af
+                    )
+                else:
+                    source = None
+                sock = _make_socket(af, socket.SOCK_STREAM, source)
+                attempt_expiration = _expiration_for_this_attempt(2.0, expiration)
+                try:
+                    _connect(
+                        sock,
+                        dns.inet.low_level_address_tuple((address, port), af),
+                        attempt_expiration,
+                    )
+                    return httpcore.backends.sync.SyncStream(sock)
+                except Exception:
+                    pass
+            raise httpcore.ConnectError
+
+        def connect_unix_socket(
+            self, path, timeout, socket_options=None
+        ):  # pylint: disable=signature-differs
+            raise NotImplementedError
+
+    class _HTTPTransport(httpx.HTTPTransport):
+        def __init__(
+            self,
+            *args,
+            local_port=0,
+            bootstrap_address=None,
+            resolver=None,
+            family=socket.AF_UNSPEC,
+            **kwargs,
+        ):
+            if resolver is None:
+                # pylint: disable=import-outside-toplevel,redefined-outer-name
+                import dns.resolver
+
+                resolver = dns.resolver.Resolver()
+            super().__init__(*args, **kwargs)
+            self._pool._network_backend = _NetworkBackend(
+                resolver, local_port, bootstrap_address, family
+            )
+
 except ImportError:  # pragma: no cover
-    pass
 
-have_doh = _have_requests or _have_httpx
+    class _HTTPTransport:  # type: ignore
+        def connect_tcp(self, host, port, timeout, local_address):
+            raise NotImplementedError
+
+
+have_doh = _have_httpx
 
 try:
     import ssl
 except ImportError:  # pragma: no cover
 
     class ssl:  # type: ignore
         class WantReadException(Exception):
@@ -101,15 +187,15 @@
 
 
 class BadResponse(dns.exception.FormError):
     """A DNS query response does not respond to the question asked."""
 
 
 class NoDOH(dns.exception.DNSException):
-    """DNS over HTTPS (DOH) was requested but the requests module is not
+    """DNS over HTTPS (DOH) was requested but the httpx module is not
     available."""
 
 
 class NoDOQ(dns.exception.DNSException):
     """DNS over QUIC (DOQ) was requested but the aioquic module is not
     available."""
 
@@ -226,29 +312,28 @@
         # URLs are ok so eat the exception
     if source:
         saf = dns.inet.af_for_address(source)
         if af:
             # We know the destination af, so source had better agree!
             if saf != af:
                 raise ValueError(
-                    "different address families for source " + "and destination"
+                    "different address families for source and destination"
                 )
         else:
             # We didn't know the destination af, but we know the source,
             # so that's our af.
             af = saf
     if source_port and not source:
         # Caller has specified a source_port but not an address, so we
         # need to return a source, and we need to use the appropriate
         # wildcard address as the address.
-        if af == socket.AF_INET:
-            source = "0.0.0.0"
-        elif af == socket.AF_INET6:
-            source = "::"
-        else:
+        try:
+            source = dns.inet.any_for_af(af)
+        except Exception:
+            # we catch this and raise ValueError for backwards compatibility
             raise ValueError("source_port specified but address family is unknown")
     # Convert high-level (address, port) tuples into low-level address
     # tuples.
     if destination:
         destination = dns.inet.low_level_address_tuple((destination, port), af)
     if source:
         source = dns.inet.low_level_address_tuple((source, source_port), af)
@@ -285,14 +370,16 @@
     one_rr_per_rrset: bool = False,
     ignore_trailing: bool = False,
     session: Optional[Any] = None,
     path: str = "/dns-query",
     post: bool = True,
     bootstrap_address: Optional[str] = None,
     verify: Union[bool, str] = True,
+    resolver: Optional["dns.resolver.Resolver"] = None,
+    family: Optional[int] = socket.AF_UNSPEC,
 ) -> dns.message.Message:
     """Return the response obtained after sending a query via DNS-over-HTTPS.
 
     *q*, a ``dns.message.Message``, the query to send.
 
     *where*, a ``str``, the nameserver IP address or the full URL. If an IP address is
     given, the URL will be constructed using the following schema:
@@ -310,131 +397,100 @@
     0.
 
     *one_rr_per_rrset*, a ``bool``. If ``True``, put each RR into its own RRset.
 
     *ignore_trailing*, a ``bool``. If ``True``, ignore trailing junk at end of the
     received message.
 
-    *session*, an ``httpx.Client`` or ``requests.session.Session``.  If provided, the
-    client/session to use to send the queries.
+    *session*, an ``httpx.Client``.  If provided, the client session to use to send the
+    queries.
 
     *path*, a ``str``. If *where* is an IP address, then *path* will be used to
     construct the URL to send the DNS query to.
 
     *post*, a ``bool``. If ``True``, the default, POST method will be used.
 
-    *bootstrap_address*, a ``str``, the IP address to use to bypass the system's DNS
-    resolver.
+    *bootstrap_address*, a ``str``, the IP address to use to bypass resolution.
 
     *verify*, a ``bool`` or ``str``.  If a ``True``, then TLS certificate verification
     of the server is done using the default CA bundle; if ``False``, then no
     verification is done; if a `str` then it specifies the path to a certificate file or
     directory which will be used for verification.
 
+    *resolver*, a ``dns.resolver.Resolver`` or ``None``, the resolver to use for
+    resolution of hostnames in URLs.  If not specified, a new resolver with a default
+    configuration will be used; note this is *not* the default resolver as that resolver
+    might have been configured to use DoH causing a chicken-and-egg problem.  This
+    parameter only has an effect if the HTTP library is httpx.
+
+    *family*, an ``int``, the address family.  If socket.AF_UNSPEC (the default), both A
+    and AAAA records will be retrieved.
+
     Returns a ``dns.message.Message``.
     """
 
     if not have_doh:
-        raise NoDOH("Neither httpx nor requests is available.")  # pragma: no cover
-
-    _httpx_ok = _have_httpx
+        raise NoDOH  # pragma: no cover
+    if session and not isinstance(session, httpx.Client):
+        raise ValueError("session parameter must be an httpx.Client")
 
     wire = q.to_wire()
-    (af, _, source) = _destination_and_source(where, port, source, source_port, False)
-    transport_adapter = None
+    (af, _, the_source) = _destination_and_source(
+        where, port, source, source_port, False
+    )
     transport = None
     headers = {"accept": "application/dns-message"}
-    if af is not None:
+    if af is not None and dns.inet.is_address(where):
         if af == socket.AF_INET:
             url = "https://{}:{}{}".format(where, port, path)
         elif af == socket.AF_INET6:
             url = "https://[{}]:{}{}".format(where, port, path)
-    elif bootstrap_address is not None:
-        _httpx_ok = False
-        split_url = urllib.parse.urlsplit(where)
-        if split_url.hostname is None:
-            raise ValueError("DoH URL has no hostname")
-        headers["Host"] = split_url.hostname
-        url = where.replace(split_url.hostname, bootstrap_address)
-        if _have_requests:
-            transport_adapter = HostHeaderSSLAdapter()
     else:
         url = where
-    if source is not None:
-        # set source port and source address
-        if _have_httpx:
-            if source_port == 0:
-                transport = httpx.HTTPTransport(local_address=source[0], verify=verify)
-            else:
-                _httpx_ok = False
-        if _have_requests:
-            transport_adapter = SourceAddressAdapter(source)
 
-    if session:
-        if _have_httpx:
-            _is_httpx = isinstance(session, httpx.Client)
-        else:
-            _is_httpx = False
-        if _is_httpx and not _httpx_ok:
-            raise NoDOH(
-                "Session is httpx, but httpx cannot be used for "
-                "the requested operation."
-            )
-    else:
-        _is_httpx = _httpx_ok
+    # set source port and source address
 
-    if not _httpx_ok and not _have_requests:
-        raise NoDOH(
-            "Cannot use httpx for this operation, and requests is not available."
-        )
+    if the_source is None:
+        local_address = None
+        local_port = 0
+    else:
+        local_address = the_source[0]
+        local_port = the_source[1]
+    transport = _HTTPTransport(
+        local_address=local_address,
+        verify=verify,
+        local_port=local_port,
+        bootstrap_address=bootstrap_address,
+        resolver=resolver,
+        family=family,
+    )
 
     if session:
         cm: contextlib.AbstractContextManager = contextlib.nullcontext(session)
-    elif _is_httpx:
+    else:
         cm = httpx.Client(
             http1=True, http2=_have_http2, verify=verify, transport=transport
         )
-    else:
-        cm = requests.sessions.Session()
     with cm as session:
-        if transport_adapter and not _is_httpx:
-            session.mount(url, transport_adapter)
-
         # see https://tools.ietf.org/html/rfc8484#section-4.1.1 for DoH
         # GET and POST examples
         if post:
             headers.update(
                 {
                     "content-type": "application/dns-message",
                     "content-length": str(len(wire)),
                 }
             )
-            if _is_httpx:
-                response = session.post(
-                    url, headers=headers, content=wire, timeout=timeout
-                )
-            else:
-                response = session.post(
-                    url, headers=headers, data=wire, timeout=timeout, verify=verify
-                )
+            response = session.post(url, headers=headers, content=wire, timeout=timeout)
         else:
             wire = base64.urlsafe_b64encode(wire).rstrip(b"=")
-            if _is_httpx:
-                twire = wire.decode()  # httpx does a repr() if we give it bytes
-                response = session.get(
-                    url, headers=headers, timeout=timeout, params={"dns": twire}
-                )
-            else:
-                response = session.get(
-                    url,
-                    headers=headers,
-                    timeout=timeout,
-                    verify=verify,
-                    params={"dns": wire},
-                )
+            twire = wire.decode()  # httpx does a repr() if we give it bytes
+            response = session.get(
+                url, headers=headers, timeout=timeout, params={"dns": twire}
+            )
 
     # see https://tools.ietf.org/html/rfc8484#section-4.2.1 for info about DoH
     # status codes
     if response.status_code < 200 or response.status_code > 299:
         raise ValueError(
             "{} responded with status code {}"
             "\nResponse body: {}".format(where, response.status_code, response.content)
@@ -1028,21 +1084,15 @@
 
     wire = q.to_wire()
     (begin_time, expiration) = _compute_times(timeout)
     (af, destination, source) = _destination_and_source(
         where, port, source, source_port
     )
     if ssl_context is None and not sock:
-        # LGTM complains about this because the default might permit TLS < 1.2
-        # for compatibility, but the python documentation says that explicit
-        # versioning is deprecated, and that as of python 3.6 it will negotiate
-        # the highest version possible.  We also set a minimum version when we
-        # can, even though this might require a future dnspython release if that
-        # version becomes deprecated.
-        ssl_context = ssl.create_default_context()  # lgtm[py/insecure-protocol]
+        ssl_context = ssl.create_default_context()
         ssl_context.minimum_version = ssl.TLSVersion.TLSv1_2
         if server_hostname is None:
             ssl_context.check_hostname = False
 
     with _make_socket(
         af,
         socket.SOCK_STREAM,
@@ -1072,14 +1122,15 @@
     port: int = 853,
     source: Optional[str] = None,
     source_port: int = 0,
     one_rr_per_rrset: bool = False,
     ignore_trailing: bool = False,
     connection: Optional[dns.quic.SyncQuicConnection] = None,
     verify: Union[bool, str] = True,
+    server_hostname: Optional[str] = None,
 ) -> dns.message.Message:
     """Return the response obtained after sending a query via DNS-over-QUIC.
 
     *q*, a ``dns.message.Message``, the query to send.
 
     *where*, a ``str``, the nameserver IP address.
 
@@ -1103,29 +1154,35 @@
     connection to use to send the query.
 
     *verify*, a ``bool`` or ``str``.  If a ``True``, then TLS certificate verification
     of the server is done using the default CA bundle; if ``False``, then no
     verification is done; if a `str` then it specifies the path to a certificate file or
     directory which will be used for verification.
 
+    *server_hostname*, a ``str`` containing the server's hostname.  The
+    default is ``None``, which means that no hostname is known, and if an
+    SSL context is created, hostname checking will be disabled.
+
     Returns a ``dns.message.Message``.
     """
 
     if not dns.quic.have_quic:
         raise NoDOQ("DNS-over-QUIC is not available.")  # pragma: no cover
 
     q.id = 0
     wire = q.to_wire()
     the_connection: dns.quic.SyncQuicConnection
     the_manager: dns.quic.SyncQuicManager
     if connection:
         manager: contextlib.AbstractContextManager = contextlib.nullcontext(None)
         the_connection = connection
     else:
-        manager = dns.quic.SyncQuicManager(verify_mode=verify)
+        manager = dns.quic.SyncQuicManager(
+            verify_mode=verify, server_name=server_hostname
+        )
         the_manager = manager  # for type checking happiness
 
     with manager:
         if not connection:
             the_connection = the_manager.connect(where, port, source, source_port)
         start = time.time()
         with the_connection.make_stream() as stream:
```

### Comparing `dnspython-2.3.0rc1/dns/quic/__init__.py` & `dnspython-2.4.0rc1/dns/quic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Copyright (C) Dnspython Contributors, see LICENSE for text of ISC license
 
 try:
     import aioquic.quic.configuration  # type: ignore
 
     import dns.asyncbackend
     from dns._asyncbackend import NullContext
-    from dns.quic._sync import SyncQuicManager, SyncQuicConnection, SyncQuicStream
     from dns.quic._asyncio import (
-        AsyncioQuicManager,
         AsyncioQuicConnection,
+        AsyncioQuicManager,
         AsyncioQuicStream,
     )
     from dns.quic._common import AsyncQuicConnection, AsyncQuicManager
+    from dns.quic._sync import SyncQuicConnection, SyncQuicManager, SyncQuicStream
 
     have_quic = True
 
     def null_factory(
         *args,  # pylint: disable=unused-argument
         **kwargs  # pylint: disable=unused-argument
     ):
@@ -29,17 +29,18 @@
     # We have a context factory and a manager factory as for trio we need to have
     # a nursery.
 
     _async_factories = {"asyncio": (null_factory, _asyncio_manager_factory)}
 
     try:
         import trio
+
         from dns.quic._trio import (  # pylint: disable=ungrouped-imports
-            TrioQuicManager,
             TrioQuicConnection,
+            TrioQuicManager,
             TrioQuicStream,
         )
 
         def _trio_context_factory():
             return trio.open_nursery()
 
         def _trio_manager_factory(context, *args, **kwargs):
```

### Comparing `dnspython-2.3.0rc1/dns/quic/_asyncio.py` & `dnspython-2.4.0rc1/dns/quic/_asyncio.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,37 +5,38 @@
 import ssl
 import struct
 import time
 
 import aioquic.quic.configuration  # type: ignore
 import aioquic.quic.connection  # type: ignore
 import aioquic.quic.events  # type: ignore
-import dns.inet
-import dns.asyncbackend
 
+import dns.asyncbackend
+import dns.inet
 from dns.quic._common import (
-    BaseQuicStream,
+    QUIC_MAX_DATAGRAM,
     AsyncQuicConnection,
     AsyncQuicManager,
-    QUIC_MAX_DATAGRAM,
+    BaseQuicStream,
+    UnexpectedEOF,
 )
 
 
 class AsyncioQuicStream(BaseQuicStream):
     def __init__(self, connection, stream_id):
         super().__init__(connection, stream_id)
         self._wake_up = asyncio.Condition()
 
     async def _wait_for_wake_up(self):
         async with self._wake_up:
             await self._wake_up.wait()
 
     async def wait_for(self, amount, expiration):
-        timeout = self._timeout_from_expiration(expiration)
         while True:
+            timeout = self._timeout_from_expiration(expiration)
             if self._buffer.have(amount):
                 return
             self._expecting = amount
             try:
                 await asyncio.wait_for(self._wait_for_wake_up(), timeout)
             except Exception:
                 pass
@@ -102,24 +103,29 @@
                     )
                     # Wake up the timer in case the sender is sleeping, as there may be
                     # stuff to send now.
                     async with self._wake_timer:
                         self._wake_timer.notify_all()
         except Exception:
             pass
+        finally:
+            self._done = True
+            async with self._wake_timer:
+                self._wake_timer.notify_all()
+            self._handshake_complete.set()
 
     async def _wait_for_wake_timer(self):
         async with self._wake_timer:
             await self._wake_timer.wait()
 
     async def _sender(self):
         await self._socket_created.wait()
         while not self._done:
             datagrams = self._connection.datagrams_to_send(time.time())
-            for (datagram, address) in datagrams:
+            for datagram, address in datagrams:
                 assert address == self._peer[0]
                 await self._socket.sendto(datagram, self._peer, None)
             (expiration, interval) = self._get_timer_values()
             try:
                 await asyncio.wait_for(self._wait_for_wake_timer(), interval)
             except Exception:
                 pass
@@ -158,14 +164,16 @@
         if self._closed:
             return
         self._receiver_task = asyncio.Task(self._receiver())
         self._sender_task = asyncio.Task(self._sender())
 
     async def make_stream(self):
         await self._handshake_complete.wait()
+        if self._done:
+            raise UnexpectedEOF
         stream_id = self._connection.get_next_available_stream_id(False)
         stream = AsyncioQuicStream(self, stream_id)
         self._streams[stream_id] = stream
         return stream
 
     async def close(self):
         if not self._closed:
@@ -181,26 +189,26 @@
             try:
                 await self._sender_task
             except asyncio.CancelledError:
                 pass
 
 
 class AsyncioQuicManager(AsyncQuicManager):
-    def __init__(self, conf=None, verify_mode=ssl.CERT_REQUIRED):
-        super().__init__(conf, verify_mode, AsyncioQuicConnection)
+    def __init__(self, conf=None, verify_mode=ssl.CERT_REQUIRED, server_name=None):
+        super().__init__(conf, verify_mode, AsyncioQuicConnection, server_name)
 
     def connect(self, address, port=853, source=None, source_port=0):
         (connection, start) = self._connect(address, port, source, source_port)
         if start:
             connection.run()
         return connection
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
-        # Copy the itertor into a list as exiting things will mutate the connections
+        # Copy the iterator into a list as exiting things will mutate the connections
         # table.
         connections = list(self._connections.values())
         for connection in connections:
             await connection.close()
         return False
```

### Comparing `dnspython-2.3.0rc1/dns/quic/_common.py` & `dnspython-2.4.0rc1/dns/quic/_common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # Copyright (C) Dnspython Contributors, see LICENSE for text of ISC license
 
 import socket
 import struct
 import time
-
 from typing import Any
 
 import aioquic.quic.configuration  # type: ignore
 import aioquic.quic.connection  # type: ignore
-import dns.inet
 
+import dns.inet
 
 QUIC_MAX_DATAGRAM = 2048
 
 
 class UnexpectedEOF(Exception):
     pass
 
@@ -136,25 +135,26 @@
 
 class AsyncQuicConnection(BaseQuicConnection):
     async def make_stream(self) -> Any:
         pass
 
 
 class BaseQuicManager:
-    def __init__(self, conf, verify_mode, connection_factory):
+    def __init__(self, conf, verify_mode, connection_factory, server_name=None):
         self._connections = {}
         self._connection_factory = connection_factory
         if conf is None:
             verify_path = None
             if isinstance(verify_mode, str):
                 verify_path = verify_mode
                 verify_mode = True
             conf = aioquic.quic.configuration.QuicConfiguration(
                 alpn_protocols=["doq", "doq-i03"],
                 verify_mode=verify_mode,
+                server_name=server_name,
             )
             if verify_path is not None:
                 conf.load_verify_locations(verify_path)
         self._conf = conf
 
     def _connect(self, address, port=853, source=None, source_port=0):
         connection = self._connections.get((address, port))
```

### Comparing `dnspython-2.3.0rc1/dns/quic/_sync.py` & `dnspython-2.4.0rc1/dns/quic/_sync.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # Copyright (C) Dnspython Contributors, see LICENSE for text of ISC license
 
+import selectors
 import socket
 import ssl
-import selectors
 import struct
 import threading
 import time
 
 import aioquic.quic.configuration  # type: ignore
 import aioquic.quic.connection  # type: ignore
 import aioquic.quic.events  # type: ignore
-import dns.inet
 
+import dns.inet
 from dns.quic._common import (
-    BaseQuicStream,
+    QUIC_MAX_DATAGRAM,
     BaseQuicConnection,
     BaseQuicManager,
-    QUIC_MAX_DATAGRAM,
+    BaseQuicStream,
+    UnexpectedEOF,
 )
 
 # Avoid circularity with dns.query
 if hasattr(selectors, "PollSelector"):
     _selector_class = selectors.PollSelector  # type: ignore
 else:
     _selector_class = selectors.SelectSelector  # type: ignore
@@ -29,22 +30,23 @@
 class SyncQuicStream(BaseQuicStream):
     def __init__(self, connection, stream_id):
         super().__init__(connection, stream_id)
         self._wake_up = threading.Condition()
         self._lock = threading.Lock()
 
     def wait_for(self, amount, expiration):
-        timeout = self._timeout_from_expiration(expiration)
         while True:
+            timeout = self._timeout_from_expiration(expiration)
             with self._lock:
                 if self._buffer.have(amount):
                     return
                 self._expecting = amount
             with self._wake_up:
-                self._wake_up.wait(timeout)
+                if not self._wake_up.wait(timeout):
+                    raise TimeoutError
             self._expecting = 0
 
     def receive(self, timeout=None):
         expiration = self._expiration_from_timeout(timeout)
         self.wait_for(2, expiration)
         with self._lock:
             (size,) = struct.unpack("!H", self._buffer.get(2))
@@ -110,32 +112,38 @@
         while True:
             try:
                 self._receive_wakeup.recv(32)
             except BlockingIOError:
                 return
 
     def _worker(self):
-        sel = _selector_class()
-        sel.register(self._socket, selectors.EVENT_READ, self._read)
-        sel.register(self._receive_wakeup, selectors.EVENT_READ, self._drain_wakeup)
-        while not self._done:
-            (expiration, interval) = self._get_timer_values(False)
-            items = sel.select(interval)
-            for (key, _) in items:
-                key.data()
+        try:
+            sel = _selector_class()
+            sel.register(self._socket, selectors.EVENT_READ, self._read)
+            sel.register(self._receive_wakeup, selectors.EVENT_READ, self._drain_wakeup)
+            while not self._done:
+                (expiration, interval) = self._get_timer_values(False)
+                items = sel.select(interval)
+                for key, _ in items:
+                    key.data()
+                with self._lock:
+                    self._handle_timer(expiration)
+                    datagrams = self._connection.datagrams_to_send(time.time())
+                for datagram, _ in datagrams:
+                    try:
+                        self._socket.send(datagram)
+                    except BlockingIOError:
+                        # we let QUIC handle any lossage
+                        pass
+                self._handle_events()
+        finally:
             with self._lock:
-                self._handle_timer(expiration)
-                datagrams = self._connection.datagrams_to_send(time.time())
-            for (datagram, _) in datagrams:
-                try:
-                    self._socket.send(datagram)
-                except BlockingIOError:
-                    # we let QUIC handle any lossage
-                    pass
-            self._handle_events()
+                self._done = True
+            # Ensure anyone waiting for this gets woken up.
+            self._handshake_complete.set()
 
     def _handle_events(self):
         while True:
             with self._lock:
                 event = self._connection.next_event()
             if event is None:
                 return
@@ -162,14 +170,16 @@
             return
         self._worker_thread = threading.Thread(target=self._worker)
         self._worker_thread.start()
 
     def make_stream(self):
         self._handshake_complete.wait()
         with self._lock:
+            if self._done:
+                raise UnexpectedEOF
             stream_id = self._connection.get_next_available_stream_id(False)
             stream = SyncQuicStream(self, stream_id)
             self._streams[stream_id] = stream
         return stream
 
     def close_stream(self, stream_id):
         with self._lock:
@@ -183,16 +193,16 @@
             self._closed = True
             self._connection.close()
             self._send_wakeup.send(b"\x01")
         self._worker_thread.join()
 
 
 class SyncQuicManager(BaseQuicManager):
-    def __init__(self, conf=None, verify_mode=ssl.CERT_REQUIRED):
-        super().__init__(conf, verify_mode, SyncQuicConnection)
+    def __init__(self, conf=None, verify_mode=ssl.CERT_REQUIRED, server_name=None):
+        super().__init__(conf, verify_mode, SyncQuicConnection, server_name)
         self._lock = threading.Lock()
 
     def connect(self, address, port=853, source=None, source_port=0):
         with self._lock:
             (connection, start) = self._connect(address, port, source, source_port)
             if start:
                 connection.run()
@@ -202,13 +212,13 @@
         with self._lock:
             super().closed(address, port)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        # Copy the itertor into a list as exiting things will mutate the connections
+        # Copy the iterator into a list as exiting things will mutate the connections
         # table.
         connections = list(self._connections.values())
         for connection in connections:
             connection.close()
         return False
```

### Comparing `dnspython-2.3.0rc1/dns/quic/_trio.py` & `dnspython-2.4.0rc1/dns/quic/_trio.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 import aioquic.quic.connection  # type: ignore
 import aioquic.quic.events  # type: ignore
 import trio
 
 import dns.inet
 from dns._asyncbackend import NullContext
 from dns.quic._common import (
-    BaseQuicStream,
+    QUIC_MAX_DATAGRAM,
     AsyncQuicConnection,
     AsyncQuicManager,
-    QUIC_MAX_DATAGRAM,
+    BaseQuicStream,
+    UnexpectedEOF,
 )
 
 
 class TrioQuicStream(BaseQuicStream):
     def __init__(self, connection, stream_id):
         super().__init__(connection, stream_id)
         self._wake_up = trio.Condition()
@@ -76,28 +77,34 @@
         if self._source:
             trio.socket.bind(dns.inet.low_level_address_tuple(self._source, self._af))
         self._handshake_complete = trio.Event()
         self._run_done = trio.Event()
         self._worker_scope = None
 
     async def _worker(self):
-        await self._socket.connect(self._peer)
-        while not self._done:
-            (expiration, interval) = self._get_timer_values(False)
-            with trio.CancelScope(
-                deadline=trio.current_time() + interval
-            ) as self._worker_scope:
-                datagram = await self._socket.recv(QUIC_MAX_DATAGRAM)
-                self._connection.receive_datagram(datagram, self._peer[0], time.time())
-            self._worker_scope = None
-            self._handle_timer(expiration)
-            datagrams = self._connection.datagrams_to_send(time.time())
-            for (datagram, _) in datagrams:
-                await self._socket.send(datagram)
-            await self._handle_events()
+        try:
+            await self._socket.connect(self._peer)
+            while not self._done:
+                (expiration, interval) = self._get_timer_values(False)
+                with trio.CancelScope(
+                    deadline=trio.current_time() + interval
+                ) as self._worker_scope:
+                    datagram = await self._socket.recv(QUIC_MAX_DATAGRAM)
+                    self._connection.receive_datagram(
+                        datagram, self._peer[0], time.time()
+                    )
+                self._worker_scope = None
+                self._handle_timer(expiration)
+                datagrams = self._connection.datagrams_to_send(time.time())
+                for datagram, _ in datagrams:
+                    await self._socket.send(datagram)
+                await self._handle_events()
+        finally:
+            self._done = True
+            self._handshake_complete.set()
 
     async def _handle_events(self):
         count = 0
         while True:
             event = self._connection.next_event()
             if event is None:
                 return
@@ -128,14 +135,16 @@
             return
         async with trio.open_nursery() as nursery:
             nursery.start_soon(self._worker)
         self._run_done.set()
 
     async def make_stream(self):
         await self._handshake_complete.wait()
+        if self._done:
+            raise UnexpectedEOF
         stream_id = self._connection.get_next_available_stream_id(False)
         stream = TrioQuicStream(self, stream_id)
         self._streams[stream_id] = stream
         return stream
 
     async def close(self):
         if not self._closed:
@@ -144,27 +153,29 @@
             self._connection.close()
             if self._worker_scope is not None:
                 self._worker_scope.cancel()
             await self._run_done.wait()
 
 
 class TrioQuicManager(AsyncQuicManager):
-    def __init__(self, nursery, conf=None, verify_mode=ssl.CERT_REQUIRED):
-        super().__init__(conf, verify_mode, TrioQuicConnection)
+    def __init__(
+        self, nursery, conf=None, verify_mode=ssl.CERT_REQUIRED, server_name=None
+    ):
+        super().__init__(conf, verify_mode, TrioQuicConnection, server_name)
         self._nursery = nursery
 
     def connect(self, address, port=853, source=None, source_port=0):
         (connection, start) = self._connect(address, port, source, source_port)
         if start:
             self._nursery.start_soon(connection.run)
         return connection
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
-        # Copy the itertor into a list as exiting things will mutate the connections
+        # Copy the iterator into a list as exiting things will mutate the connections
         # table.
         connections = list(self._connections.values())
         for connection in connections:
             await connection.close()
         return False
```

### Comparing `dnspython-2.3.0rc1/dns/rcode.py` & `dnspython-2.4.0rc1/dns/rcode.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdata.py` & `dnspython-2.4.0rc1/dns/rdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,34 +13,33 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """DNS rdata."""
 
-from typing import Any, Dict, Optional, Tuple, Union
-
-from importlib import import_module
 import base64
 import binascii
-import io
 import inspect
+import io
 import itertools
 import random
+from importlib import import_module
+from typing import Any, Dict, Optional, Tuple, Union
 
-import dns.wire
 import dns.exception
 import dns.immutable
 import dns.ipv4
 import dns.ipv6
 import dns.name
 import dns.rdataclass
 import dns.rdatatype
 import dns.tokenizer
 import dns.ttl
+import dns.wire
 
 _chunksize = 32
 
 # We currently allow comparisons for rdata with relative names for backwards
 # compatibility, but in the future we will not, as these kinds of comparisons
 # can lead to subtle bugs if code is not carefully written.
 #
@@ -354,15 +353,14 @@
 
     def __lt__(self, other):
         if (
             not isinstance(other, Rdata)
             or self.rdclass != other.rdclass
             or self.rdtype != other.rdtype
         ):
-
             return NotImplemented
         return self._cmp(other) < 0
 
     def __le__(self, other):
         if (
             not isinstance(other, Rdata)
             or self.rdclass != other.rdclass
@@ -877,20 +875,15 @@
     *is_singleton*, a ``bool``, indicating if the type is a singleton (i.e.
     RRsets of the type can have only one member.)
 
     *rdclass*, the rdataclass of the type, or ``dns.rdataclass.ANY`` if
     it applies to all classes.
     """
 
-    the_rdtype = dns.rdatatype.RdataType.make(rdtype)
-    existing_cls = get_rdata_class(rdclass, the_rdtype)
-    if existing_cls != GenericRdata or dns.rdatatype.is_metatype(the_rdtype):
-        raise RdatatypeExists(rdclass=rdclass, rdtype=the_rdtype)
-    try:
-        if dns.rdatatype.RdataType(the_rdtype).name != rdtype_text:
-            raise RdatatypeExists(rdclass=rdclass, rdtype=the_rdtype)
-    except ValueError:
-        pass
-    _rdata_classes[(rdclass, the_rdtype)] = getattr(
+    rdtype = dns.rdatatype.RdataType.make(rdtype)
+    existing_cls = get_rdata_class(rdclass, rdtype)
+    if existing_cls != GenericRdata or dns.rdatatype.is_metatype(rdtype):
+        raise RdatatypeExists(rdclass=rdclass, rdtype=rdtype)
+    _rdata_classes[(rdclass, rdtype)] = getattr(
         implementation, rdtype_text.replace("-", "_")
     )
-    dns.rdatatype.register_type(the_rdtype, rdtype_text, is_singleton)
+    dns.rdatatype.register_type(rdtype, rdtype_text, is_singleton)
```

### Comparing `dnspython-2.3.0rc1/dns/rdataclass.py` & `dnspython-2.4.0rc1/dns/rdataclass.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdataset.py` & `dnspython-2.4.0rc1/dns/rdataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,25 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """DNS rdatasets (an rdataset is a set of rdatas of a given type and class)"""
 
-from typing import Any, cast, Collection, Dict, List, Optional, Union
-
 import io
 import random
 import struct
+from typing import Any, Collection, Dict, List, Optional, Union, cast
 
 import dns.exception
 import dns.immutable
 import dns.name
-import dns.rdatatype
-import dns.rdataclass
 import dns.rdata
+import dns.rdataclass
+import dns.rdatatype
 import dns.set
 import dns.ttl
 
 # define SimpleSet here for backwards compatibility
 SimpleSet = dns.set.Set
 
 
@@ -467,17 +466,17 @@
 
     *relativize_to*, a ``dns.name.Name`` (or ``None``), the origin to use
     when relativizing names.  If not set, the *origin* value will be used.
 
     Returns a ``dns.rdataset.Rdataset`` object.
     """
 
-    the_rdclass = dns.rdataclass.RdataClass.make(rdclass)
-    the_rdtype = dns.rdatatype.RdataType.make(rdtype)
-    r = Rdataset(the_rdclass, the_rdtype)
+    rdclass = dns.rdataclass.RdataClass.make(rdclass)
+    rdtype = dns.rdatatype.RdataType.make(rdtype)
+    r = Rdataset(rdclass, rdtype)
     r.update_ttl(ttl)
     for t in text_rdatas:
         rd = dns.rdata.from_text(
             r.rdclass, r.rdtype, t, origin, relativize, relativize_to, idna_codec
         )
         r.add(rd)
     return r
```

### Comparing `dnspython-2.3.0rc1/dns/rdatatype.py` & `dnspython-2.4.0rc1/dns/rdatatype.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/AFSDB.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/AFSDB.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import dns.rdtypes.mxbase
 import dns.immutable
+import dns.rdtypes.mxbase
 
 
 @dns.immutable.immutable
 class AFSDB(dns.rdtypes.mxbase.UncompressedDowncasingMX):
 
     """AFSDB record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/AMTRELAY.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/AMTRELAY.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/AVC.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/AVC.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import dns.rdtypes.txtbase
 import dns.immutable
+import dns.rdtypes.txtbase
 
 
 @dns.immutable.immutable
 class AVC(dns.rdtypes.txtbase.TXTBase):
 
     """AVC record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/CAA.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/CAA.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/CDNSKEY.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/CDNSKEY.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import dns.rdtypes.dnskeybase  # lgtm[py/import-and-import-from]
 import dns.immutable
+import dns.rdtypes.dnskeybase  # lgtm[py/import-and-import-from]
 
 # pylint: disable=unused-import
-from dns.rdtypes.dnskeybase import (
-    SEP,
+from dns.rdtypes.dnskeybase import (  # noqa: F401  lgtm[py/unused-import]
     REVOKE,
+    SEP,
     ZONE,
-)  # noqa: F401  lgtm[py/unused-import]
+)
 
 # pylint: enable=unused-import
 
 
 @dns.immutable.immutable
 class CDNSKEY(dns.rdtypes.dnskeybase.DNSKEYBase):
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/CDS.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/CDS.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import dns.rdtypes.dsbase
 import dns.immutable
+import dns.rdtypes.dsbase
 
 
 @dns.immutable.immutable
 class CDS(dns.rdtypes.dsbase.DSBase):
 
     """CDS record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/CERT.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/CERT.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import struct
 import base64
+import struct
 
+import dns.dnssectypes
 import dns.exception
 import dns.immutable
-import dns.dnssectypes
 import dns.rdata
 import dns.tokenizer
 
 _ctype_by_value = {
     1: "PKIX",
     2: "SPKI",
     3: "PGP",
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/CNAME.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/CNAME.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import dns.rdtypes.nsbase
 import dns.immutable
+import dns.rdtypes.nsbase
 
 
 @dns.immutable.immutable
 class CNAME(dns.rdtypes.nsbase.NSBase):
 
     """CNAME record
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/CSYNC.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/CSYNC.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 import struct
 
 import dns.exception
 import dns.immutable
+import dns.name
 import dns.rdata
 import dns.rdatatype
-import dns.name
 import dns.rdtypes.util
 
 
 @dns.immutable.immutable
 class Bitmap(dns.rdtypes.util.Bitmap):
     type_name = "CSYNC"
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/DLV.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/DLV.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import dns.rdtypes.dsbase
 import dns.immutable
+import dns.rdtypes.dsbase
 
 
 @dns.immutable.immutable
 class DLV(dns.rdtypes.dsbase.DSBase):
 
     """DLV record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/DNAME.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/DNAME.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import dns.rdtypes.nsbase
 import dns.immutable
+import dns.rdtypes.nsbase
 
 
 @dns.immutable.immutable
 class DNAME(dns.rdtypes.nsbase.UncompressedNS):
 
     """DNAME record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/DNSKEY.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/DNSKEY.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import dns.rdtypes.dnskeybase  # lgtm[py/import-and-import-from]
 import dns.immutable
+import dns.rdtypes.dnskeybase  # lgtm[py/import-and-import-from]
 
 # pylint: disable=unused-import
-from dns.rdtypes.dnskeybase import (
-    SEP,
+from dns.rdtypes.dnskeybase import (  # noqa: F401  lgtm[py/unused-import]
     REVOKE,
+    SEP,
     ZONE,
-)  # noqa: F401  lgtm[py/unused-import]
+)
 
 # pylint: enable=unused-import
 
 
 @dns.immutable.immutable
 class DNSKEY(dns.rdtypes.dnskeybase.DNSKEYBase):
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/DS.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/DS.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import dns.rdtypes.dsbase
 import dns.immutable
+import dns.rdtypes.dsbase
 
 
 @dns.immutable.immutable
 class DS(dns.rdtypes.dsbase.DSBase):
 
     """DS record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/EUI48.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/EUI64.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import dns.rdtypes.euibase
 import dns.immutable
+import dns.rdtypes.euibase
 
 
 @dns.immutable.immutable
-class EUI48(dns.rdtypes.euibase.EUIBase):
+class EUI64(dns.rdtypes.euibase.EUIBase):
 
-    """EUI48 record"""
+    """EUI64 record"""
 
     # see: rfc7043.txt
 
-    byte_len = 6  # 0123456789ab (in hex)
-    text_len = byte_len * 3 - 1  # 01-23-45-67-89-ab
+    byte_len = 8  # 0123456789abcdef (in hex)
+    text_len = byte_len * 3 - 1  # 01-23-45-67-89-ab-cd-ef
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/EUI64.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/EUI48.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import dns.rdtypes.euibase
 import dns.immutable
+import dns.rdtypes.euibase
 
 
 @dns.immutable.immutable
-class EUI64(dns.rdtypes.euibase.EUIBase):
+class EUI48(dns.rdtypes.euibase.EUIBase):
 
-    """EUI64 record"""
+    """EUI48 record"""
 
     # see: rfc7043.txt
 
-    byte_len = 8  # 0123456789abcdef (in hex)
-    text_len = byte_len * 3 - 1  # 01-23-45-67-89-ab-cd-ef
+    byte_len = 6  # 0123456789ab (in hex)
+    text_len = byte_len * 3 - 1  # 01-23-45-67-89-ab
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/GPOS.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/GPOS.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/HINFO.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/HINFO.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/HIP.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/HIP.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import struct
 import base64
 import binascii
+import struct
 
 import dns.exception
 import dns.immutable
 import dns.rdata
 import dns.rdatatype
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/ISDN.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/ISDN.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/L32.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/L32.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/L64.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/L64.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/LOC.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/LOC.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 import struct
 
 import dns.exception
 import dns.immutable
 import dns.rdata
 
-
 _pows = tuple(10**i for i in range(0, 11))
 
 # default values are in centimeters
 _default_size = 100.0
 _default_hprec = 1000000.0
 _default_vprec = 1000.0
 
@@ -36,15 +35,15 @@
 _MIN_LONGITUDE = 0x80000000 - 180 * 3600000
 
 
 def _exponent_of(what, desc):
     if what == 0:
         return 0
     exp = None
-    for (i, pow) in enumerate(_pows):
+    for i, pow in enumerate(_pows):
         if what < pow:
             exp = i - 1
             break
     if exp is None or exp < 0:
         raise dns.exception.SyntaxError("%s value out of bounds" % desc)
     return exp
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/LP.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/LP.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/MX.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/MX.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import dns.rdtypes.mxbase
 import dns.immutable
+import dns.rdtypes.mxbase
 
 
 @dns.immutable.immutable
 class MX(dns.rdtypes.mxbase.MXBase):
 
     """MX record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/NID.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/NID.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/NINFO.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/NINFO.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import dns.rdtypes.txtbase
 import dns.immutable
+import dns.rdtypes.txtbase
 
 
 @dns.immutable.immutable
 class NINFO(dns.rdtypes.txtbase.TXTBase):
 
     """NINFO record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/NS.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/NS.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import dns.rdtypes.nsbase
 import dns.immutable
+import dns.rdtypes.nsbase
 
 
 @dns.immutable.immutable
 class NS(dns.rdtypes.nsbase.NSBase):
 
     """NS record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/NSEC.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/NSEC.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 import dns.exception
 import dns.immutable
+import dns.name
 import dns.rdata
 import dns.rdatatype
-import dns.name
 import dns.rdtypes.util
 
 
 @dns.immutable.immutable
 class Bitmap(dns.rdtypes.util.Bitmap):
     type_name = "NSEC"
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/NSEC3.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/NSEC3.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 import dns.exception
 import dns.immutable
 import dns.rdata
 import dns.rdatatype
 import dns.rdtypes.util
 
-
 b32_hex_to_normal = bytes.maketrans(
     b"0123456789ABCDEFGHIJKLMNOPQRSTUV", b"ABCDEFGHIJKLMNOPQRSTUVWXYZ234567"
 )
 b32_normal_to_hex = bytes.maketrans(
     b"ABCDEFGHIJKLMNOPQRSTUVWXYZ234567", b"0123456789ABCDEFGHIJKLMNOPQRSTUV"
 )
 
@@ -63,14 +62,15 @@
         self.next = self._as_bytes(next, True, 255)
         if not isinstance(windows, Bitmap):
             windows = Bitmap(windows)
         self.windows = tuple(windows.windows)
 
     def to_text(self, origin=None, relativize=True, **kw):
         next = base64.b32encode(self.next).translate(b32_normal_to_hex).lower().decode()
+        next = next.rstrip("=")
         if self.salt == b"":
             salt = "-"
         else:
             salt = binascii.hexlify(self.salt).decode()
         text = Bitmap(self.windows).to_text()
         return "%u %u %u %s %s%s" % (
             self.algorithm,
@@ -90,14 +90,18 @@
         iterations = tok.get_uint16()
         salt = tok.get_string()
         if salt == "-":
             salt = b""
         else:
             salt = binascii.unhexlify(salt.encode("ascii"))
         next = tok.get_string().encode("ascii").upper().translate(b32_hex_to_normal)
+        if next.endswith(b"="):
+            raise binascii.Error("Incorrect padding")
+        if len(next) % 8 != 0:
+            next += b"=" * (8 - len(next) % 8)
         next = base64.b32decode(next)
         bitmap = Bitmap.from_text(tok)
         return cls(rdclass, rdtype, algorithm, flags, iterations, salt, next, bitmap)
 
     def _to_wire(self, file, compress=None, origin=None, canonicalize=False):
         l = len(self.salt)
         file.write(struct.pack("!BBHB", self.algorithm, self.flags, self.iterations, l))
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/NSEC3PARAM.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/NSEC3PARAM.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import struct
 import binascii
+import struct
 
 import dns.exception
 import dns.immutable
 import dns.rdata
 
 
 @dns.immutable.immutable
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/OPENPGPKEY.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/OPENPGPKEY.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/OPT.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/OPT.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,19 +14,18 @@
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 import struct
 
 import dns.edns
-import dns.immutable
 import dns.exception
+import dns.immutable
 import dns.rdata
 
-
 # We don't implement from_text, and that's ok.
 # pylint: disable=abstract-method
 
 
 @dns.immutable.immutable
 class OPT(dns.rdata.Rdata):
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/PTR.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/PTR.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import dns.rdtypes.nsbase
 import dns.immutable
+import dns.rdtypes.nsbase
 
 
 @dns.immutable.immutable
 class PTR(dns.rdtypes.nsbase.NSBase):
 
     """PTR record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/RP.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/RP.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 import dns.exception
 import dns.immutable
-import dns.rdata
 import dns.name
+import dns.rdata
 
 
 @dns.immutable.immutable
 class RP(dns.rdata.Rdata):
 
     """RP record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/RRSIG.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/RRSIG.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 import base64
 import calendar
 import struct
 import time
 
 import dns.dnssectypes
-import dns.immutable
 import dns.exception
+import dns.immutable
 import dns.rdata
 import dns.rdatatype
 
 
 class BadSigTime(dns.exception.DNSException):
 
     """Time in DNS SIG or RRSIG resource record cannot be parsed."""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/RT.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/RT.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import dns.rdtypes.mxbase
 import dns.immutable
+import dns.rdtypes.mxbase
 
 
 @dns.immutable.immutable
 class RT(dns.rdtypes.mxbase.UncompressedDowncasingMX):
 
     """RT record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/SOA.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/SOA.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 import struct
 
 import dns.exception
 import dns.immutable
-import dns.rdata
 import dns.name
+import dns.rdata
 
 
 @dns.immutable.immutable
 class SOA(dns.rdata.Rdata):
 
     """SOA record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/SPF.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/SPF.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import dns.rdtypes.txtbase
 import dns.immutable
+import dns.rdtypes.txtbase
 
 
 @dns.immutable.immutable
 class SPF(dns.rdtypes.txtbase.TXTBase):
 
     """SPF record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/SSHFP.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/SSHFP.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import struct
 import binascii
+import struct
 
-import dns.rdata
 import dns.immutable
+import dns.rdata
 import dns.rdatatype
 
 
 @dns.immutable.immutable
 class SSHFP(dns.rdata.Rdata):
 
     """SSHFP record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/TKEY.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/TKEY.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 import base64
 import struct
 
-import dns.immutable
 import dns.exception
+import dns.immutable
 import dns.rdata
 
 
 @dns.immutable.immutable
 class TKEY(dns.rdata.Rdata):
 
     """TKEY Record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/TSIG.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/TSIG.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/TXT.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/TXT.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import dns.rdtypes.txtbase
 import dns.immutable
+import dns.rdtypes.txtbase
 
 
 @dns.immutable.immutable
 class TXT(dns.rdtypes.txtbase.TXTBase):
 
     """TXT record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/URI.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/URI.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 import struct
 
 import dns.exception
 import dns.immutable
+import dns.name
 import dns.rdata
 import dns.rdtypes.util
-import dns.name
 
 
 @dns.immutable.immutable
 class URI(dns.rdata.Rdata):
 
     """URI record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/X25.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/X25.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/ZONEMD.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/ZONEMD.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (C) Dnspython Contributors, see LICENSE for text of ISC license
 
-import struct
 import binascii
+import struct
 
 import dns.immutable
 import dns.rdata
 import dns.rdatatype
 import dns.zonetypes
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/ANY/__init__.py` & `dnspython-2.4.0rc1/dns/rdtypes/ANY/__init__.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/CH/A.py` & `dnspython-2.4.0rc1/dns/rdtypes/CH/A.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 import struct
 
-import dns.rdtypes.mxbase
 import dns.immutable
+import dns.rdtypes.mxbase
 
 
 @dns.immutable.immutable
 class A(dns.rdata.Rdata):
 
     """A record for Chaosnet"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/CH/__init__.py` & `dnspython-2.4.0rc1/dns/rdtypes/CH/__init__.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/IN/A.py` & `dnspython-2.4.0rc1/dns/rdtypes/IN/A.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/IN/AAAA.py` & `dnspython-2.4.0rc1/dns/rdtypes/IN/AAAA.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/IN/APL.py` & `dnspython-2.4.0rc1/dns/rdtypes/IN/APL.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,14 @@
 
     def _to_wire(self, file, compress=None, origin=None, canonicalize=False):
         for item in self.items:
             item.to_wire(file)
 
     @classmethod
     def from_wire_parser(cls, rdclass, rdtype, parser, origin=None):
-
         items = []
         while parser.remaining() > 0:
             header = parser.get_struct("!HBB")
             afdlen = header[2]
             if afdlen > 127:
                 negation = True
                 afdlen -= 128
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/IN/DHCID.py` & `dnspython-2.4.0rc1/dns/rdtypes/IN/DHCID.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/IN/IPSECKEY.py` & `dnspython-2.4.0rc1/dns/rdtypes/IN/IPSECKEY.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import struct
 import base64
+import struct
 
 import dns.exception
 import dns.immutable
 import dns.rdtypes.util
 
 
 class Gateway(dns.rdtypes.util.Gateway):
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/IN/KX.py` & `dnspython-2.4.0rc1/dns/rdtypes/IN/KX.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import dns.rdtypes.mxbase
 import dns.immutable
+import dns.rdtypes.mxbase
 
 
 @dns.immutable.immutable
 class KX(dns.rdtypes.mxbase.UncompressedDowncasingMX):
 
     """KX record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/IN/NAPTR.py` & `dnspython-2.4.0rc1/dns/rdtypes/IN/NAPTR.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/IN/NSAP.py` & `dnspython-2.4.0rc1/dns/rdtypes/IN/NSAP.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/IN/NSAP_PTR.py` & `dnspython-2.4.0rc1/dns/rdtypes/IN/NSAP_PTR.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import dns.rdtypes.nsbase
 import dns.immutable
+import dns.rdtypes.nsbase
 
 
 @dns.immutable.immutable
 class NSAP_PTR(dns.rdtypes.nsbase.UncompressedNS):
 
     """NSAP-PTR record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/IN/PX.py` & `dnspython-2.4.0rc1/dns/rdtypes/IN/PX.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 import struct
 
 import dns.exception
 import dns.immutable
+import dns.name
 import dns.rdata
 import dns.rdtypes.util
-import dns.name
 
 
 @dns.immutable.immutable
 class PX(dns.rdata.Rdata):
 
     """PX record."""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/IN/SRV.py` & `dnspython-2.4.0rc1/dns/rdtypes/IN/SRV.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 import struct
 
 import dns.exception
 import dns.immutable
+import dns.name
 import dns.rdata
 import dns.rdtypes.util
-import dns.name
 
 
 @dns.immutable.immutable
 class SRV(dns.rdata.Rdata):
 
     """SRV record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/IN/WKS.py` & `dnspython-2.4.0rc1/dns/rdtypes/IN/WKS.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 import socket
 import struct
 
-import dns.ipv4
 import dns.immutable
+import dns.ipv4
 import dns.rdata
 
 try:
     _proto_tcp = socket.getprotobyname("tcp")
     _proto_udp = socket.getprotobyname("udp")
 except OSError:
     # Fall back to defaults in case /etc/protocols is unavailable.
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/IN/__init__.py` & `dnspython-2.4.0rc1/dns/rdtypes/IN/__init__.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/__init__.py` & `dnspython-2.4.0rc1/dns/rdtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/dnskeybase.py` & `dnspython-2.4.0rc1/dns/rdtypes/dnskeybase.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 import base64
 import enum
 import struct
 
+import dns.dnssectypes
 import dns.exception
 import dns.immutable
-import dns.dnssectypes
 import dns.rdata
 
 # wildcard import
 __all__ = ["SEP", "REVOKE", "ZONE"]  # noqa: F822
 
 
 class Flag(enum.IntFlag):
@@ -39,15 +39,15 @@
 
     """Base class for rdata that is like a DNSKEY record"""
 
     __slots__ = ["flags", "protocol", "algorithm", "key"]
 
     def __init__(self, rdclass, rdtype, flags, protocol, algorithm, key):
         super().__init__(rdclass, rdtype)
-        self.flags = self._as_uint16(flags)
+        self.flags = Flag(self._as_uint16(flags))
         self.protocol = self._as_uint8(protocol)
         self.algorithm = dns.dnssectypes.Algorithm.make(algorithm)
         self.key = self._as_bytes(key)
 
     def to_text(self, origin=None, relativize=True, **kw):
         return "%d %d %d %s" % (
             self.flags,
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/dsbase.py` & `dnspython-2.4.0rc1/dns/rdtypes/dsbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import struct
 import binascii
+import struct
 
 import dns.dnssectypes
 import dns.immutable
 import dns.rdata
 import dns.rdatatype
 
 
@@ -40,15 +40,15 @@
         4: 48,  # SHA-384, RFC 6605 Sec. 2
     }
 
     def __init__(self, rdclass, rdtype, key_tag, algorithm, digest_type, digest):
         super().__init__(rdclass, rdtype)
         self.key_tag = self._as_uint16(key_tag)
         self.algorithm = dns.dnssectypes.Algorithm.make(algorithm)
-        self.digest_type = self._as_uint8(digest_type)
+        self.digest_type = dns.dnssectypes.DSDigest.make(self._as_uint8(digest_type))
         self.digest = self._as_bytes(digest)
         try:
             if len(self.digest) != self._digest_length_by_type[self.digest_type]:
                 raise ValueError("digest length inconsistent with digest type")
         except KeyError:
             if self.digest_type == 0:  # reserved, RFC 3658 Sec. 2.4
                 raise ValueError("digest type 0 is reserved")
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/euibase.py` & `dnspython-2.4.0rc1/dns/rdtypes/euibase.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 import binascii
 
-import dns.rdata
 import dns.immutable
+import dns.rdata
 
 
 @dns.immutable.immutable
 class EUIBase(dns.rdata.Rdata):
 
     """EUIxx record"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/mxbase.py` & `dnspython-2.4.0rc1/dns/rdtypes/mxbase.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 """MX-like base classes."""
 
 import struct
 
 import dns.exception
 import dns.immutable
-import dns.rdata
 import dns.name
+import dns.rdata
 import dns.rdtypes.util
 
 
 @dns.immutable.immutable
 class MXBase(dns.rdata.Rdata):
 
     """Base class for rdata that is like an MX record."""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/nsbase.py` & `dnspython-2.4.0rc1/dns/rdtypes/nsbase.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """NS-like base classes."""
 
 import dns.exception
 import dns.immutable
-import dns.rdata
 import dns.name
+import dns.rdata
 
 
 @dns.immutable.immutable
 class NSBase(dns.rdata.Rdata):
 
     """Base class for rdata that is like an NS record."""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/svcbbase.py` & `dnspython-2.4.0rc1/dns/rdtypes/svcbbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     MANDATORY = 0
     ALPN = 1
     NO_DEFAULT_ALPN = 2
     PORT = 3
     IPV4HINT = 4
     ECH = 5
     IPV6HINT = 6
+    DOHPATH = 7
 
     @classmethod
     def _maximum(cls):
         return 65535
 
     @classmethod
     def _short_name(cls):
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/tlsabase.py` & `dnspython-2.4.0rc1/dns/rdtypes/tlsabase.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL NOMINUM BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-import struct
 import binascii
+import struct
 
-import dns.rdata
 import dns.immutable
+import dns.rdata
 import dns.rdatatype
 
 
 @dns.immutable.immutable
 class TLSABase(dns.rdata.Rdata):
 
     """Base class for TLSA and SMIMEA records"""
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/txtbase.py` & `dnspython-2.4.0rc1/dns/rdtypes/txtbase.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,16 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """TXT-like base class."""
 
-from typing import Any, Dict, Iterable, Optional, Tuple, Union
-
 import struct
+from typing import Any, Dict, Iterable, Optional, Tuple, Union
 
 import dns.exception
 import dns.immutable
 import dns.rdata
 import dns.tokenizer
```

### Comparing `dnspython-2.3.0rc1/dns/rdtypes/util.py` & `dnspython-2.4.0rc1/dns/rdtypes/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 import collections
 import random
 import struct
+from typing import Any, List
 
 import dns.exception
 import dns.ipv4
 import dns.ipv6
 import dns.name
 import dns.rdata
 
@@ -115,48 +116,52 @@
     """A helper class for the NSEC/NSEC3/CSYNC type bitmaps"""
 
     type_name = ""
 
     def __init__(self, windows=None):
         last_window = -1
         self.windows = windows
-        for (window, bitmap) in self.windows:
+        for window, bitmap in self.windows:
             if not isinstance(window, int):
                 raise ValueError(f"bad {self.type_name} window type")
             if window <= last_window:
                 raise ValueError(f"bad {self.type_name} window order")
             if window > 256:
                 raise ValueError(f"bad {self.type_name} window number")
             last_window = window
             if not isinstance(bitmap, bytes):
                 raise ValueError(f"bad {self.type_name} octets type")
             if len(bitmap) == 0 or len(bitmap) > 32:
                 raise ValueError(f"bad {self.type_name} octets")
 
-    def to_text(self):
+    def to_text(self) -> str:
         text = ""
-        for (window, bitmap) in self.windows:
+        for window, bitmap in self.windows:
             bits = []
-            for (i, byte) in enumerate(bitmap):
+            for i, byte in enumerate(bitmap):
                 for j in range(0, 8):
                     if byte & (0x80 >> j):
                         rdtype = window * 256 + i * 8 + j
                         bits.append(dns.rdatatype.to_text(rdtype))
             text += " " + " ".join(bits)
         return text
 
     @classmethod
-    def from_text(cls, tok):
+    def from_text(cls, tok: "dns.tokenizer.Tokenizer") -> "Bitmap":
         rdtypes = []
         for token in tok.get_remaining():
             rdtype = dns.rdatatype.from_text(token.unescape().value)
             if rdtype == 0:
                 raise dns.exception.SyntaxError(f"{cls.type_name} with bit 0")
             rdtypes.append(rdtype)
-        rdtypes.sort()
+        return cls.from_rdtypes(rdtypes)
+
+    @classmethod
+    def from_rdtypes(cls, rdtypes: List[dns.rdatatype.RdataType]) -> "Bitmap":
+        rdtypes = sorted(rdtypes)
         window = 0
         octets = 0
         prior_rdtype = 0
         bitmap = bytearray(b"\0" * 32)
         windows = []
         for rdtype in rdtypes:
             if rdtype == prior_rdtype:
@@ -173,21 +178,21 @@
             bit = offset % 8
             octets = byte + 1
             bitmap[byte] = bitmap[byte] | (0x80 >> bit)
         if octets != 0:
             windows.append((window, bytes(bitmap[0:octets])))
         return cls(windows)
 
-    def to_wire(self, file):
-        for (window, bitmap) in self.windows:
+    def to_wire(self, file: Any) -> None:
+        for window, bitmap in self.windows:
             file.write(struct.pack("!BB", window, len(bitmap)))
             file.write(bitmap)
 
     @classmethod
-    def from_wire_parser(cls, parser):
+    def from_wire_parser(cls, parser: "dns.wire.Parser") -> "Bitmap":
         windows = []
         while parser.remaining() > 0:
             window = parser.get_uint8()
             bitmap = parser.get_counted_bytes()
             windows.append((window, bitmap))
         return cls(windows)
 
@@ -222,15 +227,15 @@
     by_priority = _priority_table(items)
     ordered = []
     for k in sorted(by_priority.keys()):
         rdatas = by_priority[k]
         total = sum(rdata._processing_weight() or _no_weight for rdata in rdatas)
         while len(rdatas) > 1:
             r = random.uniform(0, total)
-            for (n, rdata) in enumerate(rdatas):
+            for n, rdata in enumerate(rdatas):
                 weight = rdata._processing_weight() or _no_weight
                 if weight > r:
                     break
                 r -= weight
             total -= weight
             ordered.append(rdata)  # pylint: disable=undefined-loop-variable
             del rdatas[n]  # pylint: disable=undefined-loop-variable
```

### Comparing `dnspython-2.3.0rc1/dns/renderer.py` & `dnspython-2.4.0rc1/dns/renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,22 +15,21 @@
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """Help for building DNS wire format messages"""
 
 import contextlib
 import io
-import struct
 import random
+import struct
 import time
 
 import dns.exception
 import dns.tsig
 
-
 QUESTION = 0
 ANSWER = 1
 AUTHORITY = 2
 ADDITIONAL = 3
 
 
 class Renderer:
```

### Comparing `dnspython-2.3.0rc1/dns/resolver.py` & `dnspython-2.4.0rc1/dns/resolver.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,37 +13,39 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """DNS stub resolver."""
 
-from typing import Any, Dict, List, Optional, Tuple, Union
-
-from urllib.parse import urlparse
 import contextlib
+import random
 import socket
 import sys
 import threading
 import time
-import random
 import warnings
+from typing import Any, Dict, Iterator, List, Optional, Tuple, Union
+from urllib.parse import urlparse
 
-import dns.exception
+import dns._ddr
 import dns.edns
+import dns.exception
 import dns.flags
 import dns.inet
 import dns.ipv4
 import dns.ipv6
 import dns.message
 import dns.name
+import dns.nameserver
 import dns.query
 import dns.rcode
 import dns.rdataclass
 import dns.rdatatype
+import dns.rdtypes.svcbbase
 import dns.reversename
 import dns.tsig
 
 if sys.platform == "win32":
     import dns.win32util
 
 
@@ -68,15 +70,15 @@
         if responses is None:
             responses = {}
         elif not isinstance(responses, dict):
             raise AttributeError("responses must be a dict(qname=response)")
         kwargs = dict(qnames=qnames, responses=responses)
         return kwargs
 
-    def __str__(self):
+    def __str__(self) -> str:
         if "qnames" not in self.kwargs:
             return super().__str__()
         qnames = self.kwargs["qnames"]
         if len(qnames) > 1:
             msg = "None of DNS query names exist"
         else:
             msg = "The DNS query name does not exist"
@@ -136,27 +138,27 @@
 
 
 class YXDOMAIN(dns.exception.DNSException):
     """The DNS query name is too long after DNAME substitution."""
 
 
 ErrorTuple = Tuple[
-    Optional[str], bool, int, Union[Exception, str], Optional[dns.message.Message]
+    Optional[str],
+    bool,
+    int,
+    Union[Exception, str],
+    Optional[dns.message.Message],
 ]
 
 
 def _errors_to_text(errors: List[ErrorTuple]) -> List[str]:
     """Turn a resolution errors trace into a list of text."""
     texts = []
     for err in errors:
-        texts.append(
-            "Server {} {} port {} answered {}".format(
-                err[0], "TCP" if err[1] else "UDP", err[2], err[3]
-            )
-        )
+        texts.append("Server {} answered {}".format(err[0], err[3]))
     return texts
 
 
 class LifetimeTimeout(dns.exception.Timeout):
     """The resolution lifetime expired."""
 
     msg = "The resolution lifetime expired."
@@ -180,15 +182,15 @@
 # keep dns.resolver.Timeout defined for backwards compatibility.
 Timeout = LifetimeTimeout
 
 
 class NoAnswer(dns.exception.DNSException):
     """The DNS response does not contain an answer to the question."""
 
-    fmt = "The DNS response does not contain an answer " + "to the question: {query}"
+    fmt = "The DNS response does not contain an answer to the question: {query}"
     supp_kwargs = {"response"}
 
     # We do this as otherwise mypy complains about unexpected keyword argument
     # idna_exception
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -260,15 +262,15 @@
         self,
         qname: dns.name.Name,
         rdtype: dns.rdatatype.RdataType,
         rdclass: dns.rdataclass.RdataClass,
         response: dns.message.QueryMessage,
         nameserver: Optional[str] = None,
         port: Optional[int] = None,
-    ):
+    ) -> None:
         self.qname = qname
         self.rdtype = rdtype
         self.rdclass = rdclass
         self.response = response
         self.nameserver = nameserver
         self.port = port
         self.chaining_result = response.resolve_chaining()
@@ -288,15 +290,15 @@
         elif attr == "rdclass":
             return self.rrset.rdclass
         elif attr == "rdtype":
             return self.rrset.rdtype
         else:
             raise AttributeError(attr)
 
-    def __len__(self):
+    def __len__(self) -> int:
         return self.rrset and len(self.rrset) or 0
 
     def __iter__(self):
         return self.rrset and iter(self.rrset) or iter(tuple())
 
     def __getitem__(self, i):
         if self.rrset is None:
@@ -305,31 +307,84 @@
 
     def __delitem__(self, i):
         if self.rrset is None:
             raise IndexError
         del self.rrset[i]
 
 
+class Answers(dict):
+    """A dict of DNS stub resolver answers, indexed by type."""
+
+
+class HostAnswers(Answers):
+    """A dict of DNS stub resolver answers to a host name lookup, indexed by
+    type.
+    """
+
+    @classmethod
+    def make(
+        cls,
+        v6: Optional[Answer] = None,
+        v4: Optional[Answer] = None,
+        add_empty: bool = True,
+    ) -> "HostAnswers":
+        answers = HostAnswers()
+        if v6 is not None and (add_empty or v6.rrset):
+            answers[dns.rdatatype.AAAA] = v6
+        if v4 is not None and (add_empty or v4.rrset):
+            answers[dns.rdatatype.A] = v4
+        return answers
+
+    # Returns pairs of (address, family) from this result, potentiallys
+    # filtering by address family.
+    def addresses_and_families(
+        self, family: int = socket.AF_UNSPEC
+    ) -> Iterator[Tuple[str, int]]:
+        if family == socket.AF_UNSPEC:
+            yield from self.addresses_and_families(socket.AF_INET6)
+            yield from self.addresses_and_families(socket.AF_INET)
+            return
+        elif family == socket.AF_INET6:
+            answer = self.get(dns.rdatatype.AAAA)
+        elif family == socket.AF_INET:
+            answer = self.get(dns.rdatatype.A)
+        else:
+            raise NotImplementedError(f"unknown address family {family}")
+        if answer:
+            for rdata in answer:
+                yield (rdata.address, family)
+
+    # Returns addresses from this result, potentially filtering by
+    # address family.
+    def addresses(self, family: int = socket.AF_UNSPEC) -> Iterator[str]:
+        return (pair[0] for pair in self.addresses_and_families(family))
+
+    # Returns the canonical name from this result.
+    def canonical_name(self) -> dns.name.Name:
+        answer = self.get(dns.rdatatype.AAAA, self.get(dns.rdatatype.A))
+        return answer.canonical_name
+
+
 class CacheStatistics:
     """Cache Statistics"""
 
-    def __init__(self, hits=0, misses=0):
+    def __init__(self, hits: int = 0, misses: int = 0) -> None:
         self.hits = hits
         self.misses = misses
 
-    def reset(self):
+    def reset(self) -> None:
         self.hits = 0
         self.misses = 0
 
     def clone(self) -> "CacheStatistics":
         return CacheStatistics(self.hits, self.misses)
 
 
 class CacheBase:
-    def __init__(self):
+    def __init__(self) -> None:
         self.lock = threading.Lock()
         self.statistics = CacheStatistics()
 
     def reset_statistics(self) -> None:
         """Reset all statistics to zero."""
         with self.lock:
             self.statistics.reset()
@@ -357,15 +412,15 @@
 
 CacheKey = Tuple[dns.name.Name, dns.rdatatype.RdataType, dns.rdataclass.RdataClass]
 
 
 class Cache(CacheBase):
     """Simple thread-safe DNS answer cache."""
 
-    def __init__(self, cleaning_interval: float = 300.0):
+    def __init__(self, cleaning_interval: float = 300.0) -> None:
         """*cleaning_interval*, a ``float`` is the number of seconds between
         periodic cleanings.
         """
 
         super().__init__()
         self.data: Dict[CacheKey, Answer] = {}
         self.cleaning_interval = cleaning_interval
@@ -373,15 +428,15 @@
 
     def _maybe_clean(self) -> None:
         """Clean the cache if it's time to do so."""
 
         now = time.time()
         if self.next_cleaning <= now:
             keys_to_delete = []
-            for (k, v) in self.data.items():
+            for k, v in self.data.items():
                 if v.expiration <= now:
                     keys_to_delete.append(k)
             for k in keys_to_delete:
                 del self.data[k]
             now = time.time()
             self.next_cleaning = now + self.cleaning_interval
 
@@ -443,36 +498,36 @@
     def __init__(self, key, value):
         self.key = key
         self.value = value
         self.hits = 0
         self.prev = self
         self.next = self
 
-    def link_after(self, node):
+    def link_after(self, node: "LRUCacheNode") -> None:
         self.prev = node
         self.next = node.next
         node.next.prev = self
         node.next = self
 
-    def unlink(self):
+    def unlink(self) -> None:
         self.next.prev = self.prev
         self.prev.next = self.next
 
 
 class LRUCache(CacheBase):
     """Thread-safe, bounded, least-recently-used DNS answer cache.
 
     This cache is better than the simple cache (above) if you're
     running a web crawler or other process that does a lot of
     resolutions.  The LRUCache has a maximum number of nodes, and when
     it is full, the least-recently used node is removed to make space
     for a new one.
     """
 
-    def __init__(self, max_size: int = 100000):
+    def __init__(self, max_size: int = 100000) -> None:
         """*max_size*, an ``int``, is the maximum number of nodes to cache;
         it must be greater than 0.
         """
 
         super().__init__()
         self.data: Dict[CacheKey, LRUCacheNode] = {}
         self.set_max_size(max_size)
@@ -586,38 +641,37 @@
         resolver: "BaseResolver",
         qname: Union[dns.name.Name, str],
         rdtype: Union[dns.rdatatype.RdataType, str],
         rdclass: Union[dns.rdataclass.RdataClass, str],
         tcp: bool,
         raise_on_no_answer: bool,
         search: Optional[bool],
-    ):
+    ) -> None:
         if isinstance(qname, str):
             qname = dns.name.from_text(qname, None)
-        the_rdtype = dns.rdatatype.RdataType.make(rdtype)
-        if dns.rdatatype.is_metatype(the_rdtype):
+        rdtype = dns.rdatatype.RdataType.make(rdtype)
+        if dns.rdatatype.is_metatype(rdtype):
             raise NoMetaqueries
-        the_rdclass = dns.rdataclass.RdataClass.make(rdclass)
-        if dns.rdataclass.is_metaclass(the_rdclass):
+        rdclass = dns.rdataclass.RdataClass.make(rdclass)
+        if dns.rdataclass.is_metaclass(rdclass):
             raise NoMetaqueries
         self.resolver = resolver
         self.qnames_to_try = resolver._get_qnames_to_try(qname, search)
         self.qnames = self.qnames_to_try[:]
-        self.rdtype = the_rdtype
-        self.rdclass = the_rdclass
+        self.rdtype = rdtype
+        self.rdclass = rdclass
         self.tcp = tcp
         self.raise_on_no_answer = raise_on_no_answer
         self.nxdomain_responses: Dict[dns.name.Name, dns.message.QueryMessage] = {}
         # Initialize other things to help analysis tools
         self.qname = dns.name.empty
-        self.nameservers: List[str] = []
-        self.current_nameservers: List[str] = []
+        self.nameservers: List[dns.nameserver.Nameserver] = []
+        self.current_nameservers: List[dns.nameserver.Nameserver] = []
         self.errors: List[ErrorTuple] = []
-        self.nameserver: Optional[str] = None
-        self.port = 0
+        self.nameserver: Optional[dns.nameserver.Nameserver] = None
         self.tcp_attempt = False
         self.retry_with_tcp = False
         self.request: Optional[dns.message.QueryMessage] = None
         self.backoff = 0.0
 
     def next_request(
         self,
@@ -666,15 +720,19 @@
                 self.resolver.ednsflags,
                 self.resolver.payload,
                 options=self.resolver.ednsoptions,
             )
             if self.resolver.flags is not None:
                 request.flags = self.resolver.flags
 
-            self.nameservers = self.resolver.nameservers[:]
+            self.nameservers = self.resolver._enrich_nameservers(
+                self.resolver._nameservers,
+                self.resolver.nameserver_ports,
+                self.resolver.port,
+            )
             if self.resolver.rotate:
                 random.shuffle(self.nameservers)
             self.current_nameservers = self.nameservers[:]
             self.errors = []
             self.nameserver = None
             self.tcp_attempt = False
             self.retry_with_tcp = False
@@ -686,49 +744,53 @@
         #
         # We've tried everything and only gotten NXDOMAINs.  (We know
         # it's only NXDOMAINs as anything else would have returned
         # before now.)
         #
         raise NXDOMAIN(qnames=self.qnames_to_try, responses=self.nxdomain_responses)
 
-    def next_nameserver(self) -> Tuple[str, int, bool, float]:
+    def next_nameserver(self) -> Tuple[dns.nameserver.Nameserver, bool, float]:
         if self.retry_with_tcp:
             assert self.nameserver is not None
+            assert not self.nameserver.is_always_max_size()
             self.tcp_attempt = True
             self.retry_with_tcp = False
-            return (self.nameserver, self.port, True, 0)
+            return (self.nameserver, True, 0)
 
         backoff = 0.0
         if not self.current_nameservers:
             if len(self.nameservers) == 0:
                 # Out of things to try!
                 raise NoNameservers(request=self.request, errors=self.errors)
             self.current_nameservers = self.nameservers[:]
             backoff = self.backoff
             self.backoff = min(self.backoff * 2, 2)
 
         self.nameserver = self.current_nameservers.pop(0)
-        self.port = self.resolver.nameserver_ports.get(
-            self.nameserver, self.resolver.port
-        )
-        self.tcp_attempt = self.tcp
-        return (self.nameserver, self.port, self.tcp_attempt, backoff)
+        self.tcp_attempt = self.tcp or self.nameserver.is_always_max_size()
+        return (self.nameserver, self.tcp_attempt, backoff)
 
     def query_result(
         self, response: Optional[dns.message.Message], ex: Optional[Exception]
     ) -> Tuple[Optional[Answer], bool]:
         #
         # returns an (answer: Answer, end_loop: bool) tuple.
         #
         assert self.nameserver is not None
         if ex:
             # Exception during I/O or from_wire()
             assert response is None
             self.errors.append(
-                (self.nameserver, self.tcp_attempt, self.port, ex, response)
+                (
+                    str(self.nameserver),
+                    self.tcp_attempt,
+                    self.nameserver.answer_port(),
+                    ex,
+                    response,
+                )
             )
             if (
                 isinstance(ex, dns.exception.FormError)
                 or isinstance(ex, EOFError)
                 or isinstance(ex, OSError)
                 or isinstance(ex, NotImplementedError)
             ):
@@ -748,20 +810,26 @@
         if rcode == dns.rcode.NOERROR:
             try:
                 answer = Answer(
                     self.qname,
                     self.rdtype,
                     self.rdclass,
                     response,
-                    self.nameserver,
-                    self.port,
+                    self.nameserver.answer_nameserver(),
+                    self.nameserver.answer_port(),
                 )
             except Exception as e:
                 self.errors.append(
-                    (self.nameserver, self.tcp_attempt, self.port, e, response)
+                    (
+                        str(self.nameserver),
+                        self.tcp_attempt,
+                        self.nameserver.answer_port(),
+                        e,
+                        response,
+                    )
                 )
                 # The nameserver is no good, take it out of the mix.
                 self.nameservers.remove(self.nameserver)
                 return (None, False)
             if self.resolver.cache:
                 self.resolver.cache.put((self.qname, self.rdtype, self.rdclass), answer)
             if answer.rrset is None and self.raise_on_no_answer:
@@ -772,15 +840,21 @@
             # if we aren't going to cache it.
             try:
                 answer = Answer(
                     self.qname, dns.rdatatype.ANY, dns.rdataclass.IN, response
                 )
             except Exception as e:
                 self.errors.append(
-                    (self.nameserver, self.tcp_attempt, self.port, e, response)
+                    (
+                        str(self.nameserver),
+                        self.tcp_attempt,
+                        self.nameserver.answer_port(),
+                        e,
+                        response,
+                    )
                 )
                 # The nameserver is no good, take it out of the mix.
                 self.nameservers.remove(self.nameserver)
                 return (None, False)
             self.nxdomain_responses[self.qname] = response
             if self.resolver.cache:
                 self.resolver.cache.put(
@@ -788,29 +862,35 @@
                 )
             # Make next_nameserver() return None, so caller breaks its
             # inner loop and calls next_request().
             return (None, True)
         elif rcode == dns.rcode.YXDOMAIN:
             yex = YXDOMAIN()
             self.errors.append(
-                (self.nameserver, self.tcp_attempt, self.port, yex, response)
+                (
+                    str(self.nameserver),
+                    self.tcp_attempt,
+                    self.nameserver.answer_port(),
+                    yex,
+                    response,
+                )
             )
             raise yex
         else:
             #
             # We got a response, but we're not happy with the
             # rcode in it.
             #
             if rcode != dns.rcode.SERVFAIL or not self.resolver.retry_servfail:
                 self.nameservers.remove(self.nameserver)
             self.errors.append(
                 (
-                    self.nameserver,
+                    str(self.nameserver),
                     self.tcp_attempt,
-                    self.port,
+                    self.nameserver.answer_port(),
                     dns.rcode.to_text(rcode),
                     response,
                 )
             )
             return (None, False)
 
 
@@ -836,16 +916,19 @@
     ednsoptions: Optional[List[dns.edns.Option]]
     payload: int
     cache: Any
     flags: Optional[int]
     retry_servfail: bool
     rotate: bool
     ndots: Optional[int]
+    _nameservers: List[Union[str, dns.nameserver.Nameserver]]
 
-    def __init__(self, filename: str = "/etc/resolv.conf", configure: bool = True):
+    def __init__(
+        self, filename: str = "/etc/resolv.conf", configure: bool = True
+    ) -> None:
         """*filename*, a ``str`` or file object, specifying a file
         in standard /etc/resolv.conf format.  This parameter is meaningful
         only when *configure* is true and the platform is POSIX.
 
         *configure*, a ``bool``.  If True (the default), the resolver
         instance is configured in the normal fashion for the operating
         system the resolver is running on.  (I.e. by reading a
@@ -856,21 +939,21 @@
         self.reset()
         if configure:
             if sys.platform == "win32":
                 self.read_registry()
             elif filename:
                 self.read_resolv_conf(filename)
 
-    def reset(self):
+    def reset(self) -> None:
         """Reset all resolver configuration to the defaults."""
 
         self.domain = dns.name.Name(dns.name.from_text(socket.gethostname())[1:])
         if len(self.domain) == 0:
             self.domain = dns.name.root
-        self.nameservers = []
+        self._nameservers = []
         self.nameserver_ports = {}
         self.port = 53
         self.search = []
         self.use_search_by_default = False
         self.timeout = 2.0
         self.lifetime = 5.0
         self.keyring = None
@@ -899,14 +982,15 @@
 
         - search - search list for host-name lookup
 
         - options - supported options are rotate, timeout, edns0, and ndots
 
         """
 
+        nameservers = []
         if isinstance(f, str):
             try:
                 cm: contextlib.AbstractContextManager = open(f)
             except OSError:
                 # /etc/resolv.conf doesn't exist, can't be read, etc.
                 raise NoResolverConfiguration(f"cannot open {f}")
         else:
@@ -918,15 +1002,15 @@
                 tokens = l.split()
 
                 # Any line containing less than 2 tokens is malformed
                 if len(tokens) < 2:
                     continue
 
                 if tokens[0] == "nameserver":
-                    self.nameservers.append(tokens[1])
+                    nameservers.append(tokens[1])
                 elif tokens[0] == "domain":
                     self.domain = dns.name.from_text(tokens[1])
                     # domain and search are exclusive
                     self.search = []
                 elif tokens[0] == "search":
                     # the last search wins
                     self.search = []
@@ -946,16 +1030,19 @@
                             except (ValueError, IndexError):
                                 pass
                         elif "ndots" in opt:
                             try:
                                 self.ndots = int(opt.split(":")[1])
                             except (ValueError, IndexError):
                                 pass
-        if len(self.nameservers) == 0:
+        if len(nameservers) == 0:
             raise NoResolverConfiguration("no nameservers")
+        # Assigning directly instead of appending means we invoke the
+        # setter logic, with additonal checking and enrichment.
+        self.nameservers = nameservers
 
     def read_registry(self) -> None:
         """Extract resolver configuration from the Windows registry."""
         try:
             info = dns.win32util.get_dns_info()  # type: ignore
             if info.domain is not None:
                 self.domain = info.domain
@@ -1082,42 +1169,72 @@
         """Overrides the default flags with your own.
 
         *flags*, an ``int``, the message flags to use.
         """
 
         self.flags = flags
 
-    @property
-    def nameservers(self) -> List[str]:
-        return self._nameservers
-
-    @nameservers.setter
-    def nameservers(self, nameservers: List[str]) -> None:
-        """
-        *nameservers*, a ``list`` of nameservers.
-
-        Raises ``ValueError`` if *nameservers* is anything other than a
-        ``list``.
-        """
+    @classmethod
+    def _enrich_nameservers(
+        cls,
+        nameservers: List[Union[str, dns.nameserver.Nameserver]],
+        nameserver_ports: Dict[str, int],
+        default_port: int,
+    ) -> List[dns.nameserver.Nameserver]:
+        enriched_nameservers = []
         if isinstance(nameservers, list):
             for nameserver in nameservers:
-                if not dns.inet.is_address(nameserver):
+                enriched_nameserver: dns.nameserver.Nameserver
+                if isinstance(nameserver, dns.nameserver.Nameserver):
+                    enriched_nameserver = nameserver
+                elif dns.inet.is_address(nameserver):
+                    port = nameserver_ports.get(nameserver, default_port)
+                    enriched_nameserver = dns.nameserver.Do53Nameserver(
+                        nameserver, port
+                    )
+                else:
                     try:
                         if urlparse(nameserver).scheme != "https":
                             raise NotImplementedError
                     except Exception:
                         raise ValueError(
-                            f"nameserver {nameserver} is not an "
-                            "IP address or valid https URL"
+                            f"nameserver {nameserver} is not a "
+                            "dns.nameserver.Nameserver instance or text form, "
+                            "IP address, nor a valid https URL"
                         )
-            self._nameservers = nameservers
+                    enriched_nameserver = dns.nameserver.DoHNameserver(nameserver)
+                enriched_nameservers.append(enriched_nameserver)
         else:
             raise ValueError(
-                "nameservers must be a list (not a {})".format(type(nameservers))
+                "nameservers must be a list or tuple (not a {})".format(
+                    type(nameservers)
+                )
             )
+        return enriched_nameservers
+
+    @property
+    def nameservers(
+        self,
+    ) -> List[Union[str, dns.nameserver.Nameserver]]:
+        return self._nameservers
+
+    @nameservers.setter
+    def nameservers(
+        self, nameservers: List[Union[str, dns.nameserver.Nameserver]]
+    ) -> None:
+        """
+        *nameservers*, a ``list`` of nameservers, where a nameserver is either
+        a string interpretable as a nameserver, or a ``dns.nameserver.Nameserver``
+        instance.
+
+        Raises ``ValueError`` if *nameservers* is not a list of nameservers.
+        """
+        # We just call _enrich_nameservers() for checking
+        self._enrich_nameservers(nameservers, self.nameserver_ports, self.port)
+        self._nameservers = nameservers
 
 
 class Resolver(BaseResolver):
     """DNS stub resolver."""
 
     def resolve(
         self,
@@ -1194,41 +1311,26 @@
             # object, including in cases where its length is 0.
             if answer is not None:
                 # cache hit!
                 return answer
             assert request is not None  # needed for type checking
             done = False
             while not done:
-                (nameserver, port, tcp, backoff) = resolution.next_nameserver()
+                (nameserver, tcp, backoff) = resolution.next_nameserver()
                 if backoff:
                     time.sleep(backoff)
                 timeout = self._compute_timeout(start, lifetime, resolution.errors)
                 try:
-                    if dns.inet.is_address(nameserver):
-                        if tcp:
-                            response = dns.query.tcp(
-                                request,
-                                nameserver,
-                                timeout=timeout,
-                                port=port,
-                                source=source,
-                                source_port=source_port,
-                            )
-                        else:
-                            response = dns.query.udp(
-                                request,
-                                nameserver,
-                                timeout=timeout,
-                                port=port,
-                                source=source,
-                                source_port=source_port,
-                                raise_on_truncation=True,
-                            )
-                    else:
-                        response = dns.query.https(request, nameserver, timeout=timeout)
+                    response = nameserver.query(
+                        request,
+                        timeout=timeout,
+                        source=source,
+                        source_port=source_port,
+                        max_size=tcp,
+                    )
                 except Exception as ex:
                     (_, done) = resolution.query_result(None, ex)
                     continue
                 (answer, done) = resolution.query_result(response, None)
                 # Note we need to say "if answer is not None" and not just
                 # "if answer" because answer implements __len__, and python
                 # will call that.  We want to return if we have an answer
@@ -1289,15 +1391,80 @@
         # in the kwargs more than once.
         modified_kwargs: Dict[str, Any] = {}
         modified_kwargs.update(kwargs)
         modified_kwargs["rdtype"] = dns.rdatatype.PTR
         modified_kwargs["rdclass"] = dns.rdataclass.IN
         return self.resolve(
             dns.reversename.from_address(ipaddr), *args, **modified_kwargs
-        )  # type: ignore[arg-type]
+        )
+
+    def resolve_name(
+        self,
+        name: Union[dns.name.Name, str],
+        family: int = socket.AF_UNSPEC,
+        **kwargs: Any,
+    ) -> HostAnswers:
+        """Use a resolver to query for address records.
+
+        This utilizes the resolve() method to perform A and/or AAAA lookups on
+        the specified name.
+
+        *qname*, a ``dns.name.Name`` or ``str``, the name to resolve.
+
+        *family*, an ``int``, the address family.  If socket.AF_UNSPEC
+        (the default), both A and AAAA records will be retrieved.
+
+        All other arguments that can be passed to the resolve() function
+        except for rdtype and rdclass are also supported by this
+        function.
+        """
+        # We make a modified kwargs for type checking happiness, as otherwise
+        # we get a legit warning about possibly having rdtype and rdclass
+        # in the kwargs more than once.
+        modified_kwargs: Dict[str, Any] = {}
+        modified_kwargs.update(kwargs)
+        modified_kwargs.pop("rdtype", None)
+        modified_kwargs["rdclass"] = dns.rdataclass.IN
+
+        if family == socket.AF_INET:
+            v4 = self.resolve(name, dns.rdatatype.A, **modified_kwargs)
+            return HostAnswers.make(v4=v4)
+        elif family == socket.AF_INET6:
+            v6 = self.resolve(name, dns.rdatatype.AAAA, **modified_kwargs)
+            return HostAnswers.make(v6=v6)
+        elif family != socket.AF_UNSPEC:
+            raise NotImplementedError(f"unknown address family {family}")
+
+        raise_on_no_answer = modified_kwargs.pop("raise_on_no_answer", True)
+        lifetime = modified_kwargs.pop("lifetime", None)
+        start = time.time()
+        v6 = self.resolve(
+            name,
+            dns.rdatatype.AAAA,
+            raise_on_no_answer=False,
+            lifetime=self._compute_timeout(start, lifetime),
+            **modified_kwargs,
+        )
+        # Note that setting name ensures we query the same name
+        # for A as we did for AAAA.  (This is just in case search lists
+        # are active by default in the resolver configuration and
+        # we might be talking to a server that says NXDOMAIN when it
+        # wants to say NOERROR no data.
+        name = v6.qname
+        v4 = self.resolve(
+            name,
+            dns.rdatatype.A,
+            raise_on_no_answer=False,
+            lifetime=self._compute_timeout(start, lifetime),
+            **modified_kwargs,
+        )
+        answers = HostAnswers.make(v6=v6, v4=v4, add_empty=not raise_on_no_answer)
+        if not answers:
+            raise NoAnswer(response=v6.response)
+        return answers
 
     # pylint: disable=redefined-outer-name
 
     def canonical_name(self, name: Union[dns.name.Name, str]) -> dns.name.Name:
         """Determine the canonical name of *name*.
 
         The canonical name is the name the resolver uses for queries
@@ -1316,28 +1483,59 @@
             canonical_name = answer.canonical_name
         except dns.resolver.NXDOMAIN as e:
             canonical_name = e.canonical_name
         return canonical_name
 
     # pylint: enable=redefined-outer-name
 
+    def try_ddr(self, lifetime: float = 5.0) -> None:
+        """Try to update the resolver's nameservers using Discovery of Designated
+        Resolvers (DDR).  If successful, the resolver will subsequently use
+        DNS-over-HTTPS or DNS-over-TLS for future queries.
+
+        *lifetime*, a float, is the maximum time to spend attempting DDR.  The default
+        is 5 seconds.
+
+        If the SVCB query is successful and results in a non-empty list of nameservers,
+        then the resolver's nameservers are set to the returned servers in priority
+        order.
+
+        The current implementation does not use any address hints from the SVCB record,
+        nor does it resolve addresses for the SCVB target name, rather it assumes that
+        the bootstrap nameserver will always be one of the addresses and uses it.
+        A future revision to the code may offer fuller support.  The code verifies that
+        the bootstrap nameserver is in the Subject Alternative Name field of the
+        TLS certficate.
+        """
+        try:
+            expiration = time.time() + lifetime
+            answer = self.resolve(
+                dns._ddr._local_resolver_name, "SVCB", lifetime=lifetime
+            )
+            timeout = dns.query._remaining(expiration)
+            nameservers = dns._ddr._get_nameservers_sync(answer, timeout)
+            if len(nameservers) > 0:
+                self.nameservers = nameservers
+        except Exception:
+            pass
+
 
 #: The default resolver.
 default_resolver: Optional[Resolver] = None
 
 
 def get_default_resolver() -> Resolver:
     """Get the default resolver, initializing it if necessary."""
     if default_resolver is None:
         reset_default_resolver()
     assert default_resolver is not None
     return default_resolver
 
 
-def reset_default_resolver():
+def reset_default_resolver() -> None:
     """Re-initialize default resolver.
 
     Note that the resolver configuration (i.e. /etc/resolv.conf on UNIX
     systems) will be re-read immediately.
     """
 
     global default_resolver
@@ -1351,15 +1549,14 @@
     tcp: bool = False,
     source: Optional[str] = None,
     raise_on_no_answer: bool = True,
     source_port: int = 0,
     lifetime: Optional[float] = None,
     search: Optional[bool] = None,
 ) -> Answer:  # pragma: no cover
-
     """Query nameservers to find the answer to the question.
 
     This is a convenience function that uses the default resolver
     object to make the query.
 
     See ``dns.resolver.Resolver.resolve`` for more information on the
     parameters.
@@ -1417,24 +1614,46 @@
     See ``dns.resolver.Resolver.resolve_address`` for more information on the
     parameters.
     """
 
     return get_default_resolver().resolve_address(ipaddr, *args, **kwargs)
 
 
+def resolve_name(
+    name: Union[dns.name.Name, str], family: int = socket.AF_UNSPEC, **kwargs: Any
+) -> HostAnswers:
+    """Use a resolver to query for address records.
+
+    See ``dns.resolver.Resolver.resolve_name`` for more information on the
+    parameters.
+    """
+
+    return get_default_resolver().resolve_name(name, family, **kwargs)
+
+
 def canonical_name(name: Union[dns.name.Name, str]) -> dns.name.Name:
     """Determine the canonical name of *name*.
 
     See ``dns.resolver.Resolver.canonical_name`` for more information on the
     parameters and possible exceptions.
     """
 
     return get_default_resolver().canonical_name(name)
 
 
+def try_ddr(lifetime: float = 5.0) -> None:
+    """Try to update the default resolver's nameservers using Discovery of Designated
+    Resolvers (DDR).  If successful, the resolver will subsequently use
+    DNS-over-HTTPS or DNS-over-TLS for future queries.
+
+    See :py:func:`dns.resolver.Resolver.try_ddr` for more information.
+    """
+    return get_default_resolver().try_ddr(lifetime)
+
+
 def zone_for_name(
     name: Union[dns.name.Name, str],
     rdclass: dns.rdataclass.RdataClass = dns.rdataclass.IN,
     tcp: bool = False,
     resolver: Optional[Resolver] = None,
     lifetime: Optional[float] = None,
 ) -> dns.name.Name:
@@ -1512,14 +1731,91 @@
             # a type 3 NXDOMAIN)
         try:
             name = name.parent()
         except dns.name.NoParent:
             raise NoRootSOA
 
 
+def make_resolver_at(
+    where: Union[dns.name.Name, str],
+    port: int = 53,
+    family: int = socket.AF_UNSPEC,
+    resolver: Optional[Resolver] = None,
+) -> Resolver:
+    """Make a stub resolver using the specified destination as the full resolver.
+
+    *where*, a ``dns.name.Name`` or ``str`` the domain name or IP address of the
+    full resolver.
+
+    *port*, an ``int``, the port to use.  If not specified, the default is 53.
+
+    *family*, an ``int``, the address family to use.  This parameter is used if
+    *where* is not an address.  The default is ``socket.AF_UNSPEC`` in which case
+    the first address returned by ``resolve_name()`` will be used, otherwise the
+    first address of the specified family will be used.
+
+    *resolver*, a ``dns.resolver.Resolver`` or ``None``, the resolver to use for
+    resolution of hostnames.  If not specified, the default resolver will be used.
+
+    Returns a ``dns.resolver.Resolver`` or raises an exception.
+    """
+    if resolver is None:
+        resolver = get_default_resolver()
+    nameservers: List[Union[str, dns.nameserver.Nameserver]] = []
+    if isinstance(where, str) and dns.inet.is_address(where):
+        nameservers.append(dns.nameserver.Do53Nameserver(where, port))
+    else:
+        for address in resolver.resolve_name(where, family).addresses():
+            nameservers.append(dns.nameserver.Do53Nameserver(address, port))
+    res = dns.resolver.Resolver(configure=False)
+    res.nameservers = nameservers
+    return res
+
+
+def resolve_at(
+    where: Union[dns.name.Name, str],
+    qname: Union[dns.name.Name, str],
+    rdtype: Union[dns.rdatatype.RdataType, str] = dns.rdatatype.A,
+    rdclass: Union[dns.rdataclass.RdataClass, str] = dns.rdataclass.IN,
+    tcp: bool = False,
+    source: Optional[str] = None,
+    raise_on_no_answer: bool = True,
+    source_port: int = 0,
+    lifetime: Optional[float] = None,
+    search: Optional[bool] = None,
+    port: int = 53,
+    family: int = socket.AF_UNSPEC,
+    resolver: Optional[Resolver] = None,
+) -> Answer:
+    """Query nameservers to find the answer to the question.
+
+    This is a convenience function that calls ``dns.resolver.make_resolver_at()`` to
+    make a resolver, and then uses it to resolve the query.
+
+    See ``dns.resolver.Resolver.resolve`` for more information on the resolution
+    parameters, and ``dns.resolver.make_resolver_at`` for information about the resolver
+    parameters *where*, *port*, *family*, and *resolver*.
+
+    If making more than one query, it is more efficient to call
+    ``dns.resolver.make_resolver_at()`` and then use that resolver for the queries
+    instead of calling ``resolve_at()`` multiple times.
+    """
+    return make_resolver_at(where, port, family, resolver).resolve(
+        qname,
+        rdtype,
+        rdclass,
+        tcp,
+        source,
+        raise_on_no_answer,
+        source_port,
+        lifetime,
+        search,
+    )
+
+
 #
 # Support for overriding the system resolver for all python code in the
 # running process.
 #
 
 _protocols_for_socktype = {
     socket.SOCK_DGRAM: [socket.SOL_UDP],
@@ -1555,16 +1851,15 @@
         # EAI_BADFLAGS as the flags aren't bad, we just don't
         # implement them.
         raise socket.gaierror(
             socket.EAI_FAIL, "Non-recoverable failure in name resolution"
         )
     if host is None and service is None:
         raise socket.gaierror(socket.EAI_NONAME, "Name or service not known")
-    v6addrs = []
-    v4addrs = []
+    addrs = []
     canonical_name = None  # pylint: disable=redefined-outer-name
     # Is host None or an address literal?  If so, use the system's
     # getaddrinfo().
     if host is None:
         return _original_getaddrinfo(host, service, family, socktype, proto, flags)
     try:
         # We don't care about the result of af_for_address(), we're just
@@ -1572,32 +1867,17 @@
         # IPv6 address.
         dns.inet.af_for_address(host)
         return _original_getaddrinfo(host, service, family, socktype, proto, flags)
     except Exception:
         pass
     # Something needs resolution!
     try:
-        if family == socket.AF_INET6 or family == socket.AF_UNSPEC:
-            v6 = _resolver.resolve(host, dns.rdatatype.AAAA, raise_on_no_answer=False)
-            # Note that setting host ensures we query the same name
-            # for A as we did for AAAA.  (This is just in case search lists
-            # are active by default in the resolver configuration and
-            # we might be talking to a server that says NXDOMAIN when it
-            # wants to say NOERROR no data.
-            host = v6.qname
-            canonical_name = v6.canonical_name.to_text(True)
-            if v6.rrset is not None:
-                for rdata in v6.rrset:
-                    v6addrs.append(rdata.address)
-        if family == socket.AF_INET or family == socket.AF_UNSPEC:
-            v4 = _resolver.resolve(host, dns.rdatatype.A, raise_on_no_answer=False)
-            canonical_name = v4.canonical_name.to_text(True)
-            if v4.rrset is not None:
-                for rdata in v4.rrset:
-                    v4addrs.append(rdata.address)
+        answers = _resolver.resolve_name(host, family)
+        addrs = answers.addresses_and_families()
+        canonical_name = answers.canonical_name().to_text(True)
     except dns.resolver.NXDOMAIN:
         raise socket.gaierror(socket.EAI_NONAME, "Name or service not known")
     except Exception:
         # We raise EAI_AGAIN here as the failure may be temporary
         # (e.g. a timeout) and EAI_SYSTEM isn't defined on Windows.
         # [Issue #416]
         raise socket.gaierror(socket.EAI_AGAIN, "Temporary failure in name resolution")
@@ -1621,28 +1901,19 @@
         socktypes = [socket.SOCK_DGRAM, socket.SOCK_STREAM]
     else:
         socktypes = [socktype]
     if flags & socket.AI_CANONNAME != 0:
         cname = canonical_name
     else:
         cname = ""
-    if family == socket.AF_INET6 or family == socket.AF_UNSPEC:
-        for addr in v6addrs:
-            for socktype in socktypes:
-                for proto in _protocols_for_socktype[socktype]:
-                    tuples.append(
-                        (socket.AF_INET6, socktype, proto, cname, (addr, port, 0, 0))
-                    )
-    if family == socket.AF_INET or family == socket.AF_UNSPEC:
-        for addr in v4addrs:
-            for socktype in socktypes:
-                for proto in _protocols_for_socktype[socktype]:
-                    tuples.append(
-                        (socket.AF_INET, socktype, proto, cname, (addr, port))
-                    )
+    for addr, af in addrs:
+        for socktype in socktypes:
+            for proto in _protocols_for_socktype[socktype]:
+                addr_tuple = dns.inet.low_level_address_tuple((addr, port), af)
+                tuples.append((af, socktype, proto, cname, addr_tuple))
     if len(tuples) == 0:
         raise socket.gaierror(socket.EAI_NONAME, "Name or service not known")
     return tuples
 
 
 def _getnameinfo(sockaddr, flags=0):
     host = sockaddr[0]
```

### Comparing `dnspython-2.3.0rc1/dns/reversename.py` & `dnspython-2.4.0rc1/dns/reversename.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """DNS Reverse Map Names."""
 
 import binascii
 
-import dns.name
-import dns.ipv6
 import dns.ipv4
+import dns.ipv6
+import dns.name
 
 ipv4_reverse_domain = dns.name.from_text("in-addr.arpa.")
 ipv6_reverse_domain = dns.name.from_text("ip6.arpa.")
 
 
 def from_address(
     text: str,
```

### Comparing `dnspython-2.3.0rc1/dns/rrset.py` & `dnspython-2.4.0rc1/dns/rrset.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """DNS RRsets (an RRset is a named rdataset)"""
 
-from typing import Any, cast, Collection, Dict, Optional, Union
+from typing import Any, Collection, Dict, Optional, Union, cast
 
 import dns.name
-import dns.rdataset
 import dns.rdataclass
+import dns.rdataset
 import dns.renderer
 
 
 class RRset(dns.rdataset.Rdataset):
 
     """A DNS RRset (named rdataset).
 
@@ -210,17 +210,17 @@
     when relativizing names.  If not set, the *origin* value will be used.
 
     Returns a ``dns.rrset.RRset`` object.
     """
 
     if isinstance(name, str):
         name = dns.name.from_text(name, None, idna_codec=idna_codec)
-    the_rdclass = dns.rdataclass.RdataClass.make(rdclass)
-    the_rdtype = dns.rdatatype.RdataType.make(rdtype)
-    r = RRset(name, the_rdclass, the_rdtype)
+    rdclass = dns.rdataclass.RdataClass.make(rdclass)
+    rdtype = dns.rdatatype.RdataType.make(rdtype)
+    r = RRset(name, rdclass, rdtype)
     r.update_ttl(ttl)
     for t in text_rdatas:
         rd = dns.rdata.from_text(
             r.rdclass, r.rdtype, t, origin, relativize, relativize_to, idna_codec
         )
         r.add(rd)
     return r
```

### Comparing `dnspython-2.3.0rc1/dns/serial.py` & `dnspython-2.4.0rc1/dns/serial.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/set.py` & `dnspython-2.4.0rc1/dns/set.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/tokenizer.py` & `dnspython-2.4.0rc1/dns/tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,17 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """Tokenize DNS zone file format"""
 
-from typing import Any, Optional, List, Tuple
-
 import io
 import sys
+from typing import Any, List, Optional, Tuple
 
 import dns.exception
 import dns.name
 import dns.ttl
 
 _DELIMITERS = {" ", "\t", "\n", ";", "(", ")", '"'}
 _QUOTING_DELIMITERS = {'"'}
```

### Comparing `dnspython-2.3.0rc1/dns/transaction.py` & `dnspython-2.4.0rc1/dns/transaction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright (C) Dnspython Contributors, see LICENSE for text of ISC license
 
-from typing import Any, Callable, List, Optional, Tuple, Union
-
 import collections
+from typing import Any, Callable, Iterator, List, Optional, Tuple, Union
 
 import dns.exception
 import dns.name
 import dns.node
 import dns.rdataclass
 import dns.rdataset
 import dns.rdatatype
@@ -353,14 +352,35 @@
         The check function may safely make non-mutating transaction method
         calls, but behavior is undefined if mutating transaction methods are
         called.  The check function should raise an exception if it objects to
         the put, and otherwise should return ``None``.
         """
         self._check_delete_name.append(check)
 
+    def iterate_rdatasets(
+        self,
+    ) -> Iterator[Tuple[dns.name.Name, dns.rdataset.Rdataset]]:
+        """Iterate all the rdatasets in the transaction, returning
+        (`dns.name.Name`, `dns.rdataset.Rdataset`) tuples.
+
+        Note that as is usual with python iterators, adding or removing items
+        while iterating will invalidate the iterator and may raise `RuntimeError`
+        or fail to iterate over all entries."""
+        self._check_ended()
+        return self._iterate_rdatasets()
+
+    def iterate_names(self) -> Iterator[dns.name.Name]:
+        """Iterate all the names in the transaction.
+
+        Note that as is usual with python iterators, adding or removing names
+        while iterating will invalidate the iterator and may raise `RuntimeError`
+        or fail to iterate over all entries."""
+        self._check_ended()
+        return self._iterate_names()
+
     #
     # Helper methods
     #
 
     def _raise_if_not_empty(self, method, args):
         if len(args) != 0:
             raise TypeError(f"extra parameters to {method}")
@@ -412,15 +432,15 @@
                 rrset = arg
                 name = rrset.name
                 # rrsets are also rdatasets, but they don't print the
                 # same and can't be stored in nodes, so convert.
                 rdataset = rrset.to_rdataset()
             else:
                 raise TypeError(
-                    f"{method} requires a name or RRset " + "as the first argument"
+                    f"{method} requires a name or RRset as the first argument"
                 )
             if rdataset.rdclass != self.manager.get_class():
                 raise ValueError(f"{method} has objects of wrong RdataClass")
             if rdataset.rdtype == dns.rdatatype.SOA:
                 (_, _, origin) = self._origin_information()
                 if name != origin:
                     raise ValueError(f"{method} has non-origin SOA")
@@ -471,15 +491,15 @@
                 else:
                     rdataset = self._rdataset_from_args(method, True, args)
             elif isinstance(arg, dns.rrset.RRset):
                 rdataset = arg  # rrsets are also rdatasets
                 name = rdataset.name
             else:
                 raise TypeError(
-                    f"{method} requires a name or RRset " + "as the first argument"
+                    f"{method} requires a name or RRset as the first argument"
                 )
             self._raise_if_not_empty(method, args)
             if rdataset:
                 if rdataset.rdclass != self.manager.get_class():
                     raise ValueError(f"{method} has objects of wrong RdataClass")
                 existing = self._get_rdataset(name, rdataset.rdtype, rdataset.covers)
                 if existing is not None:
@@ -606,14 +626,18 @@
         """
         raise NotImplementedError  # pragma: no cover
 
     def _iterate_rdatasets(self):
         """Return an iterator that yields (name, rdataset) tuples."""
         raise NotImplementedError  # pragma: no cover
 
+    def _iterate_names(self):
+        """Return an iterator that yields a name."""
+        raise NotImplementedError  # pragma: no cover
+
     def _get_node(self, name):
         """Return the node at *name*, if any.
 
         Returns a node or ``None``.
         """
         raise NotImplementedError  # pragma: no cover
```

### Comparing `dnspython-2.3.0rc1/dns/tsig.py` & `dnspython-2.4.0rc1/dns/tsig.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 
 import base64
 import hashlib
 import hmac
 import struct
 
 import dns.exception
-import dns.rdataclass
 import dns.name
 import dns.rcode
+import dns.rdataclass
 
 
 class BadTime(dns.exception.DNSException):
 
     """The current time is not within the TSIG's validity time."""
 
 
@@ -183,17 +183,15 @@
         HMAC_MD5: hashlib.md5,
     }
 
     def __init__(self, key, algorithm):
         try:
             hashinfo = self._hashes[algorithm]
         except KeyError:
-            raise NotImplementedError(
-                f"TSIG algorithm {algorithm} " + "is not supported"
-            )
+            raise NotImplementedError(f"TSIG algorithm {algorithm} is not supported")
 
         # create the HMAC context
         if isinstance(hashinfo, tuple):
             self.hmac_context = hmac.new(key, digestmod=hashinfo[0])
             self.size = hashinfo[1]
         else:
             self.hmac_context = hmac.new(key, digestmod=hashinfo)
```

### Comparing `dnspython-2.3.0rc1/dns/tsigkeyring.py` & `dnspython-2.4.0rc1/dns/tsigkeyring.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,31 +13,30 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """A place to store TSIG keys."""
 
-from typing import Any, Dict
-
 import base64
+from typing import Any, Dict
 
 import dns.name
 import dns.tsig
 
 
 def from_text(textring: Dict[str, Any]) -> Dict[dns.name.Name, dns.tsig.Key]:
     """Convert a dictionary containing (textual DNS name, base64 secret)
     pairs into a binary keyring which has (dns.name.Name, bytes) pairs, or
     a dictionary containing (textual DNS name, (algorithm, base64 secret))
     pairs into a binary keyring which has (dns.name.Name, dns.tsig.Key) pairs.
     @rtype: dict"""
 
     keyring = {}
-    for (name, value) in textring.items():
+    for name, value in textring.items():
         kname = dns.name.from_text(name)
         if isinstance(value, str):
             keyring[kname] = dns.tsig.Key(kname, value).secret
         else:
             (algorithm, secret) = value
             keyring[kname] = dns.tsig.Key(kname, secret, algorithm)
     return keyring
@@ -51,15 +50,15 @@
     @rtype: dict"""
 
     textring = {}
 
     def b64encode(secret):
         return base64.encodebytes(secret).decode().rstrip()
 
-    for (name, key) in keyring.items():
+    for name, key in keyring.items():
         tname = name.to_text()
         if isinstance(key, bytes):
             textring[tname] = b64encode(key)
         else:
             if isinstance(key.secret, bytes):
                 text_secret = b64encode(key.secret)
             else:
```

### Comparing `dnspython-2.3.0rc1/dns/ttl.py` & `dnspython-2.4.0rc1/dns/ttl.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/dns/update.py` & `dnspython-2.4.0rc1/dns/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 from typing import Any, List, Optional, Union
 
 import dns.message
 import dns.name
 import dns.opcode
 import dns.rdata
 import dns.rdataclass
-import dns.rdatatype
 import dns.rdataset
+import dns.rdatatype
 import dns.tsig
 
 
 class UpdateSection(dns.enum.IntEnum):
     """Update sections"""
 
     ZONE = 0
@@ -39,15 +39,14 @@
 
     @classmethod
     def _maximum(cls):
         return 3
 
 
 class UpdateMessage(dns.message.Message):  # lgtm[py/missing-equals]
-
     # ignore the mypy error here as we mean to use a different enum
     _section_enum = UpdateSection  # type: ignore
 
     def __init__(
         self,
         zone: Optional[Union[dns.name.Name, str]] = None,
         rdclass: dns.rdataclass.RdataClass = dns.rdataclass.IN,
@@ -332,20 +331,20 @@
                 dns.rdatatype.ANY,
                 dns.rdatatype.NONE,
                 None,
                 True,
                 True,
             )
         else:
-            the_rdtype = dns.rdatatype.RdataType.make(rdtype)
+            rdtype = dns.rdatatype.RdataType.make(rdtype)
             self.find_rrset(
                 self.prerequisite,
                 name,
                 dns.rdataclass.NONE,
-                the_rdtype,
+                rdtype,
                 dns.rdatatype.NONE,
                 None,
                 True,
                 True,
             )
 
     def _get_one_rr_per_rrset(self, value):
```

### Comparing `dnspython-2.3.0rc1/dns/version.py` & `dnspython-2.4.0rc1/dns/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """dnspython release version information."""
 
 #: MAJOR
 MAJOR = 2
 #: MINOR
-MINOR = 3
+MINOR = 4
 #: MICRO
 MICRO = 0
 #: RELEASELEVEL
 RELEASELEVEL = 0x0C
 #: SERIAL
 SERIAL = 1
```

### Comparing `dnspython-2.3.0rc1/dns/versioned.py` & `dnspython-2.4.0rc1/dns/versioned.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (C) Dnspython Contributors, see LICENSE for text of ISC license
 
 """DNS Versioned Zones."""
 
-from typing import Callable, Deque, Optional, Set, Union
-
 import collections
 import threading
+from typing import Callable, Deque, Optional, Set, Union
 
 import dns.exception
 import dns.immutable
 import dns.name
 import dns.node
 import dns.rdataclass
 import dns.rdataset
@@ -28,15 +27,14 @@
 Version = dns.zone.Version
 WritableVersion = dns.zone.WritableVersion
 ImmutableVersion = dns.zone.ImmutableVersion
 Transaction = dns.zone.Transaction
 
 
 class Zone(dns.zone.Zone):  # lgtm[py/missing-equals]
-
     __slots__ = [
         "_versions",
         "_versions_lock",
         "_write_txn",
         "_write_waiters",
         "_write_event",
         "_pruning_policy",
@@ -148,15 +146,15 @@
             # We only wake one sleeper at a time, so it's important
             # that no event waiter can exit this method (e.g. via
             # cancellation) without returning a transaction or waking
             # someone else up.
             #
             # This is not a problem with Threading module threads as
             # they cannot be canceled, but could be an issue with trio
-            # or curio tasks when we do the async version of writer().
+            # tasks when we do the async version of writer().
             # I.e. we'd need to do something like:
             #
             # try:
             #     event.wait()
             # except trio.Cancelled:
             #     with self._version_lock:
             #         self._maybe_wakeup_one_waiter_unlocked()
```

### Comparing `dnspython-2.3.0rc1/dns/win32util.py` & `dnspython-2.4.0rc1/dns/win32util.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import sys
 
 if sys.platform == "win32":
-
     from typing import Any
 
     import dns.name
 
     _prefer_wmi = True
 
     import winreg  # pylint: disable=import-error
@@ -14,14 +13,15 @@
     try:
         WindowsError is None  # pylint: disable=used-before-assignment
     except KeyError:
         WindowsError = Exception
 
     try:
         import threading
+
         import pythoncom  # pylint: disable=import-error
         import wmi  # pylint: disable=import-error
 
         _have_wmi = True
     except Exception:
         _have_wmi = False
```

### Comparing `dnspython-2.3.0rc1/dns/wire.py` & `dnspython-2.4.0rc1/dns/wire.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Copyright (C) Dnspython Contributors, see LICENSE for text of ISC license
 
-from typing import Iterator, Optional, Tuple
-
 import contextlib
 import struct
+from typing import Iterator, Optional, Tuple
 
 import dns.exception
 import dns.name
 
 
 class Parser:
     def __init__(self, wire: bytes, current: int = 0):
```

### Comparing `dnspython-2.3.0rc1/dns/xfr.py` & `dnspython-2.4.0rc1/dns/xfr.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 
 from typing import Any, List, Optional, Tuple, Union
 
 import dns.exception
 import dns.message
 import dns.name
 import dns.rcode
-import dns.serial
 import dns.rdataset
 import dns.rdatatype
+import dns.serial
 import dns.transaction
 import dns.tsig
 import dns.zone
 
 
 class TransferError(dns.exception.DNSException):
     """A zone transfer response got a non-zero rcode."""
```

### Comparing `dnspython-2.3.0rc1/dns/zone.py` & `dnspython-2.4.0rc1/dns/zone.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,38 +13,37 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """DNS Zones."""
 
-from typing import Any, Dict, Iterator, Iterable, List, Optional, Set, Tuple, Union
-
 import contextlib
 import io
 import os
 import struct
+from typing import Any, Dict, Iterable, Iterator, List, Optional, Set, Tuple, Union
 
 import dns.exception
+import dns.grange
 import dns.immutable
 import dns.name
 import dns.node
-import dns.rdataclass
-import dns.rdatatype
 import dns.rdata
+import dns.rdataclass
 import dns.rdataset
+import dns.rdatatype
 import dns.rdtypes.ANY.SOA
 import dns.rdtypes.ANY.ZONEMD
 import dns.rrset
 import dns.tokenizer
 import dns.transaction
 import dns.ttl
-import dns.grange
 import dns.zonefile
-from dns.zonetypes import DigestScheme, DigestHashAlgorithm, _digest_hashers
+from dns.zonetypes import DigestHashAlgorithm, DigestScheme, _digest_hashers
 
 
 class BadZone(dns.exception.DNSException):
 
     """The DNS zone is malformed."""
 
 
@@ -317,19 +316,19 @@
 
         Raises ``KeyError`` if the name is not known and create was
         not specified, or if the name was not a subdomain of the origin.
 
         Returns a ``dns.rdataset.Rdataset``.
         """
 
-        the_name = self._validate_name(name)
-        the_rdtype = dns.rdatatype.RdataType.make(rdtype)
-        the_covers = dns.rdatatype.RdataType.make(covers)
-        node = self.find_node(the_name, create)
-        return node.find_rdataset(self.rdclass, the_rdtype, the_covers, create)
+        name = self._validate_name(name)
+        rdtype = dns.rdatatype.RdataType.make(rdtype)
+        covers = dns.rdatatype.RdataType.make(covers)
+        node = self.find_node(name, create)
+        return node.find_rdataset(self.rdclass, rdtype, covers, create)
 
     def get_rdataset(
         self,
         name: Union[dns.name.Name, str],
         rdtype: Union[dns.rdatatype.RdataType, str],
         covers: Union[dns.rdatatype.RdataType, str] = dns.rdatatype.NONE,
         create: bool = False,
@@ -400,22 +399,22 @@
         ``dns.rdatatype.SIG`` or ``dns.rdatatype.RRSIG``, then the covers value will be
         the rdata type the SIG/RRSIG covers.  The library treats the SIG and RRSIG types
         as if they were a family of types, e.g. RRSIG(A), RRSIG(NS), RRSIG(SOA). This
         makes RRSIGs much easier to work with than if RRSIGs covering different rdata
         types were aggregated into a single RRSIG rdataset.
         """
 
-        the_name = self._validate_name(name)
-        the_rdtype = dns.rdatatype.RdataType.make(rdtype)
-        the_covers = dns.rdatatype.RdataType.make(covers)
-        node = self.get_node(the_name)
+        name = self._validate_name(name)
+        rdtype = dns.rdatatype.RdataType.make(rdtype)
+        covers = dns.rdatatype.RdataType.make(covers)
+        node = self.get_node(name)
         if node is not None:
-            node.delete_rdataset(self.rdclass, the_rdtype, the_covers)
+            node.delete_rdataset(self.rdclass, rdtype, covers)
             if len(node) == 0:
-                self.delete_node(the_name)
+                self.delete_node(name)
 
     def replace_rdataset(
         self, name: Union[dns.name.Name, str], replacement: dns.rdataset.Rdataset
     ) -> None:
         """Replace an rdataset at name.
 
         It is not an error if there is no rdataset matching I{replacement}.
@@ -480,18 +479,18 @@
         Raises ``KeyError`` if the name is not known and create was
         not specified, or if the name was not a subdomain of the origin.
 
         Returns a ``dns.rrset.RRset`` or ``None``.
         """
 
         vname = self._validate_name(name)
-        the_rdtype = dns.rdatatype.RdataType.make(rdtype)
-        the_covers = dns.rdatatype.RdataType.make(covers)
-        rdataset = self.nodes[vname].find_rdataset(self.rdclass, the_rdtype, the_covers)
-        rrset = dns.rrset.RRset(vname, self.rdclass, the_rdtype, the_covers)
+        rdtype = dns.rdatatype.RdataType.make(rdtype)
+        covers = dns.rdatatype.RdataType.make(covers)
+        rdataset = self.nodes[vname].find_rdataset(self.rdclass, rdtype, covers)
+        rrset = dns.rrset.RRset(vname, self.rdclass, rdtype, covers)
         rrset.update(rdataset)
         return rrset
 
     def get_rrset(
         self,
         name: Union[dns.name.Name, str],
         rdtype: Union[dns.rdatatype.RdataType, str],
@@ -561,15 +560,15 @@
         This makes RRSIGs much easier to work with than if RRSIGs
         covering different rdata types were aggregated into a single
         RRSIG rdataset.
         """
 
         rdtype = dns.rdatatype.RdataType.make(rdtype)
         covers = dns.rdatatype.RdataType.make(covers)
-        for (name, node) in self.items():
+        for name, node in self.items():
             for rds in node:
                 if rdtype == dns.rdatatype.ANY or (
                     rds.rdtype == rdtype and rds.covers == covers
                 ):
                     yield (name, rds)
 
     def iterate_rdatas(
@@ -593,15 +592,15 @@
         This makes RRSIGs much easier to work with than if RRSIGs
         covering different rdata types were aggregated into a single
         RRSIG rdataset.
         """
 
         rdtype = dns.rdatatype.RdataType.make(rdtype)
         covers = dns.rdatatype.RdataType.make(covers)
-        for (name, node) in self.items():
+        for name, node in self.items():
             for rds in node:
                 if rdtype == dns.rdatatype.ANY or (
                     rds.rdtype == rdtype and rds.covers == covers
                 ):
                     for rdata in rds:
                         yield (name, rds.ttl, rdata)
 
@@ -791,15 +790,15 @@
 
         if self.relativize:
             origin_name = dns.name.empty
         else:
             assert self.origin is not None
             origin_name = self.origin
         hasher = hashinfo()
-        for (name, node) in sorted(self.items()):
+        for name, node in sorted(self.items()):
             rrnamebuf = name.to_digestable(self.origin)
             for rdataset in sorted(node, key=lambda rds: (rds.rdtype, rds.covers)):
                 if name == origin_name and dns.rdatatype.ZONEMD in (
                     rdataset.rdtype,
                     rdataset.covers,
                 ):
                     continue
@@ -993,14 +992,17 @@
         covers: dns.rdatatype.RdataType,
     ) -> Optional[dns.rdataset.Rdataset]:
         node = self.get_node(name)
         if node is None:
             return None
         return node.get_rdataset(self.zone.rdclass, rdtype, covers)
 
+    def keys(self):
+        return self.nodes.keys()
+
     def items(self):
         return self.nodes.items()
 
 
 class WritableVersion(Version):
     def __init__(self, zone: Zone, replacement: bool = False):
         # The zone._versions_lock must be held by our caller in a versioned
@@ -1139,18 +1141,21 @@
             self.zone._end_write(self)
 
     def _set_origin(self, origin):
         if self.version.origin is None:
             self.version.origin = origin
 
     def _iterate_rdatasets(self):
-        for (name, node) in self.version.items():
+        for name, node in self.version.items():
             for rdataset in node:
                 yield (name, rdataset)
 
+    def _iterate_names(self):
+        return self.version.keys()
+
     def _get_node(self, name):
         return self.version.get_node(name)
 
     def _origin_information(self):
         (absolute, relativize, effective) = self.manager.origin_information()
         if absolute is None and self.version.origin is not None:
             # No origin has been committed yet, but we've learned one as part of
```

### Comparing `dnspython-2.3.0rc1/dns/zonefile.py` & `dnspython-2.4.0rc1/dns/zonefile.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,31 +13,30 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 """DNS Zones."""
 
-from typing import Any, Iterable, List, Optional, Set, Tuple, Union
-
 import re
 import sys
+from typing import Any, Iterable, List, Optional, Set, Tuple, Union
 
 import dns.exception
+import dns.grange
 import dns.name
 import dns.node
+import dns.rdata
 import dns.rdataclass
 import dns.rdatatype
-import dns.rdata
 import dns.rdtypes.ANY.SOA
 import dns.rrset
 import dns.tokenizer
 import dns.transaction
 import dns.ttl
-import dns.grange
 
 
 class UnknownOrigin(dns.exception.DNSException):
     """Unknown origin"""
 
 
 class CNAMEAndOtherData(dns.exception.DNSException):
@@ -187,18 +186,14 @@
             ttl = None
             try:
                 ttl = dns.ttl.from_text(token.value)
                 self.last_ttl = ttl
                 self.last_ttl_known = True
                 token = None
             except dns.ttl.BadTTL:
-                if self.default_ttl_known:
-                    ttl = self.default_ttl
-                elif self.last_ttl_known:
-                    ttl = self.last_ttl
                 self.tok.unget(token)
 
         # Class
         if self.force_rdclass is not None:
             rdclass = self.force_rdclass
         else:
             token = self._get_identifier()
@@ -208,14 +203,30 @@
                 raise
             except Exception:
                 rdclass = self.zone_rdclass
                 self.tok.unget(token)
             if rdclass != self.zone_rdclass:
                 raise dns.exception.SyntaxError("RR class is not zone's class")
 
+        if ttl is None:
+            # support for <class> <ttl> <type> syntax
+            token = self._get_identifier()
+            ttl = None
+            try:
+                ttl = dns.ttl.from_text(token.value)
+                self.last_ttl = ttl
+                self.last_ttl_known = True
+                token = None
+            except dns.ttl.BadTTL:
+                if self.default_ttl_known:
+                    ttl = self.default_ttl
+                elif self.last_ttl_known:
+                    ttl = self.last_ttl
+                self.tok.unget(token)
+
         # Type
         if self.force_rdtype is not None:
             rdtype = self.force_rdtype
         else:
             token = self._get_identifier()
             try:
                 rdtype = dns.rdatatype.from_text(token.value)
@@ -577,15 +588,15 @@
     def _delete_rdataset(self, name, rdtype, covers):
         try:
             del self.rdatasets[(name, rdtype, covers)]
         except KeyError:
             pass
 
     def _name_exists(self, name):
-        for (n, _, _) in self.rdatasets:
+        for n, _, _ in self.rdatasets:
             if n == name:
                 return True
         return False
 
     def _changed(self):
         return len(self.rdatasets) > 0
 
@@ -602,14 +613,17 @@
 
     def _set_origin(self, origin):
         pass
 
     def _iterate_rdatasets(self):
         raise NotImplementedError  # pragma: no cover
 
+    def _iterate_names(self):
+        raise NotImplementedError  # pragma: no cover
+
 
 class RRSetsReaderManager(dns.transaction.TransactionManager):
     def __init__(
         self, origin=dns.name.root, relativize=False, rdclass=dns.rdataclass.IN
     ):
         self.origin = origin
         self.relativize = relativize
@@ -703,31 +717,31 @@
     if isinstance(name, str):
         name = dns.name.from_text(name, origin, idna_codec)
     if isinstance(ttl, str):
         ttl = dns.ttl.from_text(ttl)
     if isinstance(default_ttl, str):
         default_ttl = dns.ttl.from_text(default_ttl)
     if rdclass is not None:
-        the_rdclass = dns.rdataclass.RdataClass.make(rdclass)
+        rdclass = dns.rdataclass.RdataClass.make(rdclass)
     else:
-        the_rdclass = None
-    the_default_rdclass = dns.rdataclass.RdataClass.make(default_rdclass)
+        rdclass = None
+    default_rdclass = dns.rdataclass.RdataClass.make(default_rdclass)
     if rdtype is not None:
-        the_rdtype = dns.rdatatype.RdataType.make(rdtype)
+        rdtype = dns.rdatatype.RdataType.make(rdtype)
     else:
-        the_rdtype = None
+        rdtype = None
     manager = RRSetsReaderManager(origin, relativize, default_rdclass)
     with manager.writer(True) as txn:
         tok = dns.tokenizer.Tokenizer(text, "<input>", idna_codec=idna_codec)
         reader = Reader(
             tok,
-            the_default_rdclass,
+            default_rdclass,
             txn,
             allow_directives=False,
             force_name=name,
             force_ttl=ttl,
-            force_rdclass=the_rdclass,
-            force_rdtype=the_rdtype,
+            force_rdclass=rdclass,
+            force_rdtype=rdtype,
             default_ttl=default_ttl,
         )
         reader.read()
     return manager.rrsets
```

### Comparing `dnspython-2.3.0rc1/dns/zonetypes.py` & `dnspython-2.4.0rc1/dns/zonetypes.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/examples/async_dns.py` & `dnspython-2.4.0rc1/examples/async_dns.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,11 +21,15 @@
     q = dns.message.make_query(host, "A")
     r = await dns.asyncquery.tls(q, "8.8.8.8")
     print(r)
     a = await dns.asyncresolver.resolve(host, "A")
     print(a.response)
     zn = await dns.asyncresolver.zone_for_name(host)
     print(zn)
+    answer = await dns.asyncresolver.resolve_at("8.8.8.8", "amazon.com", "NS")
+    print("The amazon.com nameservers are:")
+    for rr in answer:
+        print(rr.target)
 
 
 if __name__ == "__main__":
     trio.run(main)
```

### Comparing `dnspython-2.3.0rc1/examples/ddns.py` & `dnspython-2.4.0rc1/examples/ddns.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/examples/doh-json.py` & `dnspython-2.4.0rc1/examples/doh-json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 import copy
 import json
-import requests
+import httpx
 
 import dns.flags
 import dns.message
 import dns.resolver
 import dns.rdataclass
 import dns.rdatatype
 
@@ -88,15 +88,15 @@
     # we don't decode the ecs_client_subnet field
     return message
 
 
 a = dns.resolver.resolve("www.dnspython.org", "a")
 p = to_doh_simple(a.response)
 print(json.dumps(p, indent=4))
-response = requests.get(
+response = httpx.get(
     "https://dns.google/resolve?",
     verify=True,
     params={"name": "www.dnspython.org", "type": 1},
 )
 p = json.loads(response.text)
 m = from_doh_simple(p, True)
 print(m)
```

### Comparing `dnspython-2.3.0rc1/examples/doq.py` & `dnspython-2.4.0rc1/examples/doq.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/examples/edns.py` & `dnspython-2.4.0rc1/examples/edns.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 )
 
 # With an ECS option using dns.edns.ECSOption to form the option
 q_list.append(
     (l, dns.message.make_query(n, t, options=[dns.edns.ECSOption("192.168.0.0", 20)]))
 )
 
-for (addr, q) in q_list:
+for addr, q in q_list:
     r = dns.query.udp(q, addr)
     if not r.options:
         print("No EDNS options returned")
     else:
         for o in r.options:
             print(o.otype.value, o.data)
     print()
```

### Comparing `dnspython-2.3.0rc1/examples/edns_resolver.py` & `dnspython-2.4.0rc1/examples/edns_resolver.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,12 +49,12 @@
 
 external_ip = urllib.request.urlopen("https://ident.me").read().decode("utf8")
 
 o_list.append((l, dict(options=[dns.edns.ECSOption(external_ip, 24)])))
 
 aresolver = dns.resolver.Resolver()
 
-for (addr, edns_kwargs) in o_list:
+for addr, edns_kwargs in o_list:
     if edns_kwargs:
         aresolver.use_edns(**edns_kwargs)
     aresolver.nameservers = ["8.8.8.8"]
     print(list(aresolver.resolve(addr, "A")))
```

### Comparing `dnspython-2.3.0rc1/examples/query_specific.py` & `dnspython-2.4.0rc1/examples/query_specific.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,24 +21,39 @@
 print("The nameservers are:")
 ns_rrset = r.find_rrset(r.answer, qname, dns.rdataclass.IN, dns.rdatatype.NS)
 for rr in ns_rrset:
     print(rr.target)
 print("")
 print("")
 
-# A higher-level way
+# A higher-level way:
 
 import dns.resolver
 
-resolver = dns.resolver.Resolver(configure=False)
-resolver.nameservers = ["8.8.8.8"]
-answer = resolver.resolve("amazon.com", "NS")
+answer = dns.resolver.resolve_at("8.8.8.8", "amazon.com", "NS")
 print("The nameservers are:")
 for rr in answer:
     print(rr.target)
+print("")
+print("")
+
+# If you're going to make a bunch of queries to the server, make the resolver once
+# and then use it multiple times:
+
+res = dns.resolver.make_resolver_at("dns.google")
+answer = res.resolve("amazon.com", "NS")
+print("The amazon.com nameservers are:")
+for rr in answer:
+    print(rr.target)
+answer = res.resolve("google.com", "NS")
+print("The google.com nameservers are:")
+for rr in answer:
+    print(rr.target)
+print("")
+print("")
 
 # Sending a query with the all flags set to 0.  This is the easiest way
 # to make a query with the RD flag off.
 #
 # This sends a query with RD=0 for the root SOA RRset to the IP address
 # for l.root-servers.net.
```

### Comparing `dnspython-2.3.0rc1/examples/receive_notify.py` & `dnspython-2.4.0rc1/examples/receive_notify.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/examples/reverse.py` & `dnspython-2.4.0rc1/examples/reverse.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import sys
 from typing import Dict, List  # pylint: disable=unused-import
 
 reverse_map = {}  # type: Dict[str, List[str]]
 
 for filename in sys.argv[1:]:
     zone = dns.zone.from_file(filename, os.path.basename(filename), relativize=False)
-    for (name, ttl, rdata) in zone.iterate_rdatas("A"):
+    for name, ttl, rdata in zone.iterate_rdatas("A"):
         print(type(rdata))
         try:
             reverse_map[rdata.address].append(name.to_text())
         except KeyError:
             reverse_map[rdata.address] = [name.to_text()]
 
 for k in sorted(reverse_map.keys(), key=dns.ipv4.inet_aton):
```

### Comparing `dnspython-2.3.0rc1/examples/zonediff.py` & `dnspython-2.4.0rc1/examples/zonediff.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/pyproject.toml` & `dnspython-2.4.0rc1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dnspython"
-version = "2.3.0rc1"
+version = "2.4.0rc1"
 description = "DNS toolkit"
 authors = ["Bob Halley <halley@dnspython.org>"]
 license = "ISC"
 packages = [
     {include = "dns"}
 ]
 include = [
@@ -34,46 +34,48 @@
 repository = "https://github.com/rthalley/dnspython.git"
 documentation = "https://dnspython.readthedocs.io/en/stable/"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/rthalley/dnspython/issues"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 httpx = {version=">=0.21.1", optional=true, python=">=3.6.2"}
 h2 = {version=">=4.1.0", optional=true, python=">=3.6.2"}
-requests-toolbelt = {version=">=0.9.1,<0.11.0", optional=true}
-requests = {version="^2.23.0", optional=true}
 idna = {version=">=2.1,<4.0", optional=true}
-cryptography = {version=">=2.6,<39.0", optional=true}
+cryptography = {version=">=2.6,<42.0", optional=true}
 trio = {version=">=0.14,<0.23", optional=true}
-curio = {version="^1.2", optional=true}
 sniffio = {version="^1.1", optional=true}
 wmi = {version="^1.5.1", optional=true}
 aioquic = {version=">=0.9.20", optional=true}
 
 [tool.poetry.dev-dependencies]
 pytest = ">=5.4.1,<8"
 pytest-cov = "^4.0.0"
 flake8 = "^5.0.3"
 sphinx = "^4.0.0"
 coverage = "^7.0"
 twine = "^4.0.0"
-wheel = "^0.38.1"
+wheel = "^0.40.0"
 pylint = "^2.7.4"
-mypy = ">=0.940"
-black = "^22.1.0"
+mypy = ">=1.0.1"
+black = "^23.1.0"
 
 [tool.poetry.extras]
-doh = ['httpx', 'h2', 'requests', 'requests-toolbelt']
+doh = ['httpx', 'h2']
 idna = ['idna']
 dnssec = ['cryptography']
 trio = ['trio']
-curio = ['curio', 'sniffio']
 wmi = ['wmi']
 doq = ['aioquic']
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.setuptools_scm]
+
+[tool.ruff]
+ignore = ['E741', 'F401']
+
+[tool.isort]
+profile = "black"
```

### Comparing `dnspython-2.3.0rc1/setup.cfg` & `dnspython-2.4.0rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = dnspython
-version = 2.3.0rc1
+version = 2.4.0rc1
 author = Bob Halley
 author_email = halley@dnspython.org
 license = ISC
 license_file = LICENSE
 description = DNS toolkit
-url = http://www.dnspython.org
+url = https://www.dnspython.org
 project_urls =
     Bug Tracker = https://github.com/rthalley/dnspython/issues
     Documentation = https://dnspython.readthedocs.io/en/stable/
     Source Code = https://github.com/rthalley/dnspython
 long_description = dnspython is a DNS toolkit for Python. It supports almost all
     record types. It can be used for queries, zone transfers, and dynamic
     updates.  It supports TSIG authenticated messages and EDNS0.
@@ -27,35 +27,35 @@
     License :: OSI Approved :: ISC License (ISCL)
     Operating System :: POSIX
     Operating System :: Microsoft :: Windows
     Programming Language :: Python
     Topic :: Internet :: Name Service (DNS)
     Topic :: Software Development :: Libraries :: Python Modules
     Programming Language :: Python :: 3
-    Programming Language :: Python :: 3.7
     Programming Language :: Python :: 3.8
     Programming Language :: Python :: 3.9
     Programming Language :: Python :: 3.10
 provides = dns
 
 [options]
 packages =
     dns
+    dns.dnssecalgs
+    dns.quic
     dns.rdtypes
     dns.rdtypes.IN
     dns.rdtypes.ANY
     dns.rdtypes.CH
-python_requires = >=3.7
+python_requires = >=3.8
 test_suite = tests
 setup_requires = setuptools>=44; setuptools_scm[toml]>=3.4.3
 
 [options.extras_require]
-DOH = httpx>=0.21.1; h2>=4.1.0; requests; requests-toolbelt
+DOH = httpx>=0.21.1; h2>=4.1.0
 IDNA = idna>=2.1
 DNSSEC = cryptography>=2.6
 trio = trio>=0.14.0
-curio = curio>=1.2; sniffio>=1.1
 wmi = wmi>=1.5.1
 DOQ = aioquic>=0.9.20
 
 [options.package_data]
 dns = py.typed
```

### Comparing `dnspython-2.3.0rc1/tests/example` & `dnspython-2.4.0rc1/tests/example`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,15 @@
 rrsig01			RRSIG	NSEC 1 3 3600 20200101000000 20030101000000 2143 foo MxFcby9k/yvedMfQgKzhH5er0Mu/vILz45IkskceFGgi WCn/GxHhai6VAuHAoNUz4YoU1tVfSCSqQYn6//11U6Nl d80jEeC8aTrO+KKmCaY= 
 rrsig02			RRSIG	NSEC 1 3 3600 1577836800 1041379200 2143 foo MxFcby9k/yvedMfQgKzhH5er0Mu/vILz45IkskceFGgi WCn/GxHhai6VAuHAoNUz4YoU1tVfSCSqQYn6//11U6Nl d80jEeC8aTrO+KKmCaY=
 nsec01			NSEC	a.secure A MX RRSIG NSEC TYPE1234
 nsec02			NSEC	. ( NSAP-PTR NSEC )
 nsec03			NSEC	. ( NSEC TYPE65535 )
 nsec301			NSEC3 1 1 12 aabbccdd 2t7b4g4vsa5smi47k61mv5bv1a22bojr MX DNSKEY NS SOA NSEC3PARAM RRSIG
 nsec302			NSEC3 1 1 12 - 2t7b4g4vsa5smi47k61mv5bv1a22bojr MX DNSKEY NS SOA NSEC3PARAM RRSIG
+nsec303			NSEC3 1 1 1 abcd alkmaao A
 dnskey01		DNSKEY	512 255 1 AQMFD5raczCJHViKtLYhWGz8hMY9UGRuniJDBzC7w0aR yzWZriO6i2odGWWQVucZqKVsENW91IOW4vqudngPZsY3 GvQ/xVA8/7pyFj6b7Esga60zyGW6LFe9r8n6paHrlG5o jqf0BaqHT+8= 
 dnskey02		DNSKEY	257 3 RSAMD5 ( AQMFD5raczCJHViKtLYhWGz8hMY9UGRuniJDBzC7w0aR yzWZriO6i2odGWWQVucZqKVsENW91IOW4vqudngPZsY3 GvQ/xVA8/7pyFj6b7Esga60zyGW6LFe9r8n6paHrlG5o jqf0BaqHT+8= )
 sshfp1			SSHFP	1 1 aa549bfe898489c02d1715d97d79c57ba2fa76ab
 spf			SPF	"v=spf1 mx -all"
 ipseckey01		IPSECKEY 10 1 2 192.0.2.38 AQNRU3mG7TVTO2BkR47usntb102uFJtugbo6BSGvgqt4AQ==
 ipseckey02		IPSECKEY 10 0 2 . AQNRU3mG7TVTO2BkR47usntb102uFJtugbo6BSGvgqt4AQ==
 ipseckey03		IPSECKEY 10 3 2 mygateway.example.com. AQNRU3mG7TVTO2BkR47usntb102uFJtugbo6BSGvgqt4AQ==
```

### Comparing `dnspython-2.3.0rc1/tests/example1.good` & `dnspython-2.4.0rc1/tests/example4.good`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+$ORIGIN example.
 @ 300 IN SOA ns1 hostmaster 1 2 3 4 5
 @ 300 IN NS ns1
 @ 300 IN NS ns2
 @ 300 IN NSEC3PARAM 1 1 12 aabbccdd
 @ 300 IN NSEC3PARAM 1 1 12 -
 * 300 IN MX 10 mail
 a 300 IN TXT "foo foo foo"
@@ -107,14 +108,15 @@
 nsap01 3600 IN NSAP 0x47000580005a0000000001e133ffffff00016100
 nsap02 3600 IN NSAP 0x47000580005a0000000001e133ffffff00016100
 nsec01 3600 IN NSEC a.secure A MX RRSIG NSEC TYPE1234
 nsec02 3600 IN NSEC . NSAP-PTR NSEC
 nsec03 3600 IN NSEC . NSEC TYPE65535
 nsec301 3600 IN NSEC3 1 1 12 aabbccdd 2t7b4g4vsa5smi47k61mv5bv1a22bojr NS SOA MX RRSIG DNSKEY NSEC3PARAM
 nsec302 3600 IN NSEC3 1 1 12 - 2t7b4g4vsa5smi47k61mv5bv1a22bojr NS SOA MX RRSIG DNSKEY NSEC3PARAM
+nsec303 3600 IN NSEC3 1 1 1 abcd alkmaao A
 openpgpkey 3600 IN OPENPGPKEY mQENBEteQDsBCADYnatn9+5t43AdJlVk9dZC2RM0idPQcmrrKcjeAWDnISqoJzkvQ8ifX6mefquTBsDZC279uXShyTffYzQtvP2r9ewkK7zmSv52Ar563TSULAMwiLpe0gGQE0ex20mX5ggtYn6czdbEtcKpW0t+AfDqRk5YcpgqfZKXapKQ+A3CwWJKP9i3ldx2Jz//kuru4YqROLBYyB8D6V2jNUFOdaP6j5C5prh9dxfYFp2O/xFeAKLWlWuH9o96INUoIhgdEyj9PHPT3c821NMZu8tCvsZgUB+QPbHA/QYGa+aollcdGkJpVxXoHhbu6aMx/B+pXg55WM5pqOxmoVjyViHIUYfPABEBAAG0IUJvYiBIYWxsZXkgPGhhbGxleUBkbnNweXRob24ub3JnPokBPgQTAQIAKAUCS15AOwIbAwUJA8JnAAYLCQgHAwIGFQgCCQoLBBYCAwECHgECF4AACgkQ6o6Gb8yUnXaflQgAhlhIqZGncRw3LV3d24JmPD+UEcEGiVh2b/Ic/1TMec46Ts7ZqRXAcOATNteQmpzqexx+BRKDWU8ZgYx12J4GZmC06jABr2JDWxgvbMX9qjkUUgDGZZgAS/B2x5AmKgy2ZnCUlaKfePcKmtKTB9yNJ8v/WERlFdGaUveEUiFU8g75xp1Hj9Wp9sXCg9yeG1K2RwQ3RQd5tLudhyE67EQdFGgqQFynR53md7cmVhAGopKLwMkpCtToKUlxxlfnDfpKZhhXThmhA0PsUQUkJptfGwYwH3O2N3KzfUw3wXRvLa3hona3TlHk3kfg7Qyd7oP4AZGbJKp97YHnfqo1kp8rObkBDQRLXkA7AQgA0ePG7g5GgZ/1SdtGZlJJiE2X15vTUc3KGfmx/kI5NaUDu4fXb+XK+yFy9I/X+UJ46JSkyhj6QvUxpoI+A7WWk9ThfjbynoZxRD820KbqidqxBSgtFF36SRWzmX8DZfKKAskT9ZGU1odeSKDXLCJF7qAbZVRTuFRiDFGwtoVIICeE6Xd65JO6ufhad+ELhgFt95vRwTiFvVrBRjwF7ZgN/nOXfYncxZ/2mpFqfwsnB2eu0A2XZBm8IngsSmr/Wrz1RQ7+SNMqt77E7CKwBX7UIAZgyoJxIRxWirJoOt1rIm5VUqRR25ubXLuzx9PaHYiC5GiQIU45pWAd0IWcTI/MJQARAQABiQElBBgBAgAPBQJLXkA7AhsMBQkDwmcAAAoJEOqOhm/MlJ12HRsIAKrB9E++9X9W6VTXBfdkShCFv0ykZVn2eVs6tkqzoub9s4f+Z5ylWw+a5nkMDMdGVe6bn4A3oIAbf0Tjykq1AetZLVPsHl/QosTbSQluis/PEvJkTQXHaKHB3bFhwA90c/3HNhrLGugt9AmcfLf9LAynXDgNLV5eYdPYqfKE+27qjEBARf6PYh/8WQ8CPKS8DILFbwCZbRxUogyrZf/7AiHAGdJi8dmpR1WPQYef2hF3kqGX6NngLBPzZ6CQRaHBhD4pHU1S/IRSlx9/3Ytww32PYD9AyO732NmCUcq3bmvqcOWy4Cc1NkEwU0Vg0qzwVBNGb84v/ex2MouwtAYScwc=
 ptr01 3600 IN PTR @
 px01 3600 IN PX 65535 foo. bar.
 px02 3600 IN PX 65535 . .
 rp01 3600 IN RP mbox-dname txt-dname
 rp02 3600 IN RP . .
 rrsig01 3600 IN RRSIG NSEC 1 3 3600 20200101000000 20030101000000 2143 foo MxFcby9k/yvedMfQgKzhH5er0Mu/vILz 45IkskceFGgiWCn/GxHhai6VAuHAoNUz 4YoU1tVfSCSqQYn6//11U6Nld80jEeC8 aTrO+KKmCaY=
```

### Comparing `dnspython-2.3.0rc1/tests/example2.good` & `dnspython-2.4.0rc1/tests/example2.good`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 nsap01.example. 3600 IN NSAP 0x47000580005a0000000001e133ffffff00016100
 nsap02.example. 3600 IN NSAP 0x47000580005a0000000001e133ffffff00016100
 nsec01.example. 3600 IN NSEC a.secure.example. A MX RRSIG NSEC TYPE1234
 nsec02.example. 3600 IN NSEC . NSAP-PTR NSEC
 nsec03.example. 3600 IN NSEC . NSEC TYPE65535
 nsec301.example. 3600 IN NSEC3 1 1 12 aabbccdd 2t7b4g4vsa5smi47k61mv5bv1a22bojr NS SOA MX RRSIG DNSKEY NSEC3PARAM
 nsec302.example. 3600 IN NSEC3 1 1 12 - 2t7b4g4vsa5smi47k61mv5bv1a22bojr NS SOA MX RRSIG DNSKEY NSEC3PARAM
+nsec303.example. 3600 IN NSEC3 1 1 1 abcd alkmaao A
 openpgpkey.example. 3600 IN OPENPGPKEY mQENBEteQDsBCADYnatn9+5t43AdJlVk9dZC2RM0idPQcmrrKcjeAWDnISqoJzkvQ8ifX6mefquTBsDZC279uXShyTffYzQtvP2r9ewkK7zmSv52Ar563TSULAMwiLpe0gGQE0ex20mX5ggtYn6czdbEtcKpW0t+AfDqRk5YcpgqfZKXapKQ+A3CwWJKP9i3ldx2Jz//kuru4YqROLBYyB8D6V2jNUFOdaP6j5C5prh9dxfYFp2O/xFeAKLWlWuH9o96INUoIhgdEyj9PHPT3c821NMZu8tCvsZgUB+QPbHA/QYGa+aollcdGkJpVxXoHhbu6aMx/B+pXg55WM5pqOxmoVjyViHIUYfPABEBAAG0IUJvYiBIYWxsZXkgPGhhbGxleUBkbnNweXRob24ub3JnPokBPgQTAQIAKAUCS15AOwIbAwUJA8JnAAYLCQgHAwIGFQgCCQoLBBYCAwECHgECF4AACgkQ6o6Gb8yUnXaflQgAhlhIqZGncRw3LV3d24JmPD+UEcEGiVh2b/Ic/1TMec46Ts7ZqRXAcOATNteQmpzqexx+BRKDWU8ZgYx12J4GZmC06jABr2JDWxgvbMX9qjkUUgDGZZgAS/B2x5AmKgy2ZnCUlaKfePcKmtKTB9yNJ8v/WERlFdGaUveEUiFU8g75xp1Hj9Wp9sXCg9yeG1K2RwQ3RQd5tLudhyE67EQdFGgqQFynR53md7cmVhAGopKLwMkpCtToKUlxxlfnDfpKZhhXThmhA0PsUQUkJptfGwYwH3O2N3KzfUw3wXRvLa3hona3TlHk3kfg7Qyd7oP4AZGbJKp97YHnfqo1kp8rObkBDQRLXkA7AQgA0ePG7g5GgZ/1SdtGZlJJiE2X15vTUc3KGfmx/kI5NaUDu4fXb+XK+yFy9I/X+UJ46JSkyhj6QvUxpoI+A7WWk9ThfjbynoZxRD820KbqidqxBSgtFF36SRWzmX8DZfKKAskT9ZGU1odeSKDXLCJF7qAbZVRTuFRiDFGwtoVIICeE6Xd65JO6ufhad+ELhgFt95vRwTiFvVrBRjwF7ZgN/nOXfYncxZ/2mpFqfwsnB2eu0A2XZBm8IngsSmr/Wrz1RQ7+SNMqt77E7CKwBX7UIAZgyoJxIRxWirJoOt1rIm5VUqRR25ubXLuzx9PaHYiC5GiQIU45pWAd0IWcTI/MJQARAQABiQElBBgBAgAPBQJLXkA7AhsMBQkDwmcAAAoJEOqOhm/MlJ12HRsIAKrB9E++9X9W6VTXBfdkShCFv0ykZVn2eVs6tkqzoub9s4f+Z5ylWw+a5nkMDMdGVe6bn4A3oIAbf0Tjykq1AetZLVPsHl/QosTbSQluis/PEvJkTQXHaKHB3bFhwA90c/3HNhrLGugt9AmcfLf9LAynXDgNLV5eYdPYqfKE+27qjEBARf6PYh/8WQ8CPKS8DILFbwCZbRxUogyrZf/7AiHAGdJi8dmpR1WPQYef2hF3kqGX6NngLBPzZ6CQRaHBhD4pHU1S/IRSlx9/3Ytww32PYD9AyO732NmCUcq3bmvqcOWy4Cc1NkEwU0Vg0qzwVBNGb84v/ex2MouwtAYScwc=
 ptr01.example. 3600 IN PTR example.
 px01.example. 3600 IN PX 65535 foo. bar.
 px02.example. 3600 IN PX 65535 . .
 rp01.example. 3600 IN RP mbox-dname.example. txt-dname.example.
 rp02.example. 3600 IN RP . .
 rrsig01.example. 3600 IN RRSIG NSEC 1 3 3600 20200101000000 20030101000000 2143 foo.example. MxFcby9k/yvedMfQgKzhH5er0Mu/vILz 45IkskceFGgiWCn/GxHhai6VAuHAoNUz 4YoU1tVfSCSqQYn6//11U6Nld80jEeC8 aTrO+KKmCaY=
```

### Comparing `dnspython-2.3.0rc1/tests/example3.good` & `dnspython-2.4.0rc1/tests/example1.good`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 nsap01 3600 IN NSAP 0x47000580005a0000000001e133ffffff00016100
 nsap02 3600 IN NSAP 0x47000580005a0000000001e133ffffff00016100
 nsec01 3600 IN NSEC a.secure A MX RRSIG NSEC TYPE1234
 nsec02 3600 IN NSEC . NSAP-PTR NSEC
 nsec03 3600 IN NSEC . NSEC TYPE65535
 nsec301 3600 IN NSEC3 1 1 12 aabbccdd 2t7b4g4vsa5smi47k61mv5bv1a22bojr NS SOA MX RRSIG DNSKEY NSEC3PARAM
 nsec302 3600 IN NSEC3 1 1 12 - 2t7b4g4vsa5smi47k61mv5bv1a22bojr NS SOA MX RRSIG DNSKEY NSEC3PARAM
+nsec303 3600 IN NSEC3 1 1 1 abcd alkmaao A
 openpgpkey 3600 IN OPENPGPKEY mQENBEteQDsBCADYnatn9+5t43AdJlVk9dZC2RM0idPQcmrrKcjeAWDnISqoJzkvQ8ifX6mefquTBsDZC279uXShyTffYzQtvP2r9ewkK7zmSv52Ar563TSULAMwiLpe0gGQE0ex20mX5ggtYn6czdbEtcKpW0t+AfDqRk5YcpgqfZKXapKQ+A3CwWJKP9i3ldx2Jz//kuru4YqROLBYyB8D6V2jNUFOdaP6j5C5prh9dxfYFp2O/xFeAKLWlWuH9o96INUoIhgdEyj9PHPT3c821NMZu8tCvsZgUB+QPbHA/QYGa+aollcdGkJpVxXoHhbu6aMx/B+pXg55WM5pqOxmoVjyViHIUYfPABEBAAG0IUJvYiBIYWxsZXkgPGhhbGxleUBkbnNweXRob24ub3JnPokBPgQTAQIAKAUCS15AOwIbAwUJA8JnAAYLCQgHAwIGFQgCCQoLBBYCAwECHgECF4AACgkQ6o6Gb8yUnXaflQgAhlhIqZGncRw3LV3d24JmPD+UEcEGiVh2b/Ic/1TMec46Ts7ZqRXAcOATNteQmpzqexx+BRKDWU8ZgYx12J4GZmC06jABr2JDWxgvbMX9qjkUUgDGZZgAS/B2x5AmKgy2ZnCUlaKfePcKmtKTB9yNJ8v/WERlFdGaUveEUiFU8g75xp1Hj9Wp9sXCg9yeG1K2RwQ3RQd5tLudhyE67EQdFGgqQFynR53md7cmVhAGopKLwMkpCtToKUlxxlfnDfpKZhhXThmhA0PsUQUkJptfGwYwH3O2N3KzfUw3wXRvLa3hona3TlHk3kfg7Qyd7oP4AZGbJKp97YHnfqo1kp8rObkBDQRLXkA7AQgA0ePG7g5GgZ/1SdtGZlJJiE2X15vTUc3KGfmx/kI5NaUDu4fXb+XK+yFy9I/X+UJ46JSkyhj6QvUxpoI+A7WWk9ThfjbynoZxRD820KbqidqxBSgtFF36SRWzmX8DZfKKAskT9ZGU1odeSKDXLCJF7qAbZVRTuFRiDFGwtoVIICeE6Xd65JO6ufhad+ELhgFt95vRwTiFvVrBRjwF7ZgN/nOXfYncxZ/2mpFqfwsnB2eu0A2XZBm8IngsSmr/Wrz1RQ7+SNMqt77E7CKwBX7UIAZgyoJxIRxWirJoOt1rIm5VUqRR25ubXLuzx9PaHYiC5GiQIU45pWAd0IWcTI/MJQARAQABiQElBBgBAgAPBQJLXkA7AhsMBQkDwmcAAAoJEOqOhm/MlJ12HRsIAKrB9E++9X9W6VTXBfdkShCFv0ykZVn2eVs6tkqzoub9s4f+Z5ylWw+a5nkMDMdGVe6bn4A3oIAbf0Tjykq1AetZLVPsHl/QosTbSQluis/PEvJkTQXHaKHB3bFhwA90c/3HNhrLGugt9AmcfLf9LAynXDgNLV5eYdPYqfKE+27qjEBARf6PYh/8WQ8CPKS8DILFbwCZbRxUogyrZf/7AiHAGdJi8dmpR1WPQYef2hF3kqGX6NngLBPzZ6CQRaHBhD4pHU1S/IRSlx9/3Ytww32PYD9AyO732NmCUcq3bmvqcOWy4Cc1NkEwU0Vg0qzwVBNGb84v/ex2MouwtAYScwc=
 ptr01 3600 IN PTR @
 px01 3600 IN PX 65535 foo. bar.
 px02 3600 IN PX 65535 . .
 rp01 3600 IN RP mbox-dname txt-dname
 rp02 3600 IN RP . .
 rrsig01 3600 IN RRSIG NSEC 1 3 3600 20200101000000 20030101000000 2143 foo MxFcby9k/yvedMfQgKzhH5er0Mu/vILz 45IkskceFGgiWCn/GxHhai6VAuHAoNUz 4YoU1tVfSCSqQYn6//11U6Nld80jEeC8 aTrO+KKmCaY=
```

### Comparing `dnspython-2.3.0rc1/tests/example4.good` & `dnspython-2.4.0rc1/tests/example3.good`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-$ORIGIN example.
 @ 300 IN SOA ns1 hostmaster 1 2 3 4 5
 @ 300 IN NS ns1
 @ 300 IN NS ns2
 @ 300 IN NSEC3PARAM 1 1 12 aabbccdd
 @ 300 IN NSEC3PARAM 1 1 12 -
 * 300 IN MX 10 mail
 a 300 IN TXT "foo foo foo"
@@ -108,14 +107,15 @@
 nsap01 3600 IN NSAP 0x47000580005a0000000001e133ffffff00016100
 nsap02 3600 IN NSAP 0x47000580005a0000000001e133ffffff00016100
 nsec01 3600 IN NSEC a.secure A MX RRSIG NSEC TYPE1234
 nsec02 3600 IN NSEC . NSAP-PTR NSEC
 nsec03 3600 IN NSEC . NSEC TYPE65535
 nsec301 3600 IN NSEC3 1 1 12 aabbccdd 2t7b4g4vsa5smi47k61mv5bv1a22bojr NS SOA MX RRSIG DNSKEY NSEC3PARAM
 nsec302 3600 IN NSEC3 1 1 12 - 2t7b4g4vsa5smi47k61mv5bv1a22bojr NS SOA MX RRSIG DNSKEY NSEC3PARAM
+nsec303 3600 IN NSEC3 1 1 1 abcd alkmaao A
 openpgpkey 3600 IN OPENPGPKEY mQENBEteQDsBCADYnatn9+5t43AdJlVk9dZC2RM0idPQcmrrKcjeAWDnISqoJzkvQ8ifX6mefquTBsDZC279uXShyTffYzQtvP2r9ewkK7zmSv52Ar563TSULAMwiLpe0gGQE0ex20mX5ggtYn6czdbEtcKpW0t+AfDqRk5YcpgqfZKXapKQ+A3CwWJKP9i3ldx2Jz//kuru4YqROLBYyB8D6V2jNUFOdaP6j5C5prh9dxfYFp2O/xFeAKLWlWuH9o96INUoIhgdEyj9PHPT3c821NMZu8tCvsZgUB+QPbHA/QYGa+aollcdGkJpVxXoHhbu6aMx/B+pXg55WM5pqOxmoVjyViHIUYfPABEBAAG0IUJvYiBIYWxsZXkgPGhhbGxleUBkbnNweXRob24ub3JnPokBPgQTAQIAKAUCS15AOwIbAwUJA8JnAAYLCQgHAwIGFQgCCQoLBBYCAwECHgECF4AACgkQ6o6Gb8yUnXaflQgAhlhIqZGncRw3LV3d24JmPD+UEcEGiVh2b/Ic/1TMec46Ts7ZqRXAcOATNteQmpzqexx+BRKDWU8ZgYx12J4GZmC06jABr2JDWxgvbMX9qjkUUgDGZZgAS/B2x5AmKgy2ZnCUlaKfePcKmtKTB9yNJ8v/WERlFdGaUveEUiFU8g75xp1Hj9Wp9sXCg9yeG1K2RwQ3RQd5tLudhyE67EQdFGgqQFynR53md7cmVhAGopKLwMkpCtToKUlxxlfnDfpKZhhXThmhA0PsUQUkJptfGwYwH3O2N3KzfUw3wXRvLa3hona3TlHk3kfg7Qyd7oP4AZGbJKp97YHnfqo1kp8rObkBDQRLXkA7AQgA0ePG7g5GgZ/1SdtGZlJJiE2X15vTUc3KGfmx/kI5NaUDu4fXb+XK+yFy9I/X+UJ46JSkyhj6QvUxpoI+A7WWk9ThfjbynoZxRD820KbqidqxBSgtFF36SRWzmX8DZfKKAskT9ZGU1odeSKDXLCJF7qAbZVRTuFRiDFGwtoVIICeE6Xd65JO6ufhad+ELhgFt95vRwTiFvVrBRjwF7ZgN/nOXfYncxZ/2mpFqfwsnB2eu0A2XZBm8IngsSmr/Wrz1RQ7+SNMqt77E7CKwBX7UIAZgyoJxIRxWirJoOt1rIm5VUqRR25ubXLuzx9PaHYiC5GiQIU45pWAd0IWcTI/MJQARAQABiQElBBgBAgAPBQJLXkA7AhsMBQkDwmcAAAoJEOqOhm/MlJ12HRsIAKrB9E++9X9W6VTXBfdkShCFv0ykZVn2eVs6tkqzoub9s4f+Z5ylWw+a5nkMDMdGVe6bn4A3oIAbf0Tjykq1AetZLVPsHl/QosTbSQluis/PEvJkTQXHaKHB3bFhwA90c/3HNhrLGugt9AmcfLf9LAynXDgNLV5eYdPYqfKE+27qjEBARf6PYh/8WQ8CPKS8DILFbwCZbRxUogyrZf/7AiHAGdJi8dmpR1WPQYef2hF3kqGX6NngLBPzZ6CQRaHBhD4pHU1S/IRSlx9/3Ytww32PYD9AyO732NmCUcq3bmvqcOWy4Cc1NkEwU0Vg0qzwVBNGb84v/ex2MouwtAYScwc=
 ptr01 3600 IN PTR @
 px01 3600 IN PX 65535 foo. bar.
 px02 3600 IN PX 65535 . .
 rp01 3600 IN RP mbox-dname txt-dname
 rp02 3600 IN RP . .
 rrsig01 3600 IN RRSIG NSEC 1 3 3600 20200101000000 20030101000000 2143 foo MxFcby9k/yvedMfQgKzhH5er0Mu/vILz 45IkskceFGgiWCn/GxHhai6VAuHAoNUz 4YoU1tVfSCSqQYn6//11U6Nld80jEeC8 aTrO+KKmCaY=
```

### Comparing `dnspython-2.3.0rc1/tests/keys.py` & `dnspython-2.4.0rc1/tests/keys.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/nanonameserver.py` & `dnspython-2.4.0rc1/tests/nanonameserver.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/nanoquic.py` & `dnspython-2.4.0rc1/tests/nanoquic.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,18 +81,20 @@
     class Server(threading.Thread):
         def __init__(self):
             super().__init__()
             self.transport = None
             self.protocol = None
             self.left = None
             self.right = None
+            self.ready = threading.Event()
 
         def __enter__(self):
             self.left, self.right = socket.socketpair()
             self.start()
+            self.ready.wait(4)
 
         def __exit__(self, ex_ty, ex_va, ex_tr):
             if self.protocol is not None:
                 self.protocol.close()
             if self.transport is not None:
                 self.transport.close()
             if self.left:
@@ -112,14 +114,15 @@
             loop = asyncio.get_event_loop()
             (self.transport, self.protocol) = await loop.create_datagram_endpoint(
                 lambda: aioquic.asyncio.server.QuicServer(
                     configuration=conf, create_protocol=NanoQuic
                 ),
                 local_addr=("127.0.0.1", 8853),
             )
+            self.ready.set()
             try:
                 await reader.read(1)
             except Exception:
                 pass
 
         def run(self):
             asyncio.run(self.arun())
```

### Comparing `dnspython-2.3.0rc1/tests/svcb_test_vectors.generic` & `dnspython-2.4.0rc1/tests/svcb_test_vectors.generic`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/svcb_test_vectors.text` & `dnspython-2.4.0rc1/tests/svcb_test_vectors.text`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_address.py` & `dnspython-2.4.0rc1/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_async.py` & `dnspython-2.4.0rc1/tests/test_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,17 +50,26 @@
     _resolver = dns.resolver.Resolver()
     if _resolver.nameservers == ["127.0.0.53"]:
         _systemd_resolved_present = True
 except Exception:
     pass
 
 query_addresses = []
+family = socket.AF_UNSPEC
 if tests.util.have_ipv4():
     query_addresses.append("8.8.8.8")
+    family = socket.AF_INET
 if tests.util.have_ipv6():
+    have_v6 = True
+    if family == socket.AF_INET:
+        # we have both working, go back to UNSPEC
+        family = socket.AF_UNSPEC
+    else:
+        # v6 only
+        family = socket.AF_INET6
     query_addresses.append("2001:4860:4860::8888")
 
 KNOWN_ANYCAST_DOH_RESOLVER_URLS = [
     "https://cloudflare-dns.com/dns-query",
     "https://dns.google/dns-query",
     # 'https://dns11.quad9.net/dns-query',
 ]
@@ -183,14 +192,58 @@
         async def run():
             return await dns.asyncresolver.resolve_address("8.8.8.8")
 
         answer = self.async_run(run)
         dnsgoogle = dns.name.from_text("dns.google.")
         self.assertEqual(answer[0].target, dnsgoogle)
 
+    def testResolveName(self):
+        async def run1():
+            return await dns.asyncresolver.resolve_name("dns.google.")
+
+        answers = self.async_run(run1)
+        seen = set(answers.addresses())
+        self.assertEqual(len(seen), 4)
+        self.assertIn("8.8.8.8", seen)
+        self.assertIn("8.8.4.4", seen)
+        self.assertIn("2001:4860:4860::8844", seen)
+        self.assertIn("2001:4860:4860::8888", seen)
+
+        async def run2():
+            return await dns.asyncresolver.resolve_name("dns.google.", socket.AF_INET)
+
+        answers = self.async_run(run2)
+        seen = set(answers.addresses())
+        self.assertEqual(len(seen), 2)
+        self.assertIn("8.8.8.8", seen)
+        self.assertIn("8.8.4.4", seen)
+
+        async def run3():
+            return await dns.asyncresolver.resolve_name("dns.google.", socket.AF_INET6)
+
+        answers = self.async_run(run3)
+        seen = set(answers.addresses())
+        self.assertEqual(len(seen), 2)
+        self.assertIn("2001:4860:4860::8844", seen)
+        self.assertIn("2001:4860:4860::8888", seen)
+
+        async def run4():
+            await dns.asyncresolver.resolve_name("nxdomain.dnspython.org")
+
+        with self.assertRaises(dns.resolver.NXDOMAIN):
+            self.async_run(run4)
+
+        async def run5():
+            await dns.asyncresolver.resolve_name(
+                dns.reversename.from_address("8.8.8.8")
+            )
+
+        with self.assertRaises(dns.resolver.NoAnswer):
+            self.async_run(run5)
+
     def testCanonicalNameNoCNAME(self):
         cname = dns.name.from_text("www.google.com")
 
         async def run():
             return await dns.asyncresolver.canonical_name("www.google.com")
 
         self.assertEqual(self.async_run(run), cname)
@@ -452,71 +505,87 @@
         def run():
             self.async_run(arun)
 
         self.assertRaises(dns.exception.Timeout, run)
 
     @unittest.skipIf(not dns.query._have_httpx, "httpx not available")
     def testDOHGetRequest(self):
-        if self.backend.name() == "curio":
-            self.skipTest("anyio dropped curio support")
-
         async def run():
             nameserver_url = random.choice(KNOWN_ANYCAST_DOH_RESOLVER_URLS)
             q = dns.message.make_query("example.com.", dns.rdatatype.A)
-            r = await dns.asyncquery.https(q, nameserver_url, post=False, timeout=4)
+            r = await dns.asyncquery.https(
+                q, nameserver_url, post=False, timeout=4, family=family
+            )
             self.assertTrue(q.is_response(r))
 
         self.async_run(run)
 
     @unittest.skipIf(not dns.query._have_httpx, "httpx not available")
     def testDOHGetRequestHttp1(self):
-        if self.backend.name() == "curio":
-            self.skipTest("anyio dropped curio support")
-
         async def run():
             saved_have_http2 = dns.query._have_http2
             try:
                 dns.query._have_http2 = False
                 nameserver_url = random.choice(KNOWN_ANYCAST_DOH_RESOLVER_URLS)
                 q = dns.message.make_query("example.com.", dns.rdatatype.A)
-                r = await dns.asyncquery.https(q, nameserver_url, post=False, timeout=4)
+                r = await dns.asyncquery.https(
+                    q, nameserver_url, post=False, timeout=4, family=family
+                )
                 self.assertTrue(q.is_response(r))
             finally:
                 dns.query._have_http2 = saved_have_http2
 
         self.async_run(run)
 
     @unittest.skipIf(not dns.query._have_httpx, "httpx not available")
     def testDOHPostRequest(self):
-        if self.backend.name() == "curio":
-            self.skipTest("anyio dropped curio support")
-
         async def run():
             nameserver_url = random.choice(KNOWN_ANYCAST_DOH_RESOLVER_URLS)
             q = dns.message.make_query("example.com.", dns.rdatatype.A)
-            r = await dns.asyncquery.https(q, nameserver_url, post=True, timeout=4)
+            r = await dns.asyncquery.https(
+                q, nameserver_url, post=True, timeout=4, family=family
+            )
             self.assertTrue(q.is_response(r))
 
         self.async_run(run)
 
     @unittest.skipIf(not dns.query._have_httpx, "httpx not available")
     def testResolverDOH(self):
-        if self.backend.name() == "curio":
-            self.skipTest("anyio dropped curio support")
-
         async def run():
             res = dns.asyncresolver.Resolver(configure=False)
             res.nameservers = ["https://dns.google/dns-query"]
             answer = await res.resolve("dns.google", "A", backend=self.backend)
             seen = set([rdata.address for rdata in answer])
             self.assertTrue("8.8.8.8" in seen)
             self.assertTrue("8.8.4.4" in seen)
 
         self.async_run(run)
 
+    @unittest.skipIf(not tests.util.have_ipv4(), "IPv4 not reachable")
+    def testResolveAtAddress(self):
+        async def run():
+            answer = await dns.asyncresolver.resolve_at("8.8.8.8", "dns.google.", "A")
+            seen = set([rdata.address for rdata in answer])
+            self.assertIn("8.8.8.8", seen)
+            self.assertIn("8.8.4.4", seen)
+
+        self.async_run(run)
+
+    @unittest.skipIf(not tests.util.have_ipv4(), "IPv4 not reachable")
+    def testResolveAtName(self):
+        async def run():
+            answer = await dns.asyncresolver.resolve_at(
+                "dns.google", "dns.google.", "A", family=socket.AF_INET
+            )
+            seen = set([rdata.address for rdata in answer])
+            self.assertIn("8.8.8.8", seen)
+            self.assertIn("8.8.4.4", seen)
+
+        self.async_run(run)
+
     def testSleep(self):
         async def run():
             before = time.time()
             await self.backend.sleep(0.1)
             after = time.time()
             self.assertTrue(after - before >= 0.1)
 
@@ -532,14 +601,15 @@
 
     def async_run(self, afunc):
         return asyncio.run(afunc())
 
     def testUseAfterTimeout(self):
         if self.connect_udp:
             self.skipTest("test needs connectionless sockets")
+
         # Test #843 fix.
         async def run():
             qname = dns.name.from_text("dns.google")
             query = dns.message.make_query(qname, "A")
             sock = await self.backend.make_socket(socket.AF_INET, socket.SOCK_DGRAM)
             async with sock:
                 # First do something that will definitely timeout.
@@ -592,41 +662,7 @@
             self.backend = dns.asyncbackend.set_default_backend("trio")
 
         def async_run(self, afunc):
             return trio.run(afunc)
 
 except ImportError:
     pass
-
-try:
-    import curio
-    import sniffio
-
-    @unittest.skipIf(sys.platform == "win32", "curio does not work in windows CI")
-    class CurioAsyncDetectionTests(AsyncDetectionTests):
-        sniff_result = "curio"
-
-        def async_run(self, afunc):
-            with curio.Kernel() as kernel:
-                return kernel.run(afunc, shutdown=True)
-
-    @unittest.skipIf(sys.platform == "win32", "curio does not work in windows CI")
-    class CurioNoSniffioAsyncDetectionTests(NoSniffioAsyncDetectionTests):
-        expect_raise = True
-
-        def async_run(self, afunc):
-            with curio.Kernel() as kernel:
-                return kernel.run(afunc, shutdown=True)
-
-    @unittest.skipIf(sys.platform == "win32", "curio does not work in windows CI")
-    class CurioAsyncTests(AsyncTests):
-        connect_udp = False
-
-        def setUp(self):
-            self.backend = dns.asyncbackend.set_default_backend("curio")
-
-        def async_run(self, afunc):
-            with curio.Kernel() as kernel:
-                return kernel.run(afunc, shutdown=True)
-
-except ImportError:
-    pass
```

### Comparing `dnspython-2.3.0rc1/tests/test_bugs.py` & `dnspython-2.4.0rc1/tests/test_bugs.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_constants.py` & `dnspython-2.4.0rc1/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_dnssec.py` & `dnspython-2.4.0rc1/tests/test_dnssec.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,26 +14,30 @@
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 # OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 from datetime import datetime, timedelta, timezone
 from typing import Any
 
+import functools
 import unittest
 
 import dns.dnssec
 import dns.name
 import dns.rdata
 import dns.rdataclass
 import dns.rdatatype
 import dns.rdtypes.ANY.CDNSKEY
 import dns.rdtypes.ANY.CDS
 import dns.rdtypes.ANY.DNSKEY
 import dns.rdtypes.ANY.DS
 import dns.rrset
+import dns.zone
+
+from dns.rdtypes.dnskeybase import Flag
 
 from .keys import test_dnskeys
 
 try:
     from cryptography.hazmat.backends import default_backend
     from cryptography.hazmat.primitives.serialization import load_pem_private_key
     from cryptography.hazmat.primitives.asymmetric import dsa, ec, ed25519, ed448, rsa
@@ -576,14 +580,66 @@
     "NS 12 1 3600 20200825161255 20200726161255 16625 example."
     " P9A+1zYke7yIiKEnxFMm+UIW2CIwy2WDvbx6"
     " g8hHiI8qISe6oeKveFW23OSk9+VwFgBiOpeM"
     " ygzzFbckY7RkGbOr4TR8ogDRANt6LhV402Hu"
     " SXTV9hCLVFWU4PS+/fxxfOHCetsY5tWWSxZi zSHfgpGfsHWzQoAamag4XYDyykc=",
 )
 
+test_zone_sans_nsec = """
+example. 3600 IN SOA foo.example. bar.example. 1 2 3 4 5
+example. 3600 IN NS ns1.example.
+example. 3600 IN NS ns2.example.
+bar.foo.example. 3600 IN MX 0 blaz.foo.example.
+ns1.example. 3600 IN A 10.0.0.1
+ns2.example. 3600 IN A 10.0.0.2
+sub.example. 3600 IN NS ns1.example.
+sub.example. 3600 IN NS ns2.example.
+sub.example. 3600 IN NS ns3.sub.example.
+sub.example. 3600 IN DS 12345 13 2 0100D208742A23024DF3C8827DFF3EB3E25126E9B72850E99D6055E18913CB2F
+sub.sub.example. 3600 IN NS ns3.sub.example.
+ns3.sub.example. 3600 IN A 10.0.0.3
+"""
+
+test_zone_rrsigs = set(
+    [
+        ("example.", dns.rdatatype.DNSKEY),
+        ("example.", dns.rdatatype.NS),
+        ("example.", dns.rdatatype.NSEC),
+        ("example.", dns.rdatatype.SOA),
+        ("bar.foo.example.", dns.rdatatype.MX),
+        ("bar.foo.example.", dns.rdatatype.NSEC),
+        ("ns1.example.", dns.rdatatype.A),
+        ("ns1.example.", dns.rdatatype.NSEC),
+        ("ns2.example.", dns.rdatatype.A),
+        ("ns2.example.", dns.rdatatype.NSEC),
+        ("sub.example.", dns.rdatatype.DS),
+        ("sub.example.", dns.rdatatype.NSEC),
+    ]
+)
+
+test_zone_with_nsec = """
+example. 3600 IN SOA foo.example. bar.example. 1 2 3 4 5
+example. 3600 IN NS ns1.example.
+example. 3600 IN NS ns2.example.
+example. 5 IN NSEC bar.foo.example. NS NSEC SOA RRSIG
+bar.foo.example. 3600 IN MX 0 blaz.foo.example.
+bar.foo.example. 5 IN NSEC ns1.example. MX NSEC RRSIG
+ns1.example. 3600 IN A 10.0.0.1
+ns1.example. 5 IN NSEC ns2.example. A NSEC RRSIG
+ns2.example. 3600 IN A 10.0.0.2
+ns2.example. 5 IN NSEC sub.example. A NSEC RRSIG
+sub.example. 3600 IN NS ns1.example.
+sub.example. 3600 IN NS ns2.example.
+sub.example. 3600 IN NS ns3.sub.example.
+sub.example. 3600 IN DS 12345 13 2 0100D208742A23024DF3C8827DFF3EB3E25126E9B72850E99D6055E18913CB2F
+sub.example. 5 IN NSEC example. DS NS NSEC RRSIG
+sub.sub.example. 3600 IN NS ns3.sub.example.
+ns3.sub.example. 3600 IN A 10.0.0.3
+"""
+
 
 @unittest.skipUnless(dns.dnssec._have_pyca, "Python Cryptography cannot be imported")
 class DNSSECValidatorTestCase(unittest.TestCase):
     def testAbsoluteRSAMD5Good(self):  # type: () -> None
         dns.dnssec.validate(
             rsamd5_ns,
             rsamd5_ns_rrsig,
@@ -764,29 +820,49 @@
         com_txt = clone_rrset(wildcard_txt, com_name)
         com_txt_rrsig = clone_rrset(wildcard_txt_rrsig, abc_name)
         with self.assertRaises(dns.dnssec.ValidationFailure):
             dns.dnssec.validate_rrsig(
                 com_txt, com_txt_rrsig[0], wildcard_keys, None, wildcard_when
             )
 
+        # check some bogus label lengths
+        a_name = dns.name.from_text("a.example.com")
+        a_txt = clone_rrset(wildcard_txt, a_name)
+        a_txt_rrsig = clone_rrset(wildcard_txt_rrsig, a_name)
+        bad_rrsig = a_txt_rrsig[0].replace(labels=99)
+        with self.assertRaises(dns.dnssec.ValidationFailure):
+            dns.dnssec.validate_rrsig(
+                a_txt, bad_rrsig, wildcard_keys, None, wildcard_when
+            )
+        bad_rrsig = a_txt_rrsig[0].replace(labels=3)
+        with self.assertRaises(dns.dnssec.ValidationFailure):
+            dns.dnssec.validate_rrsig(
+                a_txt, bad_rrsig, wildcard_keys, None, wildcard_when
+            )
+        bad_rrsig = a_txt_rrsig[0].replace(labels=1)
+        with self.assertRaises(dns.dnssec.ValidationFailure):
+            dns.dnssec.validate_rrsig(
+                a_txt, bad_rrsig, wildcard_keys, None, wildcard_when
+            )
+
     def testAlternateParameterFormats(self):  # type: () -> None
         # Pass rrset and rrsigset as (name, rdataset) tuples, not rrsets
         rrset = (abs_soa.name, abs_soa.to_rdataset())
         rrsigset = (abs_soa_rrsig.name, abs_soa_rrsig.to_rdataset())
         dns.dnssec.validate(rrset, rrsigset, abs_keys, None, when)
 
         # Pass keys as a name->node dict, not a name->rrset dict
         keys = {}
-        for (name, key_rrset) in abs_keys.items():
+        for name, key_rrset in abs_keys.items():
             keys[name] = dns.node.Node()
             keys[name].rdatasets.append(key_rrset.to_rdataset())
         dns.dnssec.validate(abs_soa, abs_soa_rrsig, keys, None, when)
         # test key not found.
         keys = {}
-        for (name, key_rrset) in abs_keys.items():
+        for name, key_rrset in abs_keys.items():
             keys[name] = dns.node.Node()
         with self.assertRaises(dns.dnssec.ValidationFailure):
             dns.dnssec.validate(abs_soa, abs_soa_rrsig, keys, None, when)
 
         # Pass origin as a string, not a name.
         dns.dnssec.validate(rel_soa, rel_soa_rrsig, rel_keys, "dnspython.org", when)
         dns.dnssec.validate_rrsig(
@@ -843,30 +919,24 @@
                 unknown_alg_ns_rrsig,
                 unknown_alg_keys,
                 None,
                 rsasha512_when,
             )
 
 
+@unittest.skipUnless(dns.dnssec._have_pyca, "Python Cryptography cannot be imported")
 class DNSSECMiscTestCase(unittest.TestCase):
     def testDigestToBig(self):
         with self.assertRaises(ValueError):
             dns.dnssec.DSDigest.make(256)
 
     def testNSEC3HashTooBig(self):
         with self.assertRaises(ValueError):
             dns.dnssec.NSEC3Hash.make(256)
 
-    def testIsNotGOST(self):
-        self.assertTrue(dns.dnssec._is_gost(dns.dnssec.Algorithm.ECCGOST))
-
-    def testUnknownHash(self):
-        with self.assertRaises(dns.dnssec.ValidationFailure):
-            dns.dnssec._make_hash(100)
-
     def testToTimestamp(self):
         REFERENCE_TIMESTAMP = 441812220
 
         ts = dns.dnssec.to_timestamp(
             datetime(year=1984, month=1, day=1, hour=13, minute=37, tzinfo=timezone.utc)
         )
         self.assertEqual(ts, REFERENCE_TIMESTAMP)
@@ -876,15 +946,98 @@
 
         ts = dns.dnssec.to_timestamp(441812220.0)
         self.assertEqual(ts, REFERENCE_TIMESTAMP)
 
         ts = dns.dnssec.to_timestamp(441812220)
         self.assertEqual(ts, REFERENCE_TIMESTAMP)
 
+    def do_test_sign_zone(self, relativize):
+        zone = dns.zone.from_text(
+            test_zone_sans_nsec, "example.", relativize=relativize
+        )
+
+        algorithm = dns.dnssec.Algorithm.ED25519
+        lifetime = 3600
+
+        ksk_private_key = ed25519.Ed25519PrivateKey.generate()
+        ksk_dnskey = dns.dnssec.make_dnskey(
+            public_key=ksk_private_key.public_key(),
+            algorithm=algorithm,
+            flags=Flag.ZONE | Flag.SEP,
+        )
+
+        zsk_private_key = ed25519.Ed25519PrivateKey.generate()
+        zsk_dnskey = dns.dnssec.make_dnskey(
+            public_key=zsk_private_key.public_key(),
+            algorithm=algorithm,
+            flags=Flag.ZONE,
+        )
+
+        keys = [(ksk_private_key, ksk_dnskey), (zsk_private_key, zsk_dnskey)]
+
+        with zone.writer() as txn:
+            dns.dnssec.sign_zone(
+                zone=zone,
+                txn=txn,
+                keys=keys,
+                lifetime=lifetime,
+            )
+
+        print(zone.to_text())
+        rrsigs = set(
+            [
+                (str(name.derelativize(zone.origin)), rdataset.covers)
+                for (name, rdataset) in zone.iterate_rdatasets()
+                if rdataset.rdtype == dns.rdatatype.RRSIG
+            ]
+        )
+        self.assertEqual(rrsigs, test_zone_rrsigs)
+
+        signers = set(
+            [
+                (
+                    str(name.derelativize(zone.origin)),
+                    rdataset.covers,
+                    rdataset[0].key_tag,
+                )
+                for (name, rdataset) in zone.iterate_rdatasets()
+                if rdataset.rdtype == dns.rdatatype.RRSIG
+            ]
+        )
+        for name, covers, key_tag in signers:
+            if covers in [
+                dns.rdatatype.DNSKEY,
+                dns.rdatatype.CDNSKEY,
+                dns.rdatatype.CDS,
+            ]:
+                self.assertEqual(key_tag, dns.dnssec.key_id(ksk_dnskey))
+            else:
+                self.assertEqual(key_tag, dns.dnssec.key_id(zsk_dnskey))
+
+    def test_sign_zone_absolute(self):
+        self.do_test_sign_zone(False)
+
+    def test_sign_zone_relative(self):
+        self.do_test_sign_zone(True)
+
+    def test_sign_zone_nsec_null_signer(self):
+        def rrset_signer(
+            txn: dns.transaction.Transaction,
+            rrset: dns.rrset.RRset,
+        ) -> None:
+            pass
+
+        zone1 = dns.zone.from_text(test_zone_sans_nsec, "example.", relativize=False)
+        dns.dnssec.sign_zone(zone1, rrset_signer=rrset_signer)
+
+        zone2 = dns.zone.from_text(test_zone_with_nsec, "example.", relativize=False)
+        self.assertEqual(zone1.to_text(), zone2.to_text())
 
+
+@unittest.skipUnless(dns.dnssec._have_pyca, "Python Cryptography cannot be imported")
 class DNSSECMakeDSTestCase(unittest.TestCase):
     def testMnemonicParser(self):
         good_ds_mnemonic = dns.rdata.from_text(
             dns.rdataclass.IN,
             dns.rdatatype.DS,
             "57349 RSASHA1 2 53A79A3E7488AB44FFC56B2D1109F0699D1796DD977E72108B841F96"
             " E47D7013",
@@ -1107,18 +1260,18 @@
 
     def testInvalidMakeDNSKEY(self):  # type: () -> None
         key = rsa.generate_private_key(
             public_exponent=65537,
             key_size=1024,
             backend=default_backend(),
         )
-        with self.assertRaises(dns.dnssec.AlgorithmKeyMismatch):
+        with self.assertRaises(dns.exception.AlgorithmKeyMismatch):
             dns.dnssec.make_dnskey(key.public_key(), dns.dnssec.Algorithm.ED448)
 
-        with self.assertRaises(TypeError):
+        with self.assertRaises(dns.exception.AlgorithmKeyMismatch):
             dns.dnssec.make_dnskey("xyzzy", dns.dnssec.Algorithm.ED448)
 
         key = dsa.generate_private_key(2048)
         with self.assertRaises(ValueError):
             dns.dnssec.make_dnskey(key.public_key(), dns.dnssec.Algorithm.DSA)
 
     def testMakeCDNSKEY(self):  # type: () -> None
@@ -1182,20 +1335,14 @@
 
     def testSignatureRSASHA256(self):  # type: () -> None
         key = rsa.generate_private_key(
             public_exponent=65537, key_size=2048, backend=default_backend()
         )
         self._test_signature(key, dns.dnssec.Algorithm.RSASHA256, abs_soa)
 
-    def testSignatureDSA(self):  # type: () -> None
-        key = dsa.generate_private_key(key_size=1024)
-        self._test_signature(
-            key, dns.dnssec.Algorithm.DSA, abs_soa, policy=dns.dnssec.allow_all_policy
-        )
-
     def testSignatureECDSAP256SHA256(self):  # type: () -> None
         key = ec.generate_private_key(curve=ec.SECP256R1, backend=default_backend())
         self._test_signature(key, dns.dnssec.Algorithm.ECDSAP256SHA256, abs_soa)
 
     def testSignatureECDSAP384SHA384(self):  # type: () -> None
         key = ec.generate_private_key(curve=ec.SECP384R1, backend=default_backend())
         self._test_signature(key, dns.dnssec.Algorithm.ECDSAP384SHA384, abs_soa)
@@ -1211,14 +1358,22 @@
     def testSignRdataset(self):  # type: () -> None
         key = ed448.Ed448PrivateKey.generate()
         name = dns.name.from_text("example.com")
         rdataset = dns.rdataset.from_text_list("in", "a", 30, ["10.0.0.1", "10.0.0.2"])
         rrset = (name, rdataset)
         self._test_signature(key, dns.dnssec.Algorithm.ED448, rrset)
 
+    def testSignWildRdataset(self):  # type: () -> None
+        key = ed448.Ed448PrivateKey.generate()
+        name = dns.name.from_text("*.example.com")
+        rdataset = dns.rdataset.from_text_list("in", "a", 30, ["10.0.0.1", "10.0.0.2"])
+        rrset = (name, rdataset)
+        rrsigset = self._test_signature(key, dns.dnssec.Algorithm.ED448, rrset)
+        self.assertEqual(rrsigset[0].labels, 2)
+
     def _test_signature(self, key, algorithm, rrset, signer=None, policy=None):
         ttl = 60
         lifetime = 3600
         if isinstance(rrset, tuple):
             rrname = rrset[0]
         else:
             rrname = rrset.name
@@ -1235,11 +1390,12 @@
             signer=signer,
             verify=True,
             policy=policy,
         )
         keys = {signer: dnskey_rrset}
         rrsigset = dns.rrset.from_rdata(rrname, ttl, rrsig)
         dns.dnssec.validate(rrset=rrset, rrsigset=rrsigset, keys=keys, policy=policy)
+        return rrsigset
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `dnspython-2.3.0rc1/tests/test_doh.py` & `dnspython-2.4.0rc1/tests/test_doh.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,167 +27,106 @@
 
 import dns.edns
 import dns.message
 import dns.query
 import dns.rdatatype
 import dns.resolver
 
-if dns.query._have_requests:
-    import requests
-    from requests.exceptions import SSLError
-
 if dns.query._have_httpx:
     import httpx
 
 import tests.util
 
 resolver_v4_addresses = []
 resolver_v6_addresses = []
+family = socket.AF_UNSPEC
 if tests.util.have_ipv4():
     resolver_v4_addresses = [
         "1.1.1.1",
         "8.8.8.8",
         # '9.9.9.9',
     ]
+    family = socket.AF_INET
 if tests.util.have_ipv6():
     resolver_v6_addresses = [
         "2606:4700:4700::1111",
         "2001:4860:4860::8888",
         # '2620:fe::fe',
     ]
+    if family == socket.AF_INET:
+        # we have both working, go back to UNSPEC
+        family = socket.AF_UNSPEC
+    else:
+        # v6 only
+        family = socket.AF_INET6
 
 KNOWN_ANYCAST_DOH_RESOLVER_URLS = [
     "https://cloudflare-dns.com/dns-query",
     "https://dns.google/dns-query",
     # 'https://dns11.quad9.net/dns-query',
 ]
 
 KNOWN_PAD_AWARE_DOH_RESOLVER_URLS = [
     "https://cloudflare-dns.com/dns-query",
     "https://dns.google/dns-query",
 ]
 
 
 @unittest.skipUnless(
-    dns.query._have_requests and tests.util.is_internet_reachable(),
-    "Python requests cannot be imported; no DNS over HTTPS (DOH)",
-)
-class DNSOverHTTPSTestCaseRequests(unittest.TestCase):
-    def setUp(self):
-        self.session = requests.sessions.Session()
-
-    def tearDown(self):
-        self.session.close()
-
-    def test_get_request(self):
-        nameserver_url = random.choice(KNOWN_ANYCAST_DOH_RESOLVER_URLS)
-        q = dns.message.make_query("example.com.", dns.rdatatype.A)
-        r = dns.query.https(
-            q, nameserver_url, session=self.session, post=False, timeout=4
-        )
-        self.assertTrue(q.is_response(r))
-
-    def test_post_request(self):
-        nameserver_url = random.choice(KNOWN_ANYCAST_DOH_RESOLVER_URLS)
-        q = dns.message.make_query("example.com.", dns.rdatatype.A)
-        r = dns.query.https(
-            q, nameserver_url, session=self.session, post=True, timeout=4
-        )
-        self.assertTrue(q.is_response(r))
-
-    def test_build_url_from_ip(self):
-        self.assertTrue(resolver_v4_addresses or resolver_v6_addresses)
-        if resolver_v4_addresses:
-            nameserver_ip = random.choice(resolver_v4_addresses)
-            q = dns.message.make_query("example.com.", dns.rdatatype.A)
-            # For some reason Google's DNS over HTTPS fails when you POST to
-            # https://8.8.8.8/dns-query
-            # So we're just going to do GET requests here
-            r = dns.query.https(
-                q, nameserver_ip, session=self.session, post=False, timeout=4
-            )
-
-            self.assertTrue(q.is_response(r))
-        if resolver_v6_addresses:
-            nameserver_ip = random.choice(resolver_v6_addresses)
-            q = dns.message.make_query("example.com.", dns.rdatatype.A)
-            r = dns.query.https(
-                q, nameserver_ip, session=self.session, post=False, timeout=4
-            )
-            self.assertTrue(q.is_response(r))
-
-    def test_bootstrap_address(self):
-        # We test this to see if v4 is available
-        if resolver_v4_addresses:
-            ip = "185.228.168.168"
-            invalid_tls_url = "https://{}/doh/family-filter/".format(ip)
-            valid_tls_url = "https://doh.cleanbrowsing.org/doh/family-filter/"
-            q = dns.message.make_query("example.com.", dns.rdatatype.A)
-            # make sure CleanBrowsing's IP address will fail TLS certificate
-            # check
-            with self.assertRaises(SSLError):
-                dns.query.https(q, invalid_tls_url, session=self.session, timeout=4)
-            # use host header
-            r = dns.query.https(
-                q, valid_tls_url, session=self.session, bootstrap_address=ip, timeout=4
-            )
-            self.assertTrue(q.is_response(r))
-
-    def test_new_session(self):
-        nameserver_url = random.choice(KNOWN_ANYCAST_DOH_RESOLVER_URLS)
-        q = dns.message.make_query("example.com.", dns.rdatatype.A)
-        r = dns.query.https(q, nameserver_url, timeout=4)
-        self.assertTrue(q.is_response(r))
-
-    def test_resolver(self):
-        res = dns.resolver.Resolver(configure=False)
-        res.nameservers = ["https://dns.google/dns-query"]
-        answer = res.resolve("dns.google", "A")
-        seen = set([rdata.address for rdata in answer])
-        self.assertTrue("8.8.8.8" in seen)
-        self.assertTrue("8.8.4.4" in seen)
-
-
-@unittest.skipUnless(
     dns.query._have_httpx and tests.util.is_internet_reachable() and _have_ssl,
     "Python httpx cannot be imported; no DNS over HTTPS (DOH)",
 )
 class DNSOverHTTPSTestCaseHttpx(unittest.TestCase):
     def setUp(self):
         self.session = httpx.Client(http1=True, http2=True, verify=True)
 
     def tearDown(self):
         self.session.close()
 
     def test_get_request(self):
         nameserver_url = random.choice(KNOWN_ANYCAST_DOH_RESOLVER_URLS)
         q = dns.message.make_query("example.com.", dns.rdatatype.A)
         r = dns.query.https(
-            q, nameserver_url, session=self.session, post=False, timeout=4
+            q,
+            nameserver_url,
+            session=self.session,
+            post=False,
+            timeout=4,
+            family=family,
         )
         self.assertTrue(q.is_response(r))
 
     def test_get_request_http1(self):
         saved_have_http2 = dns.query._have_http2
         try:
             dns.query._have_http2 = False
             nameserver_url = random.choice(KNOWN_ANYCAST_DOH_RESOLVER_URLS)
             q = dns.message.make_query("example.com.", dns.rdatatype.A)
             r = dns.query.https(
-                q, nameserver_url, session=self.session, post=False, timeout=4
+                q,
+                nameserver_url,
+                session=self.session,
+                post=False,
+                timeout=4,
+                family=family,
             )
             self.assertTrue(q.is_response(r))
         finally:
             dns.query._have_http2 = saved_have_http2
 
     def test_post_request(self):
         nameserver_url = random.choice(KNOWN_ANYCAST_DOH_RESOLVER_URLS)
         q = dns.message.make_query("example.com.", dns.rdatatype.A)
         r = dns.query.https(
-            q, nameserver_url, session=self.session, post=True, timeout=4
+            q,
+            nameserver_url,
+            session=self.session,
+            post=True,
+            timeout=4,
+            family=family,
         )
         self.assertTrue(q.is_response(r))
 
     def test_build_url_from_ip(self):
         self.assertTrue(resolver_v4_addresses or resolver_v6_addresses)
         if resolver_v4_addresses:
             nameserver_ip = random.choice(resolver_v4_addresses)
@@ -215,25 +154,23 @@
             invalid_tls_url = "https://{}/doh/family-filter/".format(ip)
             valid_tls_url = "https://doh.cleanbrowsing.org/doh/family-filter/"
             q = dns.message.make_query("example.com.", dns.rdatatype.A)
             # make sure CleanBrowsing's IP address will fail TLS certificate
             # check.
             with self.assertRaises(httpx.ConnectError):
                 dns.query.https(q, invalid_tls_url, session=self.session, timeout=4)
-            # We can't do the Host header and SNI magic with httpx, but
-            # we are demanding httpx be used by providing a session, so
-            # we should get a NoDOH exception.
-            with self.assertRaises(dns.query.NoDOH):
-                dns.query.https(
-                    q,
-                    valid_tls_url,
-                    session=self.session,
-                    bootstrap_address=ip,
-                    timeout=4,
-                )
+            # And if we don't mangle the URL, it should work.
+            r = dns.query.https(
+                q,
+                valid_tls_url,
+                session=self.session,
+                bootstrap_address=ip,
+                timeout=4,
+            )
+            self.assertTrue(q.is_response(r))
 
     def test_new_session(self):
         nameserver_url = random.choice(KNOWN_ANYCAST_DOH_RESOLVER_URLS)
         q = dns.message.make_query("example.com.", dns.rdatatype.A)
         r = dns.query.https(q, nameserver_url, timeout=4)
         self.assertTrue(q.is_response(r))
```

### Comparing `dnspython-2.3.0rc1/tests/test_doq.py` & `dnspython-2.4.0rc1/tests/test_doq.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_edns.py` & `dnspython-2.4.0rc1/tests/test_edns.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_entropy.py` & `dnspython-2.4.0rc1/tests/test_entropy.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_exceptions.py` & `dnspython-2.4.0rc1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_flags.py` & `dnspython-2.4.0rc1/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_generate.py` & `dnspython-2.4.0rc1/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_grange.py` & `dnspython-2.4.0rc1/tests/test_grange.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_immutable.py` & `dnspython-2.4.0rc1/tests/test_immutable.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         )
         for input, expected in items:
             self.assertEqual(dns.immutable.constify(input), expected)
         self.assertIsInstance(dns.immutable.constify({"a": 1}), dns.immutable.Dict)
 
 
 class DecoratorTestCase(unittest.TestCase):
-
     immutable_module = dns._immutable_ctx
 
     def make_classes(self):
         class A:
             def __init__(self, a, akw=10):
                 self.a = a
                 self.akw = akw
@@ -121,15 +120,14 @@
 
         A = self.immutable_module.immutable(A)
         a = A(10)
         self.assertEqual(a.a, 10)
         self.assertFalse(hasattr(a, "b"))
 
     def test_no_collateral_damage(self):
-
         # A and B are immutable but not related.  The magic that lets
         # us write to immutable things while initializing B should not let
         # B mess with A.
 
         class A:
             def __init__(self, a):
                 self.a = a
```

### Comparing `dnspython-2.3.0rc1/tests/test_message.py` & `dnspython-2.4.0rc1/tests/test_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,14 +281,22 @@
         a.index = None
         n = dns.name.from_text("dnspython.org.")
         rrs1 = a.get_rrset(a.answer, n, dns.rdataclass.IN, dns.rdatatype.TXT)
         rrs2 = a.get_rrset(dns.message.ANSWER, n, dns.rdataclass.IN, dns.rdatatype.TXT)
         self.assertTrue(rrs1 is None)
         self.assertEqual(rrs1, rrs2)
 
+    def test_GetRRsetStrings(self):
+        a = dns.message.from_text(answer_text)
+        a.index = None
+        n = dns.name.from_text("dnspython.org.")
+        rrs1 = a.get_rrset(a.answer, n, dns.rdataclass.IN, dns.rdatatype.SOA)
+        rrs2 = a.get_rrset("ANSWER", "dnspython.org.", "IN", "SOA")
+        self.assertEqual(rrs1, rrs2)
+
     def test_CleanTruncated(self):
         def bad():
             a = dns.message.from_text(answer_text)
             a.flags |= dns.flags.TC
             wire = a.to_wire(want_shuffle=False)
             dns.message.from_wire(wire, raise_on_truncation=True)
```

### Comparing `dnspython-2.3.0rc1/tests/test_name.py` & `dnspython-2.4.0rc1/tests/test_name.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_namedict.py` & `dnspython-2.4.0rc1/tests/test_namedict.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_nsec3.py` & `dnspython-2.4.0rc1/tests/test_nsec3.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_nsec3_hash.py` & `dnspython-2.4.0rc1/tests/test_nsec3_hash.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import unittest
 
 from dns import dnssec, name
 
 
 class NSEC3Hash(unittest.TestCase):
-
     DATA = [
         # Source: https://tools.ietf.org/html/rfc5155#appendix-A
         ("example", "aabbccdd", 12, "0p9mhaveqvm6t7vbl5lop2u3t2rp3tom", 1),
         ("a.example", "aabbccdd", 12, "35mthgpgcu1qg68fab165klnsnk3dpvl", 1),
         ("ai.example", "aabbccdd", 12, "gjeqe526plbf1g8mklp59enfd789njgi", 1),
         ("ns1.example", "aabbccdd", 12, "2t7b4g4vsa5smi47k61mv5bv1a22bojr", 1),
         ("ns2.example", "aabbccdd", 12, "q04jkcevqvmu85r014c7dkba38o0ji5r", 1),
```

### Comparing `dnspython-2.3.0rc1/tests/test_ntoaaton.py` & `dnspython-2.4.0rc1/tests/test_ntoaaton.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
 
     def test_good_v4_aton(self):
         pairs = [
             ("1.2.3.4", b"\x01\x02\x03\x04"),
             ("255.255.255.255", b"\xff\xff\xff\xff"),
             ("0.0.0.0", b"\x00\x00\x00\x00"),
         ]
-        for (t, b) in pairs:
+        for t, b in pairs:
             b1 = aton4(t)
             t1 = ntoa4(b1)
             self.assertEqual(b1, b)
             self.assertEqual(t1, t)
 
     def test_bad_v4_aton(self):
         def make_bad(a):
@@ -285,22 +285,22 @@
         def bad():
             t1 = "fe80::1%lo0%lo1"
             aton6(t1, True)
 
         self.assertRaises(dns.exception.SyntaxError, bad)
 
     def test_ptontop(self):
-        for (af, a) in [
+        for af, a in [
             (socket.AF_INET, "1.2.3.4"),
             (socket.AF_INET6, "2001:db8:0:1:1:1:1:1"),
         ]:
             self.assertEqual(dns.inet.inet_ntop(af, dns.inet.inet_pton(af, a)), a)
 
     def test_isaddress(self):
-        for (t, e) in [
+        for t, e in [
             ("1.2.3.4", True),
             ("2001:db8:0:1:1:1:1:1", True),
             ("hello world", False),
             ("http://www.dnspython.org", False),
             ("1.2.3.4a", False),
             ("2001:db8:0:1:1:1:1:q1", False),
         ]:
```

### Comparing `dnspython-2.3.0rc1/tests/test_processing_order.py` & `dnspython-2.4.0rc1/tests/test_processing_order.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_query.py` & `dnspython-2.4.0rc1/tests/test_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,15 +326,15 @@
         response = dns.message.make_response(request.message)
         response.flags |= dns.flags.AA
         response.answer.append(soa)
         items.append(response)
         response = dns.message.make_response(request.message)
         response.question = []
         response.flags |= dns.flags.AA
-        for (name, rdataset) in self.zone.iterate_rdatasets():
+        for name, rdataset in self.zone.iterate_rdatasets():
             if rdataset.rdtype == dns.rdatatype.SOA and name == dns.name.empty:
                 continue
             rrset = dns.rrset.RRset(
                 name, rdataset.rdclass, rdataset.rdtype, rdataset.covers
             )
             rrset.update(rdataset)
             response.answer.append(rrset)
```

### Comparing `dnspython-2.3.0rc1/tests/test_rdata.py` & `dnspython-2.4.0rc1/tests/test_rdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -582,21 +582,20 @@
         dns.rdata.from_text("in", "type45678", r"\# 0")
 
     def test_covered_repr(self):
         text = "NSEC 1 3 3600 20190101000000 20030101000000 " + "2143 foo Ym9ndXM="
         rd = dns.rdata.from_text("in", "rrsig", text)
         self.assertEqual(repr(rd), "<DNS IN RRSIG(NSEC) rdata: " + text + ">")
 
-    def test_bad_registration_implementing_known_type_with_wrong_name(self):
-        # Try to register an implementation at the MG codepoint that isn't
-        # called "MG"
+    def test_registration_implementing_known_and_implemented_type(self):
+        # Try to register an implementation at the A codepoint.
         with self.assertRaises(dns.rdata.RdatatypeExists):
-            dns.rdata.register_type(None, dns.rdatatype.MG, "NOTMG")
+            dns.rdata.register_type(None, dns.rdatatype.A, "ANYTHING")
 
-    def test_registration_implementing_known_type_with_right_name(self):
+    def test_registration_of_known_but_unimplmented_type(self):
         # Try to register an implementation at the MD codepoint
         dns.rdata.register_type(tests.md_module, dns.rdatatype.MD, "MD")
         rd = dns.rdata.from_text("in", "md", "foo.")
         self.assertEqual(rd.target, dns.name.from_text("foo."))
 
     def test_CERT_with_string_type(self):
         rd = dns.rdata.from_text("in", "cert", "SPKI 1 PRIVATEOID Ym9ndXM=")
```

### Comparing `dnspython-2.3.0rc1/tests/test_rdataset.py` & `dnspython-2.4.0rc1/tests/test_rdataset.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_rdtypeandclass.py` & `dnspython-2.4.0rc1/tests/test_rdtypeandclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 import unittest
 
 import dns.rdataclass
 import dns.rdatatype
 
 
 class RdTypeAndClassTestCase(unittest.TestCase):
-
     # Classes
 
     def test_class_meta1(self):
         self.assertTrue(dns.rdataclass.is_metaclass(dns.rdataclass.ANY))
 
     def test_class_meta2(self):
         self.assertFalse(dns.rdataclass.is_metaclass(dns.rdataclass.IN))
```

### Comparing `dnspython-2.3.0rc1/tests/test_rdtypeanydnskey.py` & `dnspython-2.4.0rc1/tests/test_rdtypeanydnskey.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_rdtypeanyeui.py` & `dnspython-2.4.0rc1/tests/test_rdtypeanyeui.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_rdtypeanyloc.py` & `dnspython-2.4.0rc1/tests/test_rdtypeanyloc.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_rdtypeanytkey.py` & `dnspython-2.4.0rc1/tests/test_rdtypeanytkey.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_renderer.py` & `dnspython-2.4.0rc1/tests/test_renderer.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_resolution.py` & `dnspython-2.4.0rc1/tests/test_resolution.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,30 +218,32 @@
             self.assertTrue(False)  # should not happen!
         except dns.resolver.NXDOMAIN as nx:
             self.assertTrue(nx.response(qname1) is r1)
             self.assertTrue(nx.response(qname2) is r2)
 
     def test_next_request_rotate(self):
         self.resolver.rotate = True
-        order1 = ["10.0.0.1", "10.0.0.2"]
-        order2 = ["10.0.0.2", "10.0.0.1"]
+        order1 = ["Do53:10.0.0.1@53", "Do53:10.0.0.2@53"]
+        order2 = ["Do53:10.0.0.2@53", "Do53:10.0.0.1@53"]
         seen1 = False
         seen2 = False
         # We're not interested in testing the randomness, but we'd
         # like to see some shuffling, so try up to 50 times to see
         # both orders at least once.  This test can fail even with
         # correct code, but it is *extremely* unlikely.
         for count in range(0, 50):
             self.resn = dns.resolver._Resolution(
                 self.resolver, self.qname, "A", "IN", False, True, False
             )
             self.resn.next_request()
-            if self.resn.nameservers == order1:
+            text_form = [str(n) for n in self.resn.nameservers]
+            print(text_form)
+            if text_form == order1:
                 seen1 = True
-            elif self.resn.nameservers == order2:
+            elif text_form == order2:
                 seen2 = True
             else:
                 raise ValueError  # should not happen!
             if seen1 and seen2:
                 break
         self.assertTrue(seen1 and seen2)
 
@@ -260,85 +262,88 @@
         self.resolver.flags = dns.flags.RD | dns.flags.CD
         (request, answer) = self.resn.next_request()
         self.assertFalse(request is None)
         self.assertEqual(request.flags, self.resolver.flags)
 
     def test_next_nameserver_udp(self):
         (request, answer) = self.resn.next_request()
-        (nameserver1, port, tcp, backoff) = self.resn.next_nameserver()
-        self.assertTrue(nameserver1 in self.resolver.nameservers)
-        self.assertEqual(port, 53)
+        (nameserver1, tcp, backoff) = self.resn.next_nameserver()
+        self.assertEqual(nameserver1.port, 53)
         self.assertFalse(tcp)
         self.assertEqual(backoff, 0.0)
-        (nameserver2, port, tcp, backoff) = self.resn.next_nameserver()
-        self.assertTrue(nameserver2 in self.resolver.nameservers)
+        (nameserver2, tcp, backoff) = self.resn.next_nameserver()
         self.assertTrue(nameserver2 != nameserver1)
-        self.assertEqual(port, 53)
+        self.assertEqual(nameserver2.port, 53)
         self.assertFalse(tcp)
         self.assertEqual(backoff, 0.0)
-        (nameserver3, port, tcp, backoff) = self.resn.next_nameserver()
+        (nameserver3, tcp, backoff) = self.resn.next_nameserver()
         self.assertTrue(nameserver3 is nameserver1)
-        self.assertEqual(port, 53)
         self.assertFalse(tcp)
         self.assertEqual(backoff, 0.1)
-        (nameserver4, port, tcp, backoff) = self.resn.next_nameserver()
+        (nameserver4, tcp, backoff) = self.resn.next_nameserver()
         self.assertTrue(nameserver4 is nameserver2)
-        self.assertEqual(port, 53)
         self.assertFalse(tcp)
         self.assertEqual(backoff, 0.0)
-        (nameserver5, port, tcp, backoff) = self.resn.next_nameserver()
+        (nameserver5, tcp, backoff) = self.resn.next_nameserver()
         self.assertTrue(nameserver5 is nameserver1)
-        self.assertEqual(port, 53)
         self.assertFalse(tcp)
         self.assertEqual(backoff, 0.2)
 
     def test_next_nameserver_retry_with_tcp(self):
         (request, answer) = self.resn.next_request()
-        (nameserver1, port, tcp, backoff) = self.resn.next_nameserver()
-        self.assertTrue(nameserver1 in self.resolver.nameservers)
-        self.assertEqual(port, 53)
+        (nameserver1, tcp, backoff) = self.resn.next_nameserver()
+        self.assertEqual(nameserver1.port, 53)
         self.assertFalse(tcp)
         self.assertEqual(backoff, 0.0)
         self.resn.retry_with_tcp = True
-        (nameserver2, port, tcp, backoff) = self.resn.next_nameserver()
+        (nameserver2, tcp, backoff) = self.resn.next_nameserver()
         self.assertTrue(nameserver2 is nameserver1)
-        self.assertEqual(port, 53)
         self.assertTrue(tcp)
         self.assertEqual(backoff, 0.0)
-        (nameserver3, port, tcp, backoff) = self.resn.next_nameserver()
-        self.assertTrue(nameserver3 in self.resolver.nameservers)
+        (nameserver3, tcp, backoff) = self.resn.next_nameserver()
         self.assertTrue(nameserver3 != nameserver1)
-        self.assertEqual(port, 53)
+        self.assertEqual(nameserver3.port, 53)
         self.assertFalse(tcp)
         self.assertEqual(backoff, 0.0)
 
     def test_next_nameserver_no_nameservers(self):
         (request, answer) = self.resn.next_request()
-        (nameserver, _, _, _) = self.resn.next_nameserver()
+        (nameserver, _, _) = self.resn.next_nameserver()
         self.resn.nameservers.remove(nameserver)
-        (nameserver, _, _, _) = self.resn.next_nameserver()
+        (nameserver, _, _) = self.resn.next_nameserver()
         self.resn.nameservers.remove(nameserver)
 
         def bad():
-            (nameserver, _, _, _) = self.resn.next_nameserver()
+            (nameserver, _, _) = self.resn.next_nameserver()
 
         self.assertRaises(dns.resolver.NoNameservers, bad)
 
+    def test_next_nameserver_max_size_nameserver(self):
+        # A query to a nameserver that always supports a maximum size query
+        # always counts as a "tcp attempt" for the state machine
+        self.resolver.nameservers = ["https://127.0.0.1:443/bogus"]
+        (_, _) = self.resn.next_request()
+        (nameserver, tcp_attempt, _) = self.resn.next_nameserver()
+        print(nameserver)
+        assert tcp_attempt
+
     def test_query_result_nameserver_removing_exceptions(self):
         # add some nameservers so we have enough to remove :)
-        self.resolver.nameservers.extend(["10.0.0.3", "10.0.0.4"])
+        new_nameservers = list(self.resolver.nameservers[:])
+        new_nameservers.extend(["10.0.0.3", "10.0.0.4"])
+        self.resolver.nameservers = new_nameservers
         (request, _) = self.resn.next_request()
         exceptions = [
             dns.exception.FormError(),
             EOFError(),
             NotImplementedError(),
             dns.message.Truncated(),
         ]
         for i in range(4):
-            (nameserver, _, _, _) = self.resn.next_nameserver()
+            (nameserver, _, _) = self.resn.next_nameserver()
             if i == 3:
                 # Truncated is only bad if we're doing TCP, make it look
                 # like that's the case
                 self.resn.tcp_attempt = True
             self.assertTrue(nameserver in self.resn.nameservers)
             (answer, done) = self.resn.query_result(None, exceptions[i])
             self.assertTrue(answer is None)
@@ -347,163 +352,163 @@
         self.assertEqual(len(self.resn.nameservers), 0)
 
     def test_query_result_nameserver_continuing_exception(self):
         # except for the exceptions tested in
         # test_query_result_nameserver_removing_exceptions(), we should
         # not remove any nameservers and just continue resolving.
         (_, _) = self.resn.next_request()
-        (_, _, _, _) = self.resn.next_nameserver()
+        (_, _, _) = self.resn.next_nameserver()
         nameservers = self.resn.nameservers[:]
         (answer, done) = self.resn.query_result(None, dns.exception.Timeout())
         self.assertTrue(answer is None)
         self.assertFalse(done)
         self.assertEqual(nameservers, self.resn.nameservers)
 
     def test_query_result_retry_with_tcp(self):
         (request, _) = self.resn.next_request()
-        (nameserver, _, tcp, _) = self.resn.next_nameserver()
+        (nameserver, tcp, _) = self.resn.next_nameserver()
         self.assertFalse(tcp)
         (answer, done) = self.resn.query_result(None, dns.message.Truncated())
         self.assertTrue(answer is None)
         self.assertFalse(done)
         self.assertTrue(self.resn.retry_with_tcp)
         # The rest of TCP retry logic was tested above in
         # test_next_nameserver_retry_with_tcp(), so we do not repeat
         # it.
 
     def test_query_result_no_error_with_data(self):
         q = dns.message.make_query(self.qname, dns.rdatatype.A)
         r = self.make_address_response(q)
         (_, _) = self.resn.next_request()
-        (_, _, _, _) = self.resn.next_nameserver()
+        (_, _, _) = self.resn.next_nameserver()
         (answer, done) = self.resn.query_result(r, None)
         self.assertFalse(answer is None)
         self.assertTrue(done)
         self.assertEqual(answer.qname, self.qname)
         self.assertEqual(answer.rdtype, dns.rdatatype.A)
 
     def test_query_result_no_error_with_data_cached(self):
         self.resolver.cache = dns.resolver.Cache()
         q = dns.message.make_query(self.qname, dns.rdatatype.A)
         r = self.make_address_response(q)
         (_, _) = self.resn.next_request()
-        (_, _, _, _) = self.resn.next_nameserver()
+        (_, _, _) = self.resn.next_nameserver()
         (answer, done) = self.resn.query_result(r, None)
         self.assertFalse(answer is None)
         cache_answer = self.resolver.cache.get(
             (self.qname, dns.rdatatype.A, dns.rdataclass.IN)
         )
         self.assertTrue(answer is cache_answer)
 
     def test_query_result_no_error_no_data(self):
         q = dns.message.make_query(self.qname, dns.rdatatype.A)
         r = self.make_negative_response(q)
         (_, _) = self.resn.next_request()
-        (_, _, _, _) = self.resn.next_nameserver()
+        (_, _, _) = self.resn.next_nameserver()
 
         def bad():
             (answer, done) = self.resn.query_result(r, None)
 
         self.assertRaises(dns.resolver.NoAnswer, bad)
 
     def test_query_result_nxdomain(self):
         q = dns.message.make_query(self.qname, dns.rdatatype.A)
         r = self.make_negative_response(q, True)
         (_, _) = self.resn.next_request()
-        (_, _, _, _) = self.resn.next_nameserver()
+        (_, _, _) = self.resn.next_nameserver()
         (answer, done) = self.resn.query_result(r, None)
         self.assertTrue(answer is None)
         self.assertTrue(done)
 
     def test_query_result_nxdomain_but_has_answer(self):
         q = dns.message.make_query(self.qname, dns.rdatatype.A)
         r = self.make_address_response(q)
         r.set_rcode(dns.rcode.NXDOMAIN)
         (_, _) = self.resn.next_request()
-        (nameserver, _, _, _) = self.resn.next_nameserver()
+        (nameserver, _, _) = self.resn.next_nameserver()
         (answer, done) = self.resn.query_result(r, None)
         self.assertIsNone(answer)
         self.assertFalse(done)
         self.assertTrue(nameserver not in self.resn.nameservers)
 
     def test_query_result_chain_not_too_long(self):
         q = dns.message.make_query(self.qname, dns.rdatatype.A)
         r = self.make_long_chain_response(q, 15)
         (_, _) = self.resn.next_request()
-        (_, _, _, _) = self.resn.next_nameserver()
+        (_, _, _) = self.resn.next_nameserver()
         (answer, done) = self.resn.query_result(r, None)
         self.assertIsNotNone(answer)
         self.assertTrue(done)
 
     def test_query_result_chain_too_long(self):
         q = dns.message.make_query(self.qname, dns.rdatatype.A)
         r = self.make_long_chain_response(q, 16)
         (_, _) = self.resn.next_request()
-        (nameserver, _, _, _) = self.resn.next_nameserver()
+        (nameserver, _, _) = self.resn.next_nameserver()
         (answer, done) = self.resn.query_result(r, None)
         self.assertIsNone(answer)
         self.assertFalse(done)
         self.assertTrue(nameserver not in self.resn.nameservers)
 
     def test_query_result_nxdomain_cached(self):
         self.resolver.cache = dns.resolver.Cache()
         q = dns.message.make_query(self.qname, dns.rdatatype.A)
         r = self.make_negative_response(q, True)
         (_, _) = self.resn.next_request()
-        (_, _, _, _) = self.resn.next_nameserver()
+        (_, _, _) = self.resn.next_nameserver()
         (answer, done) = self.resn.query_result(r, None)
         self.assertTrue(answer is None)
         self.assertTrue(done)
         cache_answer = self.resolver.cache.get(
             (self.qname, dns.rdatatype.ANY, dns.rdataclass.IN)
         )
         self.assertTrue(cache_answer.response is r)
 
     def test_query_result_yxdomain(self):
         q = dns.message.make_query(self.qname, dns.rdatatype.A)
         r = self.make_address_response(q)
         r.set_rcode(dns.rcode.YXDOMAIN)
         (_, _) = self.resn.next_request()
-        (_, _, _, _) = self.resn.next_nameserver()
+        (_, _, _) = self.resn.next_nameserver()
 
         def bad():
             (answer, done) = self.resn.query_result(r, None)
 
         self.assertRaises(dns.resolver.YXDOMAIN, bad)
 
     def test_query_result_servfail_no_retry(self):
         q = dns.message.make_query(self.qname, dns.rdatatype.A)
         r = self.make_address_response(q)
         r.set_rcode(dns.rcode.SERVFAIL)
         (_, _) = self.resn.next_request()
-        (nameserver, _, _, _) = self.resn.next_nameserver()
+        (nameserver, _, _) = self.resn.next_nameserver()
         (answer, done) = self.resn.query_result(r, None)
         self.assertTrue(answer is None)
         self.assertFalse(done)
         self.assertTrue(nameserver not in self.resn.nameservers)
 
     def test_query_result_servfail_with_retry(self):
         self.resolver.retry_servfail = True
         q = dns.message.make_query(self.qname, dns.rdatatype.A)
         r = self.make_address_response(q)
         r.set_rcode(dns.rcode.SERVFAIL)
         (_, _) = self.resn.next_request()
-        (_, _, _, _) = self.resn.next_nameserver()
+        (_, _, _) = self.resn.next_nameserver()
         nameservers = self.resn.nameservers[:]
         (answer, done) = self.resn.query_result(r, None)
         self.assertTrue(answer is None)
         self.assertFalse(done)
         self.assertEqual(nameservers, self.resn.nameservers)
 
     def test_query_result_other_unhappy_rcode(self):
         q = dns.message.make_query(self.qname, dns.rdatatype.A)
         r = self.make_address_response(q)
         r.set_rcode(dns.rcode.REFUSED)
         (_, _) = self.resn.next_request()
-        (nameserver, _, _, _) = self.resn.next_nameserver()
+        (nameserver, _, _) = self.resn.next_nameserver()
         (answer, done) = self.resn.query_result(r, None)
         self.assertTrue(answer is None)
         self.assertFalse(done)
         self.assertTrue(nameserver not in self.resn.nameservers)
 
     def test_no_metaqueries(self):
         def bad1():
```

### Comparing `dnspython-2.3.0rc1/tests/test_resolver.py` & `dnspython-2.4.0rc1/tests/test_resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,19 @@
 import unittest
 import pytest
 from unittest.mock import patch
 
 import dns.e164
 import dns.message
 import dns.name
+import dns.quic
 import dns.rdataclass
 import dns.rdatatype
 import dns.resolver
+import dns.reversename
 import dns.tsig
 import dns.tsigkeyring
 import tests.util
 
 # Some tests use a "nano nameserver" for testing.  It requires trio
 # and threading, so try to import it and if it doesn't work, skip
 # those tests.
@@ -660,14 +662,41 @@
         self.assertTrue("8.8.4.4" in seen)
 
     def testResolveAddress(self):
         answer = dns.resolver.resolve_address("8.8.8.8")
         dnsgoogle = dns.name.from_text("dns.google.")
         self.assertEqual(answer[0].target, dnsgoogle)
 
+    def testResolveName(self):
+        answers = dns.resolver.resolve_name("dns.google.")
+        seen = set(answers.addresses())
+        self.assertEqual(len(seen), 4)
+        self.assertIn("8.8.8.8", seen)
+        self.assertIn("8.8.4.4", seen)
+        self.assertIn("2001:4860:4860::8844", seen)
+        self.assertIn("2001:4860:4860::8888", seen)
+
+        answers = dns.resolver.resolve_name("dns.google.", socket.AF_INET)
+        seen = set(answers.addresses())
+        self.assertEqual(len(seen), 2)
+        self.assertIn("8.8.8.8", seen)
+        self.assertIn("8.8.4.4", seen)
+
+        answers = dns.resolver.resolve_name("dns.google.", socket.AF_INET6)
+        seen = set(answers.addresses())
+        self.assertEqual(len(seen), 2)
+        self.assertIn("2001:4860:4860::8844", seen)
+        self.assertIn("2001:4860:4860::8888", seen)
+
+        with self.assertRaises(dns.resolver.NXDOMAIN):
+            dns.resolver.resolve_name("nxdomain.dnspython.org")
+
+        with self.assertRaises(dns.resolver.NoAnswer):
+            dns.resolver.resolve_name(dns.reversename.from_address("8.8.8.8"))
+
     @patch.object(dns.message.Message, "use_edns")
     def testResolveEdnsOptions(self, message_use_edns_mock):
         resolver = dns.resolver.Resolver()
         options = [dns.edns.ECSOption("1.1.1.1")]
         resolver.use_edns(True, options=options)
         resolver.resolve("dns.google.", "A")
         assert {"options": options} in message_use_edns_mock.call_args
@@ -713,14 +742,51 @@
         answer1 = res.resolve("dns.google.", "A")
         seen = set([rdata.address for rdata in answer1])
         self.assertIn("8.8.8.8", seen)
         self.assertIn("8.8.4.4", seen)
         answer2 = res.resolve("dns.google.", "A")
         self.assertIs(answer2, answer1)
 
+    @unittest.skipIf(not tests.util.have_ipv4(), "IPv4 not reachable")
+    def testTLSNameserver(self):
+        res = dns.resolver.Resolver(configure=False)
+        res.nameservers = [dns.nameserver.DoTNameserver("8.8.8.8", 853)]
+        answer = res.resolve("dns.google.", "A")
+        seen = set([rdata.address for rdata in answer])
+        self.assertIn("8.8.8.8", seen)
+        self.assertIn("8.8.4.4", seen)
+
+    @unittest.skipIf(
+        not (tests.util.have_ipv4() and dns.quic.have_quic),
+        "IPv4 not reachable or QUIC not available",
+    )
+    def testQuicNameserver(self):
+        res = dns.resolver.Resolver(configure=False)
+        res.nameservers = [dns.nameserver.DoQNameserver("94.140.14.14", 784)]
+        answer = res.resolve("dns.adguard.com.", "A")
+        seen = set([rdata.address for rdata in answer])
+        self.assertIn("94.140.14.14", seen)
+        self.assertIn("94.140.15.15", seen)
+
+    @unittest.skipIf(not tests.util.have_ipv4(), "IPv4 not reachable")
+    def testResolveAtAddress(self):
+        answer = dns.resolver.resolve_at("8.8.8.8", "dns.google.", "A")
+        seen = set([rdata.address for rdata in answer])
+        self.assertIn("8.8.8.8", seen)
+        self.assertIn("8.8.4.4", seen)
+
+    @unittest.skipIf(not tests.util.have_ipv4(), "IPv4 not reachable")
+    def testResolveAtName(self):
+        answer = dns.resolver.resolve_at(
+            "dns.google", "dns.google.", "A", family=socket.AF_INET
+        )
+        seen = set([rdata.address for rdata in answer])
+        self.assertIn("8.8.8.8", seen)
+        self.assertIn("8.8.4.4", seen)
+
     def testCanonicalNameNoCNAME(self):
         cname = dns.name.from_text("www.google.com")
         self.assertEqual(dns.resolver.canonical_name("www.google.com"), cname)
 
     def testCanonicalNameCNAME(self):
         name = dns.name.from_text("www.dnspython.org")
         cname = dns.name.from_text("dmfrjf4ips8xa.cloudfront.net")
@@ -768,15 +834,14 @@
         PollingMonkeyPatchMixin, LiveResolverTests, unittest.TestCase
     ):
         def selector_class(self):
             return selectors.PollSelector
 
 
 class NXDOMAINExceptionTestCase(unittest.TestCase):
-
     # pylint: disable=broad-except
 
     def test_nxdomain_compatible(self):
         n1 = dns.name.Name(("a", "b", ""))
         n2 = dns.name.Name(("a", "b", "s", ""))
 
         try:
@@ -947,14 +1012,15 @@
     def test_set_nameservers_invalid_type(self):
         resolver = dns.resolver.Resolver(configure=False)
         invalid_nameservers = [
             None,
             "1.2.3.4",
             1234,
             (1, 2, 3, 4),
+            (),
             {"invalid": "nameserver"},
         ]
         for invalid_nameserver in invalid_nameservers:
             with self.assertRaises(ValueError):
                 resolver.nameservers = invalid_nameserver
 
 
@@ -1119,15 +1185,15 @@
         except dns.resolver.LifetimeTimeout as e:
             assert e.kwargs["timeout"] >= lifetime
             # The length of errors can vary based on how slow things are,
             # but it ought to be > 1, so we assert that.
             errors = e.kwargs["errors"]
             assert len(errors) > 1
             for error in errors:
-                assert error[0] == na.udp_address[0]  # address
+                assert str(error[0]) == f"Do53:{na.udp_address[0]}@{na.udp_address[1]}"
                 assert not error[1]  # not TCP
                 assert error[2] == na.udp_address[1]  # port
                 assert isinstance(error[3], dns.exception.Timeout)  # exception
 
 
 @pytest.mark.skipif(
     not (tests.util.is_internet_reachable() and _nanonameserver_available),
@@ -1141,15 +1207,15 @@
         try:
             a = res.resolve("www.dnspython.org")
             assert False  # should never happen
         except dns.resolver.NoNameservers as e:
             errors = e.kwargs["errors"]
             assert len(errors) == 1
             for error in errors:
-                assert error[0] == na.udp_address[0]  # address
+                assert error[0] == f"Do53:{na.udp_address[0]}@{na.udp_address[1]}"
                 assert not error[1]  # not TCP
                 assert error[2] == na.udp_address[1]  # port
                 assert error[3] == "FORMERR"
 
 
 class SlowAlwaysType3NXDOMAINNanoNameserver(Server):
     def handle(self, request):
```

### Comparing `dnspython-2.3.0rc1/tests/test_resolver_override.py` & `dnspython-2.4.0rc1/tests/test_resolver_override.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_rrset.py` & `dnspython-2.4.0rc1/tests/test_rrset.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_rrset_reader.py` & `dnspython-2.4.0rc1/tests/test_rrset_reader.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_serial.py` & `dnspython-2.4.0rc1/tests/test_serial.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_set.py` & `dnspython-2.4.0rc1/tests/test_set.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_svcb.py` & `dnspython-2.4.0rc1/tests/test_svcb.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_tokenizer.py` & `dnspython-2.4.0rc1/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_transaction.py` & `dnspython-2.4.0rc1/tests/test_transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -495,44 +495,55 @@
         with pytest.raises(KeyError):
             a99 = dns.name.from_text("a99.not-example.")
             assert txn.name_exists(a99)
 
 
 def test_zone_iteration(zone):
     expected = {}
-    for (name, rdataset) in zone.iterate_rdatasets():
+    for name, rdataset in zone.iterate_rdatasets():
         expected[(name, rdataset.rdtype, rdataset.covers)] = rdataset
     with zone.writer() as txn:
-        actual = {}
-        for (name, rdataset) in txn:
-            actual[(name, rdataset.rdtype, rdataset.covers)] = rdataset
+        actual1 = {}
+        for name, rdataset in txn:
+            actual1[(name, rdataset.rdtype, rdataset.covers)] = rdataset
+        actual2 = {}
+        for name, rdataset in txn.iterate_rdatasets():
+            actual2[(name, rdataset.rdtype, rdataset.covers)] = rdataset
+    assert actual1 == expected
+    assert actual2 == expected
+
+
+def test_zone_name_iteration(zone):
+    expected = list(zone.keys())
+    with zone.writer() as txn:
+        actual = list(txn.iterate_names())
     assert actual == expected
 
 
 def test_iteration_in_replacement_txn(zone):
     rds = dns.rdataset.from_text("in", "a", 300, "1.2.3.4", "5.6.7.8")
     expected = {}
     expected[(dns.name.empty, rds.rdtype, rds.covers)] = rds
     with zone.writer(True) as txn:
         txn.replace(dns.name.empty, rds)
         actual = {}
-        for (name, rdataset) in txn:
+        for name, rdataset in txn:
             actual[(name, rdataset.rdtype, rdataset.covers)] = rdataset
     assert actual == expected
 
 
 def test_replacement_commit(zone):
     rds = dns.rdataset.from_text("in", "a", 300, "1.2.3.4", "5.6.7.8")
     expected = {}
     expected[(dns.name.empty, rds.rdtype, rds.covers)] = rds
     with zone.writer(True) as txn:
         txn.replace(dns.name.empty, rds)
     with zone.reader() as txn:
         actual = {}
-        for (name, rdataset) in txn:
+        for name, rdataset in txn:
             actual[(name, rdataset.rdtype, rdataset.covers)] = rdataset
     assert actual == expected
 
 
 def test_replacement_get(zone):
     with zone.writer(True) as txn:
         rds = txn.get(dns.name.empty, "soa")
@@ -588,15 +599,15 @@
         vzone.set_max_versions(0)
 
 
 # for debugging if needed
 def _dump(zone):
     for v in zone._versions:
         print("VERSION", v.id)
-        for (name, n) in v.nodes.items():
+        for name, n in v.nodes.items():
             for rdataset in n:
                 print(rdataset.to_text(name))
 
 
 def test_vzone_open_txn_pins_versions(vzone):
     assert len(vzone._versions) == 1
     vzone.set_max_versions(None)  # unlimited!
```

### Comparing `dnspython-2.3.0rc1/tests/test_tsig.py` & `dnspython-2.4.0rc1/tests/test_tsig.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_tsigkeyring.py` & `dnspython-2.4.0rc1/tests/test_tsigkeyring.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_ttl.py` & `dnspython-2.4.0rc1/tests/test_ttl.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_update.py` & `dnspython-2.4.0rc1/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_wire.py` & `dnspython-2.4.0rc1/tests/test_wire.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/test_xfr.py` & `dnspython-2.4.0rc1/tests/test_xfr.py`

 * *Files 2% similar despite different names*

```diff
@@ -705,32 +705,14 @@
             await async_inbound_xfr()
 
         trio.run(run)
 
 except ImportError:
     pass
 
-try:
-    import curio
-
-    @pytest.mark.skipif(
-        (not _nanonameserver_available) or sys.platform == "win32",
-        reason="requires nanonameserver or is windows",
-    )
-    def test_curio_inbound_xfr():
-        dns.asyncbackend.set_default_backend("curio")
-
-        async def run():
-            await async_inbound_xfr()
-
-        curio.run(run)
-
-except ImportError:
-    pass
-
 
 class UDPXFRNanoNameserver(Server):
     def __init__(self):
         super().__init__(origin=dns.name.from_text("example"))
         self.did_truncation = False
 
     def handle(self, request):
```

### Comparing `dnspython-2.3.0rc1/tests/test_zone.py` & `dnspython-2.4.0rc1/tests/test_zone.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,22 @@
 @ 3600 IN NS ns1
 @ 3600 IN NS ns2
 bar.foo 300 IN MX 0 blaz.foo
 ns1 3600 IN A 10.0.0.1
 ns2 3600 IN A 10.0.0.2
 """
 
+example_text_output_class_before_ttl = """@ IN 3600 SOA foo bar 1 2 3 4 5
+@ 3600 NS ns1 ; no class
+@ NS ns2 ; no class or TTL, TTL inferred from prior record
+bar.foo IN 300 MX 0 blaz.foo
+ns1 IN 3600 A 10.0.0.1
+ns2 IN 3600 A 10.0.0.2
+"""
+
 example_generate = """@ 3600 IN SOA foo bar 1 2 3 4 5
 @ 3600 IN NS ns
 $GENERATE 9-12       a.$         A 10.0.0.$
 $GENERATE 80-254/173 b.${0,5,d}  A 10.0.1.$
 $GENERATE 80-254/173 c.${0,5,o}  A 10.0.2.$
 $GENERATE 80-254/173 d.${0,5,x}  A 10.0.3.$
 $GENERATE 80-254/173 e.${0,5,X}  A 10.0.4.$
@@ -301,15 +309,15 @@
     if zone.relativize:
         msg.origin = zone.origin
         soa_name = dns.name.empty
     else:
         soa_name = zone.origin
     soa = zone.find_rdataset(soa_name, "SOA")
     add_rdataset(msg, soa_name, soa)
-    for (name, rds) in zone.iterate_rdatasets():
+    for name, rds in zone.iterate_rdatasets():
         if rds.rdtype == dns.rdatatype.SOA:
             continue
         add_rdataset(msg, name, rds)
     add_rdataset(msg, soa_name, soa)
     return [msg]
 
 
@@ -499,14 +507,21 @@
                     self.assertEqual(rd, rd2)
 
     def testEqual(self):
         z1 = dns.zone.from_text(example_text, "example.", relativize=True)
         z2 = dns.zone.from_text(example_text_output, "example.", relativize=True)
         self.assertEqual(z1, z2)
 
+    def testEqualClassBeforeTTL(self):
+        z1 = dns.zone.from_text(
+            example_text_output_class_before_ttl, "example.", relativize=True
+        )
+        z2 = dns.zone.from_text(example_text_output, "example.", relativize=True)
+        self.assertEqual(z1, z2)
+
     def testNotEqual1(self):
         z1 = dns.zone.from_text(example_text, "example.", relativize=True)
         z2 = dns.zone.from_text(something_quite_similar, "example.", relativize=True)
         self.assertNotEqual(z1, z2)
 
     def testNotEqual2(self):
         z1 = dns.zone.from_text(example_text, "example.", relativize=True)
```

### Comparing `dnspython-2.3.0rc1/tests/test_zonedigest.py` & `dnspython-2.4.0rc1/tests/test_zonedigest.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/tls/ca.crt` & `dnspython-2.4.0rc1/tests/tls/ca.crt`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/tls/public.crt` & `dnspython-2.4.0rc1/tests/tls/public.crt`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/tests/util.py` & `dnspython-2.4.0rc1/tests/util.py`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/util/constants-tool` & `dnspython-2.4.0rc1/util/constants-tool`

 * *Files identical despite different names*

### Comparing `dnspython-2.3.0rc1/setup.py` & `dnspython-2.4.0rc1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,126 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dnspython
+Version: 2.4.0rc1
+Summary: DNS toolkit
+Home-page: https://www.dnspython.org
+License: ISC
+Author: Bob Halley
+Author-email: halley@dnspython.org
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: dnssec
+Provides-Extra: doh
+Provides-Extra: doq
+Provides-Extra: idna
+Provides-Extra: trio
+Provides-Extra: wmi
+Requires-Dist: aioquic (>=0.9.20) ; extra == "doq"
+Requires-Dist: cryptography (>=2.6,<42.0) ; extra == "dnssec"
+Requires-Dist: h2 (>=4.1.0) ; (python_full_version >= "3.6.2") and (extra == "doh")
+Requires-Dist: httpx (>=0.21.1) ; (python_full_version >= "3.6.2") and (extra == "doh")
+Requires-Dist: idna (>=2.1,<4.0) ; extra == "idna"
+Requires-Dist: sniffio (>=1.1,<2.0)
+Requires-Dist: trio (>=0.14,<0.23) ; extra == "trio"
+Requires-Dist: wmi (>=1.5.1,<2.0.0) ; extra == "wmi"
+Project-URL: Bug Tracker, https://github.com/rthalley/dnspython/issues
+Project-URL: Documentation, https://dnspython.readthedocs.io/en/stable/
+Project-URL: Repository, https://github.com/rthalley/dnspython.git
+Description-Content-Type: text/markdown
+
+# dnspython
+
+[![Build Status](https://github.com/rthalley/dnspython/actions/workflows/python-package.yml/badge.svg)](https://github.com/rthalley/dnspython/actions/)
+[![Documentation Status](https://readthedocs.org/projects/dnspython/badge/?version=latest)](https://dnspython.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/dnspython.svg)](https://badge.fury.io/py/dnspython)
+[![License: ISC](https://img.shields.io/badge/License-ISC-brightgreen.svg)](https://opensource.org/licenses/ISC)
+[![Coverage](https://codecov.io/github/rthalley/dnspython/coverage.svg?branch=master)](https://codecov.io/github/rthalley/dnspython)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+## INTRODUCTION
+
+dnspython is a DNS toolkit for Python. It supports almost all record types. It
+can be used for queries, zone transfers, and dynamic updates. It supports TSIG
+authenticated messages and EDNS0.
+
+dnspython provides both high and low level access to DNS. The high level classes
+perform queries for data of a given name, type, and class, and return an answer
+set. The low level classes allow direct manipulation of DNS zones, messages,
+names, and records.
+
+To see a few of the ways dnspython can be used, look in the `examples/`
+directory.
+
+dnspython is a utility to work with DNS, `/etc/hosts` is thus not used. For
+simple forward DNS lookups, it's better to use `socket.getaddrinfo()` or
+`socket.gethostbyname()`.
+
+dnspython originated at Nominum where it was developed
+to facilitate the testing of DNS software.
+
+## ABOUT THIS RELEASE
+
+This is dnspython 2.4.0rc1.
+Please read
+[What's New](https://dnspython.readthedocs.io/en/latest/whatsnew.html) for
+information about the changes in this release.
+
+## INSTALLATION
+
+* Many distributions have dnspython packaged for you, so you should
+  check there first.
+* To use a wheel downloaded from PyPi, run:
+
+    pip install dnspython
+
+* To install from the source code, go into the top-level of the source code
+  and run:
+
+    pip install --upgrade pip build
+    python -m build
+    pip install dist/*.whl
+
+* To install the latest from the master branch, run `pip install git+https://github.com/rthalley/dnspython.git`
+
+Dnspython's default installation does not depend on any modules other than
+those in the Python standard library.  To use some features, additional modules
+must be installed.  For convenience, pip options are defined for the
+requirements.
+
+If you want to use DNS-over-HTTPS, run
+`pip install dnspython[doh]`.
+
+If you want to use DNSSEC functionality, run
+`pip install dnspython[dnssec]`.
+
+If you want to use internationalized domain names (IDNA)
+functionality, you must run
+`pip install dnspython[idna]`
+
+If you want to use the Trio asynchronous I/O package, run
+`pip install dnspython[trio]`.
+
+If you want to use WMI on Windows to determine the active DNS settings
+instead of the default registry scanning method, run
+`pip install dnspython[wmi]`.
+
+If you want to try the experimental DNS-over-QUIC code, run
+`pip install dnspython[doq]`.
+
+Note that you can install any combination of the above, e.g.:
+`pip install dnspython[doh,dnssec,idna]`
+
+### Notices
+
+Python 2.x support ended with the release of 1.16.0.  Dnspython 2.0.0 through
+2.2.x support Python 3.6 and later.  For dnspython 2.3.x, the minimum
+supported Python version is 3.7, and for 2.4.x the minimum supported verison is 3.8.
+We plan to align future support with the lifetime of the Python 3 versions.
 
-packages = \
-['dns',
- 'dns.quic',
- 'dns.rdtypes',
- 'dns.rdtypes.ANY',
- 'dns.rdtypes.CH',
- 'dns.rdtypes.IN']
-
-package_data = \
-{'': ['*']}
-
-extras_require = \
-{'curio': ['curio>=1.2,<2.0', 'sniffio>=1.1,<2.0'],
- 'dnssec': ['cryptography>=2.6,<39.0'],
- 'doh': ['requests-toolbelt>=0.9.1,<0.11.0', 'requests>=2.23.0,<3.0.0'],
- 'doh:python_full_version >= "3.6.2"': ['httpx>=0.21.1', 'h2>=4.1.0'],
- 'doq': ['aioquic>=0.9.20'],
- 'idna': ['idna>=2.1,<4.0'],
- 'trio': ['trio>=0.14,<0.23'],
- 'wmi': ['wmi>=1.5.1,<2.0.0']}
-
-setup_kwargs = {
-    'name': 'dnspython',
-    'version': '2.3.0rc1',
-    'description': 'DNS toolkit',
-    'long_description': "# dnspython\n\n[![Build Status](https://github.com/rthalley/dnspython/actions/workflows/python-package.yml/badge.svg)](https://github.com/rthalley/dnspython/actions/)\n[![Documentation Status](https://readthedocs.org/projects/dnspython/badge/?version=latest)](https://dnspython.readthedocs.io/en/latest/?badge=latest)\n[![PyPI version](https://badge.fury.io/py/dnspython.svg)](https://badge.fury.io/py/dnspython)\n[![License: ISC](https://img.shields.io/badge/License-ISC-brightgreen.svg)](https://opensource.org/licenses/ISC)\n[![Coverage](https://codecov.io/github/rthalley/dnspython/coverage.svg?branch=master)](https://codecov.io/github/rthalley/dnspython)\n[![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/rthalley/dnspython)](https://lgtm.com/projects/g/rthalley/dnspython/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n## INTRODUCTION\n\ndnspython is a DNS toolkit for Python. It supports almost all record types. It\ncan be used for queries, zone transfers, and dynamic updates. It supports TSIG\nauthenticated messages and EDNS0.\n\ndnspython provides both high and low level access to DNS. The high level classes\nperform queries for data of a given name, type, and class, and return an answer\nset. The low level classes allow direct manipulation of DNS zones, messages,\nnames, and records.\n\nTo see a few of the ways dnspython can be used, look in the `examples/`\ndirectory.\n\ndnspython is a utility to work with DNS, `/etc/hosts` is thus not used. For\nsimple forward DNS lookups, it's better to use `socket.getaddrinfo()` or\n`socket.gethostbyname()`.\n\ndnspython originated at Nominum where it was developed\nto facilitate the testing of DNS software.\n\n## ABOUT THIS RELEASE\n\nThis is dnspython 2.3.0rc1.\nPlease read\n[What's New](https://dnspython.readthedocs.io/en/latest/whatsnew.html) for\ninformation about the changes in this release.\n\n## INSTALLATION\n\n* Many distributions have dnspython packaged for you, so you should\n  check there first.\n* If you have pip installed, you can do `pip install dnspython`\n* If not just download the source file and unzip it, then run\n  `sudo python setup.py install`\n* To install the latest from the master branch, run `pip install git+https://github.com/rthalley/dnspython.git`\n\nDnspython's default installation does not depend on any modules other than\nthose in the Python standard library.  To use some features, additional modules\nmust be installed.  For convenience, pip options are defined for the\nrequirements.\n\nIf you want to use DNS-over-HTTPS, run\n`pip install dnspython[doh]`.\n\nIf you want to use DNSSEC functionality, run\n`pip install dnspython[dnssec]`.\n\nIf you want to use internationalized domain names (IDNA)\nfunctionality, you must run\n`pip install dnspython[idna]`\n\nIf you want to use the Trio asynchronous I/O package, run\n`pip install dnspython[trio]`.\n\nIf you want to use the Curio asynchronous I/O package, run\n`pip install dnspython[curio]`.\n\nIf you want to use WMI on Windows to determine the active DNS settings\ninstead of the default registry scanning method, run\n`pip install dnspython[wmi]`.\n\nIf you want to try the experimental DNS-over-QUIC code, run\n`pip install dnspython[doq]`.\n\nNote that you can install any combination of the above, e.g.:\n`pip install dnspython[doh,dnssec,idna]`\n\n### Notices\n\nPython 2.x support ended with the release of 1.16.0.  Dnspython 2.0.0 through\n2.2.x support Python 3.6 and later.  As of dnspython 2.3.0, the minimum\nsupported Python version will be 3.7.  We plan to align future support with the\nlifetime of the Python 3 versions.\n\nDocumentation has moved to\n[dnspython.readthedocs.io](https://dnspython.readthedocs.io).\n",
-    'author': 'Bob Halley',
-    'author_email': 'halley@dnspython.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://www.dnspython.org',
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+Documentation has moved to
+[dnspython.readthedocs.io](https://dnspython.readthedocs.io).
 
-
-setup(**setup_kwargs)
```

