# Comparing `tmp/nxstools-3.8.0.tar.gz` & `tmp/nxstools-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nxstools-3.8.0.tar", last modified: Fri May 21 09:52:07 2021, max compression
+gzip compressed data, was "dist/nxstools-3.9.0.tar", last modified: Tue Jun  8 08:46:59 2021, max compression
```

## Comparing `nxstools-3.8.0.tar` & `nxstools-3.9.0.tar`

### file list

```diff
@@ -1,168 +1,180 @@
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2021-05-21 09:52:07.000000 nxstools-3.8.0/
--rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2014-03-04 09:18:25.000000 nxstools-3.8.0/COPYRIGHT
--rw-r--r--   0 jkotan   (15949) irc         (39)      203 2016-11-17 08:47:01.000000 nxstools-3.8.0/MANIFEST.in
--rw-r--r--   0 jkotan   (15949) irc         (39)     5126 2021-05-21 09:52:07.000000 nxstools-3.8.0/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)     2918 2019-10-11 17:04:12.000000 nxstools-3.8.0/README.rst
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2021-05-21 09:52:07.000000 nxstools-3.8.0/man/
--rw-r--r--   0 jkotan   (15949) irc         (39)    11401 2021-05-21 09:51:41.000000 nxstools-3.8.0/man/nxscollect.1
--rw-r--r--   0 jkotan   (15949) irc         (39)     4983 2021-05-21 09:51:41.000000 nxstools-3.8.0/man/nxsconfig.1
--rw-r--r--   0 jkotan   (15949) irc         (39)    18372 2021-05-21 09:51:41.000000 nxstools-3.8.0/man/nxscreate.1
--rw-r--r--   0 jkotan   (15949) irc         (39)     2287 2021-05-21 09:51:41.000000 nxstools-3.8.0/man/nxsdata.1
--rw-r--r--   0 jkotan   (15949) irc         (39)     6583 2021-05-21 09:51:41.000000 nxstools-3.8.0/man/nxsetup.1
--rw-r--r--   0 jkotan   (15949) irc         (39)     3071 2021-05-21 09:51:41.000000 nxstools-3.8.0/man/nxsfileinfo.1
--rw-r--r--   0 jkotan   (15949) irc         (39)   272845 2021-05-21 09:51:41.000000 nxstools-3.8.0/man/nxstools.1
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       73 2016-03-02 14:46:03.000000 nxstools-3.8.0/nxscollect
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       71 2016-11-02 14:11:38.000000 nxstools-3.8.0/nxsconfig
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       72 2016-11-08 13:51:28.000000 nxstools-3.8.0/nxscreate
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       67 2016-04-21 09:21:42.000000 nxstools-3.8.0/nxsdata
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       67 2019-02-22 09:13:56.000000 nxstools-3.8.0/nxsetup
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       75 2016-11-08 13:51:28.000000 nxstools-3.8.0/nxsfileinfo
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2021-05-21 09:52:07.000000 nxstools-3.8.0/nxstools/
--rw-r--r--   0 jkotan   (15949) irc         (39)      921 2019-02-06 13:31:32.000000 nxstools-3.8.0/nxstools/__init__.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3423 2021-01-18 12:05:16.000000 nxstools-3.8.0/nxstools/filenamegenerator.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    28443 2021-04-08 11:45:01.000000 nxstools-3.8.0/nxstools/filewriter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    55982 2021-04-08 11:45:01.000000 nxstools-3.8.0/nxstools/h5cppwriter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    45483 2021-04-08 11:45:01.000000 nxstools-3.8.0/nxstools/h5pywriter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3263 2019-02-06 13:31:32.000000 nxstools-3.8.0/nxstools/nxsargparser.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    64920 2021-04-15 09:36:00.000000 nxstools-3.8.0/nxstools/nxscollect.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    61405 2021-05-04 14:44:37.000000 nxstools-3.8.0/nxstools/nxsconfig.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    55939 2021-04-20 05:41:15.000000 nxstools-3.8.0/nxstools/nxscreate.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    74548 2021-04-28 07:36:39.000000 nxstools-3.8.0/nxstools/nxscreator.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    11192 2019-02-06 13:31:32.000000 nxstools-3.8.0/nxstools/nxsdata.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    14561 2021-02-25 11:17:48.000000 nxstools-3.8.0/nxstools/nxsdevicetools.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    55814 2021-04-13 16:06:43.000000 nxstools-3.8.0/nxstools/nxsetup.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    17779 2021-02-12 09:59:39.000000 nxstools-3.8.0/nxstools/nxsfileinfo.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     8150 2021-02-12 09:59:39.000000 nxstools-3.8.0/nxstools/nxsfileparser.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    35155 2021-05-04 14:44:37.000000 nxstools-3.8.0/nxstools/nxsparser.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    24266 2021-02-22 12:08:03.000000 nxstools-3.8.0/nxstools/nxsxml.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2021-05-21 09:52:07.000000 nxstools-3.8.0/nxstools/pyeval/
--rw-r--r--   0 jkotan   (15949) irc         (39)      848 2021-05-17 13:16:49.000000 nxstools-3.8.0/nxstools/pyeval/__init__.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1922 2021-05-19 17:11:12.000000 nxstools-3.8.0/nxstools/pyeval/absorber.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3906 2021-05-17 13:16:49.000000 nxstools-3.8.0/nxstools/pyeval/beamtimeid.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3224 2021-05-21 09:01:40.000000 nxstools-3.8.0/nxstools/pyeval/datasignal.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2061 2021-05-19 17:11:12.000000 nxstools-3.8.0/nxstools/pyeval/dcm.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     6705 2021-05-17 13:16:49.000000 nxstools-3.8.0/nxstools/pyeval/lambdavds.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1897 2021-05-19 17:11:12.000000 nxstools-3.8.0/nxstools/pyeval/mssar.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1551 2021-05-19 17:11:12.000000 nxstools-3.8.0/nxstools/pyeval/qbpm.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      911 2021-05-21 08:27:26.000000 nxstools-3.8.0/nxstools/release.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2021-05-21 09:52:07.000000 nxstools-3.8.0/nxstools/xmltemplates/
--rw-r--r--   0 jkotan   (15949) irc         (39)    56044 2021-05-21 08:27:26.000000 nxstools-3.8.0/nxstools/xmltemplates/__init__.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2183 2020-02-06 16:05:03.000000 nxstools-3.8.0/nxstools/xmltemplates/absorber.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      272 2021-05-19 17:11:12.000000 nxstools-3.8.0/nxstools/xmltemplates/absorber_foil.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      287 2021-05-19 17:11:12.000000 nxstools-3.8.0/nxstools/xmltemplates/absorber_thickness.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1995 2020-01-17 09:16:53.000000 nxstools-3.8.0/nxstools/xmltemplates/beamstop.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      146 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/beamtime_id.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      453 2021-05-17 13:16:49.000000 nxstools-3.8.0/nxstools/xmltemplates/beamtimeid.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      258 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/beamtimeid.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     6163 2020-02-06 16:05:03.000000 nxstools-3.8.0/nxstools/xmltemplates/chcut.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      239 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/chcut_crystal.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      337 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/chcut_unitcalibration.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      156 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/chemical_formula.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)       96 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/collect2.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      119 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/collect3.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      143 2020-02-06 16:05:03.000000 nxstools-3.8.0/nxstools/xmltemplates/collect4.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      166 2020-02-06 16:05:03.000000 nxstools-3.8.0/nxstools/xmltemplates/collect5.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      189 2020-02-06 16:05:03.000000 nxstools-3.8.0/nxstools/xmltemplates/collect6.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      213 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/common2_common.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      236 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/common3_common.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     3334 2021-04-15 09:36:00.000000 nxstools-3.8.0/nxstools/xmltemplates/dalsa.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1008 2021-04-22 09:24:28.000000 nxstools-3.8.0/nxstools/xmltemplates/dalsa_external_data.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      696 2021-04-13 14:56:19.000000 nxstools-3.8.0/nxstools/xmltemplates/dalsa_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      525 2021-04-28 11:00:14.000000 nxstools-3.8.0/nxstools/xmltemplates/dalsavds_nrexposedframes_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      506 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/datasignal.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)    11075 2020-02-06 16:05:03.000000 nxstools-3.8.0/nxstools/xmltemplates/dcm.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      230 2021-05-19 17:11:12.000000 nxstools-3.8.0/nxstools/xmltemplates/dcm_crystal.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      236 2021-05-19 17:11:12.000000 nxstools-3.8.0/nxstools/xmltemplates/dcm_reflection.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      246 2021-05-19 17:11:12.000000 nxstools-3.8.0/nxstools/xmltemplates/dcm_unitcalibration.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      189 2019-09-25 14:14:28.000000 nxstools-3.8.0/nxstools/xmltemplates/default.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2247 2021-02-12 09:59:39.000000 nxstools-3.8.0/nxstools/xmltemplates/defaultinstrument.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      428 2019-09-25 14:15:25.000000 nxstools-3.8.0/nxstools/xmltemplates/defaultsample.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      392 2021-05-21 08:27:26.000000 nxstools-3.8.0/nxstools/xmltemplates/defaultsignal.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1183 2021-04-28 08:22:24.000000 nxstools-3.8.0/nxstools/xmltemplates/detectorlive.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2356 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/eigerdectris.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      307 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/eigerdectris_description_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      429 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/eigerdectris_stepindex.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2491 2021-02-12 09:59:39.000000 nxstools-3.8.0/nxstools/xmltemplates/eigerdectris_triggermode_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)       49 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/empty.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      228 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/end_time.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      909 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/keithley.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     4685 2021-04-14 10:31:17.000000 nxstools-3.8.0/nxstools/xmltemplates/lambda.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     4955 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/lambda2m.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      535 2021-04-15 09:36:00.000000 nxstools-3.8.0/nxstools/xmltemplates/lambda2m_m1_external_data.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      348 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/lambda2m_m1_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      535 2021-04-15 09:36:00.000000 nxstools-3.8.0/nxstools/xmltemplates/lambda2m_m2_external_data.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      348 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/lambda2m_m2_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      535 2021-04-15 09:36:00.000000 nxstools-3.8.0/nxstools/xmltemplates/lambda2m_m3_external_data.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      348 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/lambda2m_m3_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1160 2021-04-15 09:36:00.000000 nxstools-3.8.0/nxstools/xmltemplates/lambda_external_data.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      345 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/lambda_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     4586 2021-04-20 19:07:23.000000 nxstools-3.8.0/nxstools/xmltemplates/lambdavds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      347 2021-05-17 13:16:49.000000 nxstools-3.8.0/nxstools/xmltemplates/lambdavds_framenumbers_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      342 2021-04-20 19:07:23.000000 nxstools-3.8.0/nxstools/xmltemplates/lambdavds_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      347 2021-05-17 13:16:49.000000 nxstools-3.8.0/nxstools/xmltemplates/lambdavds_savefilename_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      911 2021-05-21 09:51:13.000000 nxstools-3.8.0/nxstools/xmltemplates/lambdavds_triggermode_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     4056 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/limaccd.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      411 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/limaccd_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      467 2021-04-29 09:35:31.000000 nxstools-3.8.0/nxstools/xmltemplates/limaccd_filestartnum_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1337 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/limaccd_postrun.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      270 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/limaccd_xpixelsize.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      270 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/limaccd_ypixelsize.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     3223 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/maia.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1313 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/maiadimension.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1170 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/maiaflux.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1502 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/marccd.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      557 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/marccd_postrun.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1628 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/mcaxia.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      263 2021-05-19 17:11:12.000000 nxstools-3.8.0/nxstools/xmltemplates/msnsar_env.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      262 2021-05-19 17:11:12.000000 nxstools-3.8.0/nxstools/xmltemplates/mssar_env.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     3353 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/mythen.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     3563 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/mythen2.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      279 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/mythen_filestartnumber.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      986 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/mythen_postrun.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      264 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/nexdatas_configuration.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      212 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/nexdatas_version.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     3755 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/pco.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      265 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/pco_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      420 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/pco_filestartnum_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1226 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/pco_postrun.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     4332 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/perkinelmerdetector.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      259 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/perkinelmerdetector_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      328 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/perkinelmerdetector_fileindex_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1157 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/perkinelmerdetector_postrun.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2493 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/pilatus.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      270 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/pilatus100k_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      268 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/pilatus1m_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      268 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/pilatus2m_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      270 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/pilatus300k_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      268 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/pilatus6m_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      265 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/pilatus_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      420 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/pilatus_filestartnum_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2473 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/pilatus_mxparameters_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1227 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/pilatus_postrun.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2028 2020-05-05 09:17:06.000000 nxstools-3.8.0/nxstools/xmltemplates/pinhole.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      560 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/pointdet.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2186 2021-02-22 12:08:03.000000 nxstools-3.8.0/nxstools/xmltemplates/qbpm.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      265 2021-05-19 17:11:12.000000 nxstools-3.8.0/nxstools/xmltemplates/qbpm_foil.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      207 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/sample_name.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      596 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/samplehkl.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      311 2020-01-15 17:35:29.000000 nxstools-3.8.0/nxstools/xmltemplates/sardanaenvironment.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      146 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/signal_axes.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      146 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/signal_name.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      393 2021-05-21 08:27:26.000000 nxstools-3.8.0/nxstools/xmltemplates/signalname.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     4050 2020-05-05 09:17:06.000000 nxstools-3.8.0/nxstools/xmltemplates/slit.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      920 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/source.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      209 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/start_time.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1395 2019-09-25 10:30:34.000000 nxstools-3.8.0/nxstools/xmltemplates/tangovimba.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      957 2021-04-15 09:36:00.000000 nxstools-3.8.0/nxstools/xmltemplates/tangovimba_external_data.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      696 2021-02-03 13:50:19.000000 nxstools-3.8.0/nxstools/xmltemplates/tangovimba_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      134 2019-09-25 10:15:20.000000 nxstools-3.8.0/nxstools/xmltemplates/title.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2369 2020-02-06 16:05:03.000000 nxstools-3.8.0/nxstools/xmltemplates/undulator.xml
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2021-05-21 09:52:07.000000 nxstools-3.8.0/nxstools.egg-info/
--rw-r--r--   0 jkotan   (15949) irc         (39)     5126 2021-05-21 09:52:07.000000 nxstools-3.8.0/nxstools.egg-info/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)     5812 2021-05-21 09:52:07.000000 nxstools-3.8.0/nxstools.egg-info/SOURCES.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2021-05-21 09:52:07.000000 nxstools-3.8.0/nxstools.egg-info/dependency_links.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2019-10-10 18:35:39.000000 nxstools-3.8.0/nxstools.egg-info/not-zip-safe
--rw-r--r--   0 jkotan   (15949) irc         (39)       45 2021-05-21 09:52:07.000000 nxstools-3.8.0/nxstools.egg-info/requires.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        9 2021-05-21 09:52:07.000000 nxstools-3.8.0/nxstools.egg-info/top_level.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)      201 2021-05-21 09:52:07.000000 nxstools-3.8.0/setup.cfg
--rw-r--r--   0 jkotan   (15949) irc         (39)     4372 2021-05-17 13:16:49.000000 nxstools-3.8.0/setup.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2021-06-08 08:46:59.000000 nxstools-3.9.0/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2014-03-04 09:18:25.000000 nxstools-3.9.0/COPYRIGHT
+-rw-r--r--   0 jkotan   (15949) irc         (39)      203 2016-11-17 08:47:01.000000 nxstools-3.9.0/MANIFEST.in
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5126 2021-06-08 08:46:59.000000 nxstools-3.9.0/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2918 2019-10-11 17:04:12.000000 nxstools-3.9.0/README.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2021-06-08 08:46:59.000000 nxstools-3.9.0/man/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11288 2021-06-08 08:44:41.000000 nxstools-3.9.0/man/nxscollect.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4981 2021-06-08 08:44:41.000000 nxstools-3.9.0/man/nxsconfig.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)    18340 2021-06-08 08:44:41.000000 nxstools-3.9.0/man/nxscreate.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2287 2021-06-08 08:44:41.000000 nxstools-3.9.0/man/nxsdata.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6583 2021-06-08 08:44:41.000000 nxstools-3.9.0/man/nxsetup.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3067 2021-06-08 08:44:41.000000 nxstools-3.9.0/man/nxsfileinfo.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)   272377 2021-06-08 08:44:41.000000 nxstools-3.9.0/man/nxstools.1
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       73 2016-03-02 14:46:03.000000 nxstools-3.9.0/nxscollect
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       71 2016-11-02 14:11:38.000000 nxstools-3.9.0/nxsconfig
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       72 2016-11-08 13:51:28.000000 nxstools-3.9.0/nxscreate
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       67 2016-04-21 09:21:42.000000 nxstools-3.9.0/nxsdata
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       67 2019-02-22 09:13:56.000000 nxstools-3.9.0/nxsetup
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       75 2016-11-08 13:51:28.000000 nxstools-3.9.0/nxsfileinfo
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2021-06-08 08:46:59.000000 nxstools-3.9.0/nxstools/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      921 2019-02-06 13:31:32.000000 nxstools-3.9.0/nxstools/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3423 2021-01-18 12:05:16.000000 nxstools-3.9.0/nxstools/filenamegenerator.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    28443 2021-04-08 11:45:01.000000 nxstools-3.9.0/nxstools/filewriter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    55982 2021-04-08 11:45:01.000000 nxstools-3.9.0/nxstools/h5cppwriter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    45483 2021-04-08 11:45:01.000000 nxstools-3.9.0/nxstools/h5pywriter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3263 2019-02-06 13:31:32.000000 nxstools-3.9.0/nxstools/nxsargparser.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    64920 2021-04-15 09:36:00.000000 nxstools-3.9.0/nxstools/nxscollect.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    61405 2021-05-04 14:44:37.000000 nxstools-3.9.0/nxstools/nxsconfig.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    55939 2021-04-20 05:41:15.000000 nxstools-3.9.0/nxstools/nxscreate.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    74548 2021-04-28 07:36:39.000000 nxstools-3.9.0/nxstools/nxscreator.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11192 2019-02-06 13:31:32.000000 nxstools-3.9.0/nxstools/nxsdata.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    14561 2021-02-25 11:17:48.000000 nxstools-3.9.0/nxstools/nxsdevicetools.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    55814 2021-04-13 16:06:43.000000 nxstools-3.9.0/nxstools/nxsetup.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    17779 2021-02-12 09:59:39.000000 nxstools-3.9.0/nxstools/nxsfileinfo.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     8150 2021-02-12 09:59:39.000000 nxstools-3.9.0/nxstools/nxsfileparser.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35155 2021-05-04 14:44:37.000000 nxstools-3.9.0/nxstools/nxsparser.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    24266 2021-02-22 12:08:03.000000 nxstools-3.9.0/nxstools/nxsxml.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2021-06-08 08:46:59.000000 nxstools-3.9.0/nxstools/pyeval/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      848 2021-05-17 13:16:49.000000 nxstools-3.9.0/nxstools/pyeval/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1922 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/pyeval/absorber.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3906 2021-05-17 13:16:49.000000 nxstools-3.9.0/nxstools/pyeval/beamtimeid.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3234 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/common.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2307 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/dalsa.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3224 2021-05-21 09:01:40.000000 nxstools-3.9.0/nxstools/pyeval/datasignal.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2063 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/dcm.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4551 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/eigerdectris.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6553 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/lambdavds.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2876 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/limaccd.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3894 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/lmbd.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1722 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/marccd.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1897 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/pyeval/mssar.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2279 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/mythen.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2629 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/pco.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2975 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/pe.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5841 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/pilatus.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1551 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/pyeval/qbpm.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2253 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/tangovimba.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      911 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/release.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2021-06-08 08:46:59.000000 nxstools-3.9.0/nxstools/xmltemplates/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    56094 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2183 2020-02-06 16:05:03.000000 nxstools-3.9.0/nxstools/xmltemplates/absorber.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      272 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/xmltemplates/absorber_foil.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      287 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/xmltemplates/absorber_thickness.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1995 2020-01-17 09:16:53.000000 nxstools-3.9.0/nxstools/xmltemplates/beamstop.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      146 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/beamtime_id.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      453 2021-05-17 13:16:49.000000 nxstools-3.9.0/nxstools/xmltemplates/beamtimeid.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      258 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/beamtimeid.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6163 2020-02-06 16:05:03.000000 nxstools-3.9.0/nxstools/xmltemplates/chcut.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      239 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/chcut_crystal.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      337 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/chcut_unitcalibration.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      156 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/chemical_formula.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)       96 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/collect2.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      119 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/collect3.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      143 2020-02-06 16:05:03.000000 nxstools-3.9.0/nxstools/xmltemplates/collect4.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      166 2020-02-06 16:05:03.000000 nxstools-3.9.0/nxstools/xmltemplates/collect5.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      189 2020-02-06 16:05:03.000000 nxstools-3.9.0/nxstools/xmltemplates/collect6.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      213 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/common2_common.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      236 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/common3_common.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3334 2021-04-15 09:36:00.000000 nxstools-3.9.0/nxstools/xmltemplates/dalsa.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      463 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/dalsa_external_data.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      598 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/dalsa_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      525 2021-04-28 11:00:14.000000 nxstools-3.9.0/nxstools/xmltemplates/dalsavds_nrexposedframes_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      506 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/datasignal.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11075 2020-02-06 16:05:03.000000 nxstools-3.9.0/nxstools/xmltemplates/dcm.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      230 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/xmltemplates/dcm_crystal.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      236 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/xmltemplates/dcm_reflection.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      246 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/xmltemplates/dcm_unitcalibration.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      189 2019-09-25 14:14:28.000000 nxstools-3.9.0/nxstools/xmltemplates/default.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2247 2021-02-12 09:59:39.000000 nxstools-3.9.0/nxstools/xmltemplates/defaultinstrument.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      428 2019-09-25 14:15:25.000000 nxstools-3.9.0/nxstools/xmltemplates/defaultsample.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      392 2021-05-21 08:27:26.000000 nxstools-3.9.0/nxstools/xmltemplates/defaultsignal.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1183 2021-04-28 08:22:24.000000 nxstools-3.9.0/nxstools/xmltemplates/detectorlive.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2356 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/eigerdectris.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      319 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/eigerdectris_description_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      375 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/eigerdectris_stepindex.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      609 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/eigerdectris_triggermode_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)       49 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/empty.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      228 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/end_time.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      909 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/keithley.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4685 2021-04-14 10:31:17.000000 nxstools-3.9.0/nxstools/xmltemplates/lambda.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4955 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/lambda2m.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      481 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/lambda2m_m1_external_data.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      348 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/lambda2m_m1_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      481 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/lambda2m_m2_external_data.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      348 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/lambda2m_m2_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      481 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/lambda2m_m3_external_data.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      348 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/lambda2m_m3_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      599 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/lambda_external_data.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      345 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/lambda_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4643 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/lambdavds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      307 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/lambdavds_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      342 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/lambdavds_framenumbers_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      342 2021-04-20 19:07:23.000000 nxstools-3.9.0/nxstools/xmltemplates/lambdavds_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      339 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/lambdavds_savefilename_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      911 2021-05-21 09:51:13.000000 nxstools-3.9.0/nxstools/xmltemplates/lambdavds_triggermode_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4056 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/limaccd.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      413 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/limaccd_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      421 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/limaccd_filestartnum_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      679 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/limaccd_postrun.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      295 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/limaccd_xpixelsize.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      295 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/limaccd_ypixelsize.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3223 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/maia.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1313 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/maiadimension.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1170 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/maiaflux.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1502 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/marccd.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      431 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/marccd_postrun.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1628 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/mcaxia.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      263 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/xmltemplates/msnsar_env.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      262 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/xmltemplates/mssar_env.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3353 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/mythen.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3563 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/mythen2.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      279 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/mythen_filestartnumber.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      431 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/mythen_postrun.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      264 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/nexdatas_configuration.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      212 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/nexdatas_version.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3755 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/pco.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      278 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pco_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      391 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pco_filestartnum_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      549 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pco_postrun.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4332 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/perkinelmerdetector.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      270 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/perkinelmerdetector_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      313 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/perkinelmerdetector_fileindex_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      494 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/perkinelmerdetector_postrun.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2493 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/pilatus.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      278 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pilatus100k_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      276 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pilatus1m_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      276 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pilatus2m_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      278 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pilatus300k_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      276 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pilatus6m_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      278 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pilatus_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      400 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pilatus_filestartnum_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      393 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pilatus_mxparameters_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      558 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pilatus_postrun.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2028 2020-05-05 09:17:06.000000 nxstools-3.9.0/nxstools/xmltemplates/pinhole.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      560 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/pointdet.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2186 2021-02-22 12:08:03.000000 nxstools-3.9.0/nxstools/xmltemplates/qbpm.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      265 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/xmltemplates/qbpm_foil.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      207 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/sample_name.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      596 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/samplehkl.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      311 2020-01-15 17:35:29.000000 nxstools-3.9.0/nxstools/xmltemplates/sardanaenvironment.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      146 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/signal_axes.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      146 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/signal_name.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      393 2021-05-21 08:27:26.000000 nxstools-3.9.0/nxstools/xmltemplates/signalname.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4050 2020-05-05 09:17:06.000000 nxstools-3.9.0/nxstools/xmltemplates/slit.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      920 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/source.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      209 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/start_time.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1395 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/tangovimba.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      503 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/tangovimba_external_data.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      598 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/tangovimba_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      134 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/title.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2369 2020-02-06 16:05:03.000000 nxstools-3.9.0/nxstools/xmltemplates/undulator.xml
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2021-06-08 08:46:59.000000 nxstools-3.9.0/nxstools.egg-info/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5126 2021-06-08 08:46:59.000000 nxstools-3.9.0/nxstools.egg-info/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6151 2021-06-08 08:46:59.000000 nxstools-3.9.0/nxstools.egg-info/SOURCES.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2021-06-08 08:46:59.000000 nxstools-3.9.0/nxstools.egg-info/dependency_links.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2019-10-10 18:35:39.000000 nxstools-3.9.0/nxstools.egg-info/not-zip-safe
+-rw-r--r--   0 jkotan   (15949) irc         (39)       45 2021-06-08 08:46:59.000000 nxstools-3.9.0/nxstools.egg-info/requires.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        9 2021-06-08 08:46:59.000000 nxstools-3.9.0/nxstools.egg-info/top_level.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)      201 2021-06-08 08:46:59.000000 nxstools-3.9.0/setup.cfg
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4372 2021-05-17 13:16:49.000000 nxstools-3.9.0/setup.py
```

### Comparing `nxstools-3.8.0/COPYRIGHT` & `nxstools-3.9.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/PKG-INFO` & `nxstools-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: nxstools
-Version: 3.8.0
+Version: 3.9.0
 Summary: Configuration tools for NeXDaTaS Tango Servers
 Home-page: http://github.com/nexdatas/tools
 Author: ('Jan Kotanski, Eugen Wintersberger , Halil Pasic',)
 Author-email: jankotan@gmail.com, eugen.wintersberger@gmail.com, halil.pasic@gmail.com
 Maintainer: Jan Kotanski, Eugen Wintersberger , Halil Pasic
 Maintainer-email: jankotan@gmail.com, eugen.wintersberger@gmail.com, halil.pasic@gmail.com
 License: ('GNU GENERAL PUBLIC LICENSE, version 3',)
```

### Comparing `nxstools-3.8.0/README.rst` & `nxstools-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/man/nxsconfig.1` & `nxstools-3.9.0/man/nxsconfig.1`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "NXSCONFIG" "1" "May 21, 2021" "3.8" "NXSTools"
+.TH "NXSCONFIG" "1" "Jun 08, 2021" "3.9" "NXSTools"
 .SH NAME
 nxsconfig \- read NeXus Configuration Server settings
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -58,78 +58,78 @@
 .TP
 .B list \-d [\-s <config_server>] [\-n]
 list names of available datasources
 .TP
 .B list \-r [\-s <config_server>] [\-n]
 list names of available profiles
 .TP
-.B show [\-s <config_server>] [\-m] [\-o <dir>] component_name1 component_name2 ...
+.B show [\-s <config_server>] [\-m] [\-o <dir>] component_name1 component_name2 …
 show components with given names
 .TP
-.B show \-d [\-s <config_server>]  [\-o <dir>] dsource_name1 dsource_name2 ...
+.B show \-d [\-s <config_server>]  [\-o <dir>] dsource_name1 dsource_name2 …
 show datasources with given names
 .TP
-.B show \-r [\-s <config_server>]  [\-o <dir>] profile_name1 profile_name2 ...
+.B show \-r [\-s <config_server>]  [\-o <dir>] profile_name1 profile_name2 …
 show profiles with given names
 .TP
-.B upload [\-s <config_server>] [\-m] [\-i <dir>] [\-f] component_name1 component_name2 ...
+.B upload [\-s <config_server>] [\-m] [\-i <dir>] [\-f] component_name1 component_name2 …
 load components from given files
 .TP
-.B upload \-d [\-s <config_server>]  [\-i <dir>] [\-f] dsource_name1 dsource_name2 ...
+.B upload \-d [\-s <config_server>]  [\-i <dir>] [\-f] dsource_name1 dsource_name2 …
 load datasources from given files
 .TP
-.B upload \-r [\-s <config_server>]  [\-i <dir>] [\-f] profile_name1 profile_name2 ...
+.B upload \-r [\-s <config_server>]  [\-i <dir>] [\-f] profile_name1 profile_name2 …
 load profiles from given files
 .TP
-.B get [\-s <config_server>]  [\-n] component_name1 component_name2 ...
+.B get [\-s <config_server>]  [\-n] component_name1 component_name2 …
 get merged configuration of components
 .TP
-.B delete [\-s <config_server>] [\-f] component_name1 component_name2 ...
+.B delete [\-s <config_server>] [\-f] component_name1 component_name2 …
 delete components with given names
 .TP
-.B delete \-d [\-s <config_server>] [\-f] dsource_name1 dsource_name2 ...
+.B delete \-d [\-s <config_server>] [\-f] dsource_name1 dsource_name2 …
 delete datasources with given names
 .TP
-.B delete \-r [\-s <config_server>] [\-f] profile_name1 profile_name2 ...
+.B delete \-r [\-s <config_server>] [\-f] profile_name1 profile_name2 …
 delete profiles with given names
 .TP
-.B sources [\-s <config_server>] [\-m] [\-n] component_name1 component_name2 ...
+.B sources [\-s <config_server>] [\-m] [\-n] component_name1 component_name2 …
 get a list of component datasources
 .TP
-.B components [\-s <config_server>] [\-n] component_name1 component_name2 ...
+.B components [\-s <config_server>] [\-n] component_name1 component_name2 …
 get a list of dependent components
 .TP
-.B variables [\-s <config_server>] [\-m] [\-n] component_name1 component_name2 ...
+.B variables [\-s <config_server>] [\-m] [\-n] component_name1 component_name2 …
 get a list of component variables
 .TP
 .B data [\-s <config_server>] json_data
 set values of component variables
 .TP
 .B record [\-s <config_server>] [\-n] component_name1
 get a list of datasource record names from component
 .TP
 .B record \-d [\-s <config_server>] [\-n] datasource_name1
 get a list of datasource record names
 .TP
 .B servers [\-s <config_server/host>] [\-n]
 get lists of configuration servers from the current tango host
 .TP
-.B describe [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 ...
+.B describe [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 …
 show all parameters of given components
 .TP
-.B describe|info \-d [\-s <config_server>] [\-n] dsource_name1 dsource_name2 ...
+.B describe|info \-d [\-s <config_server>] [\-n] dsource_name1 dsource_name2 …
 show all parameters of given datasources
 .TP
-.B info [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 ...
+.B info [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 …
 show source parameters of given components
 .TP
-.B info \-r [\-s <config_server>]  [\-n] profile_name1 profile_name2 ...
+.B info \-r [\-s <config_server>]  [\-n] profile_name1 profile_name2 …
 show general parameters of given profiles
 .TP
-.B geometry [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 ...
+.B geometry [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 …
 show transformation parameters of given components
 .UNINDENT
 .TP
 .B Options:
 .INDENT 7.0
 .TP
 .B \-h\fP,\fB  \-\-help
@@ -141,15 +141,15 @@
 .B \-d\fP,\fB  \-\-datasources
 perform operation on datasources
 .TP
 .B \-m\fP,\fB  \-\-mandatory
 make use mandatory components as well
 .TP
 .B \-p\fP,\fB  \-\-private
-make use private components, i.e. starting with \(aq__\(aq
+make use private components, i.e. starting with ‘__’
 .TP
 .B \-n\fP,\fB  \-\-no\-newlines
 split result with space characters
 .TP
 .B \-f\fP,\fB  \-\-force
 do not ask
 .UNINDENT
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nxstools-3.8.0/man/nxscreate.1` & `nxstools-3.9.0/man/nxscreate.1`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "NXSCREATE" "1" "May 21, 2021" "3.8" "NXSTools"
+.TH "NXSCREATE" "1" "Jun 08, 2021" "3.9" "NXSTools"
 .SH NAME
 nxscreate \- create NeXus Configuration component
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -62,15 +62,15 @@
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is \(aq.\(aq
+default <directory> is ‘.’
 .IP \(bu 2
 default <server> is taken from Tango DB
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
@@ -99,15 +99,15 @@
 .BI \-s \ DSOURCE\fP,\fB \ \-\-datasource\-prefix\fB= DSOURCE
 datasource prefix, i.e. counter (useful for avoiding duplicated datasource names)
 .TP
 .B \-b\fP,\fB  \-\-database
 store datasources in Configuration Server database
 .TP
 .B \-m\fP,\fB  \-\-minimal_device
-device name without first \(aq0\(aq
+device name without first ‘0’
 .TP
 .BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
@@ -139,19 +139,19 @@
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is \(aq.\(aq
+default <directory> is ‘.’
 .IP \(bu 2
 default <server> is taken from Tango DB
 .IP \(bu 2
-default <datasource> is \(aqexp_mot\(aq
+default <datasource> is ‘exp_mot’
 .IP \(bu 2
 default <host>, <port> are taken from <server>
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
@@ -237,19 +237,19 @@
 .IP \(bu 2
 without <dv_attr1>: datasources for all attributes are created
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is \(aq.\(aq
+default <directory> is ‘.’
 .IP \(bu 2
 default <server> is taken from Tango DB
 .IP \(bu 2
-default <datasource> is \(aqexp_mot\(aq
+default <datasource> is ‘exp_mot’
 .IP \(bu 2
 default <host>, <port> are taken from <server>
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
@@ -275,15 +275,15 @@
 .BI \-t \ PORT\fP,\fB \ \-\-port\fB= PORT
 tango host port
 .TP
 .B \-b\fP,\fB  \-\-database
 store datasources in Configuration Server database
 .TP
 .B \-n\fP,\fB  \-\-no\-group
-don\(aqt create common group with a name of datasource
+don’t create common group with a name of datasource
 prefix
 .TP
 .BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .UNINDENT
 .UNINDENT
 .SS Example
@@ -317,15 +317,15 @@
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 with \-d <directory>: datasources are created on the local filesystem
 .IP \(bu 2
 without \-b or \-d <directory>: run in the test mode
 .IP \(bu 2
-default <inputFile> is \(aq/online_dir/online.xml\(aq
+default <inputFile> is ‘/online_dir/online.xml’
 .IP \(bu 2
 default <server> is taken from Tango DB
 .UNINDENT
 .sp
 \fIonlineds\fP overwrites existing datasources
 .INDENT 0.0
 .TP
@@ -395,15 +395,15 @@
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 with \-d <directory>: datasources are created on the local filesystem
 .IP \(bu 2
 without \-b or \-d <directory>: run in the test mode
 .IP \(bu 2
-default <channel> is \(aqALL\(aq
+default <channel> is ‘ALL’
 .IP \(bu 2
 default <server> is taken from Tango DB
 .IP \(bu 2
 default <pool> is taken from Tango DB
 .UNINDENT
 .sp
 \fIpoolds\fP overwrites existing datasources
@@ -466,23 +466,23 @@
 nxscreate onlinecp [options] inputFile
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
-without \(aq\-c <component>\(aq: show a list of possible components
+without ‘\-c <component>’: show a list of possible components
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is \(aq.\(aq
+default <directory> is ‘.’
 .IP \(bu 2
-default <inputFile> is \(aq/online_dir/online.xml\(aq
+default <inputFile> is ‘/online_dir/online.xml’
 .IP \(bu 2
 default <server> is taken from Tango DB
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
@@ -566,25 +566,25 @@
 nxscreate stdcomp [options] [name1 value1 [name2 value2] ...]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
-without \(aq\-t <type>\(aq: show a list of possible component types
+without ‘\-t <type>’: show a list of possible component types
 .IP \(bu 2
-with \(aq\-t <type>  and without \-c <component>: show a list of component variables for the given component type
+with ‘\-t <type>  and without \-c <component>: show a list of component variables for the given component type
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is \(aq.\(aq
+default <directory> is ‘.’
 .IP \(bu 2
-[name1 value1 [name2 value2] ...] sequence  defines component variable values
+[name1 value1 [name2 value2] …] sequence  defines component variable values
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
 .B \-h\fP,\fB  \-\-help
@@ -657,25 +657,25 @@
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is \(aq.\(aq
+default <directory> is ‘.’
 .IP \(bu 2
 default <server> is taken from Tango DB
 .IP \(bu 2
 default <strategy> is step
 .IP \(bu 2
 default <type> is NX_FLOAT
 .IP \(bu 2
 default <chunk> is SCALAR
 .IP \(bu 2
-default <nexuspath> is "/$var.entryname#\(aqscan\(aq$var.serialno:NXentry/instrument/collection/"
+default <nexuspath> is “/$var.entryname#’scan’$var.serialno:NXentry/instrument/collection/”
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
 .B \-h\fP,\fB  \-\-help
@@ -723,15 +723,15 @@
 .BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .TP
 .BI \-c \ CHUNK\fP,\fB \ \-\-chunk\fB= CHUNK
 chunk format, i.e. SCALAR, SPECTRUM, IMAGE
 .TP
 .B \-m\fP,\fB  \-\-minimal_device
-device name without first \(aq0\(aq
+device name without first ‘0’
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
@@ -757,15 +757,15 @@
 nxscreate compare [\-h] [\-n] online_file [online_file]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
-default: second <online_file> is \(aq/online_dir/online.xml\(aq if only file is given
+default: second <online_file> is ‘/online_dir/online.xml’ if only file is given
 .UNINDENT
 .INDENT 0.0
 .TP
 .B positional arguments:
 online_file    online.xml files
 .TP
 .B optional arguments:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nxstools-3.8.0/man/nxsdata.1` & `nxstools-3.9.0/man/nxsdata.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "NXSDATA" "1" "May 21, 2021" "3.8" "NXSTools"
+.TH "NXSDATA" "1" "Jun 08, 2021" "3.9" "NXSTools"
 .SH NAME
 nxsdata \- run NeXus Data Writer
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `nxstools-3.8.0/man/nxsetup.1` & `nxstools-3.9.0/man/nxsetup.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "NXSETUP" "1" "May 21, 2021" "3.8" "NXSTools"
+.TH "NXSETUP" "1" "Jun 08, 2021" "3.9" "NXSTools"
 .SH NAME
 nxsetup \- set NeXDaTaS Tango Server environment up
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `nxstools-3.8.0/man/nxsfileinfo.1` & `nxstools-3.9.0/man/nxsfileinfo.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "NXSFILEINFO" "1" "May 21, 2021" "3.8" "NXSTools"
+.TH "NXSFILEINFO" "1" "Jun 08, 2021" "3.9" "NXSTools"
 .SH NAME
 nxsfileinfo \- show metadata of the NeXus file
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -108,15 +108,15 @@
 .B \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
 .BI \-c \ HEADERS\fP,\fB \ \-\-columns\fB= HEADERS
 names of column to be shown (separated by commas without spaces). The possible names are: depends_on, dtype, full_path, nexus_path, nexus_type, shape, source, source_name, source_type, strategy, trans_type, trans_offset, trans_vector, units, value
 .TP
 .BI \-f \ FILTERS\fP,\fB \ \-\-filters\fB= FILTERS
-full_path filters (separated by commas without spaces). Default: \(aq*\(aq. E.g. \(aq\fI:NXsample/\fP\(aq
+full_path filters (separated by commas without spaces). Default: ‘*’. E.g. ‘\fI:NXsample/\fP’
 .TP
 .BI \-v \ VALUES\fP,\fB \ \-\-values\fB= VALUES
 field names which value should be stored (separated by commas without spaces). Default: depends_on
 .TP
 .B \-g\fP,\fB  \-\-geometry
 show fields with geometry full_path filters, i.e. \fI:NXtransformations/\fP,*/depends_on. It works only when \-f is not defined
 .TP
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nxstools-3.8.0/man/nxstools.1` & `nxstools-3.9.0/man/nxstools.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "NXSTOOLS" "1" "May 21, 2021" "3.8" "NXSTools"
+.TH "NXSTOOLS" "1" "Jun 08, 2021" "3.9" "NXSTools"
 .SH NAME
 nxstools \- nxstools Documentation
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -253,35 +253,35 @@
 .INDENT 7.0
 .TP
 .B \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
 .BI \-c \ COMPRESSION\fP,\fB \ \-\-compression \ COMPRESSION
 deflate compression rate from 0 to 9 (default: 2) or
-<filterid>:opt1,opt2,... e.g. \-c 32008:0,2 for
+<filterid>:opt1,opt2,… e.g. \-c 32008:0,2 for
 bitshuffle with lz4
 .TP
 .BI \-p \ PATH\fP,\fB \ \-\-path \ PATH
 nexus path for the output field, e.g.
 /scan/instrument/pilatus/data
 .TP
 .BI \-i \ INPUTFILES\fP,\fB \ \-\-input_files \ INPUTFILES
 input data files defined with a pattern or separated
-by \(aq,\(aq e.g.\(aqscan_%05d.tif:0:100\(aq
+by ‘,’ e.g.’scan_%05d.tif:0:100’
 .TP
 .BI \-\-separator \ SEPARATOR
-input data files separator (default: \(aq,\(aq)
+input data files separator (default: ‘,’)
 .TP
 .BI \-\-dtype \ DATATYPE
 datatype of input data \- only for raw data, e.g.
-\(aquint8\(aq
+‘uint8’
 .TP
 .BI \-\-shape \ SHAPE
 shape of input data \- only for raw data, e.g.
-\(aq[4096,2048]\(aq
+‘[4096,2048]’
 .TP
 .B \-s\fP,\fB  \-\-skip_missing
 skip missing files
 .TP
 .B \-r\fP,\fB  \-\-replace_nexus_file
 if it is set the old file is not copied into a file
 with .__nxscollect__old__* extension
@@ -396,107 +396,107 @@
 .INDENT 3.5
 .INDENT 0.0
 .TP
 .B \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
 .BI \-t \ DTYPE\fP,\fB \ \-\-dtype \ DTYPE
-datatype of the VDS field, e.g. \(aquint8\(aq
+datatype of the VDS field, e.g. ‘uint8’
 .TP
 .BI \-s \ SHAPE\fP,\fB \ \-\-shape \ SHAPE
-shape of the VDS field, e.g. \(aq[U,4096,2048]\(aq or
-U,4096,2048 where U means span along the field\(aq
+shape of the VDS field, e.g. ‘[U,4096,2048]’ or
+U,4096,2048 where U means span along the field’
 .TP
 .BI \-f \ FILLVALUE\fP,\fB \ \-\-fill\-value \ FILLVALUE
 fill value for the gaps, default is 0
 .TP
 .BI \-e \ TARGETFIELDS\fP,\fB \ \-\-target\-fields \ TARGETFIELDS
 external fields with their NeXus file paths defined
-with a pattern or separated by \(aq,\(aq
-e.g.\(aqscan_123/lambda_%05d.nxs://entry/data/\fI\%data:0:3\fP\(aq
+with a pattern or separated by ‘,’
+e.g.’scan_123/lambda_%05d.nxs://entry/data/\fI\%data:0:3\fP’
 .TP
 .BI \-\-separator \ SEPARATOR
-input data files separator (default: \(aq,\(aq)
+input data files separator (default: ‘,’)
 .TP
 .BI \-p \ SHAPES\fP,\fB \ \-\-shapes \ SHAPES
 shapes in the VDS layout hyperslab for the
 corresponding target fields with coordinates sepatated
-by \(aq,\(aq and different fields separated by \(aq;\(aq, \(aq:\(aq or
-spaces e.g.\(aq,,;,300,;,600,0\(aq where an empty coordinate
+by ‘,’ and different fields separated by ‘;’, ‘:’ or
+spaces e.g.’,,;,300,;,600,0’ where an empty coordinate
 means 0
 .TP
 .BI \-o \ OFFSETS\fP,\fB \ \-\-offsets \ OFFSETS
 offsets in the VDS layout hyperslab for the
 corresponding target fields with coordinates sepatated
-by \(aq,\(aq and different fields separated by \(aq;\(aq, \(aq:\(aq or
-spaces e.g.\(aq,,;,300,;,600,0\(aq where an empty coordinate
+by ‘,’ and different fields separated by ‘;’, ‘:’ or
+spaces e.g.’,,;,300,;,600,0’ where an empty coordinate
 means 0
 .TP
 .BI \-b \ BLOCKS\fP,\fB \ \-\-blocks \ BLOCKS
 block sizes in the VDS layout hyperslab for the
 corresponding target fields with coordinates sepatated
-by \(aq,\(aq and different fields separated by \(aq;\(aq, \(aq:\(aq or
-spaces e.g. \(aq,256,512;,256,512;,256,512\(aq where an
+by ‘,’ and different fields separated by ‘;’, ‘:’ or
+spaces e.g. ‘,256,512;,256,512;,256,512’ where an
 empty coordinate means 1
 .TP
 .BI \-c \ COUNTS\fP,\fB \ \-\-counts \ COUNTS
 count numbers in the VDS layout hyperslabfor the
 corresponding target fields with coordinates sepatated
-by \(aq,\(aq and different fields separated by \(aq;\(aq, \(aq:\(aq or
-spaces e.g. \(aq,1,1;,1,1;,1,1\(aq where an empty coordinate
+by ‘,’ and different fields separated by ‘;’, ‘:’ or
+spaces e.g. ‘,1,1;,1,1;,1,1’ where an empty coordinate
 means span along the layout
 .TP
 .BI \-d \ STRIDES\fP,\fB \ \-\-strides \ STRIDES
 stride sizes in the VDS layout hyperslabfor the
 corresponding target fields with coordinates sepatated
-by \(aq,\(aq and different fields separated by \(aq;\(aq, \(aq:\(aq or
-spaces e.g. \(aq,,;,,;,,\(aq where an empty coordinate means
+by ‘,’ and different fields separated by ‘;’, ‘:’ or
+spaces e.g. ‘,,;,,;,,’ where an empty coordinate means
 1
 .TP
 .BI \-l \ SLICES\fP,\fB \ \-\-slices \ SLICES
 mapping slices in the VDS layoutfor the corresponding
-target fields with coordinates sepatated by \(aq,\(aq and
-different fields separated by \(aq;\(aq or spaces e.g.
-\(aq:,0:50,: :,50:100,:\(aq where U means span along the
+target fields with coordinates sepatated by ‘,’ and
+different fields separated by ‘;’ or spaces e.g.
+‘:,0:50,: :,50:100,:’ where U means span along the
 layout
 .TP
 .BI \-P \ TARGETSHAPES\fP,\fB \ \-\-target\-shapes \ TARGETSHAPES
-field shapes with coordinates sepatated by \(aq,\(aq and
-different fields separated by \(aq;\(aq, \(aq:\(aq or spaces
-e.g.\(aq,,;,300,;,600,0\(aq
+field shapes with coordinates sepatated by ‘,’ and
+different fields separated by ‘;’, ‘:’ or spaces
+e.g.’,,;,300,;,600,0’
 .TP
 .BI \-O \ TARGETOFFSETS\fP,\fB \ \-\-target\-offsets \ TARGETOFFSETS
 offsets in the view hyperslab of target fieldswith
-coordinates sepatated by \(aq,\(aq and different fields
-separated by \(aq;\(aq, \(aq:\(aq or spaces e.g.\(aq,,;,300,;,600,0\(aq
+coordinates sepatated by ‘,’ and different fields
+separated by ‘;’, ‘:’ or spaces e.g.’,,;,300,;,600,0’
 where an empty coordinate means 0
 .TP
 .BI \-B \ TARGETBLOCKS\fP,\fB \ \-\-target\-blocks \ TARGETBLOCKS
 block sizes in the view hyperslab of target fields
-with coordinates sepatated by \(aq,\(aq and different fields
-separated by \(aq;\(aq, \(aq:\(aq or spaces e.g.
-\(aq,256,512;,256,512;,256,512\(aq where an empty coordinate
+with coordinates sepatated by ‘,’ and different fields
+separated by ‘;’, ‘:’ or spaces e.g.
+‘,256,512;,256,512;,256,512’ where an empty coordinate
 means 1
 .TP
 .BI \-C \ TARGETCOUNTS\fP,\fB \ \-\-target\-counts \ TARGETCOUNTS
 count numbers in the view hyperslab of target fields
-with coordinates sepatated by \(aq,\(aq and different fields
-separated by \(aq;\(aq, \(aq:\(aq or spaces e.g. \(aq,1,1;,1,1;,1,1\(aq
+with coordinates sepatated by ‘,’ and different fields
+separated by ‘;’, ‘:’ or spaces e.g. ‘,1,1;,1,1;,1,1’
 where an empty coordinate means span along the layout
 .TP
 .BI \-D \ TARGETSTRIDES\fP,\fB \ \-\-target\-strides \ TARGETSTRIDES
 stride sizes numbers in the view hyperslab of target
-fields with coordinates sepatated by \(aq,\(aq and different
-fields separated by \(aq;\(aq, \(aq:\(aq or spaces e.g. \(aq,,;,,;,,\(aq
+fields with coordinates sepatated by ‘,’ and different
+fields separated by ‘;’, ‘:’ or spaces e.g. ‘,,;,,;,,’
 where an empty coordinate means 1
 .TP
 .BI \-L \ TARGETSLICES\fP,\fB \ \-\-target\-slices \ TARGETSLICES
 view slices of target fields with coordinates
-sepatated by \(aq,\(aq and different fields separated by \(aq;\(aq
-or spaces e.g. \(aq:,0:50,: :,0:50,:\(aq where U means span
+sepatated by ‘,’ and different fields separated by ‘;’
+or spaces e.g. ‘:,0:50,: :,0:50,:’ where U means span
 along the layout
 .TP
 .B \-r\fP,\fB  \-\-replace\-nexus\-file
 if it is set the old file is not copied into a file
 with .__nxscollect__old__* extension
 .TP
 .B \-\-test
@@ -563,78 +563,78 @@
 .TP
 .B list \-d [\-s <config_server>] [\-n]
 list names of available datasources
 .TP
 .B list \-r [\-s <config_server>] [\-n]
 list names of available profiles
 .TP
-.B show [\-s <config_server>] [\-m] [\-o <dir>] component_name1 component_name2 ...
+.B show [\-s <config_server>] [\-m] [\-o <dir>] component_name1 component_name2 …
 show components with given names
 .TP
-.B show \-d [\-s <config_server>]  [\-o <dir>] dsource_name1 dsource_name2 ...
+.B show \-d [\-s <config_server>]  [\-o <dir>] dsource_name1 dsource_name2 …
 show datasources with given names
 .TP
-.B show \-r [\-s <config_server>]  [\-o <dir>] profile_name1 profile_name2 ...
+.B show \-r [\-s <config_server>]  [\-o <dir>] profile_name1 profile_name2 …
 show profiles with given names
 .TP
-.B upload [\-s <config_server>] [\-m] [\-i <dir>] [\-f] component_name1 component_name2 ...
+.B upload [\-s <config_server>] [\-m] [\-i <dir>] [\-f] component_name1 component_name2 …
 load components from given files
 .TP
-.B upload \-d [\-s <config_server>]  [\-i <dir>] [\-f] dsource_name1 dsource_name2 ...
+.B upload \-d [\-s <config_server>]  [\-i <dir>] [\-f] dsource_name1 dsource_name2 …
 load datasources from given files
 .TP
-.B upload \-r [\-s <config_server>]  [\-i <dir>] [\-f] profile_name1 profile_name2 ...
+.B upload \-r [\-s <config_server>]  [\-i <dir>] [\-f] profile_name1 profile_name2 …
 load profiles from given files
 .TP
-.B get [\-s <config_server>]  [\-n] component_name1 component_name2 ...
+.B get [\-s <config_server>]  [\-n] component_name1 component_name2 …
 get merged configuration of components
 .TP
-.B delete [\-s <config_server>] [\-f] component_name1 component_name2 ...
+.B delete [\-s <config_server>] [\-f] component_name1 component_name2 …
 delete components with given names
 .TP
-.B delete \-d [\-s <config_server>] [\-f] dsource_name1 dsource_name2 ...
+.B delete \-d [\-s <config_server>] [\-f] dsource_name1 dsource_name2 …
 delete datasources with given names
 .TP
-.B delete \-r [\-s <config_server>] [\-f] profile_name1 profile_name2 ...
+.B delete \-r [\-s <config_server>] [\-f] profile_name1 profile_name2 …
 delete profiles with given names
 .TP
-.B sources [\-s <config_server>] [\-m] [\-n] component_name1 component_name2 ...
+.B sources [\-s <config_server>] [\-m] [\-n] component_name1 component_name2 …
 get a list of component datasources
 .TP
-.B components [\-s <config_server>] [\-n] component_name1 component_name2 ...
+.B components [\-s <config_server>] [\-n] component_name1 component_name2 …
 get a list of dependent components
 .TP
-.B variables [\-s <config_server>] [\-m] [\-n] component_name1 component_name2 ...
+.B variables [\-s <config_server>] [\-m] [\-n] component_name1 component_name2 …
 get a list of component variables
 .TP
 .B data [\-s <config_server>] json_data
 set values of component variables
 .TP
 .B record [\-s <config_server>] [\-n] component_name1
 get a list of datasource record names from component
 .TP
 .B record \-d [\-s <config_server>] [\-n] datasource_name1
 get a list of datasource record names
 .TP
 .B servers [\-s <config_server/host>] [\-n]
 get lists of configuration servers from the current tango host
 .TP
-.B describe [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 ...
+.B describe [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 …
 show all parameters of given components
 .TP
-.B describe|info \-d [\-s <config_server>] [\-n] dsource_name1 dsource_name2 ...
+.B describe|info \-d [\-s <config_server>] [\-n] dsource_name1 dsource_name2 …
 show all parameters of given datasources
 .TP
-.B info [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 ...
+.B info [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 …
 show source parameters of given components
 .TP
-.B info \-r [\-s <config_server>]  [\-n] profile_name1 profile_name2 ...
+.B info \-r [\-s <config_server>]  [\-n] profile_name1 profile_name2 …
 show general parameters of given profiles
 .TP
-.B geometry [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 ...
+.B geometry [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 …
 show transformation parameters of given components
 .UNINDENT
 .TP
 .B Options:
 .INDENT 7.0
 .TP
 .B \-h\fP,\fB  \-\-help
@@ -646,15 +646,15 @@
 .B \-d\fP,\fB  \-\-datasources
 perform operation on datasources
 .TP
 .B \-m\fP,\fB  \-\-mandatory
 make use mandatory components as well
 .TP
 .B \-p\fP,\fB  \-\-private
-make use private components, i.e. starting with \(aq__\(aq
+make use private components, i.e. starting with ‘__’
 .TP
 .B \-n\fP,\fB  \-\-no\-newlines
 split result with space characters
 .TP
 .B \-f\fP,\fB  \-\-force
 do not ask
 .UNINDENT
@@ -705,15 +705,15 @@
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is \(aq.\(aq
+default <directory> is ‘.’
 .IP \(bu 2
 default <server> is taken from Tango DB
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
@@ -742,15 +742,15 @@
 .BI \-s \ DSOURCE\fP,\fB \ \-\-datasource\-prefix\fB= DSOURCE
 datasource prefix, i.e. counter (useful for avoiding duplicated datasource names)
 .TP
 .B \-b\fP,\fB  \-\-database
 store datasources in Configuration Server database
 .TP
 .B \-m\fP,\fB  \-\-minimal_device
-device name without first \(aq0\(aq
+device name without first ‘0’
 .TP
 .BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
@@ -782,19 +782,19 @@
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is \(aq.\(aq
+default <directory> is ‘.’
 .IP \(bu 2
 default <server> is taken from Tango DB
 .IP \(bu 2
-default <datasource> is \(aqexp_mot\(aq
+default <datasource> is ‘exp_mot’
 .IP \(bu 2
 default <host>, <port> are taken from <server>
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
@@ -880,19 +880,19 @@
 .IP \(bu 2
 without <dv_attr1>: datasources for all attributes are created
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is \(aq.\(aq
+default <directory> is ‘.’
 .IP \(bu 2
 default <server> is taken from Tango DB
 .IP \(bu 2
-default <datasource> is \(aqexp_mot\(aq
+default <datasource> is ‘exp_mot’
 .IP \(bu 2
 default <host>, <port> are taken from <server>
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
@@ -918,15 +918,15 @@
 .BI \-t \ PORT\fP,\fB \ \-\-port\fB= PORT
 tango host port
 .TP
 .B \-b\fP,\fB  \-\-database
 store datasources in Configuration Server database
 .TP
 .B \-n\fP,\fB  \-\-no\-group
-don\(aqt create common group with a name of datasource
+don’t create common group with a name of datasource
 prefix
 .TP
 .BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .UNINDENT
 .UNINDENT
 .SS Example
@@ -960,15 +960,15 @@
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 with \-d <directory>: datasources are created on the local filesystem
 .IP \(bu 2
 without \-b or \-d <directory>: run in the test mode
 .IP \(bu 2
-default <inputFile> is \(aq/online_dir/online.xml\(aq
+default <inputFile> is ‘/online_dir/online.xml’
 .IP \(bu 2
 default <server> is taken from Tango DB
 .UNINDENT
 .sp
 \fIonlineds\fP overwrites existing datasources
 .INDENT 0.0
 .TP
@@ -1038,15 +1038,15 @@
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 with \-d <directory>: datasources are created on the local filesystem
 .IP \(bu 2
 without \-b or \-d <directory>: run in the test mode
 .IP \(bu 2
-default <channel> is \(aqALL\(aq
+default <channel> is ‘ALL’
 .IP \(bu 2
 default <server> is taken from Tango DB
 .IP \(bu 2
 default <pool> is taken from Tango DB
 .UNINDENT
 .sp
 \fIpoolds\fP overwrites existing datasources
@@ -1109,23 +1109,23 @@
 nxscreate onlinecp [options] inputFile
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
-without \(aq\-c <component>\(aq: show a list of possible components
+without ‘\-c <component>’: show a list of possible components
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is \(aq.\(aq
+default <directory> is ‘.’
 .IP \(bu 2
-default <inputFile> is \(aq/online_dir/online.xml\(aq
+default <inputFile> is ‘/online_dir/online.xml’
 .IP \(bu 2
 default <server> is taken from Tango DB
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
@@ -1209,25 +1209,25 @@
 nxscreate stdcomp [options] [name1 value1 [name2 value2] ...]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
-without \(aq\-t <type>\(aq: show a list of possible component types
+without ‘\-t <type>’: show a list of possible component types
 .IP \(bu 2
-with \(aq\-t <type>  and without \-c <component>: show a list of component variables for the given component type
+with ‘\-t <type>  and without \-c <component>: show a list of component variables for the given component type
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is \(aq.\(aq
+default <directory> is ‘.’
 .IP \(bu 2
-[name1 value1 [name2 value2] ...] sequence  defines component variable values
+[name1 value1 [name2 value2] …] sequence  defines component variable values
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
 .B \-h\fP,\fB  \-\-help
@@ -1300,25 +1300,25 @@
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is \(aq.\(aq
+default <directory> is ‘.’
 .IP \(bu 2
 default <server> is taken from Tango DB
 .IP \(bu 2
 default <strategy> is step
 .IP \(bu 2
 default <type> is NX_FLOAT
 .IP \(bu 2
 default <chunk> is SCALAR
 .IP \(bu 2
-default <nexuspath> is "/$var.entryname#\(aqscan\(aq$var.serialno:NXentry/instrument/collection/"
+default <nexuspath> is “/$var.entryname#’scan’$var.serialno:NXentry/instrument/collection/”
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
 .B \-h\fP,\fB  \-\-help
@@ -1366,15 +1366,15 @@
 .BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .TP
 .BI \-c \ CHUNK\fP,\fB \ \-\-chunk\fB= CHUNK
 chunk format, i.e. SCALAR, SPECTRUM, IMAGE
 .TP
 .B \-m\fP,\fB  \-\-minimal_device
-device name without first \(aq0\(aq
+device name without first ‘0’
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
@@ -1400,15 +1400,15 @@
 nxscreate compare [\-h] [\-n] online_file [online_file]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
-default: second <online_file> is \(aq/online_dir/online.xml\(aq if only file is given
+default: second <online_file> is ‘/online_dir/online.xml’ if only file is given
 .UNINDENT
 .INDENT 0.0
 .TP
 .B positional arguments:
 online_file    online.xml files
 .TP
 .B optional arguments:
@@ -1578,15 +1578,15 @@
 .B \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
 .BI \-c \ HEADERS\fP,\fB \ \-\-columns\fB= HEADERS
 names of column to be shown (separated by commas without spaces). The possible names are: depends_on, dtype, full_path, nexus_path, nexus_type, shape, source, source_name, source_type, strategy, trans_type, trans_offset, trans_vector, units, value
 .TP
 .BI \-f \ FILTERS\fP,\fB \ \-\-filters\fB= FILTERS
-full_path filters (separated by commas without spaces). Default: \(aq*\(aq. E.g. \(aq\fI:NXsample/\fP\(aq
+full_path filters (separated by commas without spaces). Default: ‘*’. E.g. ‘\fI:NXsample/\fP’
 .TP
 .BI \-v \ VALUES\fP,\fB \ \-\-values\fB= VALUES
 field names which value should be stored (separated by commas without spaces). Default: depends_on
 .TP
 .B \-g\fP,\fB  \-\-geometry
 show fields with geometry full_path filters, i.e. \fI:NXtransformations/\fP,*/depends_on. It works only when \-f is not defined
 .TP
@@ -1832,25 +1832,25 @@
 .sp
 The constructor creates the collector object
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBnexusfilename\fP (\fI\%str\fP) \-\- the nexus file name
+\fBnexusfilename\fP (\fI\%str\fP) – the nexus file name
 .IP \(bu 2
-\fBcompression\fP (\fI\%int\fP) \-\- compression rate
+\fBcompression\fP (\fI\%int\fP) – compression rate
 .IP \(bu 2
-\fBskipmissing\fP (\fI\%bool\fP) \-\- if skip missing images
+\fBskipmissing\fP (\fI\%bool\fP) – if skip missing images
 .IP \(bu 2
-\fBstoreold\fP (\fI\%bool\fP) \-\- if backup the input file
+\fBstoreold\fP (\fI\%bool\fP) – if backup the input file
 .IP \(bu 2
-\fBtestmode\fP (\fI\%bool\fP) \-\- if run in a test mode
+\fBtestmode\fP (\fI\%bool\fP) – if run in a test mode
 .IP \(bu 2
-\fBwriter\fP (\fI\%str\fP) \-\- the writer module
+\fBwriter\fP (\fI\%str\fP) – the writer module
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B collect(path=None, inputfiles=None, datatype=None, shape=None)
 creates a temporary file,
 collects the all image files defined by hdf5
@@ -1858,21 +1858,21 @@
 to the origin one if the action was successful
 or appends specific data if path and inputfiles are given
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBpath\fP (\fI\%str\fP) \-\- nexus path of the data field
+\fBpath\fP (\fI\%str\fP) – nexus path of the data field
 .IP \(bu 2
-\fBinputfiles\fP (\fI\%list\fP <\fI\%str\fP>) \-\- a list of file strings
+\fBinputfiles\fP (\fI\%list\fP <\fI\%str\fP>) – a list of file strings
 .IP \(bu 2
-\fBdatatype\fP (\fI\%str\fP) \-\- field data type
+\fBdatatype\fP (\fI\%str\fP) – field data type
 .IP \(bu 2
-\fBshape\fP (\fI\%list\fP <\fI\%int\fP >) \-\- field shape
+\fBshape\fP (\fI\%list\fP <\fI\%int\fP >) – field shape
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxscollect.Execute(parser)
@@ -1880,15 +1880,15 @@
 .sp
 Execute runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -1909,32 +1909,32 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxscollect.LayoutField(target, hyperslab=None)
 Bases: \fI\%object\fP
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBhyperslab\fP (\fBfilewriter.FTHyperslab\fP) \-\- target field object
+\fBhyperslab\fP (\fBfilewriter.FTHyperslab\fP) – target field object
 .IP \(bu 2
-\fBhyperslab\fP \-\- field hyperslab or slices
+\fBhyperslab\fP – field hyperslab or slices
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B hyperslab = None
 \fBfilewriter.FTHyperslab\fP layout hyperslab or slices
 .UNINDENT
@@ -1961,15 +1961,15 @@
 .sp
 Execute runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -1990,15 +1990,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxscollect.Linker(nexusfilepath, target, name=None, storeold=False, testmode=False, writer=None)
 Bases: \fI\%object\fP
@@ -2007,23 +2007,23 @@
 .sp
 The constructor creates the collector object
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBnexusfilepath\fP (\fI\%str\fP) \-\- the nexus file name and nexus path
+\fBnexusfilepath\fP (\fI\%str\fP) – the nexus file name and nexus path
 .IP \(bu 2
-\fBtarget\fP (\fI\%str\fP) \-\- the nexus file name and nexus path
+\fBtarget\fP (\fI\%str\fP) – the nexus file name and nexus path
 .IP \(bu 2
-\fBstoreold\fP (\fI\%bool\fP) \-\- if backup the input file
+\fBstoreold\fP (\fI\%bool\fP) – if backup the input file
 .IP \(bu 2
-\fBtestmode\fP (\fI\%bool\fP) \-\- if run in a test mode
+\fBtestmode\fP (\fI\%bool\fP) – if run in a test mode
 .IP \(bu 2
-\fBwriter\fP (\fI\%str\fP) \-\- the writer module
+\fBwriter\fP (\fI\%str\fP) – the writer module
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B link()
 creates NeXus link
 .UNINDENT
@@ -2037,23 +2037,23 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBfilename\fP (\fI\%str\fP) \-\- file name
+\fBfilename\fP (\fI\%str\fP) – file name
 .IP \(bu 2
-\fBpath\fP (\fI\%str\fP) \-\- nexus field path with its name
+\fBpath\fP (\fI\%str\fP) – nexus field path with its name
 .IP \(bu 2
-\fBshape\fP (\fI\%list\fP <\fI\%int\fP>) \-\- field shape
+\fBshape\fP (\fI\%list\fP <\fI\%int\fP>) – field shape
 .IP \(bu 2
-\fBhyperslab\fP (\fBfilewriter.FTHyperslab\fP) \-\- field hyperslab or slices
+\fBhyperslab\fP (\fBfilewriter.FTHyperslab\fP) – field hyperslab or slices
 .IP \(bu 2
-\fBmaxshape\fP (\fI\%list\fP <\fI\%int\fP>) \-\- maximal field shape
+\fBmaxshape\fP (\fI\%list\fP <\fI\%int\fP>) – maximal field shape
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B filename = None
 \fI\%str\fP file name
 .UNINDENT
@@ -2090,94 +2090,94 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBexfieldpaths\fP (\fI\%str\fP) \-\- target field paths
+\fBexfieldpaths\fP (\fI\%str\fP) – target field paths
 .IP \(bu 2
-\fBexfieldshapes\fP (\fI\%str\fP) \-\- target field shapes
+\fBexfieldshapes\fP (\fI\%str\fP) – target field shapes
 .IP \(bu 2
-\fBshapes\fP (\fBlist\(ga<:obj:\(gatuple\(ga<:obj:\(gaint\fP> >) \-\- target field shapes
+\fBshapes\fP (\fBlist\(ga<:obj:\(gatuple\(ga<:obj:\(gaint\fP> >) – target field shapes
 .IP \(bu 2
-\fBexfieldpaths\fP \-\- separator of field path strings
+\fBexfieldpaths\fP – separator of field path strings
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B add_layout_hyperslabs(offsets, blocks, counts, strides)
 add layout hyperslabs
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoffsets\fP (\fI\%str\fP) \-\- layout offsets
+\fBoffsets\fP (\fI\%str\fP) – layout offsets
 .IP \(bu 2
-\fBblocks\fP (\fI\%str\fP) \-\- layout blocks
+\fBblocks\fP (\fI\%str\fP) – layout blocks
 .IP \(bu 2
-\fBcounts\fP (\fI\%str\fP) \-\- layout counts
+\fBcounts\fP (\fI\%str\fP) – layout counts
 .IP \(bu 2
-\fBstrides\fP (\fI\%str\fP) \-\- layout strides
+\fBstrides\fP (\fI\%str\fP) – layout strides
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B add_layout_slices(slices)
 add layout slices
 .INDENT 7.0
 .TP
 .B Parameters
-\fBslices\fP (\fI\%str\fP) \-\- layout slices
+\fBslices\fP (\fI\%str\fP) – layout slices
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B add_target_hyperslabs(offsets, blocks, counts, strides)
 add target hyperslabs
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoffsets\fP (\fI\%str\fP) \-\- target offsets
+\fBoffsets\fP (\fI\%str\fP) – target offsets
 .IP \(bu 2
-\fBblocks\fP (\fI\%str\fP) \-\- target blocks
+\fBblocks\fP (\fI\%str\fP) – target blocks
 .IP \(bu 2
-\fBcounts\fP (\fI\%str\fP) \-\- target counts
+\fBcounts\fP (\fI\%str\fP) – target counts
 .IP \(bu 2
-\fBstrides\fP (\fI\%str\fP) \-\- target strides
+\fBstrides\fP (\fI\%str\fP) – target strides
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B add_target_slices(slices)
 add taget slices
 .INDENT 7.0
 .TP
 .B Parameters
-\fBslices\fP (\fI\%str\fP) \-\- target slices
+\fBslices\fP (\fI\%str\fP) – target slices
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxscollect.VDS(parser)
 Bases: \fI\%nxstools.nxsargparser.Runner\fP
 .sp
 Execute runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -2198,15 +2198,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxscollect.VirtualDataset(nexusfilepath, options, writer=None)
 Bases: \fI\%object\fP
@@ -2215,19 +2215,19 @@
 .sp
 The constructor creates the collector object
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBnexusfilepath\fP (\fI\%str\fP) \-\- the nexus file name and nexus path
+\fBnexusfilepath\fP (\fI\%str\fP) – the nexus file name and nexus path
 .IP \(bu 2
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .IP \(bu 2
-\fBwriter\fP (\fI\%str\fP) \-\- the writer module
+\fBwriter\fP (\fI\%str\fP) – the writer module
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates VDS
 .UNINDENT
@@ -2235,15 +2235,15 @@
 .INDENT 0.0
 .TP
 .B nxstools.nxscollect.crdtoint(crd)
 convert coorinate to int or  None or Unlimited
 .INDENT 7.0
 .TP
 .B Parameters
-\fBcrd\fP (\fIcordinate as string\fP) \-\- cordinate as string
+\fBcrd\fP (\fIcordinate as string\fP) – cordinate as string
 .TP
 .B Returns
 converted coordinate
 .TP
 .B Return type
 \fI\%int\fP
 .UNINDENT
@@ -2251,15 +2251,15 @@
 .INDENT 0.0
 .TP
 .B nxstools.nxscollect.filegenerator(filestr, pattern=None)
 provides file name generator from file string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBfilestr\fP \-\- file string
+\fBfilestr\fP – file string
 .TP
 .B Type
 filestr: \fI\%str\fP
 .TP
 .B Returns
 file name generator or a list of file names
 .TP
@@ -2269,24 +2269,24 @@
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.nxscollect.getcompression(compression)
 .INDENT 7.0
 .TP
 .B converts compression string to a deflate level parameter
-or list with [filterid, opt1, opt2, ...]
+or list with [filterid, opt1, opt2, …]
 .UNINDENT
 .INDENT 7.0
 .TP
 .B Parameters
-\fBcompression\fP (\fI\%str\fP) \-\- compression string
+\fBcompression\fP (\fI\%str\fP) – compression string
 .TP
 .B Returns
 deflate level parameter
-or list with [filterid, opt1, opt2, ...]
+or list with [filterid, opt1, opt2, …]
 .TP
 .B Return type
 \fI\%int\fP or \fI\%list\fP < \fI\%int\fP > or \fINone\fP
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
@@ -2296,15 +2296,15 @@
 .INDENT 0.0
 .TP
 .B nxstools.nxscollect.splitcoords(crdstr)
 splits coordinate string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBcrdstr\fP (\fIcordinate string\fP) \-\- cordinate string
+\fBcrdstr\fP (\fIcordinate string\fP) – cordinate string
 .TP
 .B Returns
 a list ofr coordinates in tuples
 .TP
 .B Return type
 \fI\%list\fP <\fI\%tuple\fP < \fI\%int\fP >>
 .UNINDENT
@@ -2312,15 +2312,15 @@
 .INDENT 0.0
 .TP
 .B nxstools.nxscollect.splitslices(crdstr)
 splits coordinate string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBcrdstr\fP (\fIcordinate string\fP) \-\- cordinate string
+\fBcrdstr\fP (\fIcordinate string\fP) – cordinate string
 .TP
 .B Returns
 a list ofr coordinates in tuples
 .TP
 .B Return type
 \fI\%list\fP <\fI\%tuple\fP < \fI\%int\fP >>
 .UNINDENT
@@ -2335,15 +2335,15 @@
 .sp
 Components runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -2359,15 +2359,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -2382,17 +2382,17 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBdevice\fP (\fI\%str\fP) \-\- device name of the configuration server
+\fBdevice\fP (\fI\%str\fP) – device name of the configuration server
 .IP \(bu 2
-\fBnonewline\fP (\fI\%bool\fP) \-\- if the output should not be separated
+\fBnonewline\fP (\fI\%bool\fP) – if the output should not be separated
 by the new line character
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B char = None
 (\fI\%str\fP) spliting character
@@ -2400,15 +2400,15 @@
 .INDENT 7.0
 .TP
 .B componentsCmd(components)
 lists components of the components
 .INDENT 7.0
 .TP
 .B Parameters
-\fBcomponents\fP (\fI\%list\fP <\fI\%str\fP>) \-\- given components
+\fBcomponents\fP (\fI\%list\fP <\fI\%str\fP>) – given components
 .TP
 .B Returns
 list of component names
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
 .UNINDENT
@@ -2416,15 +2416,15 @@
 .INDENT 7.0
 .TP
 .B dataCmd(args)
 provides varaible values
 .INDENT 7.0
 .TP
 .B Parameters
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of item names
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) – list of item names
 .TP
 .B Returns
 JSON with variables
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -2434,21 +2434,21 @@
 .B deleteCmd(ds, args, ask=True, profiles=False)
 delete the DB items
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBds\fP (\fI\%bool\fP) \-\- flag set True for datasources
+\fBds\fP (\fI\%bool\fP) – flag set True for datasources
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of item names
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) – list of item names
 .IP \(bu 2
-\fBask\fP (\fI\%bool\fP) \-\- ask flag
+\fBask\fP (\fI\%bool\fP) – ask flag
 .IP \(bu 2
-\fBprofiles\fP (\fI\%bool\fP) \-\- flag set True for profiles
+\fBprofiles\fP (\fI\%bool\fP) – flag set True for profiles
 .UNINDENT
 .TP
 .B Returns
 list of XML items
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
@@ -2459,25 +2459,25 @@
 .B describeCmd(ds, args, md, pr, headers=None, filters=None)
 provides description of configuration elements
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBds\fP (\fI\%bool\fP) \-\- flag set True for datasources
+\fBds\fP (\fI\%bool\fP) – flag set True for datasources
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of item names
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) – list of item names
 .IP \(bu 2
-\fBmd\fP (\fI\%bool\fP) \-\- flag set True for mandatory components
+\fBmd\fP (\fI\%bool\fP) – flag set True for mandatory components
 .IP \(bu 2
-\fBpr\fP (\fI\%str\fP) \-\- flag set True for private components
+\fBpr\fP (\fI\%str\fP) – flag set True for private components
 .IP \(bu 2
-\fBpr\fP \-\- column headers
+\fBpr\fP – column headers
 .IP \(bu 2
-\fBfilters\fP (\fI\%str\fP) \-\- filters for first column names separated by comma
+\fBfilters\fP (\fI\%str\fP) – filters for first column names separated by comma
 .UNINDENT
 .TP
 .B Returns
 list with description
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
@@ -2488,19 +2488,19 @@
 .B geometryCmd(args, md, pr)
 provides geometry info for given elements
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of item names
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) – list of item names
 .IP \(bu 2
-\fBmd\fP (\fI\%bool\fP) \-\- flag set True for mandatory components
+\fBmd\fP (\fI\%bool\fP) – flag set True for mandatory components
 .IP \(bu 2
-\fBpr\fP (\fI\%bool\fP) \-\- flag set True for private components
+\fBpr\fP (\fI\%bool\fP) – flag set True for private components
 .UNINDENT
 .TP
 .B Returns
 list with description
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
@@ -2509,15 +2509,15 @@
 .INDENT 7.0
 .TP
 .B getCmd(args)
 provides final configuration
 .INDENT 7.0
 .TP
 .B Parameters
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of item names
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) – list of item names
 .TP
 .B Returns
 XML configuration string
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -2527,23 +2527,23 @@
 .B infoCmd(ds, args, md, pr, profiles)
 Provides info for given elements
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBds\fP (\fI\%bool\fP) \-\- flag set True for datasources
+\fBds\fP (\fI\%bool\fP) – flag set True for datasources
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of item names
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) – list of item names
 .IP \(bu 2
-\fBmd\fP (\fI\%bool\fP) \-\- flag set True for mandatory components
+\fBmd\fP (\fI\%bool\fP) – flag set True for mandatory components
 .IP \(bu 2
-\fBpr\fP (\fI\%bool\fP) \-\- flag set True for private components
+\fBpr\fP (\fI\%bool\fP) – flag set True for private components
 .IP \(bu 2
-\fBprofiles\fP (\fI\%bool\fP) \-\- flag set True for profiles
+\fBprofiles\fP (\fI\%bool\fP) – flag set True for profiles
 .UNINDENT
 .TP
 .B Returns
 list with description
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
@@ -2554,21 +2554,21 @@
 .B listCmd(ds, mandatory=False, private=False, profiles=False)
 lists the DB item names
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBds\fP (\fI\%bool\fP) \-\- flag set True for datasources
+\fBds\fP (\fI\%bool\fP) – flag set True for datasources
 .IP \(bu 2
-\fBmandatory\fP (\fI\%bool\fP) \-\- flag set True for mandatory components
+\fBmandatory\fP (\fI\%bool\fP) – flag set True for mandatory components
 .IP \(bu 2
-\fBprivate\fP (\fI\%bool\fP) \-\- flag set True for components starting with \(aq__\(aq
+\fBprivate\fP (\fI\%bool\fP) – flag set True for components starting with ‘__’
 .IP \(bu 2
-\fBprofiles\fP (\fI\%bool\fP) \-\- flag set True for profiles
+\fBprofiles\fP (\fI\%bool\fP) – flag set True for profiles
 .UNINDENT
 .TP
 .B Returns
 list op item names
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
@@ -2577,15 +2577,15 @@
 .INDENT 7.0
 .TP
 .B mergeCmd(args)
 provides merged components
 .INDENT 7.0
 .TP
 .B Parameters
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of item names
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) – list of item names
 .TP
 .B Returns
 XML configuration string with merged components
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -2595,17 +2595,17 @@
 .B recordCmd(ds, name)
 lists datasources of the component
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBds\fP (\fI\%bool\fP) \-\- flag set True for datasources
+\fBds\fP (\fI\%bool\fP) – flag set True for datasources
 .IP \(bu 2
-\fBname\fP (\fI\%str\fP) \-\- given component or datasource
+\fBname\fP (\fI\%str\fP) – given component or datasource
 .UNINDENT
 .TP
 .B Returns
 list of record names
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
@@ -2616,23 +2616,23 @@
 .B showCmd(ds, args, mandatory=False, profiles=False, directory=None)
 shows the DB items
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBds\fP (\fI\%bool\fP) \-\- flag set True for datasources
+\fBds\fP (\fI\%bool\fP) – flag set True for datasources
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of item names
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) – list of item names
 .IP \(bu 2
-\fBmandatory\fP (\fI\%bool\fP) \-\- flag set True for mandatory components
+\fBmandatory\fP (\fI\%bool\fP) – flag set True for mandatory components
 .IP \(bu 2
-\fBprofiles\fP (\fI\%bool\fP) \-\- flag set True for profiles
+\fBprofiles\fP (\fI\%bool\fP) – flag set True for profiles
 .IP \(bu 2
-\fBdirectory\fP (\fI\%str\fP) \-\- output file directory
+\fBdirectory\fP (\fI\%str\fP) – output file directory
 .UNINDENT
 .TP
 .B Returns
 list of XML items
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
@@ -2641,15 +2641,15 @@
 .INDENT 7.0
 .TP
 .B sourcesCmd(components, mandatory=False)
 lists datasources of the components
 .INDENT 7.0
 .TP
 .B Parameters
-\fBcomponents\fP (\fI\%list\fP <\fI\%str\fP>) \-\- given components
+\fBcomponents\fP (\fI\%list\fP <\fI\%str\fP>) – given components
 .TP
 .B Returns
 list of datasource names
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
 .UNINDENT
@@ -2659,27 +2659,27 @@
 .B uploadCmd(ds, args, force=False, profiles=False, directory=\(aq.\(aq, mandatory=False, external=None)
 upload the DB items from files
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBds\fP (\fI\%bool\fP) \-\- flag set True for datasources
+\fBds\fP (\fI\%bool\fP) – flag set True for datasources
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of item names
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) – list of item names
 .IP \(bu 2
-\fBforce\fP (\fI\%bool\fP) \-\- force flag
+\fBforce\fP (\fI\%bool\fP) – force flag
 .IP \(bu 2
-\fBprofiles\fP (\fI\%bool\fP) \-\- flag set True for profiles
+\fBprofiles\fP (\fI\%bool\fP) – flag set True for profiles
 .IP \(bu 2
-\fBdirectory\fP (\fI\%str\fP) \-\- input file directory
+\fBdirectory\fP (\fI\%str\fP) – input file directory
 .IP \(bu 2
-\fBmandatory\fP (\fI\%bool\fP) \-\- mandatory flag
+\fBmandatory\fP (\fI\%bool\fP) – mandatory flag
 .IP \(bu 2
-\fBexternal\fP (\fI\%str\fP) \-\- external import type
+\fBexternal\fP (\fI\%str\fP) – external import type
 .UNINDENT
 .TP
 .B Returns
 list of XML items
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
@@ -2688,15 +2688,15 @@
 .INDENT 7.0
 .TP
 .B variablesCmd(components, mandatory=False)
 lists variable of the components
 .INDENT 7.0
 .TP
 .B Parameters
-\fBcomponents\fP (\fI\%list\fP <\fI\%str\fP>) \-\- given components
+\fBcomponents\fP (\fI\%list\fP <\fI\%str\fP>) – given components
 .TP
 .B Returns
 list of datasource names
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
 .UNINDENT
@@ -2709,15 +2709,15 @@
 .sp
 Data runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -2733,15 +2733,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -2754,15 +2754,15 @@
 .sp
 Show runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -2778,15 +2778,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -2799,15 +2799,15 @@
 .sp
 Describe runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -2823,15 +2823,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -2844,15 +2844,15 @@
 .sp
 List runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -2867,15 +2867,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -2888,15 +2888,15 @@
 .sp
 Get runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -2912,15 +2912,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -2933,15 +2933,15 @@
 .sp
 List runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -2957,15 +2957,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -2978,15 +2978,15 @@
 .sp
 List runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -3002,15 +3002,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -3023,15 +3023,15 @@
 .sp
 Merge runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -3047,15 +3047,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -3068,15 +3068,15 @@
 .sp
 Record runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -3092,15 +3092,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -3113,15 +3113,15 @@
 .sp
 Servers runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -3137,15 +3137,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -3158,15 +3158,15 @@
 .sp
 Show runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -3182,15 +3182,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -3203,15 +3203,15 @@
 .sp
 Sources runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -3227,15 +3227,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -3248,15 +3248,15 @@
 .sp
 Store runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -3272,15 +3272,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -3293,15 +3293,15 @@
 .sp
 Variables runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -3317,15 +3317,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -3346,15 +3346,15 @@
 .sp
 clientds runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 parser creator
 .UNINDENT
 .INDENT 7.0
@@ -3370,30 +3370,30 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxscreate.Comp(parser)
 Bases: \fI\%nxstools.nxsargparser.Runner\fP
 .sp
 comp runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -3409,30 +3409,30 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxscreate.Compare(parser)
 Bases: \fI\%nxstools.nxsargparser.Runner\fP
 .sp
 compare runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -3453,30 +3453,30 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxscreate.DeviceDS(parser)
 Bases: \fI\%nxstools.nxsargparser.Runner\fP
 .sp
 deviceds runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -3492,30 +3492,30 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxscreate.OnlineCP(parser)
 Bases: \fI\%nxstools.nxsargparser.Runner\fP
 .sp
 onlinecp runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -3536,30 +3536,30 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxscreate.OnlineDS(parser)
 Bases: \fI\%nxstools.nxsargparser.Runner\fP
 .sp
 onlineds runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -3580,15 +3580,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.nxscreate.PYTANGO = True
 (\fI\%bool\fP) True if PyTango available
@@ -3600,15 +3600,15 @@
 .sp
 poolds runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -3629,30 +3629,30 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxscreate.StdComp(parser)
 Bases: \fI\%nxstools.nxsargparser.Runner\fP
 .sp
 stdcomp runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -3668,30 +3668,30 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxscreate.TangoDS(parser)
 Bases: \fI\%nxstools.nxsargparser.Runner\fP
 .sp
 tangods runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -3707,15 +3707,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.nxscreate.main()
 the main program function
@@ -3730,15 +3730,15 @@
 .sp
 CloseEntry runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -3753,15 +3753,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -3774,15 +3774,15 @@
 .sp
 CloseFile runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -3797,15 +3797,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -3818,15 +3818,15 @@
 .sp
 configuration server adapter
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
-\fBdevice\fP (\fI\%str\fP) \-\- device name of configuration server
+\fBdevice\fP (\fI\%str\fP) – device name of configuration server
 .UNINDENT
 .INDENT 7.0
 .TP
 .B closeEntry()
 closes the entry
 .UNINDENT
 .INDENT 7.0
@@ -3837,45 +3837,45 @@
 .INDENT 7.0
 .TP
 .B openEntry(xmlconfig)
 opens an entry
 .INDENT 7.0
 .TP
 .B Parameters
-\fBxmlconfig\fP (\fI\%str\fP) \-\- xml configuration string
+\fBxmlconfig\fP (\fI\%str\fP) – xml configuration string
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B openFile(filename)
 opens the h5 file
 .INDENT 7.0
 .TP
 .B Parameters
-\fBfilename\fP (\fI\%str\fP) \-\- h5 file name
+\fBfilename\fP (\fI\%str\fP) – h5 file name
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B record(jsondata)
 records one step
 .INDENT 7.0
 .TP
 .B Parameters
-\fBjsondata\fP (\fI\%str\fP) \-\- step JSON data
+\fBjsondata\fP (\fI\%str\fP) – step JSON data
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B setData(jsondata)
 sets the global JSON data
 .INDENT 7.0
 .TP
 .B Parameters
-\fBjsondata\fP (\fI\%str\fP) \-\- global JSON data
+\fBjsondata\fP (\fI\%str\fP) – global JSON data
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B tdwServer = None
 (\fBPyTango.DeviceProxy\fP) NeXus writer device proxy
 .UNINDENT
@@ -3887,15 +3887,15 @@
 .sp
 OpenEntry runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -3910,15 +3910,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -3931,15 +3931,15 @@
 .sp
 OpenFile runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -3959,15 +3959,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -3980,15 +3980,15 @@
 .sp
 Record runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -4003,15 +4003,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -4024,15 +4024,15 @@
 .sp
 Servers runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -4047,15 +4047,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -4068,15 +4068,15 @@
 .sp
 SetData runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -4091,15 +4091,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -4120,15 +4120,15 @@
 .sp
 add\-recorder\-path runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -4149,30 +4149,30 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxsetup.ChangeProp(parser)
 Bases: \fI\%nxstools.nxsargparser.Runner\fP
 .sp
 change\-prop runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -4188,30 +4188,30 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxsetup.MoveProp(parser)
 Bases: \fI\%nxstools.nxsargparser.Runner\fP
 .sp
 move\-prop runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -4227,30 +4227,30 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxsetup.Restart(parser)
 Bases: \fI\%nxstools.nxsargparser.Runner\fP
 .sp
 restart runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -4266,30 +4266,30 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxsetup.Set(parser)
 Bases: \fI\%nxstools.nxsargparser.Runner\fP
 .sp
 set runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -4305,15 +4305,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxsetup.SetUp
 Bases: \fI\%object\fP
@@ -4326,21 +4326,21 @@
 .B changePropertyName(server, oldname, newname, sclass=None)
 changes property name
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBserver\fP (\fI\%str\fP) \-\- server name
+\fBserver\fP (\fI\%str\fP) – server name
 .IP \(bu 2
-\fBoldname\fP (\fI\%str\fP) \-\- old property name
+\fBoldname\fP (\fI\%str\fP) – old property name
 .IP \(bu 2
-\fBnewname\fP (\fI\%str\fP) \-\- new property name
+\fBnewname\fP (\fI\%str\fP) – new property name
 .IP \(bu 2
-\fBsclass\fP (\fI\%str\fP) \-\- server class name
+\fBsclass\fP (\fI\%str\fP) – server class name
 .UNINDENT
 .TP
 .B Returns
 True if property name was changed
 .TP
 .B Return type
 \fI\%bool\fP
@@ -4351,21 +4351,21 @@
 .B changePropertyValue(server, newname, newvalue, sclass=None)
 changes/sets property value
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBserver\fP (\fI\%str\fP) \-\- server name
+\fBserver\fP (\fI\%str\fP) – server name
 .IP \(bu 2
-\fBnewvalue\fP (\fI\%str\fP) \-\- new property value
+\fBnewvalue\fP (\fI\%str\fP) – new property value
 .IP \(bu 2
-\fBnewname\fP (\fI\%str\fP) \-\- new property name
+\fBnewname\fP (\fI\%str\fP) – new property name
 .IP \(bu 2
-\fBsclass\fP (\fI\%str\fP) \-\- server class name
+\fBsclass\fP (\fI\%str\fP) – server class name
 .UNINDENT
 .TP
 .B Returns
 True if property name was changed
 .TP
 .B Return type
 \fI\%bool\fP
@@ -4376,17 +4376,17 @@
 .B changeRecorderPath(path, instance=None)
 adds a new recorder path
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBpath\fP (\fI\%str\fP) \-\- new recorder path
+\fBpath\fP (\fI\%str\fP) – new recorder path
 .IP \(bu 2
-\fBinstance\fP (\fI\%str\fP) \-\- MacroServer instance name
+\fBinstance\fP (\fI\%str\fP) – MacroServer instance name
 .UNINDENT
 .TP
 .B Returns
 True if record path was added
 .TP
 .B Return type
 \fI\%bool\fP
@@ -4397,19 +4397,19 @@
 .B createConfigServer(beamline, masterhost, jsonsettings=None)
 creates configuration server
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBbeamline\fP (\fI\%str\fP) \-\- beamline name
+\fBbeamline\fP (\fI\%str\fP) – beamline name
 .IP \(bu 2
-\fBmasterhost\fP (\fI\%str\fP) \-\- master host of data writer
+\fBmasterhost\fP (\fI\%str\fP) – master host of data writer
 .IP \(bu 2
-\fBjsonsettings\fP (\fI\%str\fP) \-\- connection settings to DB in json
+\fBjsonsettings\fP (\fI\%str\fP) – connection settings to DB in json
 .UNINDENT
 .TP
 .B Returns
 True if server was created
 .TP
 .B Return type
 \fI\%bool\fP
@@ -4420,17 +4420,17 @@
 .B createDataWriter(beamline, masterhost)
 creates data writer
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBbeamline\fP (\fI\%str\fP) \-\- beamline name
+\fBbeamline\fP (\fI\%str\fP) – beamline name
 .IP \(bu 2
-\fBmasterhost\fP (\fI\%str\fP) \-\- master host of data writer
+\fBmasterhost\fP (\fI\%str\fP) – master host of data writer
 .UNINDENT
 .TP
 .B Returns
 True if server was created
 .TP
 .B Return type
 \fI\%bool\fP
@@ -4441,21 +4441,21 @@
 .B createSelector(beamline, masterhost, writer=None, cserver=None)
 creates selector server
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBbeamline\fP (\fI\%str\fP) \-\- beamline name
+\fBbeamline\fP (\fI\%str\fP) – beamline name
 .IP \(bu 2
-\fBmasterhost\fP (\fI\%str\fP) \-\- master host of data writer
+\fBmasterhost\fP (\fI\%str\fP) – master host of data writer
 .IP \(bu 2
-\fBwriter\fP (\fI\%str\fP) \-\- writer device name
+\fBwriter\fP (\fI\%str\fP) – writer device name
 .IP \(bu 2
-\fBcserver\fP (\fI\%str\fP) \-\- configuration server device name
+\fBcserver\fP (\fI\%str\fP) – configuration server device name
 .UNINDENT
 .TP
 .B Returns
 True if server was created
 .TP
 .B Return type
 \fI\%bool\fP
@@ -4474,15 +4474,15 @@
 .INDENT 7.0
 .TP
 .B getStarterName(host)
 restarts server
 .INDENT 7.0
 .TP
 .B Parameters
-\fBhost\fP (\fI\%str\fP) \-\- server host name
+\fBhost\fP (\fI\%str\fP) – server host name
 .TP
 .B Returns
 starter device name
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -4492,59 +4492,59 @@
 .B restartServer(name, host=None, level=None, restart=True)
 restarts server
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBname\fP (\fI\%str\fP) \-\- server name
+\fBname\fP (\fI\%str\fP) – server name
 .IP \(bu 2
-\fBhost\fP (\fI\%str\fP) \-\- server host name
+\fBhost\fP (\fI\%str\fP) – server host name
 .IP \(bu 2
-\fBlevel\fP (\fI\%int\fP) \-\- start up level
+\fBlevel\fP (\fI\%int\fP) – start up level
 .IP \(bu 2
-\fBrestart\fP (\fI\%bool\fP) \-\- if server should be restarted
+\fBrestart\fP (\fI\%bool\fP) – if server should be restarted
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B stopServer(name, host=None)
 restarts server
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBname\fP (\fI\%str\fP) \-\- server name
+\fBname\fP (\fI\%str\fP) – server name
 .IP \(bu 2
-\fBhost\fP (\fI\%str\fP) \-\- server host name
+\fBhost\fP (\fI\%str\fP) – server host name
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B waitServerNotRunning(server=None, device=None, adminproxy=None, maxcnt=1000, verbose=True, waitforproc=True)
 wait until device is exported and server is running
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBserver\fP (\fI\%str\fP) \-\- server name, check if running when not None
+\fBserver\fP (\fI\%str\fP) – server name, check if running when not None
 .IP \(bu 2
-\fBdevice\fP (\fI\%str\fP) \-\- device name, check if exported when not None
+\fBdevice\fP (\fI\%str\fP) – device name, check if exported when not None
 .IP \(bu 2
-\fBadminproxy\fP (\fI\%tango.DeviceProxy\fP) \-\- Starter device proxy
+\fBadminproxy\fP (\fI\%tango.DeviceProxy\fP) – Starter device proxy
 .IP \(bu 2
-\fBmaxcnt\fP (\fI\%int\fP) \-\- maximal waiting time in 10ms
+\fBmaxcnt\fP (\fI\%int\fP) – maximal waiting time in 10ms
 .IP \(bu 2
-\fBverbose\fP (\fI\%bool\fP) \-\- verbose mode
+\fBverbose\fP (\fI\%bool\fP) – verbose mode
 .IP \(bu 2
-\fBwaitforproc\fP \-\- wait for process list update
+\fBwaitforproc\fP – wait for process list update
 .UNINDENT
 .TP
 .B Returns
 True if server is running
 .TP
 .B Return type
 \fI\%bool\fP
@@ -4555,25 +4555,25 @@
 .B waitServerRunning(server=None, device=None, adminproxy=None, maxcnt=1000, verbose=True, waitforproc=True)
 wait until device is exported and server is running
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBserver\fP (\fI\%str\fP) \-\- server name, check if running when not None
+\fBserver\fP (\fI\%str\fP) – server name, check if running when not None
 .IP \(bu 2
-\fBdevice\fP (\fI\%str\fP) \-\- device name, check if exported when not None
+\fBdevice\fP (\fI\%str\fP) – device name, check if exported when not None
 .IP \(bu 2
-\fBadminproxy\fP (\fI\%tango.DeviceProxy\fP) \-\- Starter device proxy
+\fBadminproxy\fP (\fI\%tango.DeviceProxy\fP) – Starter device proxy
 .IP \(bu 2
-\fBmaxcnt\fP (\fI\%int\fP) \-\- maximal waiting time in 10ms
+\fBmaxcnt\fP (\fI\%int\fP) – maximal waiting time in 10ms
 .IP \(bu 2
-\fBverbose\fP (\fI\%bool\fP) \-\- verbose mode
+\fBverbose\fP (\fI\%bool\fP) – verbose mode
 .IP \(bu 2
-\fBwaitforproc\fP \-\- wait for process list update
+\fBwaitforproc\fP – wait for process list update
 .UNINDENT
 .TP
 .B Returns
 True if server is running
 .TP
 .B Return type
 \fI\%bool\fP
@@ -4592,15 +4592,15 @@
 .sp
 start runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -4616,30 +4616,30 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxsetup.Stop(parser)
 Bases: \fI\%nxstools.nxsargparser.Runner\fP
 .sp
 Stop runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -4655,15 +4655,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.nxsetup.knownHosts = {\(aqcfeld\-pcx27083\(aq: {\(aqbeamline\(aq: \(aqcfeld\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqcfeld\-pcx27083\(aq, \(aquser\(aq: \(aqritzkowf\(aq}, \(aqhas6117b\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhas6117b\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhascmexp\(aq: {\(aqbeamline\(aq: \(aqcmexp\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhascmexp\(aq, \(aquser\(aq: \(aqcmexp\(aq}, \(aqhasdelay\(aq: {\(aqbeamline\(aq: \(aqdelay\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasdelay\(aq, \(aquser\(aq: \(aqdelayusr\(aq}, \(aqhasdelay2\(aq: {\(aqbeamline\(aq: \(aqdelsauto\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasdelay2\(aq, \(aquser\(aq: \(aqdelayusr\(aq}, \(aqhasep211eh\(aq: {\(aqbeamline\(aq: \(aqp211\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep211eh\(aq, \(aquser\(aq: \(aqp211user\(aq}, \(aqhasep212lab\(aq: {\(aqbeamline\(aq: \(aqp21\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep212lab\(aq, \(aquser\(aq: \(aqp212user\(aq}, \(aqhasep212oh\(aq: {\(aqbeamline\(aq: \(aqp21\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep212oh\(aq, \(aquser\(aq: \(aqp212user\(aq}, \(aqhasep22ch1\(aq: {\(aqbeamline\(aq: \(aqp22\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep22ch1\(aq, \(aquser\(aq: \(aqp22user\(aq}, \(aqhasep22ch2\(aq: {\(aqbeamline\(aq: \(aqp22\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep22ch2\(aq, \(aquser\(aq: \(aqp22user\(aq}, \(aqhasep22oh\(aq: {\(aqbeamline\(aq: \(aqp22\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep22oh\(aq, \(aquser\(aq: \(aqp22user\(aq}, \(aqhasep23ch\(aq: {\(aqbeamline\(aq: \(aqp23\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep23ch\(aq, \(aquser\(aq: \(aqp23user\(aq}, \(aqhasep23dev\(aq: {\(aqbeamline\(aq: \(aqp23\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep23dev\(aq, \(aquser\(aq: \(aqp23user\(aq}, \(aqhasep23eh\(aq: {\(aqbeamline\(aq: \(aqp23\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep23eh\(aq, \(aquser\(aq: \(aqp23user\(aq}, \(aqhasep24\(aq: {\(aqbeamline\(aq: \(aqp24\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep24\(aq, \(aquser\(aq: \(aqp24user\(aq}, \(aqhasep24eh1\(aq: {\(aqbeamline\(aq: \(aqp24\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep24eh1\(aq, \(aquser\(aq: \(aqp24user\(aq}, \(aqhasfmirr\(aq: {\(aqbeamline\(aq: \(aqflash\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasfmirr\(aq, \(aquser\(aq: \(aqmusixusr\(aq}, \(aqhasfpgm1\(aq: {\(aqbeamline\(aq: \(aqflash\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasfpgm1\(aq, \(aquser\(aq: \(aqvuvfuser\(aq}, \(aqhasfvls\(aq: {\(aqbeamline\(aq: \(aqflash\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasfvls\(aq, \(aquser\(aq: \(aqvuvfuser\(aq}, \(aqhaskmusixtng\(aq: {\(aqbeamline\(aq: \(aqflash\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaskmusixtng\(aq, \(aquser\(aq: \(aqvuvfuser\(aq}, \(aqhasmfmc\(aq: {\(aqbeamline\(aq: \(aqfmc\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasmfmc\(aq, \(aquser\(aq: \(aqdelayusr\(aq}, \(aqhasmlqj\(aq: {\(aqbeamline\(aq: \(aqlqj\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasmlqj\(aq, \(aquser\(aq: \(aqlqjuser\(aq}, \(aqhasmrixs\(aq: {\(aqbeamline\(aq: \(aqrix\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasmrixs\(aq, \(aquser\(aq: \(aqrixuser\(aq}, \(aqhasnp61ch1\(aq: {\(aqbeamline\(aq: \(aqp61\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasnp61ch1\(aq, \(aquser\(aq: \(aqp61user\(aq}, \(aqhasnp64\(aq: {\(aqbeamline\(aq: \(aqp64\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasnp64\(aq, \(aquser\(aq: \(aqp64user\(aq}, \(aqhasnp64oh\(aq: {\(aqbeamline\(aq: \(aqp64\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasnp64oh\(aq, \(aquser\(aq: \(aqp64user\(aq}, \(aqhasnp65\(aq: {\(aqbeamline\(aq: \(aqp65\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasnp65\(aq, \(aquser\(aq: \(aqp65user\(aq}, \(aqhasnp66\(aq: {\(aqbeamline\(aq: \(aqp66\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasnp66\(aq, \(aquser\(aq: \(aqp66user\(aq}, \(aqhaso107d1\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso107d1\(aq, \(aquser\(aq: \(aqkracht\(aq}, \(aqhaso107klx\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso107klx\(aq, \(aquser\(aq: \(aqkracht\(aq}, \(aqhaso107tk\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso107tk\(aq, \(aquser\(aq: \(aqkracht\(aq}, \(aqhaso111n\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso111n\(aq, \(aquser\(aq: \(aqtnunez\(aq}, \(aqhaso111o\(aq: {\(aqbeamline\(aq: \(aqp09\(aq}, \(aqhaso111tb\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso111tb\(aq, \(aquser\(aq: \(aqtnunez\(aq}, \(aqhaso113b\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso113b\(aq, \(aquser\(aq: \(aqblume\(aq}, \(aqhaso113u\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso113u\(aq, \(aquser\(aq: \(aqkracht\(aq}, \(aqhaso204n\(aq: {\(aqbeamline\(aq: \(aqp23\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso204n\(aq, \(aquser\(aq: \(aqp23user\(aq}, \(aqhaso213p\(aq: {\(aqbeamline\(aq: \(aqp22\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso213p\(aq, \(aquser\(aq: \(aqspiec\(aq}, \(aqhaso224w\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso224w\(aq, \(aquser\(aq: \(aqp021user\(aq}, \(aqhaso228jk\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso228jk\(aq, \(aquser\(aq: \(aqjkotan\(aq}, \(aqhaso232s\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp232s\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhasodlsauto\(aq: {\(aqbeamline\(aq: \(aqdlsauto\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasodlsauto\(aq, \(aquser\(aq: \(aqdlsuser\(aq}, \(aqhasp029rack\(aq: {\(aqbeamline\(aq: \(aqp06\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasp029rack\(aq, \(aquser\(aq: \(aqp06user\(aq}, \(aqhasp068xlab\(aq: {\(aqbeamline\(aq: \(aqp06\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasp068xlab\(aq, \(aquser\(aq: \(aqp06user\(aq}, \(aqhaspecsicl4\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspecsicl4\(aq, \(aquser\(aq: \(aqlacluser\(aq}, \(aqhaspllabcl1\(aq: {\(aqbeamline\(aq: \(aqllab\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspllabcl1\(aq, \(aquser\(aq: \(aqlacluser\(aq}, \(aqhaspp01eh1\(aq: {\(aqbeamline\(aq: \(aqp01\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp01eh1\(aq, \(aquser\(aq: \(aqp01user\(aq}, \(aqhaspp01eh2\(aq: {\(aqbeamline\(aq: \(aqp01\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp01eh2\(aq, \(aquser\(aq: \(aqp01user\(aq}, \(aqhaspp01eh3\(aq: {\(aqbeamline\(aq: \(aqp01\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp01eh3\(aq, \(aquser\(aq: \(aqp01user\(aq}, \(aqhaspp021ch1\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp021ch1\(aq, \(aquser\(aq: \(aqp021user\(aq}, \(aqhaspp021ch1a\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp021ch1a\(aq, \(aquser\(aq: \(aqp021user\(aq}, \(aqhaspp021jenkins\(aq: {\(aqbeamline\(aq: \(aqp021\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp021jenkins\(aq, \(aquser\(aq: \(aqp021user\(aq}, \(aqhaspp022ch\(aq: {\(aqbeamline\(aq: \(aqp022\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp022ch\(aq, \(aquser\(aq: \(aqp022user\(aq}, \(aqhaspp02ch1\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp02ch1\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhaspp02ch1a\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp02ch1a\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhaspp02ch2\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp02ch2\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhaspp02lakl\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp02lakl\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhaspp02oh1\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp02oh1\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhaspp03\(aq: {\(aqbeamline\(aq: \(aqp03\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp03\(aq, \(aquser\(aq: \(aqp03user\(aq}, \(aqhaspp03nano\(aq: {\(aqbeamline\(aq: \(aqp03nano\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp03nano\(aq, \(aquser\(aq: \(aqp03nano\(aq}, \(aqhaspp04exp1\(aq: {\(aqbeamline\(aq: \(aqp04\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp04exp1\(aq, \(aquser\(aq: \(aqp04user\(aq}, \(aqhaspp04exp2\(aq: {\(aqbeamline\(aq: \(aqp04\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp04exp2\(aq, \(aquser\(aq: \(aqp04user\(aq}, \(aqhaspp06ctrl\(aq: {\(aqbeamline\(aq: \(aqp06\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp06ctrl\(aq, \(aquser\(aq: \(aqp06user\(aq}, \(aqhaspp06mc01\(aq: {\(aqbeamline\(aq: \(aqp06\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp06mc01\(aq, \(aquser\(aq: \(aqp06user\(aq}, \(aqhaspp06nc1\(aq: {\(aqbeamline\(aq: \(aqp06\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp06nc1\(aq, \(aquser\(aq: \(aqp06user\(aq}, \(aqhaspp07eh2\(aq: {\(aqbeamline\(aq: \(aqp07\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp07eh2\(aq, \(aquser\(aq: \(aqp07user\(aq}, \(aqhaspp08\(aq: {\(aqbeamline\(aq: \(aqp08\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp08\(aq, \(aquser\(aq: \(aqp08user\(aq}, \(aqhaspp08lisa2\(aq: {\(aqbeamline\(aq: \(aqp08\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp08lisa2\(aq, \(aquser\(aq: \(aqp08user\(aq}, \(aqhaspp09\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp09\(aq, \(aquser\(aq: \(aqp09user\(aq}, \(aqhaspp09dif\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp09dif\(aq, \(aquser\(aq: \(aqp09user\(aq}, \(aqhaspp09haxps\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp09maxps\(aq, \(aquser\(aq: \(aqp09haxps\(aq}, \(aqhaspp09mag\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp09mag\(aq, \(aquser\(aq: \(aqp09user\(aq}, \(aqhaspp10e1\(aq: {\(aqbeamline\(aq: \(aqp10\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp10e1\(aq, \(aquser\(aq: \(aqp10user\(aq}, \(aqhaspp10e2\(aq: {\(aqbeamline\(aq: \(aqp10\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp10e2\(aq, \(aquser\(aq: \(aqp10user\(aq}, \(aqhaspp10lab\(aq: {\(aqbeamline\(aq: \(aqp10\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp10lab\(aq, \(aquser\(aq: \(aqp10user\(aq}, \(aqhaspp10lcx\(aq: {\(aqbeamline\(aq: \(aqp10\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp10lcx\(aq, \(aquser\(aq: \(aqp10user\(aq}, \(aqhaspp11oh\(aq: {\(aqbeamline\(aq: \(aqp11\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp11oh\(aq, \(aquser\(aq: \(aqp11user\(aq}, \(aqhaspp11sardana\(aq: {\(aqbeamline\(aq: \(aqp11\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp11sardana\(aq, \(aquser\(aq: \(aqp11user\(aq}, \(aqhaspp11user02\(aq: {\(aqbeamline\(aq: \(aqp11\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp11user02\(aq, \(aquser\(aq: \(aqp11user\(aq}, \(aqhaspp212oh\(aq: {\(aqbeamline\(aq: \(aqp21\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep212oh\(aq, \(aquser\(aq: \(aqp21user\(aq}, \(aqhaspp21eh2\(aq: {\(aqbeamline\(aq: \(aqp21\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep21eh2\(aq, \(aquser\(aq: \(aqp21user\(aq}, \(aqhaspp21eh3\(aq: {\(aqbeamline\(aq: \(aqp21\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep21eh3\(aq, \(aquser\(aq: \(aqp21user\(aq}, \(aqhaspp21lab\(aq: {\(aqbeamline\(aq: \(aqp21\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp21lab\(aq, \(aquser\(aq: \(aqp21user\(aq}, \(aqhastodt\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhastodt\(aq, \(aquser\(aq: \(aqkracht\(aq}, \(aqhzgpp07eh1\(aq: {\(aqbeamline\(aq: \(aqp07\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhzgpp07eh1\(aq, \(aquser\(aq: \(aqp07user\(aq}, \(aqhzgpp07eh3\(aq: {\(aqbeamline\(aq: \(aqp07\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhzgpp07eh3\(aq, \(aquser\(aq: \(aqp07user\(aq}, \(aqhzgpp07eh4\(aq: {\(aqbeamline\(aq: \(aqp07\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhzgpp07eh4\(aq, \(aquser\(aq: \(aqp07user\(aq}}
 (\fI\%dict\fP <\fI\%dict\fP <\fI\%str\fP , \fI\%str\fP > > )
@@ -4686,19 +4686,19 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+\fBoptions\fP (\fBoptparse.Values\fP) – command options
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP >) \-\- command arguments
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP >) – command arguments
 .IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B components = None
 (\fI\%dict\fP <\fI\%str\fP, \fI\%str\fP >) component xml dictionary
 .UNINDENT
@@ -4745,19 +4745,19 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+\fBoptions\fP (\fBoptparse.Values\fP) – command options
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) \-\- command arguments
+\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) – command arguments
 .IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates a client datasource xml and stores it in DB or filesytem
 .UNINDENT
@@ -4771,19 +4771,19 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+\fBoptions\fP (\fBoptparse.Values\fP) – command options
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) \-\- command arguments
+\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) – command arguments
 .IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B args = None
 (\fI\%list\fP < \fI\%str\fP >) creator arguments
 .UNINDENT
@@ -4806,19 +4806,19 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+\fBoptions\fP (\fBoptparse.Values\fP) – command options
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) \-\- command arguments
+\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) – command arguments
 .IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates a component xml and stores it in DB or filesytem
 .UNINDENT
@@ -4832,19 +4832,19 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+\fBoptions\fP (\fBoptparse.Values\fP) – command options
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) \-\- command arguments
+\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) – command arguments
 .IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B args = None
 (\fI\%list\fP < \fI\%str\fP >) creator arguments
 .UNINDENT
@@ -4886,28 +4886,28 @@
 .B findAttribute(tangohost, clientlike=False)
 sets attribute and datasource group of online.xml device
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBtangohost\fP (\fI\%str\fP) \-\- tango host
+\fBtangohost\fP (\fI\%str\fP) – tango host
 .IP \(bu 2
-\fBclientlike\fP (\fI\%bool\fP) \-\- tango motors to be client like
+\fBclientlike\fP (\fI\%bool\fP) – tango motors to be client like
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B findDevice(tangohost)
 sets sardana device name and sardana host/port of online.xml device
 .INDENT 7.0
 .TP
 .B Parameters
-\fBtangohost\fP (\fI\%str\fP) \-\- tango host
+\fBtangohost\fP (\fI\%str\fP) – tango host
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B group
 (\fI\%str\fP) datasource tango group
 .UNINDENT
@@ -4954,15 +4954,15 @@
 .INDENT 7.0
 .TP
 .B setSardanaName(tolower)
 sets sardana name
 .INDENT 7.0
 .TP
 .B Parameters
-\fBtolower\fP (\fI\%bool\fP) \-\- If True name in lowercase
+\fBtolower\fP (\fI\%bool\fP) – If True name in lowercase
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B shost
 (\fI\%str\fP) sardana host without port
 .UNINDENT
@@ -5006,19 +5006,19 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+\fBoptions\fP (\fBoptparse.Values\fP) – command options
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) \-\- command arguments
+\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) – command arguments
 .IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates a tango datasources xml of given device
 and stores it in DB or filesytem
@@ -5033,19 +5033,19 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+\fBoptions\fP (\fBoptparse.Values\fP) – command options
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) \-\- command arguments
+\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) – command arguments
 .IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B createXMLs()
 creates component xmls of all online.xml complex devices
 .UNINDENT
@@ -5085,19 +5085,19 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+\fBoptions\fP (\fBoptparse.Values\fP) – command options
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP >) \-\- command arguments
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP >) – command arguments
 .IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates datasources of all online.xml simple devices
 .UNINDENT
@@ -5136,19 +5136,19 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+\fBoptions\fP (\fBoptparse.Values\fP) – command options
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP >) \-\- command arguments
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP >) – command arguments
 .IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates datasources of all online.xml simple devices
 .UNINDENT
@@ -5172,19 +5172,19 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+\fBoptions\fP (\fBoptparse.Values\fP) – command options
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) \-\- command arguments
+\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) – command arguments
 .IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B createXMLs()
 creates component xmls of all online.xml complex devices
 .UNINDENT
@@ -5224,19 +5224,19 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+\fBoptions\fP (\fBoptparse.Values\fP) – command options
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) \-\- command arguments
+\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) – command arguments
 .IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates a tango datasource xml and stores it in DB or filesytem
 .UNINDENT
@@ -5258,15 +5258,15 @@
 .sp
 Field runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -5287,15 +5287,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -5305,17 +5305,17 @@
 .B show(root, options)
 the main function
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .IP \(bu 2
-\fBroot\fP (class:\fIfilewriter.FTGroup\fP) \-\- nexus file root
+\fBroot\fP (class:\fIfilewriter.FTGroup\fP) – nexus file root
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxsfileinfo.General(parser)
@@ -5323,15 +5323,15 @@
 .sp
 General runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
@@ -5349,17 +5349,17 @@
 .B classmethod parseentry(entry, description)
 parse entry of nexus file
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBentry\fP (\fBfilewriter.FTGroup\fP) \-\- nexus entry node
+\fBentry\fP (\fBfilewriter.FTGroup\fP) – nexus entry node
 .IP \(bu 2
-\fBdescription\fP (\fI\%list\fP <\fI\%dict\fP <\fI\%str\fP, \fIany\fP > >) \-\- dict description list
+\fBdescription\fP (\fI\%list\fP <\fI\%dict\fP <\fI\%str\fP, \fIany\fP > >) – dict description list
 .UNINDENT
 .TP
 .B Returns
 (key, value) name pair of table headers
 .TP
 .B Return type
 [\fI\%str\fP, \fI\%str\fP]
@@ -5373,15 +5373,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -5389,15 +5389,15 @@
 .INDENT 7.0
 .TP
 .B show(root)
 show general informations
 .INDENT 7.0
 .TP
 .B Parameters
-\fBroot\fP (class:\fIfilewriter.FTGroup\fP) \-\- nexus file root
+\fBroot\fP (class:\fIfilewriter.FTGroup\fP) – nexus file root
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.nxsfileinfo.main()
 the main program function
@@ -5412,29 +5412,29 @@
 .sp
 Metadata parser for NeXus files
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
-\fBroot\fP (\fBfilewriter.FTGroup\fP) \-\- nexus root node
+\fBroot\fP (\fBfilewriter.FTGroup\fP) – nexus root node
 .UNINDENT
 .INDENT 7.0
 .TP
 .B filters = None
 (\fBlist\(ga< :obj:\(gastr\fP>)  filters for \fIfull_path\fP names
 .UNINDENT
 .INDENT 7.0
 .TP
 .B classmethod getpath(path)
 converts full_path with NX_classes into nexus_path
 .INDENT 7.0
 .TP
 .B Parameters
-\fBpath\fP (\fI\%str\fP) \-\- nexus full_path
+\fBpath\fP (\fI\%str\fP) – nexus full_path
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B parse()
 parses the file and creates the filtered description list
 .UNINDENT
@@ -5447,35 +5447,35 @@
 .INDENT 0.0
 .TP
 .B nxstools.nxsfileparser.getdsname(xmlstring)
 provides datasource name from datasource xml string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBxmlstring\fP (\fI\%str\fP) \-\- datasource xml string
+\fBxmlstring\fP (\fI\%str\fP) – datasource xml string
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.nxsfileparser.getdssource(xmlstring)
 provides source from datasource xml string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBxmlstring\fP (\fI\%str\fP) \-\- datasource xml string
+\fBxmlstring\fP (\fI\%str\fP) – datasource xml string
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.nxsfileparser.getdstype(xmlstring)
 provides datasource type from datasource xml string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBxmlstring\fP (\fI\%str\fP) \-\- datasource xml string
+\fBxmlstring\fP (\fI\%str\fP) – datasource xml string
 .UNINDENT
 .UNINDENT
 .SS nxstools.nxsargparser module
 .sp
 NeXus tool argumen parser
 .INDENT 0.0
 .TP
@@ -5491,15 +5491,15 @@
 .sp
 Argument parser with error exception
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
-\fBkwargs\fP \-\- \fI\%argparse.ArgumentParser\fP
+\fBkwargs\fP – \fI\%argparse.ArgumentParser\fP
 parameter dictionary
 .UNINDENT
 .INDENT 7.0
 .TP
 .B createSubParsers()
 creates command\-line parameters parser
 .INDENT 7.0
@@ -5514,30 +5514,30 @@
 .INDENT 7.0
 .TP
 .B error(message)
 error handler
 .INDENT 7.0
 .TP
 .B Parameters
-\fBmessage\fP (\fI\%str\fP) \-\- error message
+\fBmessage\fP (\fI\%str\fP) – error message
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxsargparser.Runner(parser)
 Bases: \fI\%object\fP
 .sp
 abstract runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 parser creator
 .UNINDENT
 .INDENT 7.0
@@ -5558,15 +5558,15 @@
 .INDENT 7.0
 .TP
 .B run(options)
 run commandthe main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .SS nxstools.nxsparser module
 .sp
 Command\-line tool for ascess to the nexdatas configuration server
 .INDENT 0.0
@@ -5580,15 +5580,15 @@
 .INDENT 7.0
 .TP
 .B convert(text)
 converts ESRF xml configuration to nxsdatawriter format
 .INDENT 7.0
 .TP
 .B Parameters
-\fBtext\fP (\fI\%str\fP) \-\- input xml string
+\fBtext\fP (\fI\%str\fP) – input xml string
 .TP
 .B Returns
 output xml string
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -5603,15 +5603,15 @@
 .INDENT 7.0
 .TP
 .B classmethod getRecord(node)
 fetches record name or query from datasource node
 .INDENT 7.0
 .TP
 .B Parameters
-\fBnode\fP (\fBlxml.etree.Element\fP) \-\- datasource node
+\fBnode\fP (\fBlxml.etree.Element\fP) – datasource node
 .TP
 .B Returns
 record name or query
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -5623,15 +5623,15 @@
 .TP
 .B merges the xmls list of definitions xml strings
 to one output xml string
 .UNINDENT
 .INDENT 7.0
 .TP
 .B Parameters
-\fBxmls\fP (\fI\%list\fP <\fI\%str\fP>) \-\- a list of xml string with definitions
+\fBxmls\fP (\fI\%list\fP <\fI\%str\fP>) – a list of xml string with definitions
 .TP
 .B Returns
 one output xml string
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -5639,15 +5639,15 @@
 .INDENT 7.0
 .TP
 .B classmethod parseAttributes(xmlc)
 provides datasources and its records from xml string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBxmlc\fP (\fI\%str\fP) \-\- xml string
+\fBxmlc\fP (\fI\%str\fP) – xml string
 .TP
 .B Returns
 list of datasource descriptions
 .TP
 .B Return type
 \fI\%list\fP < \fI\%dict\fP <\fI\%str\fP, \fIany\fP> >
 .UNINDENT
@@ -5655,15 +5655,15 @@
 .INDENT 7.0
 .TP
 .B classmethod parseDataSources(xmlc)
 provides datasources and its records from xml string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBxmlc\fP (\fI\%str\fP) \-\- xml string
+\fBxmlc\fP (\fI\%str\fP) – xml string
 .TP
 .B Returns
 list of datasource descriptions
 .TP
 .B Return type
 \fI\%list\fP <\fI\%dict\fP <\fI\%str\fP, \fI\%str\fP>>
 .UNINDENT
@@ -5671,15 +5671,15 @@
 .INDENT 7.0
 .TP
 .B classmethod parseFields(xmlc)
 provides datasources and its records from xml string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBxmlc\fP (\fI\%str\fP) \-\- xml string
+\fBxmlc\fP (\fI\%str\fP) – xml string
 .TP
 .B Returns
 list of datasource descriptions
 .TP
 .B Return type
 \fI\%list\fP < \fI\%dict\fP <\fI\%str\fP, \fIany\fP> >
 .UNINDENT
@@ -5687,15 +5687,15 @@
 .INDENT 7.0
 .TP
 .B classmethod parseLinks(xmlc)
 provides datasources and its records from xml string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBxmlc\fP (\fI\%str\fP) \-\- xml string
+\fBxmlc\fP (\fI\%str\fP) – xml string
 .TP
 .B Returns
 list of datasource descriptions
 .TP
 .B Return type
 \fI\%list\fP < \fI\%dict\fP <\fI\%str\fP, \fIany\fP> >
 .UNINDENT
@@ -5703,15 +5703,15 @@
 .INDENT 7.0
 .TP
 .B classmethod parseRecord(xmlc)
 provides source record from xml string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBxmlc\fP (\fI\%str\fP) \-\- xml string
+\fBxmlc\fP (\fI\%str\fP) – xml string
 .TP
 .B Returns
 source record
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -5726,17 +5726,17 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBdescription\fP (\fI\%list\fP <\fI\%str\fP>) \-\- description list
+\fBdescription\fP (\fI\%list\fP <\fI\%str\fP>) – description list
 .IP \(bu 2
-\fBnonone\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of parameters which have to exist to be shown
+\fBnonone\fP (\fI\%list\fP <\fI\%str\fP>) – list of parameters which have to exist to be shown
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B generateList()
 generate row lists of table
 .INDENT 7.0
@@ -5769,21 +5769,21 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBdescription\fP (\fI\%list\fP <\fI\%str\fP>) \-\- description list
+\fBdescription\fP (\fI\%list\fP <\fI\%str\fP>) – description list
 .IP \(bu 2
-\fBnonone\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of parameters which have to exist to be shown
+\fBnonone\fP (\fI\%list\fP <\fI\%str\fP>) – list of parameters which have to exist to be shown
 .IP \(bu 2
-\fBheaders\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of output parameters
+\fBheaders\fP (\fI\%list\fP <\fI\%str\fP>) – list of output parameters
 .IP \(bu 2
-\fBfilters\fP (\fI\%list\fP <\fI\%str\fP>) \-\- filters for first column names
+\fBfilters\fP (\fI\%list\fP <\fI\%str\fP>) – filters for first column names
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B filters = None
 (\fI\%list\fP <\fI\%str\fP>) filter list
 .UNINDENT
@@ -5808,15 +5808,15 @@
 .INDENT 7.0
 .TP
 .B loadDescription(description)
 loads description
 .INDENT 7.0
 .TP
 .B Parameters
-\fBdescription\fP (\fI\%list\fP <\fI\%str\fP>) \-\- description list
+\fBdescription\fP (\fI\%list\fP <\fI\%str\fP>) – description list
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B title = None
 (\fI\%str\fP) table title
 .UNINDENT
@@ -5833,38 +5833,38 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBparent\fP (\fI\%NTag\fP) \-\- parent tag element
+\fBparent\fP (\fI\%NTag\fP) – parent tag element
 .IP \(bu 2
-\fBnameAttr\fP (\fI\%str\fP) \-\- name attribute
+\fBnameAttr\fP (\fI\%str\fP) – name attribute
 .IP \(bu 2
-\fBtypeAttr\fP (\fI\%str\fP) \-\- type attribute
+\fBtypeAttr\fP (\fI\%str\fP) – type attribute
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B setStrategy(mode=\(aqSTEP\(aq, trigger=None, value=None, canfail=None)
 sets the attribute strategy
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBmode\fP (\fI\%str\fP) \-\- mode data writing, i.e. INIT, STEP, FINAL, POSTRUN
+\fBmode\fP (\fI\%str\fP) – mode data writing, i.e. INIT, STEP, FINAL, POSTRUN
 .IP \(bu 2
-\fBtrigger\fP (\fI\%str\fP) \-\- for asynchronous writting,
+\fBtrigger\fP (\fI\%str\fP) – for asynchronous writting,
 e.g. with different subentries
 .IP \(bu 2
-\fBvalue\fP (\fI\%str\fP) \-\- label for postrun mode
+\fBvalue\fP (\fI\%str\fP) – label for postrun mode
 .IP \(bu 2
-\fBcanfail\fP (\fI\%bool\fP) \-\- can fail strategy flag
+\fBcanfail\fP (\fI\%bool\fP) – can fail strategy flag
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxsxml.NDSource(parent)
@@ -5872,99 +5872,99 @@
 .sp
 Source tag wrapper
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparent\fP (\fI\%NTag\fP) \-\- parent tag element
+\fBparent\fP (\fI\%NTag\fP) – parent tag element
 .UNINDENT
 .INDENT 7.0
 .TP
 .B addDoc(doc)
 adds doc tag content
 .INDENT 7.0
 .TP
 .B Parameters
-\fBdoc\fP (\fI\%str\fP) \-\- doc tag content
+\fBdoc\fP (\fI\%str\fP) – doc tag content
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B initClient(name, recordName)
 sets paramters for Client data
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBname\fP (\fI\%str\fP) \-\- name of datasource
+\fBname\fP (\fI\%str\fP) – name of datasource
 .IP \(bu 2
-\fBrecordName\fP (\fI\%str\fP) \-\- name of the data object
+\fBrecordName\fP (\fI\%str\fP) – name of the data object
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B initDBase(name, dbtype, query, dbname=None, rank=None, mycnf=None, user=None, passwd=None, dsn=None, mode=None, host=None, port=None)
 sets parameters of DataBase
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBname\fP (\fI\%str\fP) \-\- name of datasource
+\fBname\fP (\fI\%str\fP) – name of datasource
 .IP \(bu 2
-\fBdbname\fP (\fI\%str\fP) \-\- name of used DataBase
+\fBdbname\fP (\fI\%str\fP) – name of used DataBase
 .IP \(bu 2
-\fBquery\fP (\fI\%str\fP) \-\- database query
+\fBquery\fP (\fI\%str\fP) – database query
 .IP \(bu 2
-\fBdbtype\fP (\fI\%str\fP) \-\- type of the database, i.e. MYSQL, PGSQL, ORACLE
+\fBdbtype\fP (\fI\%str\fP) – type of the database, i.e. MYSQL, PGSQL, ORACLE
 .IP \(bu 2
-\fBrank\fP (\fI\%str\fP) \-\- rank of the query output, i.e. SCALAR, SPECTRUM, IMAGE
+\fBrank\fP (\fI\%str\fP) – rank of the query output, i.e. SCALAR, SPECTRUM, IMAGE
 .IP \(bu 2
-\fBmycnf\fP (\fI\%str\fP) \-\- MYSQL config file
+\fBmycnf\fP (\fI\%str\fP) – MYSQL config file
 .IP \(bu 2
-\fBuser\fP (\fI\%str\fP) \-\- database user name
+\fBuser\fP (\fI\%str\fP) – database user name
 .IP \(bu 2
-\fBpasswd\fP (\fI\%str\fP) \-\- database user password
+\fBpasswd\fP (\fI\%str\fP) – database user password
 .IP \(bu 2
-\fBdsn\fP (\fI\%str\fP) \-\- DSN string to initialize ORACLE and PGSQL databases
+\fBdsn\fP (\fI\%str\fP) – DSN string to initialize ORACLE and PGSQL databases
 .IP \(bu 2
-\fBmode\fP (\fI\%str\fP) \-\- mode for ORACLE databases, i.e. SYSDBA or SYSOPER
+\fBmode\fP (\fI\%str\fP) – mode for ORACLE databases, i.e. SYSDBA or SYSOPER
 .IP \(bu 2
-\fBhost\fP (\fI\%str\fP) \-\- name of the host
+\fBhost\fP (\fI\%str\fP) – name of the host
 .IP \(bu 2
-\fBport\fP (\fI\%str\fP) \-\- port number
+\fBport\fP (\fI\%str\fP) – port number
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B initTango(name, device, memberType, recordName, host=None, port=None, encoding=None, group=None)
 sets paramters for Tango device
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBname\fP (\fI\%str\fP) \-\- name of datasource
+\fBname\fP (\fI\%str\fP) – name of datasource
 .IP \(bu 2
-\fBdevice\fP (\fI\%str\fP) \-\- device name
+\fBdevice\fP (\fI\%str\fP) – device name
 .IP \(bu 2
-\fBmemberType\fP (\fI\%str\fP) \-\- type of the data object, i.e. attribute,
+\fBmemberType\fP (\fI\%str\fP) – type of the data object, i.e. attribute,
 property, command
 .IP \(bu 2
-\fBrecordName\fP (\fI\%str\fP) \-\- name of the data object
+\fBrecordName\fP (\fI\%str\fP) – name of the data object
 .IP \(bu 2
-\fBhost\fP (\fI\%str\fP) \-\- host name
+\fBhost\fP (\fI\%str\fP) – host name
 .IP \(bu 2
-\fBport\fP (\fI\%str\fP) \-\- port
+\fBport\fP (\fI\%str\fP) – port
 .IP \(bu 2
-\fBencoding\fP (\fI\%str\fP) \-\- encoding of DevEncoded data
+\fBencoding\fP (\fI\%str\fP) – encoding of DevEncoded data
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxsxml.NDeviceGroup(parent, deviceName, nameAttr, typeAttr=\(aq\(aq, commands=True, blackAttrs=None)
@@ -5974,25 +5974,25 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBparent\fP (\fI\%NTag\fP) \-\- parent tag element
+\fBparent\fP (\fI\%NTag\fP) – parent tag element
 .IP \(bu 2
-\fBdeviceName\fP (\fI\%str\fP) \-\- tango device name
+\fBdeviceName\fP (\fI\%str\fP) – tango device name
 .IP \(bu 2
-\fBnameAttr\fP (\fI\%str\fP) \-\- name attribute
+\fBnameAttr\fP (\fI\%str\fP) – name attribute
 .IP \(bu 2
-\fBtypeAttr\fP (\fI\%str\fP) \-\- type attribute
+\fBtypeAttr\fP (\fI\%str\fP) – type attribute
 .IP \(bu 2
-\fBcommands\fP (\fI\%bool\fP) \-\- if we call the commands
+\fBcommands\fP (\fI\%bool\fP) – if we call the commands
 .IP \(bu 2
-\fBblackAttrs\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of excluded attributes
+\fBblackAttrs\fP (\fI\%list\fP <\fI\%str\fP>) – list of excluded attributes
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B nTypes = [\(aqNX_CHAR\(aq, \(aqNX_BOOLEAN\(aq, \(aqNX_INT32\(aq, \(aqNX_INT32\(aq, \(aqNX_FLOAT32\(aq, \(aqNX_FLOAT64\(aq, \(aqNX_UINT32\(aq, \(aqNX_UINT32\(aq, \(aqNX_CHAR\(aq, \(aqNX_CHAR\(aq, \(aqNX_INT32\(aq, \(aqNX_INT32\(aq, \(aqNX_FLOAT32\(aq, \(aqNX_FLOAT64\(aq, \(aqNX_UINT32\(aq, \(aqNX_UINT32\(aq, \(aqNX_CHAR\(aq, \(aqNX_CHAR\(aq, \(aqNX_CHAR\(aq, \(aqNX_CHAR\(aq, \(aqNX_CHAR\(aq, \(aqNX_BOOLEAN\(aq, \(aqNX_CHAR\(aq, \(aqNX_INT64\(aq, \(aqNX_UINT64\(aq, \(aqNX_INT64\(aq, \(aqNX_UINT64\(aq, \(aqNX_INT32\(aq, \(aqNX_CHAR\(aq]
 (\fI\%list\fP <\fI\%str\fP>) NeXuS types corresponding to the Tango types
 .UNINDENT
@@ -6011,19 +6011,19 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBparent\fP (\fI\%NTag\fP) \-\- parent tag element
+\fBparent\fP (\fI\%NTag\fP) – parent tag element
 .IP \(bu 2
-\fBindexAttr\fP (\fI\%str\fP) \-\- index attribute
+\fBindexAttr\fP (\fI\%str\fP) – index attribute
 .IP \(bu 2
-\fBvalueAttr\fP (\fI\%str\fP) \-\- value attribute
+\fBvalueAttr\fP (\fI\%str\fP) – value attribute
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxsxml.NDimensions(parent, rankAttr)
 Bases: \fI\%nxstools.nxsxml.NTag\fP
@@ -6032,31 +6032,31 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBparent\fP (\fI\%NTag\fP) \-\- parent tag element
+\fBparent\fP (\fI\%NTag\fP) – parent tag element
 .IP \(bu 2
-\fBrankAttr\fP (\fI\%str\fP) \-\- rank attribute
+\fBrankAttr\fP (\fI\%str\fP) – rank attribute
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B dim(indexAttr, valueAttr)
 adds dim tag
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBindexAttr\fP (\fI\%str\fP) \-\- index attribute
+\fBindexAttr\fP (\fI\%str\fP) – index attribute
 .IP \(bu 2
-\fBvalueAttr\fP (\fI\%str\fP) \-\- value attribute
+\fBvalueAttr\fP (\fI\%str\fP) – value attribute
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B dims = None
 (\fI\%dict\fP <\fI\%str\fP, \fI\%NDim\fP>)
@@ -6072,84 +6072,84 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBparent\fP (\fI\%NTag\fP) \-\- parent tag element
+\fBparent\fP (\fI\%NTag\fP) – parent tag element
 .IP \(bu 2
-\fBnameAttr\fP (\fI\%str\fP) \-\- name attribute
+\fBnameAttr\fP (\fI\%str\fP) – name attribute
 .IP \(bu 2
-\fBtypeAttr\fP (\fI\%str\fP) \-\- type attribute
+\fBtypeAttr\fP (\fI\%str\fP) – type attribute
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B addAttr(attrName, attrType, attrValue=\(aq\(aq)
 adds attribute tag
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBattrName\fP (\fI\%str\fP) \-\- name attribute
+\fBattrName\fP (\fI\%str\fP) – name attribute
 .IP \(bu 2
-\fBattrType\fP (\fI\%str\fP) \-\- type attribute
+\fBattrType\fP (\fI\%str\fP) – type attribute
 .IP \(bu 2
-\fBattrValue\fP (\fI\%str\fP) \-\- content of the attribute tag
+\fBattrValue\fP (\fI\%str\fP) – content of the attribute tag
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B addDoc(doc)
 adds doc tag content
 .INDENT 7.0
 .TP
 .B Parameters
-\fBdoc\fP (\fI\%str\fP) \-\- doc tag content
+\fBdoc\fP (\fI\%str\fP) – doc tag content
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B setStrategy(mode=\(aqSTEP\(aq, trigger=None, value=None, grows=None, compression=False, rate=None, shuffle=None, canfail=None, compression_opts=None)
 sets the field strategy
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBmode\fP (\fI\%str\fP) \-\- mode data writing, i.e. INIT, STEP, FINAL, POSTRUN
+\fBmode\fP (\fI\%str\fP) – mode data writing, i.e. INIT, STEP, FINAL, POSTRUN
 .IP \(bu 2
-\fBtrigger\fP (\fI\%str\fP) \-\- for asynchronous writting,
+\fBtrigger\fP (\fI\%str\fP) – for asynchronous writting,
 e.g. with different subentries
 .IP \(bu 2
-\fBvalue\fP (\fI\%str\fP) \-\- label for postrun mode
+\fBvalue\fP (\fI\%str\fP) – label for postrun mode
 .IP \(bu 2
-\fBgrows\fP (\fI\%str\fP) \-\- growing dimension
+\fBgrows\fP (\fI\%str\fP) – growing dimension
 .IP \(bu 2
-\fBcompression\fP (\fI\%str\fP) \-\- flag if compression shuold be applied
+\fBcompression\fP (\fI\%str\fP) – flag if compression shuold be applied
 .IP \(bu 2
-\fBrate\fP (\fI\%str\fP) \-\- compression rate
+\fBrate\fP (\fI\%str\fP) – compression rate
 .IP \(bu 2
-\fBshuffle\fP (\fI\%str\fP) \-\- flag if compression shuffle
+\fBshuffle\fP (\fI\%str\fP) – flag if compression shuffle
 .IP \(bu 2
-\fBcanfail\fP (\fI\%bool\fP) \-\- can fail strategy flag
+\fBcanfail\fP (\fI\%bool\fP) – can fail strategy flag
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B setUnits(unitsAttr)
 sets the field unit
 .INDENT 7.0
 .TP
 .B Parameters
-\fBunitsAttr\fP (\fI\%str\fP) \-\- the field unit
+\fBunitsAttr\fP (\fI\%str\fP) – the field unit
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxsxml.NGroup(parent, nameAttr, typeAttr=\(aq\(aq)
 Bases: \fI\%nxstools.nxsxml.NTag\fP
@@ -6158,46 +6158,46 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBparent\fP (\fI\%NTag\fP) \-\- parent tag element
+\fBparent\fP (\fI\%NTag\fP) – parent tag element
 .IP \(bu 2
-\fBnameAttr\fP (\fI\%str\fP) \-\- name attribute
+\fBnameAttr\fP (\fI\%str\fP) – name attribute
 .IP \(bu 2
-\fBtypeAttr\fP (\fI\%str\fP) \-\- type attribute
+\fBtypeAttr\fP (\fI\%str\fP) – type attribute
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B addAttr(attrName, attrType, attrValue=\(aq\(aq)
 adds attribute: tag
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBattrName\fP (\fI\%str\fP) \-\- name attribute
+\fBattrName\fP (\fI\%str\fP) – name attribute
 .IP \(bu 2
-\fBattrType\fP (\fI\%str\fP) \-\- type attribute
+\fBattrType\fP (\fI\%str\fP) – type attribute
 .IP \(bu 2
-\fBattrValue\fP (\fI\%str\fP) \-\- content of the attribute tag
+\fBattrValue\fP (\fI\%str\fP) – content of the attribute tag
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B addDoc(doc)
 adds doc tag content
 .INDENT 7.0
 .TP
 .B Parameters
-\fBdoc\fP (\fI\%str\fP) \-\- doc tag content
+\fBdoc\fP (\fI\%str\fP) – doc tag content
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxsxml.NLink(parent, nameAttr, gTarget)
 Bases: \fI\%nxstools.nxsxml.NTag\fP
@@ -6206,29 +6206,29 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBparent\fP (\fI\%NTag\fP) \-\- parent tag element
+\fBparent\fP (\fI\%NTag\fP) – parent tag element
 .IP \(bu 2
-\fBnameAttr\fP (\fI\%str\fP) \-\- name attribute
+\fBnameAttr\fP (\fI\%str\fP) – name attribute
 .IP \(bu 2
-\fBgTarget\fP (\fI\%str\fP) \-\- target attribute
+\fBgTarget\fP (\fI\%str\fP) – target attribute
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B addDoc(doc)
 adds doc tag content
 .INDENT 7.0
 .TP
 .B Parameters
-\fBdoc\fP (\fI\%str\fP) \-\- doc tag content
+\fBdoc\fP (\fI\%str\fP) – doc tag content
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxsxml.NTag(parent, tagName, nameAttr=\(aq\(aq, typeAttr=\(aq\(aq)
 Bases: \fI\%object\fP
@@ -6237,76 +6237,76 @@
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBparent\fP (\fI\%NTag\fP) \-\- parent tag element
+\fBparent\fP (\fI\%NTag\fP) – parent tag element
 .IP \(bu 2
-\fBtagName\fP (\fI\%str\fP) \-\- tag name
+\fBtagName\fP (\fI\%str\fP) – tag name
 .IP \(bu 2
-\fBnameAttr\fP (\fI\%str\fP) \-\- value of name attribute
+\fBnameAttr\fP (\fI\%str\fP) – value of name attribute
 .IP \(bu 2
-\fBtypeAttr\fP (\fI\%str\fP) \-\- value of type attribute
+\fBtypeAttr\fP (\fI\%str\fP) – value of type attribute
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B addTagAttr(name, value)
 adds tag attribute
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBname\fP (\fI\%str\fP) \-\- attribute name
+\fBname\fP (\fI\%str\fP) – attribute name
 .IP \(bu 2
-\fBvalue\fP (\fI\%str\fP) \-\- attribute value
+\fBvalue\fP (\fI\%str\fP) – attribute value
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B addText(text)
 adds tag content
 .INDENT 7.0
 .TP
 .B Parameters
-\fBtext\fP (\fI\%str\fP) \-\- tag content
+\fBtext\fP (\fI\%str\fP) – tag content
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B elem = None
 (\fBlxml.etree.Element\fP) tag element from etree
 .UNINDENT
 .INDENT 7.0
 .TP
 .B setText(text)
 sets tag content
 .INDENT 7.0
 .TP
 .B Parameters
-\fBtext\fP (\fI\%str\fP) \-\- tag content
+\fBtext\fP (\fI\%str\fP) – tag content
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B class nxstools.nxsxml.XMLFile(fname)
 Bases: \fI\%object\fP
 .sp
 XML file object
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
-\fBfname\fP (\fI\%str\fP) \-\- XML file name
+\fBfname\fP (\fI\%str\fP) – XML file name
 .UNINDENT
 .INDENT 7.0
 .TP
 .B dump()
 dumps XML structure into the XML file
 .INDENT 7.0
 .TP
@@ -6327,15 +6327,15 @@
 .INDENT 7.0
 .TP
 .B prettyPrint(etNode=None)
 prints pretty XML making use of etree
 .INDENT 7.0
 .TP
 .B Parameters
-\fBetNode\fP (\fBlxml.etree.Element\fP) \-\- node
+\fBetNode\fP (\fBlxml.etree.Element\fP) – node
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.nxsxml.main()
 the main function
@@ -6355,35 +6355,35 @@
 .sp
 xml templates package loader
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
-\fBpackagename\fP (\fI\%str\fP) \-\- full package name
+\fBpackagename\fP (\fI\%str\fP) – full package name
 .UNINDENT
 .INDENT 7.0
 .TP
 .B loadXMLTemplates(packagename)
 load xml template module variables
 .INDENT 7.0
 .TP
 .B Parameters
-\fBpackagename\fP (\fI\%str\fP) \-\- full package name
+\fBpackagename\fP (\fI\%str\fP) – full package name
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.nxsdevicetools.checkServer(name=\(aqNXSConfigServer\(aq)
 provides server device name if only one or error in the other case
 .INDENT 7.0
 .TP
 .B Parameters
-\fBname\fP (\fI\%str\fP) \-\- server name
+\fBname\fP (\fI\%str\fP) – server name
 .TP
 .B Returns
 server device name or empty string if error appears
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -6396,15 +6396,15 @@
 .INDENT 0.0
 .TP
 .B nxstools.nxsdevicetools.findClassName(server, name)
 finds class name
 .INDENT 7.0
 .TP
 .B Parameters
-\fBname\fP (\fI\%str\fP) \-\- device name
+\fBname\fP (\fI\%str\fP) – device name
 .TP
 .B Returns
 class name
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -6414,19 +6414,19 @@
 .B nxstools.nxsdevicetools.generateDeviceNames(prefix, first, last, minimal=False)
 generates device names
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBprefix\fP (\fI\%str\fP) \-\- device name prefix
+\fBprefix\fP (\fI\%str\fP) – device name prefix
 .IP \(bu 2
-\fBfirst\fP (\fI\%int\fP) \-\- first device index
+\fBfirst\fP (\fI\%int\fP) – first device index
 .IP \(bu 2
-\fBlast\fP (\fI\%int\fP) \-\- last device index
+\fBlast\fP (\fI\%int\fP) – last device index
 .UNINDENT
 .TP
 .B Returns
 device names
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
@@ -6437,19 +6437,19 @@
 .B nxstools.nxsdevicetools.getAttributes(device, host=None, port=10000)
 provides a list of device attributes
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBdevice\fP (\fI\%str\fP) \-\- tango device name
+\fBdevice\fP (\fI\%str\fP) – tango device name
 .IP \(bu 2
-\fBhost\fP (\fI\%str\fP) \-\- device host
+\fBhost\fP (\fI\%str\fP) – device host
 .IP \(bu 2
-\fBport\fP (\fI\%int\fP) \-\- device port
+\fBport\fP (\fI\%int\fP) – device port
 .UNINDENT
 .TP
 .B Returns
 list of device attributes
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
@@ -6458,15 +6458,15 @@
 .INDENT 0.0
 .TP
 .B nxstools.nxsdevicetools.getClassName(devicename)
 provides device class name
 .INDENT 7.0
 .TP
 .B Parameters
-\fBdevicename\fP (\fI\%str\fP) \-\- device name
+\fBdevicename\fP (\fI\%str\fP) – device name
 .TP
 .B Returns
 class name
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -6476,17 +6476,17 @@
 .B nxstools.nxsdevicetools.getDataSourceComponents(server, verbose=False)
 gets datasource components
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBserver\fP (\fI\%str\fP) \-\- configuration server
+\fBserver\fP (\fI\%str\fP) – configuration server
 .IP \(bu 2
-\fBverbose\fP (\fI\%bool\fP) \-\- additional printouts
+\fBverbose\fP (\fI\%bool\fP) – additional printouts
 .UNINDENT
 .TP
 .B Returns
 dictionary with datasource components
 .TP
 .B Return type
 \fI\%dict\fP <\fI\%str\fP, \fI\%list\fP <\fI\%str\fP>>
@@ -6495,15 +6495,15 @@
 .INDENT 0.0
 .TP
 .B nxstools.nxsdevicetools.getServerTangoHost(server)
 fetches the server tango_host:tango_port
 .INDENT 7.0
 .TP
 .B Parameters
-\fBserver\fP (\fI\%str\fP) \-\- tango server
+\fBserver\fP (\fI\%str\fP) – tango server
 .TP
 .B Returns
 tango host
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -6511,15 +6511,15 @@
 .INDENT 0.0
 .TP
 .B nxstools.nxsdevicetools.getServers(name=\(aqNXSConfigServer\(aq)
 provides server device names
 .INDENT 7.0
 .TP
 .B Parameters
-\fBname\fP (\fI\%str\fP) \-\- server instance name
+\fBname\fP (\fI\%str\fP) – server instance name
 .TP
 .B Returns
 list of the server device names
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
 .UNINDENT
@@ -6532,15 +6532,15 @@
 .INDENT 0.0
 .TP
 .B nxstools.nxsdevicetools.listServers(server, name=\(aqNXSConfigServer\(aq)
 finds server names
 .INDENT 7.0
 .TP
 .B Parameters
-\fBname\fP (\fI\%str\fP) \-\- server instance name
+\fBname\fP (\fI\%str\fP) – server instance name
 .TP
 .B Returns
 server list
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
 .UNINDENT
@@ -6549,15 +6549,15 @@
 .TP
 .B nxstools.nxsdevicetools.moduleMultiAttributes = {\(aqdalsa\(aq: [\(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileSaving\(aq, \(aqFileStartNum\(aq, \(aqTriggerMode\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqExtendedExposure\(aq, \(aqBinComment\(aq, \(aqFramesProcessed\(aq, \(aqImage16\(aq, \(aqImage8\(aq, \(aqImageRaw\(aq, \(aqFramesReceived\(aq, \(aqFrameRate\(aq, \(aqFramesPerNXFile\(aq, \(aqNXFileCompression\(aq, \(aqTurboMode\(aq, \(aqImageEnc\(aq, \(aqViewingMode\(aq, \(aqThrashedBuffers\(aq, \(aqFramesToAcquire\(aq, \(aqAcquisitionFrameCount\(aq, \(aqAcquisitionMode\(aq, \(aqAcquisitionFrameMode\(aq, \(aqLinearityEqualizer\(aq, \(aqNrExposedFrames\(aq, \(aqNrOffsetFrames\(aq, \(aqOffset\(aq, \(aqPixelFormat\(aq, \(aqReadOutMode\(aq, \(aqStandby\(aq, \(aqSumScheme\(aq], \(aqeigerdectris\(aq: [\(aqTriggerMode\(aq, \(aqNbTriggers\(aq, \(aqDescription\(aq, \(aqNbImages\(aq, \(aqBitDepth\(aq, \(aqReadoutTime\(aq, \(aqCountTime\(aq, \(aqEnergyThreshold\(aq, \(aqFrameTime\(aq, \(aqRateCorrectionEnabled\(aq, \(aqFlatFieldEnabled\(aq, \(aqTemperature\(aq, \(aqAutoSummationEnabled\(aq, \(aqHumidity\(aq, \(aqPhotonEnergy\(aq, \(aqWavelength\(aq], \(aqlambda\(aq: [\(aqTriggerMode\(aq, \(aqShutterTime\(aq, \(aqDelayTime\(aq, \(aqFrameNumbers\(aq, \(aqThreadNo\(aq, \(aqEnergyThreshold\(aq, \(aqOperatingMode\(aq, \(aqConfigFilePath\(aq, \(aqSaveAllImages\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqFilePreExt\(aq, \(aqFilePostfix\(aq, \(aqSaveFilePath\(aq, \(aqSaveFileName\(aq, \(aqLatestImageNumber\(aq, \(aqLiveMode\(aq, \(aqTotalLossFrames\(aq, \(aqCompressorShuffle\(aq, \(aqCompressionRate\(aq, \(aqCompressionEnabled\(aq, \(aqLayout\(aq, \(aqShutterTimeMax\(aq, \(aqShutterTimeMin\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqDepth\(aq, \(aqLiveFrameNo\(aq, \(aqDistortionCorrection\(aq, \(aqLiveLastImageData\(aq, \(aqFramesPerFile\(aq, \(aqOpMode\(aq], \(aqlambda2m\(aq: [\(aqTriggerMode\(aq, \(aqShutterTime\(aq, \(aqDelayTime\(aq, \(aqFrameNumbers\(aq, \(aqThreadNo\(aq, \(aqEnergyThreshold\(aq, \(aqOperatingMode\(aq, \(aqConfigFilePath\(aq, \(aqSaveAllImages\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqFilePreExt\(aq, \(aqFilePostfix\(aq, \(aqSaveFilePath\(aq, \(aqSaveFileName\(aq, \(aqLatestImageNumber\(aq, \(aqLiveMode\(aq, \(aqTotalLossFrames\(aq, \(aqCompressorShuffle\(aq, \(aqCompressionRate\(aq, \(aqCompressionEnabled\(aq, \(aqLayout\(aq, \(aqShutterTimeMax\(aq, \(aqShutterTimeMin\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqDepth\(aq, \(aqLiveFrameNo\(aq, \(aqDistortionCorrection\(aq, \(aqLiveLastImageData\(aq, \(aqOpMode\(aq], \(aqlambdavds\(aq: [\(aqTriggerMode\(aq, \(aqShutterTime\(aq, \(aqDelayTime\(aq, \(aqFrameNumbers\(aq, \(aqThreadNo\(aq, \(aqEnergyThreshold\(aq, \(aqOperatingMode\(aq, \(aqConfigFilePath\(aq, \(aqSaveAllImages\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqFilePreExt\(aq, \(aqFilePostfix\(aq, \(aqSaveFilePath\(aq, \(aqSaveFileName\(aq, \(aqLatestImageNumber\(aq, \(aqLiveMode\(aq, \(aqTotalLossFrames\(aq, \(aqCompressorShuffle\(aq, \(aqCompressionRate\(aq, \(aqCompressionEnabled\(aq, \(aqLayout\(aq, \(aqShutterTimeMax\(aq, \(aqShutterTimeMin\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqDepth\(aq, \(aqLiveFrameNo\(aq, \(aqDistortionCorrection\(aq, \(aqLiveLastImageData\(aq, \(aqFramesPerFile\(aq, \(aqOpMode\(aq], \(aqlimaccd\(aq: [\(aqcamera_type\(aq, \(aqcamera_pixelsize\(aq, \(aqcamera_model\(aq, \(aqacq_mode\(aq, \(aqacq_nb_frames\(aq, \(aqacq_trigger_mode\(aq, \(aqlast_image_saved\(aq, \(aqlatency_time\(aq, \(aqacc_max_expo_time\(aq, \(aqacc_expo_time\(aq, \(aqacc_time_mode\(aq, \(aqacc_dead_time\(aq, \(aqacc_live_time\(aq, \(aqsaving_mode\(aq, \(aqsaving_directory\(aq, \(aqsaving_prefix\(aq, \(aqsaving_suffix\(aq, \(aqsaving_next_number\(aq, \(aqsaving_format\(aq, \(aqsaving_frame_per_file\(aq, \(aqimage_type\(aq, \(aqimage_width\(aq, \(aqimage_height\(aq, \(aqimage_sizes\(aq, \(aqimage_roi\(aq, \(aqimage_bin\(aq, \(aqimage_flip\(aq, \(aqimage_rotation\(aq, \(aqshutter_mode\(aq, \(aqshutter_open_time\(aq], \(aqlimaccds\(aq: [\(aqcamera_type\(aq, \(aqcamera_pixelsize\(aq, \(aqcamera_model\(aq, \(aqacq_mode\(aq, \(aqacq_nb_frames\(aq, \(aqacq_trigger_mode\(aq, \(aqlast_image_saved\(aq, \(aqlatency_time\(aq, \(aqacc_max_expo_time\(aq, \(aqacc_expo_time\(aq, \(aqacc_time_mode\(aq, \(aqacc_dead_time\(aq, \(aqacc_live_time\(aq, \(aqsaving_mode\(aq, \(aqsaving_directory\(aq, \(aqsaving_prefix\(aq, \(aqsaving_suffix\(aq, \(aqsaving_next_number\(aq, \(aqsaving_format\(aq, \(aqsaving_frame_per_file\(aq, \(aqimage_type\(aq, \(aqimage_width\(aq, \(aqimage_height\(aq, \(aqimage_sizes\(aq, \(aqimage_roi\(aq, \(aqimage_bin\(aq, \(aqimage_flip\(aq, \(aqimage_rotation\(aq, \(aqshutter_mode\(aq, \(aqshutter_open_time\(aq], \(aqmaiadimension\(aq: [\(aqName\(aq, \(aqPositionSource\(aq, \(aqPixelPitch\(aq, \(aqPixelOrigin\(aq, \(aqPixelHysteresis\(aq, \(aqPositionUnit\(aq, \(aqPixelCoordExtent\(aq], \(aqmaiaflux\(aq: [\(aqFluxCoeff\(aq, \(aqFluxName\(aq, \(aqFluxUnit\(aq, \(aqFluxSource\(aq], \(aqmaiainterlock\(aq: [\(aqBiasPeltierInterlock\(aq, \(aqBiasPeltierInterlockUptime\(aq, \(aqPressure\(aq], \(aqmaialogger\(aq: [\(aqRunNumber\(aq], \(aqmaiaprocessing\(aq: [\(aqGaintrimEnable\(aq, \(aqLineariseEnable\(aq, \(aqPhotonEnable\(aq, \(aqPileupRejectEnable\(aq, \(aqPixelEnable\(aq, \(aqThrottleEnable\(aq], \(aqmaiasensor\(aq: [\(aqBiasVoltage\(aq, \(aqLeakageCurrent\(aq, \(aqPeltierCurrent\(aq, \(aqWaterTemperature\(aq, \(aqDetectorTemperature\(aq, \(aqMosfetTemperature\(aq, \(aqIdentity\(aq], \(aqmarccd\(aq: [\(aqFrameShift\(aq, \(aqSavingDirectory\(aq, \(aqSavingPostfix\(aq, \(aqSavingPrefix\(aq], \(aqmca_xia\(aq: [\(aqICR\(aq, \(aqOCR\(aq], \(aqmca_xia@pool\(aq: [\(aqCountsRoI\(aq, \(aqRoIEnd\(aq, \(aqRoIStart\(aq], \(aqmythen\(aq: [\(aqCounts1\(aq, \(aqCounts2\(aq, \(aqCountsMax\(aq, \(aqCountsTotal\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFileIndex\(aq, \(aqFilePrefix\(aq, \(aqData\(aq, \(aqRoI1\(aq, \(aqRoI2\(aq], \(aqmythen2\(aq: [\(aqCounts1\(aq, \(aqCounts2\(aq, \(aqCountsMax\(aq, \(aqCountsTotal\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFileIndex\(aq, \(aqFilePrefix\(aq, \(aqData\(aq, \(aqEnergy\(aq, \(aqNbFrames\(aq, \(aqRoI1End\(aq, \(aqRoI2End\(aq, \(aqRoI1Start\(aq, \(aqRoI2Start\(aq, \(aqThreshold\(aq], \(aqpco\(aq: [\(aqDelayTime\(aq, \(aqExposureTime\(aq, \(aqNbFrames\(aq, \(aqTriggerMode\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqBinning_x\(aq, \(aqBinning_y\(aq, \(aqROI_x_min\(aq, \(aqROI_x_max\(aq, \(aqROI_y_min\(aq, \(aqROI_y_max\(aq, \(aqPixelrate\(aq, \(aqADCs\(aq, \(aqCoolingTemp\(aq, \(aqCoolingTempSet\(aq, \(aqImageTimeStamp\(aq, \(aqRecorderMode\(aq], \(aqpco4000\(aq: [\(aqDelayTime\(aq, \(aqExposureTime\(aq, \(aqNbFrames\(aq, \(aqTriggerMode\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqBinning_x\(aq, \(aqBinning_y\(aq, \(aqROI_x_min\(aq, \(aqROI_x_max\(aq, \(aqROI_y_min\(aq, \(aqROI_y_max\(aq, \(aqPixelrate\(aq, \(aqADCs\(aq, \(aqCoolingTemp\(aq, \(aqCoolingTempSet\(aq, \(aqImageTimeStamp\(aq, \(aqRecorderMode\(aq], \(aqpcoedge\(aq: [\(aqDelayTime\(aq, \(aqExposureTime\(aq, \(aqNbFrames\(aq, \(aqTriggerMode\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqBinning_x\(aq, \(aqBinning_y\(aq, \(aqROI_x_min\(aq, \(aqROI_x_max\(aq, \(aqROI_y_min\(aq, \(aqROI_y_max\(aq, \(aqPixelrate\(aq, \(aqADCs\(aq, \(aqCoolingTemp\(aq, \(aqCoolingTempSet\(aq, \(aqImageTimeStamp\(aq, \(aqRecorderMode\(aq], \(aqpedetector\(aq: [\(aqBinningMode\(aq, \(aqFileIndex\(aq, \(aqExposureTime\(aq, \(aqSkippedAtStart\(aq, \(aqSummedSaveImages\(aq, \(aqSkippedBetweenSaved\(aq, \(aqFilesAfterTrigger\(aq, \(aqFilesBeforeTrigger\(aq, \(aqSummedDarkImages\(aq, \(aqOutputDirectory\(aq, \(aqFilePattern\(aq, \(aqFileName\(aq, \(aqLogFile\(aq, \(aqUserComment1\(aq, \(aqCameraGain\(aq, \(aqUserComment2\(aq, \(aqUserComment3\(aq, \(aqUserComment4\(aq, \(aqSaveRawImages\(aq, \(aqSaveDarkImages\(aq, \(aqPerformIntegration\(aq, \(aqSaveIntegratedData\(aq, \(aqSaveSubtracted\(aq, \(aqPerformDarkSubtraction\(aq], \(aqperkinelmer\(aq: [\(aqBinningMode\(aq, \(aqFileIndex\(aq, \(aqExposureTime\(aq, \(aqSkippedAtStart\(aq, \(aqSummedSaveImages\(aq, \(aqSkippedBetweenSaved\(aq, \(aqFilesAfterTrigger\(aq, \(aqFilesBeforeTrigger\(aq, \(aqSummedDarkImages\(aq, \(aqOutputDirectory\(aq, \(aqFilePattern\(aq, \(aqFileName\(aq, \(aqLogFile\(aq, \(aqUserComment1\(aq, \(aqCameraGain\(aq, \(aqUserComment2\(aq, \(aqUserComment3\(aq, \(aqUserComment4\(aq, \(aqSaveRawImages\(aq, \(aqSaveDarkImages\(aq, \(aqPerformIntegration\(aq, \(aqSaveIntegratedData\(aq, \(aqSaveSubtracted\(aq, \(aqPerformDarkSubtraction\(aq], \(aqperkinelmerdetector\(aq: [\(aqBinningMode\(aq, \(aqFileIndex\(aq, \(aqExposureTime\(aq, \(aqSkippedAtStart\(aq, \(aqSummedSaveImages\(aq, \(aqSkippedBetweenSaved\(aq, \(aqFilesAfterTrigger\(aq, \(aqFilesBeforeTrigger\(aq, \(aqSummedDarkImages\(aq, \(aqOutputDirectory\(aq, \(aqFilePattern\(aq, \(aqFileName\(aq, \(aqLogFile\(aq, \(aqUserComment1\(aq, \(aqCameraGain\(aq, \(aqUserComment2\(aq, \(aqUserComment3\(aq, \(aqUserComment4\(aq, \(aqSaveRawImages\(aq, \(aqSaveDarkImages\(aq, \(aqPerformIntegration\(aq, \(aqSaveIntegratedData\(aq, \(aqSaveSubtracted\(aq, \(aqPerformDarkSubtraction\(aq], \(aqpilatus\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus100k\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus1m\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus2m\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus300k\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus6m\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqtangovimba\(aq: [\(aqWidth\(aq, \(aqWidthMax\(aq, \(aqTriggerSource\(aq, \(aqPixelFormat\(aq, \(aqOffsetY\(aq, \(aqOffsetX\(aq, \(aqHeightMax\(aq, \(aqHeight\(aq, \(aqGainRaw\(aq, \(aqExposureTimeAbs\(aq, \(aqAcquisitionFrameRateAbs\(aq, \(aqAcquisitionFrameRateLimit\(aq, \(aqStreamBytesPerSecond\(aq, \(aqBinComment\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileSaving\(aq, \(aqFileStartNum\(aq, \(aqFramesProcessed\(aq, \(aqImage16\(aq, \(aqImage8\(aq, \(aqImageRaw\(aq, \(aqMaxLoad\(aq, \(aqReadMode\(aq, \(aqTuneMode\(aq, \(aqViewingMode\(aq]}
 (\fI\%dict\fP <\fI\%str\fP , \fI\%list\fP <\fI\%str\fP> >)
 important attributes of modules
 .UNINDENT
 .INDENT 0.0
 .TP
-.B nxstools.nxsdevicetools.moduleTemplateFiles = {\(aqdalsa\(aq: [\(aqdalsa.xml\(aq, \(aqdalsa_nxdata.ds.xml\(aq, \(aqdalsa_external_data.ds.xml\(aq], \(aqeigerdectris\(aq: [\(aqeigerdectris.xml\(aq, \(aqeigerdectris_stepindex.ds.xml\(aq, \(aqeigerdectris_description_cb.ds.xml\(aq, \(aqeigerdectris_triggermode_cb.ds.xml\(aq], \(aqlambda\(aq: [\(aqlambda.xml\(aq, \(aqlambda_nxdata.ds.xml\(aq, \(aqlambda_external_data.ds.xml\(aq], \(aqlambda2m\(aq: [\(aqlambda2m.xml\(aq, \(aqlambda2m_m1_nxdata.ds.xml\(aq, \(aqlambda2m_m2_nxdata.ds.xml\(aq, \(aqlambda2m_m3_nxdata.ds.xml\(aq, \(aqlambda2m_m1_external_data.ds.xml\(aq, \(aqlambda2m_m2_external_data.ds.xml\(aq, \(aqlambda2m_m3_external_data.ds.xml\(aq], \(aqlambdavds\(aq: [\(aqlambdavds.xml\(aq, \(aqlambdavds_nxdata.ds.xml\(aq, \(aqlambdavds_triggermode_cb.ds.xml\(aq, \(aqlambdavds_framenumbers_cb.ds.xml\(aq, \(aqlambdavds_savefilename_cb.ds.xml\(aq], \(aqlimaccd\(aq: [\(aqlimaccd.xml\(aq, \(aqlimaccd_postrun.ds.xml\(aq, \(aqlimaccd_xpixelsize.ds.xml\(aq, \(aqlimaccd_ypixelsize.ds.xml\(aq, \(aqlimaccd_description.ds.xml\(aq, \(aqlimaccd_filestartnum_cb.ds.xml\(aq], \(aqlimaccds\(aq: [\(aqlimaccd.xml\(aq, \(aqlimaccd_postrun.ds.xml\(aq, \(aqlimaccd_xpixelsize.ds.xml\(aq, \(aqlimaccd_ypixelsize.ds.xml\(aq, \(aqlimaccd_description.ds.xml\(aq, \(aqlimaccd_filestartnum_cb.ds.xml\(aq], \(aqmarccd\(aq: [\(aqmarccd.xml\(aq, \(aqmarccd_postrun.ds.xml\(aq], \(aqmca_xia\(aq: [\(aqmcaxia.xml\(aq], \(aqmythen\(aq: [\(aqmythen.xml\(aq, \(aqmythen_postrun.ds.xml\(aq, \(aqmythen_filestartnumber.ds.xml\(aq], \(aqmythen2\(aq: [\(aqmythen2.xml\(aq], \(aqpco\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpco4000\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpcoedge\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpedetector\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqperkinelmer\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqperkinelmerdetector\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqpilatus\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus100k\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus100k_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus1m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus1m_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus2m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus6m_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus300k\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus300k_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus6m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus6m_description.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqtangovimba\(aq: [\(aqtangovimba.xml\(aq, \(aqtangovimba_nxdata.ds.xml\(aq, \(aqtangovimba_external_data.ds.xml\(aq]}
+.B nxstools.nxsdevicetools.moduleTemplateFiles = {\(aqdalsa\(aq: [\(aqdalsa.xml\(aq, \(aqdalsa_nxdata.ds.xml\(aq, \(aqdalsa_external_data.ds.xml\(aq], \(aqeigerdectris\(aq: [\(aqeigerdectris.xml\(aq, \(aqeigerdectris_stepindex.ds.xml\(aq, \(aqeigerdectris_description_cb.ds.xml\(aq, \(aqeigerdectris_triggermode_cb.ds.xml\(aq], \(aqlambda\(aq: [\(aqlambda.xml\(aq, \(aqlambda_nxdata.ds.xml\(aq, \(aqlambda_external_data.ds.xml\(aq], \(aqlambda2m\(aq: [\(aqlambda2m.xml\(aq, \(aqlambda2m_m1_nxdata.ds.xml\(aq, \(aqlambda2m_m2_nxdata.ds.xml\(aq, \(aqlambda2m_m3_nxdata.ds.xml\(aq, \(aqlambda2m_m1_external_data.ds.xml\(aq, \(aqlambda2m_m2_external_data.ds.xml\(aq, \(aqlambda2m_m3_external_data.ds.xml\(aq], \(aqlambdavds\(aq: [\(aqlambdavds.xml\(aq, \(aqlambdavds_nxdata.ds.xml\(aq, \(aqlambdavds_description.ds.xml\(aq, \(aqlambdavds_triggermode_cb.ds.xml\(aq, \(aqlambdavds_framenumbers_cb.ds.xml\(aq, \(aqlambdavds_savefilename_cb.ds.xml\(aq], \(aqlimaccd\(aq: [\(aqlimaccd.xml\(aq, \(aqlimaccd_postrun.ds.xml\(aq, \(aqlimaccd_xpixelsize.ds.xml\(aq, \(aqlimaccd_ypixelsize.ds.xml\(aq, \(aqlimaccd_description.ds.xml\(aq, \(aqlimaccd_filestartnum_cb.ds.xml\(aq], \(aqlimaccds\(aq: [\(aqlimaccd.xml\(aq, \(aqlimaccd_postrun.ds.xml\(aq, \(aqlimaccd_xpixelsize.ds.xml\(aq, \(aqlimaccd_ypixelsize.ds.xml\(aq, \(aqlimaccd_description.ds.xml\(aq, \(aqlimaccd_filestartnum_cb.ds.xml\(aq], \(aqmarccd\(aq: [\(aqmarccd.xml\(aq, \(aqmarccd_postrun.ds.xml\(aq], \(aqmca_xia\(aq: [\(aqmcaxia.xml\(aq], \(aqmythen\(aq: [\(aqmythen.xml\(aq, \(aqmythen_postrun.ds.xml\(aq, \(aqmythen_filestartnumber.ds.xml\(aq], \(aqmythen2\(aq: [\(aqmythen2.xml\(aq], \(aqpco\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpco4000\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpcoedge\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpedetector\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqperkinelmer\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqperkinelmerdetector\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqpilatus\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus100k\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus100k_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus1m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus1m_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus2m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus6m_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus300k\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus300k_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus6m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus6m_description.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqtangovimba\(aq: [\(aqtangovimba.xml\(aq, \(aqtangovimba_nxdata.ds.xml\(aq, \(aqtangovimba_external_data.ds.xml\(aq]}
 (\fI\%dict\fP <\fI\%str\fP , \fI\%list\fP <\fI\%str\fP> >)
 xml template files of modules
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.nxsdevicetools.motorModules = [\(aqabsbox\(aq, \(aqmotor_tango\(aq, \(aqkohzu\(aq, \(aqsmchydra\(aq, \(aqlom\(aq, \(aqoms58\(aq, \(aqe6c\(aq, \(aqomsmaxv\(aq, \(aqspk\(aq, \(aqpie710\(aq, \(aqpie712\(aq, \(aqe6c_p09_eh2\(aq, \(aqsmaract\(aq]
 (\fI\%list\fP <\fI\%str\fP>) modules of motors
@@ -6570,15 +6570,15 @@
 .INDENT 0.0
 .TP
 .B nxstools.nxsdevicetools.openServer(device)
 opens connection to the configuration server
 .INDENT 7.0
 .TP
 .B Parameters
-\fBconfiguration\fP (\fI\%str\fP) \-\- server device name
+\fBconfiguration\fP (\fI\%str\fP) – server device name
 .TP
 .B Returns
 configuration server proxy
 .TP
 .B Return type
 \fBPyTango.DeviceProxy\fP
 .UNINDENT
@@ -6601,38 +6601,38 @@
 .B nxstools.nxsdevicetools.storeComponent(name, xml, server, mandatory=False)
 stores components in Configuration Server
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBname\fP (\fI\%str\fP) \-\- component name
+\fBname\fP (\fI\%str\fP) – component name
 .IP \(bu 2
-\fBxml\fP (\fI\%str\fP) \-\- component xml string
+\fBxml\fP (\fI\%str\fP) – component xml string
 .IP \(bu 2
-\fBserver\fP (\fI\%str\fP) \-\- configuration server
+\fBserver\fP (\fI\%str\fP) – configuration server
 .IP \(bu 2
-\fBmandatory\fP (\fI\%bool\fP) \-\- set component as mandatory
+\fBmandatory\fP (\fI\%bool\fP) – set component as mandatory
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.nxsdevicetools.storeDataSource(name, xml, server)
 stores datasources in Configuration Server
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBname\fP (\fI\%str\fP) \-\- datasource name
+\fBname\fP (\fI\%str\fP) – datasource name
 .IP \(bu 2
-\fBxml\fP (\fI\%str\fP) \-\- datasource xml string
+\fBxml\fP (\fI\%str\fP) – datasource xml string
 .IP \(bu 2
-\fBserver\fP (\fI\%str\fP) \-\- configuration server
+\fBserver\fP (\fI\%str\fP) – configuration server
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.nxsdevicetools.twoDModules = [\(aqpilatus100k\(aq, \(aqpilatus300k\(aq, \(aqpilatus1m\(aq, \(aqpilatus2m\(aq, \(aqpilatus6m\(aq, \(aqpco4000\(aq, \(aqperkinelmerdetector\(aq, \(aqlambda\(aq, \(aqpedetector\(aq, \(aqperkinelmer\(aq, \(aqpco\(aq, \(aqpcoedge\(aq, \(aqmarccd\(aq, \(aqperkinelmer\(aq, \(aqlcxcamera\(aq, \(aqlimaccd\(aq, \(aqeigerpsi\(aq, \(aqeigerdectris\(aq]
 (\fI\%list\fP <\fI\%str\fP>) modules of 2d detectors
@@ -6676,19 +6676,19 @@
 .sp
 Generator class creating image file names.
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBfname_template\fP (\fI\%str\fP) \-\- file name template
+\fBfname_template\fP (\fI\%str\fP) – file name template
 .IP \(bu 2
-\fBstart_index\fP (\fI\%int\fP) \-\- file start index
+\fBstart_index\fP (\fI\%int\fP) – file start index
 .IP \(bu 2
-\fBstop_index\fP (\fI\%int\fP) \-\- file stop index
+\fBstop_index\fP (\fI\%int\fP) – file stop index
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B file_index = None
 (\fI\%int\fP) file start index
 .UNINDENT
@@ -6701,15 +6701,15 @@
 .TP
 .B static from_slice(file_template)
 Static factory method to create a filename_generator instance
 from a sliced user input
 .INDENT 7.0
 .TP
 .B Parameters
-\fBfile_template\fP (\fI\%str\fP) \-\- file template
+\fBfile_template\fP (\fI\%str\fP) – file template
 .TP
 .B Returns
 filename generator object
 .TP
 .B Return type
 \fI\%FilenameGenerator\fP
 .UNINDENT
@@ -6732,15 +6732,15 @@
 .TP
 .B nxstools.xmltemplates.moduleMultiAttributes = {\(aqdalsa\(aq: [\(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileSaving\(aq, \(aqFileStartNum\(aq, \(aqTriggerMode\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqExtendedExposure\(aq, \(aqBinComment\(aq, \(aqFramesProcessed\(aq, \(aqImage16\(aq, \(aqImage8\(aq, \(aqImageRaw\(aq, \(aqFramesReceived\(aq, \(aqFrameRate\(aq, \(aqFramesPerNXFile\(aq, \(aqNXFileCompression\(aq, \(aqTurboMode\(aq, \(aqImageEnc\(aq, \(aqViewingMode\(aq, \(aqThrashedBuffers\(aq, \(aqFramesToAcquire\(aq, \(aqAcquisitionFrameCount\(aq, \(aqAcquisitionMode\(aq, \(aqAcquisitionFrameMode\(aq, \(aqLinearityEqualizer\(aq, \(aqNrExposedFrames\(aq, \(aqNrOffsetFrames\(aq, \(aqOffset\(aq, \(aqPixelFormat\(aq, \(aqReadOutMode\(aq, \(aqStandby\(aq, \(aqSumScheme\(aq], \(aqeigerdectris\(aq: [\(aqTriggerMode\(aq, \(aqNbTriggers\(aq, \(aqDescription\(aq, \(aqNbImages\(aq, \(aqBitDepth\(aq, \(aqReadoutTime\(aq, \(aqCountTime\(aq, \(aqEnergyThreshold\(aq, \(aqFrameTime\(aq, \(aqRateCorrectionEnabled\(aq, \(aqFlatFieldEnabled\(aq, \(aqTemperature\(aq, \(aqAutoSummationEnabled\(aq, \(aqHumidity\(aq, \(aqPhotonEnergy\(aq, \(aqWavelength\(aq], \(aqlambda\(aq: [\(aqTriggerMode\(aq, \(aqShutterTime\(aq, \(aqDelayTime\(aq, \(aqFrameNumbers\(aq, \(aqThreadNo\(aq, \(aqEnergyThreshold\(aq, \(aqOperatingMode\(aq, \(aqConfigFilePath\(aq, \(aqSaveAllImages\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqFilePreExt\(aq, \(aqFilePostfix\(aq, \(aqSaveFilePath\(aq, \(aqSaveFileName\(aq, \(aqLatestImageNumber\(aq, \(aqLiveMode\(aq, \(aqTotalLossFrames\(aq, \(aqCompressorShuffle\(aq, \(aqCompressionRate\(aq, \(aqCompressionEnabled\(aq, \(aqLayout\(aq, \(aqShutterTimeMax\(aq, \(aqShutterTimeMin\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqDepth\(aq, \(aqLiveFrameNo\(aq, \(aqDistortionCorrection\(aq, \(aqLiveLastImageData\(aq, \(aqFramesPerFile\(aq, \(aqOpMode\(aq], \(aqlambda2m\(aq: [\(aqTriggerMode\(aq, \(aqShutterTime\(aq, \(aqDelayTime\(aq, \(aqFrameNumbers\(aq, \(aqThreadNo\(aq, \(aqEnergyThreshold\(aq, \(aqOperatingMode\(aq, \(aqConfigFilePath\(aq, \(aqSaveAllImages\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqFilePreExt\(aq, \(aqFilePostfix\(aq, \(aqSaveFilePath\(aq, \(aqSaveFileName\(aq, \(aqLatestImageNumber\(aq, \(aqLiveMode\(aq, \(aqTotalLossFrames\(aq, \(aqCompressorShuffle\(aq, \(aqCompressionRate\(aq, \(aqCompressionEnabled\(aq, \(aqLayout\(aq, \(aqShutterTimeMax\(aq, \(aqShutterTimeMin\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqDepth\(aq, \(aqLiveFrameNo\(aq, \(aqDistortionCorrection\(aq, \(aqLiveLastImageData\(aq, \(aqOpMode\(aq], \(aqlambdavds\(aq: [\(aqTriggerMode\(aq, \(aqShutterTime\(aq, \(aqDelayTime\(aq, \(aqFrameNumbers\(aq, \(aqThreadNo\(aq, \(aqEnergyThreshold\(aq, \(aqOperatingMode\(aq, \(aqConfigFilePath\(aq, \(aqSaveAllImages\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqFilePreExt\(aq, \(aqFilePostfix\(aq, \(aqSaveFilePath\(aq, \(aqSaveFileName\(aq, \(aqLatestImageNumber\(aq, \(aqLiveMode\(aq, \(aqTotalLossFrames\(aq, \(aqCompressorShuffle\(aq, \(aqCompressionRate\(aq, \(aqCompressionEnabled\(aq, \(aqLayout\(aq, \(aqShutterTimeMax\(aq, \(aqShutterTimeMin\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqDepth\(aq, \(aqLiveFrameNo\(aq, \(aqDistortionCorrection\(aq, \(aqLiveLastImageData\(aq, \(aqFramesPerFile\(aq, \(aqOpMode\(aq], \(aqlimaccd\(aq: [\(aqcamera_type\(aq, \(aqcamera_pixelsize\(aq, \(aqcamera_model\(aq, \(aqacq_mode\(aq, \(aqacq_nb_frames\(aq, \(aqacq_trigger_mode\(aq, \(aqlast_image_saved\(aq, \(aqlatency_time\(aq, \(aqacc_max_expo_time\(aq, \(aqacc_expo_time\(aq, \(aqacc_time_mode\(aq, \(aqacc_dead_time\(aq, \(aqacc_live_time\(aq, \(aqsaving_mode\(aq, \(aqsaving_directory\(aq, \(aqsaving_prefix\(aq, \(aqsaving_suffix\(aq, \(aqsaving_next_number\(aq, \(aqsaving_format\(aq, \(aqsaving_frame_per_file\(aq, \(aqimage_type\(aq, \(aqimage_width\(aq, \(aqimage_height\(aq, \(aqimage_sizes\(aq, \(aqimage_roi\(aq, \(aqimage_bin\(aq, \(aqimage_flip\(aq, \(aqimage_rotation\(aq, \(aqshutter_mode\(aq, \(aqshutter_open_time\(aq], \(aqlimaccds\(aq: [\(aqcamera_type\(aq, \(aqcamera_pixelsize\(aq, \(aqcamera_model\(aq, \(aqacq_mode\(aq, \(aqacq_nb_frames\(aq, \(aqacq_trigger_mode\(aq, \(aqlast_image_saved\(aq, \(aqlatency_time\(aq, \(aqacc_max_expo_time\(aq, \(aqacc_expo_time\(aq, \(aqacc_time_mode\(aq, \(aqacc_dead_time\(aq, \(aqacc_live_time\(aq, \(aqsaving_mode\(aq, \(aqsaving_directory\(aq, \(aqsaving_prefix\(aq, \(aqsaving_suffix\(aq, \(aqsaving_next_number\(aq, \(aqsaving_format\(aq, \(aqsaving_frame_per_file\(aq, \(aqimage_type\(aq, \(aqimage_width\(aq, \(aqimage_height\(aq, \(aqimage_sizes\(aq, \(aqimage_roi\(aq, \(aqimage_bin\(aq, \(aqimage_flip\(aq, \(aqimage_rotation\(aq, \(aqshutter_mode\(aq, \(aqshutter_open_time\(aq], \(aqmaiadimension\(aq: [\(aqName\(aq, \(aqPositionSource\(aq, \(aqPixelPitch\(aq, \(aqPixelOrigin\(aq, \(aqPixelHysteresis\(aq, \(aqPositionUnit\(aq, \(aqPixelCoordExtent\(aq], \(aqmaiaflux\(aq: [\(aqFluxCoeff\(aq, \(aqFluxName\(aq, \(aqFluxUnit\(aq, \(aqFluxSource\(aq], \(aqmaiainterlock\(aq: [\(aqBiasPeltierInterlock\(aq, \(aqBiasPeltierInterlockUptime\(aq, \(aqPressure\(aq], \(aqmaialogger\(aq: [\(aqRunNumber\(aq], \(aqmaiaprocessing\(aq: [\(aqGaintrimEnable\(aq, \(aqLineariseEnable\(aq, \(aqPhotonEnable\(aq, \(aqPileupRejectEnable\(aq, \(aqPixelEnable\(aq, \(aqThrottleEnable\(aq], \(aqmaiasensor\(aq: [\(aqBiasVoltage\(aq, \(aqLeakageCurrent\(aq, \(aqPeltierCurrent\(aq, \(aqWaterTemperature\(aq, \(aqDetectorTemperature\(aq, \(aqMosfetTemperature\(aq, \(aqIdentity\(aq], \(aqmarccd\(aq: [\(aqFrameShift\(aq, \(aqSavingDirectory\(aq, \(aqSavingPostfix\(aq, \(aqSavingPrefix\(aq], \(aqmca_xia\(aq: [\(aqICR\(aq, \(aqOCR\(aq], \(aqmca_xia@pool\(aq: [\(aqCountsRoI\(aq, \(aqRoIEnd\(aq, \(aqRoIStart\(aq], \(aqmythen\(aq: [\(aqCounts1\(aq, \(aqCounts2\(aq, \(aqCountsMax\(aq, \(aqCountsTotal\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFileIndex\(aq, \(aqFilePrefix\(aq, \(aqData\(aq, \(aqRoI1\(aq, \(aqRoI2\(aq], \(aqmythen2\(aq: [\(aqCounts1\(aq, \(aqCounts2\(aq, \(aqCountsMax\(aq, \(aqCountsTotal\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFileIndex\(aq, \(aqFilePrefix\(aq, \(aqData\(aq, \(aqEnergy\(aq, \(aqNbFrames\(aq, \(aqRoI1End\(aq, \(aqRoI2End\(aq, \(aqRoI1Start\(aq, \(aqRoI2Start\(aq, \(aqThreshold\(aq], \(aqpco\(aq: [\(aqDelayTime\(aq, \(aqExposureTime\(aq, \(aqNbFrames\(aq, \(aqTriggerMode\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqBinning_x\(aq, \(aqBinning_y\(aq, \(aqROI_x_min\(aq, \(aqROI_x_max\(aq, \(aqROI_y_min\(aq, \(aqROI_y_max\(aq, \(aqPixelrate\(aq, \(aqADCs\(aq, \(aqCoolingTemp\(aq, \(aqCoolingTempSet\(aq, \(aqImageTimeStamp\(aq, \(aqRecorderMode\(aq], \(aqpco4000\(aq: [\(aqDelayTime\(aq, \(aqExposureTime\(aq, \(aqNbFrames\(aq, \(aqTriggerMode\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqBinning_x\(aq, \(aqBinning_y\(aq, \(aqROI_x_min\(aq, \(aqROI_x_max\(aq, \(aqROI_y_min\(aq, \(aqROI_y_max\(aq, \(aqPixelrate\(aq, \(aqADCs\(aq, \(aqCoolingTemp\(aq, \(aqCoolingTempSet\(aq, \(aqImageTimeStamp\(aq, \(aqRecorderMode\(aq], \(aqpcoedge\(aq: [\(aqDelayTime\(aq, \(aqExposureTime\(aq, \(aqNbFrames\(aq, \(aqTriggerMode\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqBinning_x\(aq, \(aqBinning_y\(aq, \(aqROI_x_min\(aq, \(aqROI_x_max\(aq, \(aqROI_y_min\(aq, \(aqROI_y_max\(aq, \(aqPixelrate\(aq, \(aqADCs\(aq, \(aqCoolingTemp\(aq, \(aqCoolingTempSet\(aq, \(aqImageTimeStamp\(aq, \(aqRecorderMode\(aq], \(aqpedetector\(aq: [\(aqBinningMode\(aq, \(aqFileIndex\(aq, \(aqExposureTime\(aq, \(aqSkippedAtStart\(aq, \(aqSummedSaveImages\(aq, \(aqSkippedBetweenSaved\(aq, \(aqFilesAfterTrigger\(aq, \(aqFilesBeforeTrigger\(aq, \(aqSummedDarkImages\(aq, \(aqOutputDirectory\(aq, \(aqFilePattern\(aq, \(aqFileName\(aq, \(aqLogFile\(aq, \(aqUserComment1\(aq, \(aqCameraGain\(aq, \(aqUserComment2\(aq, \(aqUserComment3\(aq, \(aqUserComment4\(aq, \(aqSaveRawImages\(aq, \(aqSaveDarkImages\(aq, \(aqPerformIntegration\(aq, \(aqSaveIntegratedData\(aq, \(aqSaveSubtracted\(aq, \(aqPerformDarkSubtraction\(aq], \(aqperkinelmer\(aq: [\(aqBinningMode\(aq, \(aqFileIndex\(aq, \(aqExposureTime\(aq, \(aqSkippedAtStart\(aq, \(aqSummedSaveImages\(aq, \(aqSkippedBetweenSaved\(aq, \(aqFilesAfterTrigger\(aq, \(aqFilesBeforeTrigger\(aq, \(aqSummedDarkImages\(aq, \(aqOutputDirectory\(aq, \(aqFilePattern\(aq, \(aqFileName\(aq, \(aqLogFile\(aq, \(aqUserComment1\(aq, \(aqCameraGain\(aq, \(aqUserComment2\(aq, \(aqUserComment3\(aq, \(aqUserComment4\(aq, \(aqSaveRawImages\(aq, \(aqSaveDarkImages\(aq, \(aqPerformIntegration\(aq, \(aqSaveIntegratedData\(aq, \(aqSaveSubtracted\(aq, \(aqPerformDarkSubtraction\(aq], \(aqperkinelmerdetector\(aq: [\(aqBinningMode\(aq, \(aqFileIndex\(aq, \(aqExposureTime\(aq, \(aqSkippedAtStart\(aq, \(aqSummedSaveImages\(aq, \(aqSkippedBetweenSaved\(aq, \(aqFilesAfterTrigger\(aq, \(aqFilesBeforeTrigger\(aq, \(aqSummedDarkImages\(aq, \(aqOutputDirectory\(aq, \(aqFilePattern\(aq, \(aqFileName\(aq, \(aqLogFile\(aq, \(aqUserComment1\(aq, \(aqCameraGain\(aq, \(aqUserComment2\(aq, \(aqUserComment3\(aq, \(aqUserComment4\(aq, \(aqSaveRawImages\(aq, \(aqSaveDarkImages\(aq, \(aqPerformIntegration\(aq, \(aqSaveIntegratedData\(aq, \(aqSaveSubtracted\(aq, \(aqPerformDarkSubtraction\(aq], \(aqpilatus\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus100k\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus1m\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus2m\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus300k\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus6m\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqtangovimba\(aq: [\(aqWidth\(aq, \(aqWidthMax\(aq, \(aqTriggerSource\(aq, \(aqPixelFormat\(aq, \(aqOffsetY\(aq, \(aqOffsetX\(aq, \(aqHeightMax\(aq, \(aqHeight\(aq, \(aqGainRaw\(aq, \(aqExposureTimeAbs\(aq, \(aqAcquisitionFrameRateAbs\(aq, \(aqAcquisitionFrameRateLimit\(aq, \(aqStreamBytesPerSecond\(aq, \(aqBinComment\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileSaving\(aq, \(aqFileStartNum\(aq, \(aqFramesProcessed\(aq, \(aqImage16\(aq, \(aqImage8\(aq, \(aqImageRaw\(aq, \(aqMaxLoad\(aq, \(aqReadMode\(aq, \(aqTuneMode\(aq, \(aqViewingMode\(aq]}
 (\fI\%dict\fP <\fI\%str\fP , \fI\%list\fP <\fI\%str\fP> >)
 important attributes of modules
 .UNINDENT
 .INDENT 0.0
 .TP
-.B nxstools.xmltemplates.moduleTemplateFiles = {\(aqdalsa\(aq: [\(aqdalsa.xml\(aq, \(aqdalsa_nxdata.ds.xml\(aq, \(aqdalsa_external_data.ds.xml\(aq], \(aqeigerdectris\(aq: [\(aqeigerdectris.xml\(aq, \(aqeigerdectris_stepindex.ds.xml\(aq, \(aqeigerdectris_description_cb.ds.xml\(aq, \(aqeigerdectris_triggermode_cb.ds.xml\(aq], \(aqlambda\(aq: [\(aqlambda.xml\(aq, \(aqlambda_nxdata.ds.xml\(aq, \(aqlambda_external_data.ds.xml\(aq], \(aqlambda2m\(aq: [\(aqlambda2m.xml\(aq, \(aqlambda2m_m1_nxdata.ds.xml\(aq, \(aqlambda2m_m2_nxdata.ds.xml\(aq, \(aqlambda2m_m3_nxdata.ds.xml\(aq, \(aqlambda2m_m1_external_data.ds.xml\(aq, \(aqlambda2m_m2_external_data.ds.xml\(aq, \(aqlambda2m_m3_external_data.ds.xml\(aq], \(aqlambdavds\(aq: [\(aqlambdavds.xml\(aq, \(aqlambdavds_nxdata.ds.xml\(aq, \(aqlambdavds_triggermode_cb.ds.xml\(aq, \(aqlambdavds_framenumbers_cb.ds.xml\(aq, \(aqlambdavds_savefilename_cb.ds.xml\(aq], \(aqlimaccd\(aq: [\(aqlimaccd.xml\(aq, \(aqlimaccd_postrun.ds.xml\(aq, \(aqlimaccd_xpixelsize.ds.xml\(aq, \(aqlimaccd_ypixelsize.ds.xml\(aq, \(aqlimaccd_description.ds.xml\(aq, \(aqlimaccd_filestartnum_cb.ds.xml\(aq], \(aqlimaccds\(aq: [\(aqlimaccd.xml\(aq, \(aqlimaccd_postrun.ds.xml\(aq, \(aqlimaccd_xpixelsize.ds.xml\(aq, \(aqlimaccd_ypixelsize.ds.xml\(aq, \(aqlimaccd_description.ds.xml\(aq, \(aqlimaccd_filestartnum_cb.ds.xml\(aq], \(aqmarccd\(aq: [\(aqmarccd.xml\(aq, \(aqmarccd_postrun.ds.xml\(aq], \(aqmca_xia\(aq: [\(aqmcaxia.xml\(aq], \(aqmythen\(aq: [\(aqmythen.xml\(aq, \(aqmythen_postrun.ds.xml\(aq, \(aqmythen_filestartnumber.ds.xml\(aq], \(aqmythen2\(aq: [\(aqmythen2.xml\(aq], \(aqpco\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpco4000\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpcoedge\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpedetector\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqperkinelmer\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqperkinelmerdetector\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqpilatus\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus100k\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus100k_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus1m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus1m_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus2m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus6m_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus300k\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus300k_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus6m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus6m_description.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqtangovimba\(aq: [\(aqtangovimba.xml\(aq, \(aqtangovimba_nxdata.ds.xml\(aq, \(aqtangovimba_external_data.ds.xml\(aq]}
+.B nxstools.xmltemplates.moduleTemplateFiles = {\(aqdalsa\(aq: [\(aqdalsa.xml\(aq, \(aqdalsa_nxdata.ds.xml\(aq, \(aqdalsa_external_data.ds.xml\(aq], \(aqeigerdectris\(aq: [\(aqeigerdectris.xml\(aq, \(aqeigerdectris_stepindex.ds.xml\(aq, \(aqeigerdectris_description_cb.ds.xml\(aq, \(aqeigerdectris_triggermode_cb.ds.xml\(aq], \(aqlambda\(aq: [\(aqlambda.xml\(aq, \(aqlambda_nxdata.ds.xml\(aq, \(aqlambda_external_data.ds.xml\(aq], \(aqlambda2m\(aq: [\(aqlambda2m.xml\(aq, \(aqlambda2m_m1_nxdata.ds.xml\(aq, \(aqlambda2m_m2_nxdata.ds.xml\(aq, \(aqlambda2m_m3_nxdata.ds.xml\(aq, \(aqlambda2m_m1_external_data.ds.xml\(aq, \(aqlambda2m_m2_external_data.ds.xml\(aq, \(aqlambda2m_m3_external_data.ds.xml\(aq], \(aqlambdavds\(aq: [\(aqlambdavds.xml\(aq, \(aqlambdavds_nxdata.ds.xml\(aq, \(aqlambdavds_description.ds.xml\(aq, \(aqlambdavds_triggermode_cb.ds.xml\(aq, \(aqlambdavds_framenumbers_cb.ds.xml\(aq, \(aqlambdavds_savefilename_cb.ds.xml\(aq], \(aqlimaccd\(aq: [\(aqlimaccd.xml\(aq, \(aqlimaccd_postrun.ds.xml\(aq, \(aqlimaccd_xpixelsize.ds.xml\(aq, \(aqlimaccd_ypixelsize.ds.xml\(aq, \(aqlimaccd_description.ds.xml\(aq, \(aqlimaccd_filestartnum_cb.ds.xml\(aq], \(aqlimaccds\(aq: [\(aqlimaccd.xml\(aq, \(aqlimaccd_postrun.ds.xml\(aq, \(aqlimaccd_xpixelsize.ds.xml\(aq, \(aqlimaccd_ypixelsize.ds.xml\(aq, \(aqlimaccd_description.ds.xml\(aq, \(aqlimaccd_filestartnum_cb.ds.xml\(aq], \(aqmarccd\(aq: [\(aqmarccd.xml\(aq, \(aqmarccd_postrun.ds.xml\(aq], \(aqmca_xia\(aq: [\(aqmcaxia.xml\(aq], \(aqmythen\(aq: [\(aqmythen.xml\(aq, \(aqmythen_postrun.ds.xml\(aq, \(aqmythen_filestartnumber.ds.xml\(aq], \(aqmythen2\(aq: [\(aqmythen2.xml\(aq], \(aqpco\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpco4000\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpcoedge\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpedetector\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqperkinelmer\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqperkinelmerdetector\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqpilatus\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus100k\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus100k_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus1m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus1m_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus2m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus6m_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus300k\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus300k_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus6m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus6m_description.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqtangovimba\(aq: [\(aqtangovimba.xml\(aq, \(aqtangovimba_nxdata.ds.xml\(aq, \(aqtangovimba_external_data.ds.xml\(aq]}
 (\fI\%dict\fP <\fI\%str\fP , \fI\%list\fP <\fI\%str\fP> >)
 xml template files of modules
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.xmltemplates.standardComponentTemplateFiles = {\(aqabsorber\(aq: [\(aqabsorber_foil.ds.xml\(aq, \(aqabsorber_thickness.ds.xml\(aq, \(aqabsorber.xml\(aq], \(aqbeamstop\(aq: [\(aqbeamstop.xml\(aq], \(aqbeamtimeid\(aq: [\(aqbeamtimeid.xml\(aq, \(aqbeamtimeid.ds.xml\(aq, \(aqstart_time.ds.xml\(aq], \(aqchcut\(aq: [\(aqchcut.xml\(aq, \(aqchcut_unitcalibration.ds.xml\(aq, \(aqchcut_crystal.ds.xml\(aq], \(aqcollect2\(aq: [\(aqcollect2.xml\(aq], \(aqcollect3\(aq: [\(aqcollect3.xml\(aq], \(aqcollect4\(aq: [\(aqcollect4.xml\(aq], \(aqcollect5\(aq: [\(aqcollect5.xml\(aq], \(aqcollect6\(aq: [\(aqcollect6.xml\(aq], \(aqcommon2\(aq: [\(aqcommon2_common.ds.xml\(aq], \(aqcommon3\(aq: [\(aqcommon3_common.ds.xml\(aq], \(aqdatasignal\(aq: [\(aqdatasignal.xml\(aq, \(aqdefaultsignal.ds.xml\(aq, \(aqsignal_name.ds.xml\(aq, \(aqsignalname.ds.xml\(aq, \(aqsignal_axes.ds.xml\(aq], \(aqdcm\(aq: [\(aqdcm.xml\(aq, \(aqdcm_reflection.ds.xml\(aq, \(aqdcm_unitcalibration.ds.xml\(aq, \(aqdcm_crystal.ds.xml\(aq], \(aqdefault\(aq: [\(aqdefault.xml\(aq, \(aqdefaultsample.xml\(aq, \(aqdefaultinstrument.xml\(aq, \(aqsample_name.ds.xml\(aq, \(aqchemical_formula.ds.xml\(aq, \(aqbeamtime_id.ds.xml\(aq, \(aqstart_time.ds.xml\(aq, \(aqend_time.ds.xml\(aq, \(aqnexdatas_version.ds.xml\(aq, \(aqnexdatas_configuration.ds.xml\(aq, \(aqtitle.ds.xml\(aq], \(aqdefaultinstrument\(aq: [\(aqdefaultinstrument.xml\(aq, \(aqbeamtime_id.ds.xml\(aq, \(aqstart_time.ds.xml\(aq, \(aqend_time.ds.xml\(aq, \(aqnexdatas_version.ds.xml\(aq, \(aqnexdatas_configuration.ds.xml\(aq, \(aqtitle.ds.xml\(aq], \(aqdefaultsample\(aq: [\(aqdefaultsample.xml\(aq, \(aqsample_name.ds.xml\(aq, \(aqchemical_formula.ds.xml\(aq], \(aqdetectorlive\(aq: [\(aqdetectorlive.xml\(aq], \(aqempty\(aq: [\(aqempty.xml\(aq], \(aqkeithley\(aq: [\(aqkeithley.xml\(aq], \(aqmaia\(aq: [\(aqmaia.xml\(aq, \(aqempty.xml\(aq], \(aqmaiadimension\(aq: [\(aqmaiadimension.xml\(aq], \(aqmaiaflux\(aq: [\(aqmaiaflux.xml\(aq], \(aqmsnsar\(aq: [\(aqmsnsar_env.ds.xml\(aq, \(aqsardanaenvironment.ds.xml\(aq], \(aqmssar\(aq: [\(aqmssar_env.ds.xml\(aq, \(aqsardanaenvironment.ds.xml\(aq], \(aqpinhole\(aq: [\(aqpinhole.xml\(aq], \(aqpointdet\(aq: [\(aqpointdet.xml\(aq], \(aqqbpm\(aq: [\(aqqbpm_foil.ds.xml\(aq, \(aqqbpm.xml\(aq], \(aqsamplehkl\(aq: [\(aqsamplehkl.xml\(aq], \(aqslit\(aq: [\(aqslit.xml\(aq], \(aqsource\(aq: [\(aqsource.xml\(aq], \(aqundulator\(aq: [\(aqundulator.xml\(aq]}
 (\fI\%dict\fP <\fI\%str\fP , \fI\%list\fP <\fI\%str\fP> >)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nxstools-3.8.0/nxstools/__init__.py` & `nxstools-3.9.0/nxstools/__init__.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/filenamegenerator.py` & `nxstools-3.9.0/nxstools/filenamegenerator.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/filewriter.py` & `nxstools-3.9.0/nxstools/filewriter.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/h5cppwriter.py` & `nxstools-3.9.0/nxstools/h5cppwriter.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/h5pywriter.py` & `nxstools-3.9.0/nxstools/h5pywriter.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/nxsargparser.py` & `nxstools-3.9.0/nxstools/nxsargparser.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/nxscollect.py` & `nxstools-3.9.0/nxstools/nxscollect.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/nxsconfig.py` & `nxstools-3.9.0/nxstools/nxsconfig.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/nxscreate.py` & `nxstools-3.9.0/nxstools/nxscreate.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/nxscreator.py` & `nxstools-3.9.0/nxstools/nxscreator.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/nxsdata.py` & `nxstools-3.9.0/nxstools/nxsdata.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/nxsdevicetools.py` & `nxstools-3.9.0/nxstools/nxsdevicetools.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/nxsetup.py` & `nxstools-3.9.0/nxstools/nxsetup.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/nxsfileinfo.py` & `nxstools-3.9.0/nxstools/nxsfileinfo.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/nxsfileparser.py` & `nxstools-3.9.0/nxstools/nxsfileparser.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/nxsparser.py` & `nxstools-3.9.0/nxstools/nxsparser.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/nxsxml.py` & `nxstools-3.9.0/nxstools/nxsxml.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/pyeval/__init__.py` & `nxstools-3.9.0/nxstools/pyeval/__init__.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/pyeval/absorber.py` & `nxstools-3.9.0/nxstools/pyeval/absorber.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/pyeval/beamtimeid.py` & `nxstools-3.9.0/nxstools/pyeval/beamtimeid.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/pyeval/datasignal.py` & `nxstools-3.9.0/nxstools/pyeval/datasignal.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/pyeval/dcm.py` & `nxstools-3.9.0/nxstools/pyeval/dcm.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 def unitcalibration(dcmdevice):
     """ code for dcm unitcalibration datasource
 
     :param dcmdevice:  dcm device name
     :type dcmdevice: :obj:`str`
     :returns: unit calibration
-    :rtype: :obj:`str`
+    :rtype: :obj:`float`
     """
     dp = tango.DeviceProxy(dcmdevice)
     bdv = dp.get_property("BraggDevice")['BraggDevice'][0]
     bdp = tango.DeviceProxy(bdv)
     return bdp.unitcalibration
```

### Comparing `nxstools-3.8.0/nxstools/pyeval/lambdavds.py` & `nxstools-3.9.0/nxstools/pyeval/lambdavds.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,51 +15,50 @@
 #
 #    You should have received a copy of the GNU General Public License
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 """  pyeval helper functions for lambdavds """
 
+try:
+    from . import common
+except Exception:
+    import common
+
 
 def savefilename_cb(commonblock, savefilename, savefilename_str):
     """ code for savefilename_cb  datasource
 
     :param commonblock: commonblock of nxswriter
     :type commonblock: :obj:`dict`<:obj:`str`, `any`>
     :param savefilename:  name of saved file
     :type savefilename: :obj:`str`
     :param savefilename_str: name of savefilename datasource
     :type savefilename_str: :obj:`str`
     :returns:   name of saved file
     :rtype: :obj:`str`
     """
-    if savefilename_str not in commonblock:
-        commonblock[savefilename_str] = [savefilename]
-    else:
-        commonblock[savefilename_str].append(savefilename)
-    return savefilename
+    return common.blockitem_add(
+        commonblock, savefilename_str, savefilename)
 
 
 def framenumbers_cb(commonblock, framenumbers, framenumbers_str):
     """ code for triggermode_cb  datasource
 
     :param commonblock: commonblock of nxswriter
     :type commonblock: :obj:`dict`<:obj:`str`, `any`>
     :param framenumbers:  number of frames
     :type framenumbers: :obj:`str` or :obj:`int`
     :param framenumbers_str: name of framenumbers datasource
     :type framenumbers_str: :obj:`str`
     :returns:  number of frames
     :rtype: :obj:`str` or :obj:`int`
     """
-    if framenumbers_str not in commonblock:
-        commonblock[framenumbers_str] = [int(framenumbers)]
-    else:
-        commonblock[framenumbers_str].append(int(framenumbers))
-    return framenumbers
+    return common.blockitem_addint(
+        commonblock, framenumbers_str, framenumbers)
 
 
 def triggermode_cb(commonblock, name, triggermode, saveallimages,
                    framesperfile, height, width, opmode,
                    filepostfix, savefilename_str, framenumbers_str,
                    filename_str, entry_str):
     """ code for triggermode_cb  datasource
```

### Comparing `nxstools-3.8.0/nxstools/pyeval/mssar.py` & `nxstools-3.9.0/nxstools/pyeval/mssar.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/pyeval/qbpm.py` & `nxstools-3.9.0/nxstools/pyeval/qbpm.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/release.py` & `nxstools-3.9.0/nxstools/release.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 #    You should have received a copy of the GNU General Public License
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 """  NXS tools release version"""
 
 #: (:obj:`str`) package version
-__version__ = "3.8.0"
+__version__ = "3.9.0"
```

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/__init__.py` & `nxstools-3.9.0/nxstools/xmltemplates/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1479,14 +1479,15 @@
                 'pco_description.ds.xml',
                 'pco_filestartnum_cb.ds.xml'],
     'lambda': ['lambda.xml',
                'lambda_nxdata.ds.xml',
                'lambda_external_data.ds.xml'],
     'lambdavds': ['lambdavds.xml',
                   'lambdavds_nxdata.ds.xml',
+                  'lambdavds_description.ds.xml',
                   'lambdavds_triggermode_cb.ds.xml',
                   'lambdavds_framenumbers_cb.ds.xml',
                   'lambdavds_savefilename_cb.ds.xml'],
     'tangovimba': ['tangovimba.xml',
                    'tangovimba_nxdata.ds.xml',
                    'tangovimba_external_data.ds.xml'],
     'dalsa': ['dalsa.xml',
```

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/absorber.xml` & `nxstools-3.9.0/nxstools/xmltemplates/absorber.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/beamstop.xml` & `nxstools-3.9.0/nxstools/xmltemplates/beamstop.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/chcut.xml` & `nxstools-3.9.0/nxstools/xmltemplates/chcut.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/dalsa.xml` & `nxstools-3.9.0/nxstools/xmltemplates/dalsa.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/dalsa_external_data.ds.xml` & `nxstools-3.9.0/nxstools/xmltemplates/pco_postrun.ds.xml`

 * *Files 26% similar despite different names*

#### Comparing `nxstools-3.8.0/nxstools/xmltemplates/dalsa_external_data.ds.xml` & `nxstools-3.9.0/nxstools/xmltemplates/pco_postrun.ds.xml`

```diff
@@ -1,30 +1,19 @@
 <?xml version="1.0" encoding="utf-8"?>
 <definition>
-  <datasource type="PYEVAL" name="$(name)_external_data">
-    <result name="result">ds.result = &quot;&quot;
-try:
-    filestartnum = int(ds.$(name)_filestartnum)
-    if filestartnum &gt; 0:
-        filestartnum -= 1
-except Exception:
-    filestartnum = 0
-
-if ds.$(name)_fileprefix  and ds.$(name)_filepostfix:
-    postfix = str(ds.$(name)_filepostfix)
-    if not postfix.startswith(&quot;.&quot;):
-        postfix = &quot;.&quot; + postfix
-    if postfix in [&quot;.nxs&quot;, &quot;.nx&quot;]:
-        prefix = str(ds.$(name)_fileprefix)
-        if not prefix.endswith(&quot;_&quot;):
-            prefix = prefix + &quot;_&quot;
-        if &quot;$var.filename&quot;:
-            ds.result = (&quot;$var.filename&quot;).split(&quot;/&quot;)[-1].split(&quot;.&quot;)[0] + &quot;/&quot;
-
-        ds.result += &quot;$(name)/&quot; + prefix + &quot;%06i&quot; % filestartnum + postfix + &quot;://entry/instrument/detector&quot;</result>
-    $datasources.$(name)_filedir
- $datasources.$(name)_fileprefix
+  <datasource type="PYEVAL" name="$(name)_postrun">
+    <result name="result">from nxstools.pyeval import pco
+ds.result = pco.postrun(
+    commonblock,
+    ds.$(name)_filestartnum,
+    ds.$(name)_filedir,
+    ds.$(name)_nbframes,
+    ds.$(name)_filepostfix,
+    ds.$(name)_fileprefix,
+    &quot;$(name)_filestartnum&quot;)</result>
+    $datasources.$(name)_filestartnum
+ $datasources.$(name)_filedir
+ $datasources.$(name)_nbframes
  $datasources.$(name)_filepostfix
- $datasources.$(name)_filestartnum
- $datasources.$(name)_filesaving
+ $datasources.$(name)_fileprefix
   </datasource>
 </definition>
```

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/dalsa_nxdata.ds.xml` & `nxstools-3.9.0/nxstools/xmltemplates/dalsa_nxdata.ds.xml`

 * *Files 15% similar despite different names*

#### Comparing `nxstools-3.8.0/nxstools/xmltemplates/dalsa_nxdata.ds.xml` & `nxstools-3.9.0/nxstools/xmltemplates/dalsa_nxdata.ds.xml`

```diff
@@ -5,14 +5,11 @@
 if ds.$(name)_fileprefix and ds.$(name)_filepostfix:
     postfix = str(ds.$(name)_filepostfix)
     if not postfix.startswith(&quot;.&quot;):
         postfix = &quot;.&quot; + postfix
     if postfix in [&quot;.nxs&quot;, &quot;.nx&quot;]:
         prefix = str(ds.$(name)_fileprefix)
         ds.result = &quot;$var.entryname#'$(__entryname__)'$var.serialno:NXentry/$(__insname__)/$(name)_external:NXdetector/data&quot;</result>
-    $datasources.$(name)_filedir
- $datasources.$(name)_fileprefix
+    $datasources.$(name)_fileprefix
  $datasources.$(name)_filepostfix
- $datasources.$(name)_filestartnum
- $datasources.$(name)_filesaving
   </datasource>
 </definition>
```

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/dalsavds_nrexposedframes_cb.ds.xml` & `nxstools-3.9.0/nxstools/xmltemplates/dalsavds_nrexposedframes_cb.ds.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/dcm.xml` & `nxstools-3.9.0/nxstools/xmltemplates/dcm.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/defaultinstrument.xml` & `nxstools-3.9.0/nxstools/xmltemplates/defaultinstrument.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/detectorlive.xml` & `nxstools-3.9.0/nxstools/xmltemplates/detectorlive.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/eigerdectris.xml` & `nxstools-3.9.0/nxstools/xmltemplates/eigerdectris.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/keithley.xml` & `nxstools-3.9.0/nxstools/xmltemplates/keithley.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/lambda.xml` & `nxstools-3.9.0/nxstools/xmltemplates/lambda.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/lambda2m.xml` & `nxstools-3.9.0/nxstools/xmltemplates/lambda2m.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/lambda_external_data.ds.xml` & `nxstools-3.9.0/nxstools/xmltemplates/lambdavds_triggermode_cb.ds.xml`

 * *Files 26% similar despite different names*

#### Comparing `nxstools-3.8.0/nxstools/xmltemplates/lambda_external_data.ds.xml` & `nxstools-3.9.0/nxstools/xmltemplates/lambdavds_triggermode_cb.ds.xml`

```diff
@@ -1,28 +1,29 @@
 <?xml version="1.0" encoding="utf-8"?>
 <definition>
-  <datasource type="PYEVAL" name="$(name)_external_data">
-    <result name="result">ds.result = &quot;&quot;
-if ds.$(name)_saveallimages:
-    if &quot;$var.filename&quot;:
-        ds.result = (&quot;$var.filename&quot;).split(&quot;/&quot;)[-1].split(&quot;.&quot;)[0] + &quot;/&quot;
-    fpf = ds.$(name)_framesperfile
-    fn = ds.$(name)_framenumbers
-    spf = 0
-    cfid = 0
-    if fpf != fn:
-        if &quot;__root__&quot; in commonblock.keys():
-            root = commonblock[&quot;__root__&quot;]
-            if hasattr(root, &quot;currentfileid&quot;) and hasattr(root, &quot;stepsperfile&quot;):
-                spf = root.stepsperfile
-                cfid = root.currentfileid
-    if spf &gt; 0 and cfid &gt; 0:
-        ds.result += &quot;$(name)/&quot; + str(ds.$(name)_savefilename) + &quot;_part%05d.&quot; % (cfid - 1) + str(ds.$(name)_filepostfix) + &quot;://entry/instrument/detector&quot;
-    else:
-        ds.result += &quot;$(name)/&quot; + str(ds.$(name)_savefilename) + &quot;.&quot; + str(ds.$(name)_filepostfix) + &quot;://entry/instrument/detector&quot;</result>
+  <datasource type="PYEVAL" name="$(name)_triggermode_cb">
+    <result name="result">from nxstools.pyeval import lambdavds
+ds.result = lambdavds.triggermode_cb(
+    commonblock,
+    &quot;$(name)&quot;,
+    ds.$(name)_triggermode,
+    ds.$(name)_saveallimages,
+    ds.$(name)_framesperfile,
+    ds.$(name)_height,
+    ds.$(name)_width,
+    ds.$(name)_opmode,
+    ds.$(name)_filepostfix,
+    &quot;$(name)_savefilename&quot;,
+    &quot;$(name)_framenumbers&quot;,
+    &quot;$var.filename&quot;,
+    &quot;$var.entryname#'$(__entryname__)'$var.serialno&quot;)</result>
+    $datasources.$(name)_triggermode
+    $datasources.$(name)_opmode
     $datasources.$(name)_savefilename
- $datasources.$(name)_saveallimages
- $datasources.$(name)_framesperfile
- $datasources.$(name)_framenumbers
- $datasources.$(name)_filepostfix
+    $datasources.$(name)_saveallimages
+    $datasources.$(name)_framesperfile
+    $datasources.$(name)_framenumbers
+    $datasources.$(name)_filepostfix
+    $datasources.$(name)_height
+    $datasources.$(name)_width
   </datasource>
 </definition>
```

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/lambdavds.xml` & `nxstools-3.9.0/nxstools/xmltemplates/lambdavds.xml`

 * *Files 1% similar despite different names*

#### Comparing `nxstools-3.8.0/nxstools/xmltemplates/lambdavds.xml` & `nxstools-3.9.0/nxstools/xmltemplates/lambdavds.xml`

```diff
@@ -11,15 +11,18 @@
           55
           <strategy mode="INIT"/>
         </field>
         <field type="NX_CHAR" name="layout">
           area
           <strategy mode="INIT"/>
         </field>
-        <field type="NX_CHAR" name="description">$(name)</field>
+        <field type="NX_CHAR" name="description">
+          $datasources.$(name)_description
+          <strategy mode="INIT"/>
+        </field>
         <field units="eV" type="NX_FLOAT32" name="threshold_energy">
           <strategy mode="FINAL"/>
           $datasources.$(name)_energythreshold
         </field>
         <group type="NXcollection" name="collection">
           <field type="NX_INT16" name="trigger_mode">
             <strategy mode="FINAL"/>
```

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/lambdavds_triggermode_cb.ds.xml` & `nxstools-3.9.0/nxstools/xmltemplates/lambda_external_data.ds.xml`

 * *Files 22% similar despite different names*

#### Comparing `nxstools-3.8.0/nxstools/xmltemplates/lambdavds_triggermode_cb.ds.xml` & `nxstools-3.9.0/nxstools/xmltemplates/lambda_external_data.ds.xml`

```diff
@@ -1,29 +1,20 @@
 <?xml version="1.0" encoding="utf-8"?>
 <definition>
-  <datasource type="PYEVAL" name="$(name)_triggermode_cb">
-    <result name="result">from nxstools.pyeval import lambdavds
-ds.result = lambdavds.triggermode_cb(
+  <datasource type="PYEVAL" name="$(name)_external_data">
+    <result name="result">from nxstools.pyeval import lmbd
+ds.result = lmbd.external_data(
     commonblock,
     &quot;$(name)&quot;,
-    ds.$(name)_triggermode,
+    ds.$(name)_savefilename,
     ds.$(name)_saveallimages,
     ds.$(name)_framesperfile,
-    ds.$(name)_height,
-    ds.$(name)_width,
-    ds.$(name)_opmode,
+    ds.$(name)_framenumbers,
     ds.$(name)_filepostfix,
-    &quot;$(name)_savefilename&quot;,
-    &quot;$(name)_framenumbers&quot;,
-    &quot;$var.filename&quot;,
-    &quot;$var.entryname#'$(__entryname__)'$var.serialno&quot;)</result>
-    $datasources.$(name)_triggermode
-    $datasources.$(name)_opmode
+    &quot;$var.filename&quot;)</result>
     $datasources.$(name)_savefilename
-    $datasources.$(name)_saveallimages
-    $datasources.$(name)_framesperfile
-    $datasources.$(name)_framenumbers
-    $datasources.$(name)_filepostfix
-    $datasources.$(name)_height
-    $datasources.$(name)_width
+ $datasources.$(name)_saveallimages
+ $datasources.$(name)_framesperfile
+ $datasources.$(name)_framenumbers
+ $datasources.$(name)_filepostfix
   </datasource>
 </definition>
```

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/limaccd.xml` & `nxstools-3.9.0/nxstools/xmltemplates/limaccd.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/maia.xml` & `nxstools-3.9.0/nxstools/xmltemplates/maia.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/maiadimension.xml` & `nxstools-3.9.0/nxstools/xmltemplates/maiadimension.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/maiaflux.xml` & `nxstools-3.9.0/nxstools/xmltemplates/maiaflux.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/marccd.xml` & `nxstools-3.9.0/nxstools/xmltemplates/marccd.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/mcaxia.xml` & `nxstools-3.9.0/nxstools/xmltemplates/mcaxia.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/mythen.xml` & `nxstools-3.9.0/nxstools/xmltemplates/mythen.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/mythen2.xml` & `nxstools-3.9.0/nxstools/xmltemplates/mythen2.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/pco.xml` & `nxstools-3.9.0/nxstools/xmltemplates/pco.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/perkinelmerdetector.xml` & `nxstools-3.9.0/nxstools/xmltemplates/perkinelmerdetector.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/pilatus.xml` & `nxstools-3.9.0/nxstools/xmltemplates/pilatus.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/pinhole.xml` & `nxstools-3.9.0/nxstools/xmltemplates/pinhole.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/pointdet.xml` & `nxstools-3.9.0/nxstools/xmltemplates/pointdet.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/qbpm.xml` & `nxstools-3.9.0/nxstools/xmltemplates/qbpm.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/samplehkl.xml` & `nxstools-3.9.0/nxstools/xmltemplates/samplehkl.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/slit.xml` & `nxstools-3.9.0/nxstools/xmltemplates/slit.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/source.xml` & `nxstools-3.9.0/nxstools/xmltemplates/source.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/tangovimba.xml` & `nxstools-3.9.0/nxstools/xmltemplates/tangovimba.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/tangovimba_nxdata.ds.xml` & `nxstools-3.9.0/nxstools/xmltemplates/tangovimba_nxdata.ds.xml`

 * *Files 15% similar despite different names*

#### Comparing `nxstools-3.8.0/nxstools/xmltemplates/tangovimba_nxdata.ds.xml` & `nxstools-3.9.0/nxstools/xmltemplates/tangovimba_nxdata.ds.xml`

```diff
@@ -5,14 +5,11 @@
 if ds.$(name)_fileprefix and ds.$(name)_filepostfix:
     postfix = str(ds.$(name)_filepostfix)
     if not postfix.startswith(&quot;.&quot;):
         postfix = &quot;.&quot; + postfix
     if postfix in [&quot;.nxs&quot;, &quot;.nx&quot;]:
         prefix = str(ds.$(name)_fileprefix)
         ds.result = &quot;$var.entryname#'$(__entryname__)'$var.serialno:NXentry/$(__insname__)/$(name)_external:NXdetector/data&quot;</result>
-    $datasources.$(name)_filedir
- $datasources.$(name)_fileprefix
+    $datasources.$(name)_fileprefix
  $datasources.$(name)_filepostfix
- $datasources.$(name)_filestartnum
- $datasources.$(name)_filesaving
   </datasource>
 </definition>
```

### Comparing `nxstools-3.8.0/nxstools/xmltemplates/undulator.xml` & `nxstools-3.9.0/nxstools/xmltemplates/undulator.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.8.0/nxstools.egg-info/PKG-INFO` & `nxstools-3.9.0/nxstools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: nxstools
-Version: 3.8.0
+Version: 3.9.0
 Summary: Configuration tools for NeXDaTaS Tango Servers
 Home-page: http://github.com/nexdatas/tools
 Author: ('Jan Kotanski, Eugen Wintersberger , Halil Pasic',)
 Author-email: jankotan@gmail.com, eugen.wintersberger@gmail.com, halil.pasic@gmail.com
 Maintainer: Jan Kotanski, Eugen Wintersberger , Halil Pasic
 Maintainer-email: jankotan@gmail.com, eugen.wintersberger@gmail.com, halil.pasic@gmail.com
 License: ('GNU GENERAL PUBLIC LICENSE, version 3',)
```

### Comparing `nxstools-3.8.0/nxstools.egg-info/SOURCES.txt` & `nxstools-3.9.0/nxstools.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -39,19 +39,30 @@
 nxstools.egg-info/dependency_links.txt
 nxstools.egg-info/not-zip-safe
 nxstools.egg-info/requires.txt
 nxstools.egg-info/top_level.txt
 nxstools/pyeval/__init__.py
 nxstools/pyeval/absorber.py
 nxstools/pyeval/beamtimeid.py
+nxstools/pyeval/common.py
+nxstools/pyeval/dalsa.py
 nxstools/pyeval/datasignal.py
 nxstools/pyeval/dcm.py
+nxstools/pyeval/eigerdectris.py
 nxstools/pyeval/lambdavds.py
+nxstools/pyeval/limaccd.py
+nxstools/pyeval/lmbd.py
+nxstools/pyeval/marccd.py
 nxstools/pyeval/mssar.py
+nxstools/pyeval/mythen.py
+nxstools/pyeval/pco.py
+nxstools/pyeval/pe.py
+nxstools/pyeval/pilatus.py
 nxstools/pyeval/qbpm.py
+nxstools/pyeval/tangovimba.py
 nxstools/xmltemplates/__init__.py
 nxstools/xmltemplates/absorber.xml
 nxstools/xmltemplates/absorber_foil.ds.xml
 nxstools/xmltemplates/absorber_thickness.ds.xml
 nxstools/xmltemplates/beamstop.xml
 nxstools/xmltemplates/beamtime_id.ds.xml
 nxstools/xmltemplates/beamtimeid.ds.xml
@@ -95,14 +106,15 @@
 nxstools/xmltemplates/lambda2m_m2_external_data.ds.xml
 nxstools/xmltemplates/lambda2m_m2_nxdata.ds.xml
 nxstools/xmltemplates/lambda2m_m3_external_data.ds.xml
 nxstools/xmltemplates/lambda2m_m3_nxdata.ds.xml
 nxstools/xmltemplates/lambda_external_data.ds.xml
 nxstools/xmltemplates/lambda_nxdata.ds.xml
 nxstools/xmltemplates/lambdavds.xml
+nxstools/xmltemplates/lambdavds_description.ds.xml
 nxstools/xmltemplates/lambdavds_framenumbers_cb.ds.xml
 nxstools/xmltemplates/lambdavds_nxdata.ds.xml
 nxstools/xmltemplates/lambdavds_savefilename_cb.ds.xml
 nxstools/xmltemplates/lambdavds_triggermode_cb.ds.xml
 nxstools/xmltemplates/limaccd.xml
 nxstools/xmltemplates/limaccd_description.ds.xml
 nxstools/xmltemplates/limaccd_filestartnum_cb.ds.xml
```

### Comparing `nxstools-3.8.0/setup.py` & `nxstools-3.9.0/setup.py`

 * *Files identical despite different names*

