# Comparing `tmp/KrakenOS-1.0.0.7.tar.gz` & `tmp/KrakenOS-1.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KrakenOS-1.0.0.7.tar", last modified: Mon Jan 24 21:03:18 2022, max compression
+gzip compressed data, was "KrakenOS-1.0.0.9.tar", last modified: Tue Jan 25 00:49:48 2022, max compression
```

## Comparing `KrakenOS-1.0.0.7.tar` & `KrakenOS-1.0.0.9.tar`

### file list

```diff
@@ -1,136 +1,135 @@
-drwxr-xr-x   0 joelherreravazquez   (501) staff       (20)        0 2022-01-24 21:03:18.064028 KrakenOS-1.0.0.7/
-drwxr-xr-x   0 joelherreravazquez   (501) staff       (20)        0 2022-01-24 21:03:18.016005 KrakenOS-1.0.0.7/KrakenOS/
-drwxr-xr-x   0 joelherreravazquez   (501) staff       (20)        0 2022-01-24 21:03:18.018878 KrakenOS-1.0.0.7/KrakenOS/AstroAtmosphere/
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)      936 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.7/KrakenOS/AstroAtmosphere/AtmosP 3.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)      937 2021-08-29 21:05:19.000000 KrakenOS-1.0.0.7/KrakenOS/AstroAtmosphere/AtmosP.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)      265 2021-08-27 17:45:53.000000 KrakenOS-1.0.0.7/KrakenOS/AstroAtmosphere/__init__.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    17979 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.7/KrakenOS/AstroAtmosphere/ciddorModel.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    30232 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.7/KrakenOS/AstroAtmosphere/dispersionModels.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    11355 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.7/KrakenOS/AstroAtmosphere/misc.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    22166 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.7/KrakenOS/AstroAtmosphere/neoslalib.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2877 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.7/KrakenOS/AstroAtmosphere/observatories.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    18492 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.7/KrakenOS/AstroAtmosphere/refractionModels.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    19964 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.7/KrakenOS/AstroAtmosphere/refractivityModels.py
-drwxr-xr-x   0 joelherreravazquez   (501) staff       (20)        0 2022-01-24 21:03:18.037600 KrakenOS-1.0.0.7/KrakenOS/Cat/
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     8196 2021-12-16 06:14:17.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/.DS_Store
--rwxr-xr-x   0 joelherreravazquez   (501) staff       (20)     5569 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/Alum.csv
--rwxr-xr-x   0 joelherreravazquez   (501) staff       (20)   418630 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/SCHOTT-2.AGF
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)   418630 2021-12-16 06:08:05.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/SCHOTT.AGF
--rwxr-xr-x   0 joelherreravazquez   (501) staff       (20)     1591 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/UTILIDADES.AGF
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    24757 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/archer.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3344 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/arton.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    64489 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/birefringent.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)   271332 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/cdgm.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)   147112 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/corning.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2062 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/heraeus.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)   538064 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/hikari.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)  1214752 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/hoya.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    50293 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/infrared.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2114 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/isuzu.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2343 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/liebetraut.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    14802 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/lightpath.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    93256 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/lzos.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    25326 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/misc.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)   652183 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/nikon.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)   715345 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/ohara.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     4336 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/rad_hard.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    61862 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/rpo.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)   228484 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/schott-1.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)   142366 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/sumita.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     1611 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/topas.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     1782 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/umicore.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2078 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.7/KrakenOS/Cat/zeon.agf
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    14654 2021-12-28 18:37:03.000000 KrakenOS-1.0.0.7/KrakenOS/Display.py
-drwxr-xr-x   0 joelherreravazquez   (501) staff       (20)        0 2022-01-24 21:03:18.038046 KrakenOS-1.0.0.7/KrakenOS/Docs/
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     6148 2021-10-07 01:21:28.000000 KrakenOS-1.0.0.7/KrakenOS/Docs/.DS_Store
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)  4677716 2021-09-06 21:35:21.000000 KrakenOS-1.0.0.7/KrakenOS/Docs/USER_MANUAL_KrakenOS_Provisional.pdf
-drwxr-xr-x   0 joelherreravazquez   (501) staff       (20)        0 2022-01-24 21:03:18.061573 KrakenOS-1.0.0.7/KrakenOS/Examples/
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     6148 2021-11-28 02:39:00.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/.DS_Store
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     1566 2021-12-17 16:08:16.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp-Tel-6.5m-RAY.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     7427 2021-11-28 01:26:45.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp-Tel-6.5m.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2025 2021-10-16 16:52:26.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Axicon.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2240 2021-11-28 01:23:58.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Axicon_And_Cylinder.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2659 2021-12-07 17:10:35.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Diffraction_Grating_Reflection.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2819 2021-11-28 01:23:58.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Diffraction_Grating_Transmission.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2445 2021-10-16 16:52:39.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens-ParaxMatrix.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3231 2021-11-28 01:19:51.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2415 2021-11-28 01:23:58.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens_3Dcolor.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3038 2021-11-28 01:23:58.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens_CommandsSystem.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2445 2021-12-09 20:11:53.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens_Cylinder.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2345 2021-11-28 01:23:59.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens_NonSec.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3162 2021-12-28 20:08:22.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens_Pupil.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3448 2021-11-28 01:23:59.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens_Pupil_Seidel.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2779 2021-11-28 01:23:59.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens_Tilt-Nulls.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2426 2021-11-28 01:20:09.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens_Tilt.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2348 2021-11-28 01:23:59.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens_Tilt_non_sec.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2245 2021-10-16 16:52:53.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens_Zernike.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2095 2021-12-28 12:33:09.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_ExtraShape_Micro_Lens_Array.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     1875 2021-10-16 16:57:43.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_ExtraShape_Radial_Sine.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     1923 2021-10-16 16:57:29.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_ExtraShape_XY_Cosines.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3229 2021-11-28 01:23:58.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Flat_Mirror_45Deg.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3470 2021-10-16 16:57:17.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_MultiCore.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     1654 2021-10-16 16:57:08.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_ParaboleMirror_Shift.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2379 2021-10-16 16:57:04.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Perfect_lens.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     1866 2021-10-16 16:56:52.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Ray.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2551 2021-11-28 01:36:12.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_RonchiTest.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2915 2021-12-05 14:35:15.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Solid_Object_STL.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3904 2021-10-16 16:56:42.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Solid_Object_STL_ARRAY.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3204 2021-10-16 16:56:37.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Sourse_Distribution_Function.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3714 2021-11-28 01:34:24.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_SpeedTest.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     6417 2021-11-28 01:23:58.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Tel_2M-STL_ImageSlicer.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2958 2021-10-16 16:53:10.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Tel_2M.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     4071 2021-10-16 16:56:11.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Tel_2M_Atmospheric_Refraction_Corrector.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     6365 2021-12-20 02:50:04.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Tel_2M_Echelle.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3138 2021-10-16 16:56:05.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Tel_2M_Error_Map.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3013 2021-10-16 16:56:00.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Tel_2M_Pupila.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3154 2021-10-16 16:55:55.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Tel_2M_Spyder_Spot_Diagram.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3529 2021-10-16 16:55:39.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Tel_2M_Spyder_Spot_RMS.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     6326 2021-12-02 18:41:07.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Tel_2M_Wavefront_Fitting.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     4139 2021-11-28 02:32:30.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Tel_2M_Wavefront_Fitting_optimization.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     4206 2021-12-09 04:32:29.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Grating.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2467 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Jherrera-ImageSlicerBW-00.scad
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     1784 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Jherrera-ImageSlicerBW-00.stl
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     4386 2021-11-28 02:38:12.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Petzval_TiltShift.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2435 2021-11-28 01:19:28.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Petzval_TiltShift_2.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2742 2021-12-16 08:38:53.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Petzval_TiltShift_Ray.py
--rwxr-xr-x   0 joelherreravazquez   (501) staff       (20)     1266 2021-08-27 16:43:29.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/Prisma.stl
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)      334 2021-09-05 08:58:57.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/TestAll.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)  1215684 2021-11-28 02:14:54.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/salida.stl
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)   715752 2021-10-16 17:03:35.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/savedRays.npy
--rw-------   0 joelherreravazquez   (501) staff       (20)    46645 2021-06-22 08:12:53.000000 KrakenOS-1.0.0.7/KrakenOS/Examples/thar_uves.dat.txt
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    12373 2021-12-16 08:39:15.000000 KrakenOS-1.0.0.7/KrakenOS/HitOnSurf.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    13465 2021-12-20 02:22:11.000000 KrakenOS-1.0.0.7/KrakenOS/InterNormalCalc.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    24832 2021-12-20 02:10:30.000000 KrakenOS-1.0.0.7/KrakenOS/KrakenSys.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     1175 2021-08-28 15:51:48.000000 KrakenOS-1.0.0.7/KrakenOS/LibRMS.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    12776 2021-12-10 20:16:49.000000 KrakenOS-1.0.0.7/KrakenOS/MathShapesClass.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)      614 2021-11-24 02:45:39.000000 KrakenOS-1.0.0.7/KrakenOS/NewthonRaphson.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3432 2021-12-02 05:16:16.000000 KrakenOS-1.0.0.7/KrakenOS/PSFCalc.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    11332 2021-11-28 02:00:08.000000 KrakenOS-1.0.0.7/KrakenOS/PhaseCalc.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     8876 2021-11-27 21:05:06.000000 KrakenOS-1.0.0.7/KrakenOS/Physics.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     7153 2021-12-09 19:51:00.000000 KrakenOS-1.0.0.7/KrakenOS/PhysicsClass.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    11307 2021-12-10 05:53:37.000000 KrakenOS-1.0.0.7/KrakenOS/Prerequisites3D.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    15725 2021-11-28 03:21:30.000000 KrakenOS-1.0.0.7/KrakenOS/PupilTool.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)      325 2021-08-28 15:51:50.000000 KrakenOS-1.0.0.7/KrakenOS/RandProb.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    21250 2021-12-03 15:07:04.000000 KrakenOS-1.0.0.7/KrakenOS/RayKeeper.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     9266 2021-09-05 07:35:38.000000 KrakenOS-1.0.0.7/KrakenOS/SeidelTool.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)      832 2021-12-10 18:22:49.000000 KrakenOS-1.0.0.7/KrakenOS/SetupClass.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2320 2021-09-09 00:43:56.000000 KrakenOS-1.0.0.7/KrakenOS/SourceRand.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    11517 2021-12-10 05:39:48.000000 KrakenOS-1.0.0.7/KrakenOS/SurfClass.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)      757 2021-11-01 00:32:30.000000 KrakenOS-1.0.0.7/KrakenOS/SurfTools.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     5632 2021-11-27 21:07:30.000000 KrakenOS-1.0.0.7/KrakenOS/SystemTools.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)      962 2021-08-28 15:51:49.000000 KrakenOS-1.0.0.7/KrakenOS/TraceLoopTool.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     1381 2021-11-05 23:33:53.000000 KrakenOS-1.0.0.7/KrakenOS/WavePlot.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     5195 2021-11-22 14:33:54.000000 KrakenOS-1.0.0.7/KrakenOS/WavefrontFit.py
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     8634 2021-10-23 02:43:03.000000 KrakenOS-1.0.0.7/KrakenOS/__init__.py
-drwxr-xr-x   0 joelherreravazquez   (501) staff       (20)        0 2022-01-24 21:03:18.016731 KrakenOS-1.0.0.7/KrakenOS.egg-info/
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)      322 2022-01-24 21:03:17.000000 KrakenOS-1.0.0.7/KrakenOS.egg-info/PKG-INFO
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)     4303 2022-01-24 21:03:17.000000 KrakenOS-1.0.0.7/KrakenOS.egg-info/SOURCES.txt
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)        1 2022-01-24 21:03:17.000000 KrakenOS-1.0.0.7/KrakenOS.egg-info/dependency_links.txt
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)       54 2022-01-24 21:03:17.000000 KrakenOS-1.0.0.7/KrakenOS.egg-info/requires.txt
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)        9 2022-01-24 21:03:17.000000 KrakenOS-1.0.0.7/KrakenOS.egg-info/top_level.txt
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    35149 2021-09-06 21:09:17.000000 KrakenOS-1.0.0.7/LICENSE.txt
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)      143 2021-09-08 17:37:10.000000 KrakenOS-1.0.0.7/MANIFEST.in
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)      322 2022-01-24 21:03:18.063812 KrakenOS-1.0.0.7/PKG-INFO
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)    22850 2021-10-07 01:28:57.000000 KrakenOS-1.0.0.7/README.md
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)       38 2022-01-24 21:03:18.064088 KrakenOS-1.0.0.7/setup.cfg
--rw-r--r--   0 joelherreravazquez   (501) staff       (20)      663 2022-01-24 21:01:25.000000 KrakenOS-1.0.0.7/setup.py
+drwxr-xr-x   0 joelherreravazquez   (501) staff       (20)        0 2022-01-25 00:49:48.299607 KrakenOS-1.0.0.9/
+drwxr-xr-x   0 joelherreravazquez   (501) staff       (20)        0 2022-01-25 00:49:48.254636 KrakenOS-1.0.0.9/KrakenOS/
+drwxr-xr-x   0 joelherreravazquez   (501) staff       (20)        0 2022-01-25 00:49:48.257539 KrakenOS-1.0.0.9/KrakenOS/AstroAtmosphere/
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)      936 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.9/KrakenOS/AstroAtmosphere/AtmosP 3.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)      937 2021-08-29 21:05:19.000000 KrakenOS-1.0.0.9/KrakenOS/AstroAtmosphere/AtmosP.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)      265 2021-08-27 17:45:53.000000 KrakenOS-1.0.0.9/KrakenOS/AstroAtmosphere/__init__.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    17979 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.9/KrakenOS/AstroAtmosphere/ciddorModel.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    30232 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.9/KrakenOS/AstroAtmosphere/dispersionModels.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    11355 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.9/KrakenOS/AstroAtmosphere/misc.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    22166 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.9/KrakenOS/AstroAtmosphere/neoslalib.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2877 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.9/KrakenOS/AstroAtmosphere/observatories.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    18492 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.9/KrakenOS/AstroAtmosphere/refractionModels.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    19964 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.9/KrakenOS/AstroAtmosphere/refractivityModels.py
+drwxr-xr-x   0 joelherreravazquez   (501) staff       (20)        0 2022-01-25 00:49:48.274742 KrakenOS-1.0.0.9/KrakenOS/Cat/
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     8196 2021-12-16 06:14:17.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/.DS_Store
+-rwxr-xr-x   0 joelherreravazquez   (501) staff       (20)     5569 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/Alum.csv
+-rwxr-xr-x   0 joelherreravazquez   (501) staff       (20)   418630 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/SCHOTT-2.AGF
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)   418630 2021-12-16 06:08:05.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/SCHOTT.AGF
+-rwxr-xr-x   0 joelherreravazquez   (501) staff       (20)     1591 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/UTILIDADES.AGF
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    24757 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/archer.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3344 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/arton.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    64489 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/birefringent.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)   271332 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/cdgm.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)   147112 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/corning.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2062 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/heraeus.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)   538064 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/hikari.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)  1214752 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/hoya.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    50293 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/infrared.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2114 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/isuzu.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2343 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/liebetraut.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    14802 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/lightpath.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    93256 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/lzos.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    25326 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/misc.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)   652183 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/nikon.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)   715345 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/ohara.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     4336 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/rad_hard.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    61862 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/rpo.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)   228484 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/schott-1.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)   142366 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/sumita.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     1611 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/topas.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     1782 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/umicore.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2078 2019-12-26 00:32:18.000000 KrakenOS-1.0.0.9/KrakenOS/Cat/zeon.agf
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    14654 2021-12-28 18:37:03.000000 KrakenOS-1.0.0.9/KrakenOS/Display.py
+drwxr-xr-x   0 joelherreravazquez   (501) staff       (20)        0 2022-01-25 00:49:48.275146 KrakenOS-1.0.0.9/KrakenOS/Docs/
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     6148 2021-10-07 01:21:28.000000 KrakenOS-1.0.0.9/KrakenOS/Docs/.DS_Store
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)  4677716 2021-09-06 21:35:21.000000 KrakenOS-1.0.0.9/KrakenOS/Docs/USER_MANUAL_KrakenOS_Provisional.pdf
+drwxr-xr-x   0 joelherreravazquez   (501) staff       (20)        0 2022-01-25 00:49:48.298019 KrakenOS-1.0.0.9/KrakenOS/Examples/
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     6148 2022-01-25 00:49:21.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/.DS_Store
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     1566 2021-12-17 16:08:16.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp-Tel-6.5m-RAY.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     7427 2021-11-28 01:26:45.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp-Tel-6.5m.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2025 2021-10-16 16:52:26.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Axicon.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2240 2021-11-28 01:23:58.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Axicon_And_Cylinder.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2659 2021-12-07 17:10:35.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Diffraction_Grating_Reflection.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2819 2021-11-28 01:23:58.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Diffraction_Grating_Transmission.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2445 2021-10-16 16:52:39.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens-ParaxMatrix.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3231 2021-11-28 01:19:51.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2415 2021-11-28 01:23:58.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens_3Dcolor.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3038 2021-11-28 01:23:58.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens_CommandsSystem.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2445 2021-12-09 20:11:53.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens_Cylinder.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2345 2021-11-28 01:23:59.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens_NonSec.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3162 2021-12-28 20:08:22.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens_Pupil.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3448 2021-11-28 01:23:59.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens_Pupil_Seidel.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2779 2021-11-28 01:23:59.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens_Tilt-Nulls.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2426 2021-11-28 01:20:09.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens_Tilt.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2348 2021-11-28 01:23:59.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens_Tilt_non_sec.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2249 2022-01-25 00:45:51.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens_Zernike.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2095 2021-12-28 12:33:09.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_ExtraShape_Micro_Lens_Array.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     1875 2021-10-16 16:57:43.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_ExtraShape_Radial_Sine.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     1923 2021-10-16 16:57:29.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_ExtraShape_XY_Cosines.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3229 2021-11-28 01:23:58.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Flat_Mirror_45Deg.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3470 2021-10-16 16:57:17.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_MultiCore.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     1654 2021-10-16 16:57:08.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_ParaboleMirror_Shift.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2379 2021-10-16 16:57:04.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Perfect_lens.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     1866 2021-10-16 16:56:52.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Ray.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2551 2021-11-28 01:36:12.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_RonchiTest.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2915 2021-12-05 14:35:15.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Solid_Object_STL.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3904 2021-10-16 16:56:42.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Solid_Object_STL_ARRAY.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3204 2021-10-16 16:56:37.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Sourse_Distribution_Function.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3714 2021-11-28 01:34:24.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_SpeedTest.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     6417 2021-11-28 01:23:58.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Tel_2M-STL_ImageSlicer.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2958 2021-10-16 16:53:10.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Tel_2M.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     4071 2021-10-16 16:56:11.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Tel_2M_Atmospheric_Refraction_Corrector.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3138 2021-10-16 16:56:05.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Tel_2M_Error_Map.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3013 2021-10-16 16:56:00.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Tel_2M_Pupila.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3154 2021-10-16 16:55:55.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Tel_2M_Spyder_Spot_Diagram.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3529 2021-10-16 16:55:39.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Tel_2M_Spyder_Spot_RMS.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     6326 2021-12-02 18:41:07.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Tel_2M_Wavefront_Fitting.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     4139 2021-11-28 02:32:30.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Tel_2M_Wavefront_Fitting_optimization.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     4206 2021-12-09 04:32:29.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Grating.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2467 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Jherrera-ImageSlicerBW-00.scad
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     1784 2021-08-27 16:43:28.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Jherrera-ImageSlicerBW-00.stl
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     4386 2021-11-28 02:38:12.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Petzval_TiltShift.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2435 2021-11-28 01:19:28.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Petzval_TiltShift_2.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2742 2021-12-16 08:38:53.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Petzval_TiltShift_Ray.py
+-rwxr-xr-x   0 joelherreravazquez   (501) staff       (20)     1266 2021-08-27 16:43:29.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/Prisma.stl
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)      334 2021-09-05 08:58:57.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/TestAll.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)  1215684 2022-01-24 22:24:33.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/salida.stl
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)   715752 2021-10-16 17:03:35.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/savedRays.npy
+-rw-------   0 joelherreravazquez   (501) staff       (20)    46645 2021-06-22 08:12:53.000000 KrakenOS-1.0.0.9/KrakenOS/Examples/thar_uves.dat.txt
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    12373 2021-12-16 08:39:15.000000 KrakenOS-1.0.0.9/KrakenOS/HitOnSurf.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    13465 2021-12-20 02:22:11.000000 KrakenOS-1.0.0.9/KrakenOS/InterNormalCalc.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    24832 2021-12-20 02:10:30.000000 KrakenOS-1.0.0.9/KrakenOS/KrakenSys.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     1175 2021-08-28 15:51:48.000000 KrakenOS-1.0.0.9/KrakenOS/LibRMS.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    12802 2022-01-25 00:24:38.000000 KrakenOS-1.0.0.9/KrakenOS/MathShapesClass.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)      614 2021-11-24 02:45:39.000000 KrakenOS-1.0.0.9/KrakenOS/NewthonRaphson.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     3432 2021-12-02 05:16:16.000000 KrakenOS-1.0.0.9/KrakenOS/PSFCalc.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    11332 2021-11-28 02:00:08.000000 KrakenOS-1.0.0.9/KrakenOS/PhaseCalc.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     8876 2021-11-27 21:05:06.000000 KrakenOS-1.0.0.9/KrakenOS/Physics.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     7153 2021-12-09 19:51:00.000000 KrakenOS-1.0.0.9/KrakenOS/PhysicsClass.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    11307 2021-12-10 05:53:37.000000 KrakenOS-1.0.0.9/KrakenOS/Prerequisites3D.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    15725 2021-11-28 03:21:30.000000 KrakenOS-1.0.0.9/KrakenOS/PupilTool.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)      325 2021-08-28 15:51:50.000000 KrakenOS-1.0.0.9/KrakenOS/RandProb.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    21250 2021-12-03 15:07:04.000000 KrakenOS-1.0.0.9/KrakenOS/RayKeeper.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     9266 2021-09-05 07:35:38.000000 KrakenOS-1.0.0.9/KrakenOS/SeidelTool.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)      832 2021-12-10 18:22:49.000000 KrakenOS-1.0.0.9/KrakenOS/SetupClass.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     2320 2021-09-09 00:43:56.000000 KrakenOS-1.0.0.9/KrakenOS/SourceRand.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    11517 2021-12-10 05:39:48.000000 KrakenOS-1.0.0.9/KrakenOS/SurfClass.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)      757 2021-11-01 00:32:30.000000 KrakenOS-1.0.0.9/KrakenOS/SurfTools.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     5632 2021-11-27 21:07:30.000000 KrakenOS-1.0.0.9/KrakenOS/SystemTools.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)      962 2021-08-28 15:51:49.000000 KrakenOS-1.0.0.9/KrakenOS/TraceLoopTool.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     1381 2021-11-05 23:33:53.000000 KrakenOS-1.0.0.9/KrakenOS/WavePlot.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     5195 2021-11-22 14:33:54.000000 KrakenOS-1.0.0.9/KrakenOS/WavefrontFit.py
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     8634 2021-10-23 02:43:03.000000 KrakenOS-1.0.0.9/KrakenOS/__init__.py
+drwxr-xr-x   0 joelherreravazquez   (501) staff       (20)        0 2022-01-25 00:49:48.255380 KrakenOS-1.0.0.9/KrakenOS.egg-info/
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)      322 2022-01-25 00:49:48.000000 KrakenOS-1.0.0.9/KrakenOS.egg-info/PKG-INFO
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)     4261 2022-01-25 00:49:48.000000 KrakenOS-1.0.0.9/KrakenOS.egg-info/SOURCES.txt
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)        1 2022-01-25 00:49:48.000000 KrakenOS-1.0.0.9/KrakenOS.egg-info/dependency_links.txt
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)       54 2022-01-25 00:49:48.000000 KrakenOS-1.0.0.9/KrakenOS.egg-info/requires.txt
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)        9 2022-01-25 00:49:48.000000 KrakenOS-1.0.0.9/KrakenOS.egg-info/top_level.txt
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    35149 2021-09-06 21:09:17.000000 KrakenOS-1.0.0.9/LICENSE.txt
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)      143 2021-09-08 17:37:10.000000 KrakenOS-1.0.0.9/MANIFEST.in
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)      322 2022-01-25 00:49:48.299423 KrakenOS-1.0.0.9/PKG-INFO
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)    22850 2021-10-07 01:28:57.000000 KrakenOS-1.0.0.9/README.md
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)       38 2022-01-25 00:49:48.299669 KrakenOS-1.0.0.9/setup.cfg
+-rw-r--r--   0 joelherreravazquez   (501) staff       (20)      663 2022-01-25 00:49:32.000000 KrakenOS-1.0.0.9/setup.py
```

### Comparing `KrakenOS-1.0.0.7/KrakenOS/AstroAtmosphere/AtmosP 3.py` & `KrakenOS-1.0.0.9/KrakenOS/AstroAtmosphere/AtmosP 3.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/AstroAtmosphere/AtmosP.py` & `KrakenOS-1.0.0.9/KrakenOS/AstroAtmosphere/AtmosP.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/AstroAtmosphere/ciddorModel.py` & `KrakenOS-1.0.0.9/KrakenOS/AstroAtmosphere/ciddorModel.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/AstroAtmosphere/dispersionModels.py` & `KrakenOS-1.0.0.9/KrakenOS/AstroAtmosphere/dispersionModels.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/AstroAtmosphere/misc.py` & `KrakenOS-1.0.0.9/KrakenOS/AstroAtmosphere/misc.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/AstroAtmosphere/neoslalib.py` & `KrakenOS-1.0.0.9/KrakenOS/AstroAtmosphere/neoslalib.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/AstroAtmosphere/observatories.py` & `KrakenOS-1.0.0.9/KrakenOS/AstroAtmosphere/observatories.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/AstroAtmosphere/refractionModels.py` & `KrakenOS-1.0.0.9/KrakenOS/AstroAtmosphere/refractionModels.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/AstroAtmosphere/refractivityModels.py` & `KrakenOS-1.0.0.9/KrakenOS/AstroAtmosphere/refractivityModels.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/.DS_Store` & `KrakenOS-1.0.0.9/KrakenOS/Cat/.DS_Store`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/Alum.csv` & `KrakenOS-1.0.0.9/KrakenOS/Cat/Alum.csv`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/SCHOTT-2.AGF` & `KrakenOS-1.0.0.9/KrakenOS/Cat/SCHOTT-2.AGF`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/SCHOTT.AGF` & `KrakenOS-1.0.0.9/KrakenOS/Cat/SCHOTT.AGF`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/UTILIDADES.AGF` & `KrakenOS-1.0.0.9/KrakenOS/Cat/UTILIDADES.AGF`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/archer.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/archer.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/arton.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/arton.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/birefringent.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/birefringent.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/cdgm.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/cdgm.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/corning.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/corning.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/heraeus.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/heraeus.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/hikari.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/hikari.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/hoya.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/hoya.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/infrared.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/infrared.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/isuzu.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/isuzu.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/liebetraut.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/liebetraut.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/lightpath.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/lightpath.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/lzos.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/lzos.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/misc.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/misc.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/nikon.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/nikon.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/ohara.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/ohara.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/rad_hard.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/rad_hard.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/rpo.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/rpo.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/schott-1.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/schott-1.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/sumita.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/sumita.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/topas.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/topas.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/umicore.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/umicore.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Cat/zeon.agf` & `KrakenOS-1.0.0.9/KrakenOS/Cat/zeon.agf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Display.py` & `KrakenOS-1.0.0.9/KrakenOS/Display.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Docs/.DS_Store` & `KrakenOS-1.0.0.9/KrakenOS/Docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Docs/USER_MANUAL_KrakenOS_Provisional.pdf` & `KrakenOS-1.0.0.9/KrakenOS/Docs/USER_MANUAL_KrakenOS_Provisional.pdf`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/.DS_Store` & `KrakenOS-1.0.0.9/KrakenOS/Examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp-Tel-6.5m-RAY.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp-Tel-6.5m-RAY.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp-Tel-6.5m.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp-Tel-6.5m.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Axicon.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Axicon.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Axicon_And_Cylinder.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Axicon_And_Cylinder.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Diffraction_Grating_Reflection.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Diffraction_Grating_Reflection.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Diffraction_Grating_Transmission.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Diffraction_Grating_Transmission.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens-ParaxMatrix.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens-ParaxMatrix.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens_3Dcolor.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens_3Dcolor.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens_CommandsSystem.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens_CommandsSystem.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens_Cylinder.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens_Cylinder.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens_NonSec.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens_NonSec.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens_Pupil.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens_Pupil.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens_Pupil_Seidel.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens_Pupil_Seidel.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens_Tilt-Nulls.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens_Tilt-Nulls.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens_Tilt.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens_Tilt.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens_Tilt_non_sec.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens_Tilt_non_sec.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Doublet_Lens_Zernike.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Doublet_Lens_Zernike.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 P_Ima.Diameter = 100.0
 
 # ______________________________________#
 
 A = [P_Obj, L1a, L1b, L1c, P_Ima]
 configuracion_1 = Kos.Setup()
 
+
 # ______________________________________#
 
 Doblete = Kos.system(A, configuracion_1)
 Rayos = Kos.raykeeper(Doblete)
 
 # ______________________________________#
 
@@ -95,13 +96,14 @@
         r = np.sqrt((x_0 * x_0) + (y_0 * y_0))
         if r < rad:
             tet = 0.0
             pSource_0 = [x_0, y_0, 0.0]
             dCos = [0.0, np.sin(np.deg2rad(tet)), np.cos(np.deg2rad(tet))]
             W = 0.4
             Doblete.Trace(pSource_0, dCos, W)
+
             Rayos.push()
 
 # ______________________________________#
 
 Kos.display3d(Doblete, Rayos, 2)
 Kos.display2d(Doblete, Rayos, 1)
```

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_ExtraShape_Micro_Lens_Array.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_ExtraShape_Micro_Lens_Array.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_ExtraShape_Radial_Sine.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_ExtraShape_Radial_Sine.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_ExtraShape_XY_Cosines.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_ExtraShape_XY_Cosines.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Flat_Mirror_45Deg.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Flat_Mirror_45Deg.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_MultiCore.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_MultiCore.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_ParaboleMirror_Shift.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_ParaboleMirror_Shift.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Perfect_lens.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Perfect_lens.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Ray.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Ray.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_RonchiTest.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_RonchiTest.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Solid_Object_STL.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Solid_Object_STL.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Solid_Object_STL_ARRAY.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Solid_Object_STL_ARRAY.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Sourse_Distribution_Function.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Sourse_Distribution_Function.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_SpeedTest.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_SpeedTest.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Tel_2M-STL_ImageSlicer.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Tel_2M-STL_ImageSlicer.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Tel_2M.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Tel_2M.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Tel_2M_Atmospheric_Refraction_Corrector.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Tel_2M_Atmospheric_Refraction_Corrector.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Tel_2M_Error_Map.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Tel_2M_Error_Map.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Tel_2M_Pupila.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Tel_2M_Pupila.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Tel_2M_Spyder_Spot_Diagram.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Tel_2M_Spyder_Spot_Diagram.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Tel_2M_Spyder_Spot_RMS.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Tel_2M_Spyder_Spot_RMS.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Tel_2M_Wavefront_Fitting.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Tel_2M_Wavefront_Fitting.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Examp_Tel_2M_Wavefront_Fitting_optimization.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Examp_Tel_2M_Wavefront_Fitting_optimization.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Grating.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Grating.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Jherrera-ImageSlicerBW-00.scad` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Jherrera-ImageSlicerBW-00.scad`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Jherrera-ImageSlicerBW-00.stl` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Jherrera-ImageSlicerBW-00.stl`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Petzval_TiltShift.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Petzval_TiltShift.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Petzval_TiltShift_2.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Petzval_TiltShift_2.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Petzval_TiltShift_Ray.py` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Petzval_TiltShift_Ray.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/Prisma.stl` & `KrakenOS-1.0.0.9/KrakenOS/Examples/Prisma.stl`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/salida.stl` & `KrakenOS-1.0.0.9/KrakenOS/Examples/salida.stl`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/savedRays.npy` & `KrakenOS-1.0.0.9/KrakenOS/Examples/savedRays.npy`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Examples/thar_uves.dat.txt` & `KrakenOS-1.0.0.9/KrakenOS/Examples/thar_uves.dat.txt`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/HitOnSurf.py` & `KrakenOS-1.0.0.9/KrakenOS/HitOnSurf.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/InterNormalCalc.py` & `KrakenOS-1.0.0.9/KrakenOS/InterNormalCalc.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/KrakenSys.py` & `KrakenOS-1.0.0.9/KrakenOS/KrakenSys.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/LibRMS.py` & `KrakenOS-1.0.0.9/KrakenOS/LibRMS.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/MathShapesClass.py` & `KrakenOS-1.0.0.9/KrakenOS/MathShapesClass.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from numba import jit
-from numba.experimental import jitclass
-from numba import int32, float32
+# from numba import jit
+# from numba.experimental import jitclass
+# from numba import int32, float32
 
 # @jit(forceobj=True)
 import numpy as np
 from scipy.interpolate import griddata
 
 
 
@@ -35,15 +35,15 @@
         y :
             y
         """
         Z = self.user_surface(x, y, self.COEF)
         return Z
 
 
-@jit(forceobj=True)
+# @jit(forceobj=True)
 def even_asphere(x, y, E):
     """even_asphere.
 
     Parameters
     ----------
     x :
         x
@@ -126,15 +126,15 @@
             y
         """
 
         z = CalculateCon(x, y, self.R_C , self.C_RXY_RATIO, self.KON)
 
         return z
 
-@jit(nopython=True)
+# @jit(nopython=True)
 def CalculateCon(x, y, R_C , C_RXY_RATIO, KON):
     """calculate.
 
     Parameters
     ----------
     x :
         x
@@ -186,15 +186,15 @@
         #     z_axicon = (s * np.tan(np.deg2rad(self.AXC)))
         # else:
         #     z_axicon = np.zeros_like(x)
 
         z_axicon = CalculateAxic( x, y, self.C_RXY_RATIO, self.AXC)
         return z_axicon
 
-@jit(nopython=True)
+# @jit(nopython=True)
 def CalculateAxic( x, y, C_RXY_RATIO, AXC):
     """calculate.
 
     Parameters
     ----------
     x :
         x
@@ -337,15 +337,15 @@
         #         ZSP = (ZSP + (self.COEF[i] * zernike_polynomials(i, p, f, self.Z_POL, self.Z_POW)))
 
         ZSP = CalculateZern(x, y, self.Z_POL, self.Z_POW, self.COEF, self.DMTR)
         return ZSP
 
 
 
-@jit(forceobj=True)
+# @jit(forceobj=True)
 def CalculateZern( x, y, Z_POL, Z_POW, COEF, DMTR):
     """calculate.
 
     Parameters
     ----------
     x :
         x
@@ -360,15 +360,15 @@
             ZSP = (ZSP + (COEF[i] * zernike_polynomials(i, p, f, Z_POL, Z_POW)))
     return ZSP
 
 
 
 
 
-@jit(forceobj=True)
+# @jit(forceobj=True)
 def zernike_polynomials(term, ro, theta, Zern_pol, z_pow):
     """zernike_polynomials.
 
     Parameters
     ----------
     term :
         term
@@ -397,15 +397,15 @@
     return S
 
 
 
 
 
 
-@jit(forceobj=True)
+# @jit(forceobj=True)
 def z_parity(num):
     """z_parity.
 
     Parameters
     ----------
     num :
         num
@@ -420,15 +420,15 @@
 
 
 
 
 
 
 
-@jit(forceobj=True)
+# @jit(forceobj=True)
 def r_zern(m, n):
     """r_zern.
 
     Parameters
     ----------
     m :
         m
@@ -454,15 +454,15 @@
 
 
 
 
 
 
 
-@jit(forceobj=True)
+# @jit(forceobj=True)
 def zernike_expand(L):
     """zernike_expand.
 
     Parameters
     ----------
     L :
         L
@@ -507,15 +507,15 @@
 
 
 
 
 
 
 
-@jit(forceobj=True)
+# @jit(forceobj=True)
 def zernike_math_notation(term, Zern_pol, z_pow):
     """zernike_math_notation.
 
     Parameters
     ----------
     term :
         term
@@ -552,15 +552,15 @@
     else:
         x = ''
     return ((S + '   ') + x)
 
 
 
 
-@jit(forceobj=True)
+# @jit(forceobj=True)
 def Wavefront_Zernike_Phase(x, y, COEF):
     """Wavefront_Zernike_Phase.
 
     Parameters
     ----------
     x :
         x
```

### Comparing `KrakenOS-1.0.0.7/KrakenOS/NewthonRaphson.py` & `KrakenOS-1.0.0.9/KrakenOS/NewthonRaphson.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/PSFCalc.py` & `KrakenOS-1.0.0.9/KrakenOS/PSFCalc.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/PhaseCalc.py` & `KrakenOS-1.0.0.9/KrakenOS/PhaseCalc.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Physics.py` & `KrakenOS-1.0.0.9/KrakenOS/Physics.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/PhysicsClass.py` & `KrakenOS-1.0.0.9/KrakenOS/PhysicsClass.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/Prerequisites3D.py` & `KrakenOS-1.0.0.9/KrakenOS/Prerequisites3D.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/PupilTool.py` & `KrakenOS-1.0.0.9/KrakenOS/PupilTool.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/RayKeeper.py` & `KrakenOS-1.0.0.9/KrakenOS/RayKeeper.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/SeidelTool.py` & `KrakenOS-1.0.0.9/KrakenOS/SeidelTool.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/SetupClass.py` & `KrakenOS-1.0.0.9/KrakenOS/SetupClass.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/SourceRand.py` & `KrakenOS-1.0.0.9/KrakenOS/SourceRand.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/SurfClass.py` & `KrakenOS-1.0.0.9/KrakenOS/SurfClass.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/SurfTools.py` & `KrakenOS-1.0.0.9/KrakenOS/SurfTools.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/SystemTools.py` & `KrakenOS-1.0.0.9/KrakenOS/SystemTools.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/TraceLoopTool.py` & `KrakenOS-1.0.0.9/KrakenOS/TraceLoopTool.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/WavePlot.py` & `KrakenOS-1.0.0.9/KrakenOS/WavePlot.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/WavefrontFit.py` & `KrakenOS-1.0.0.9/KrakenOS/WavefrontFit.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS/__init__.py` & `KrakenOS-1.0.0.9/KrakenOS/__init__.py`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/KrakenOS.egg-info/SOURCES.txt` & `KrakenOS-1.0.0.9/KrakenOS.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,14 @@
 KrakenOS/Examples/Examp_Solid_Object_STL.py
 KrakenOS/Examples/Examp_Solid_Object_STL_ARRAY.py
 KrakenOS/Examples/Examp_Sourse_Distribution_Function.py
 KrakenOS/Examples/Examp_SpeedTest.py
 KrakenOS/Examples/Examp_Tel_2M-STL_ImageSlicer.py
 KrakenOS/Examples/Examp_Tel_2M.py
 KrakenOS/Examples/Examp_Tel_2M_Atmospheric_Refraction_Corrector.py
-KrakenOS/Examples/Examp_Tel_2M_Echelle.py
 KrakenOS/Examples/Examp_Tel_2M_Error_Map.py
 KrakenOS/Examples/Examp_Tel_2M_Pupila.py
 KrakenOS/Examples/Examp_Tel_2M_Spyder_Spot_Diagram.py
 KrakenOS/Examples/Examp_Tel_2M_Spyder_Spot_RMS.py
 KrakenOS/Examples/Examp_Tel_2M_Wavefront_Fitting.py
 KrakenOS/Examples/Examp_Tel_2M_Wavefront_Fitting_optimization.py
 KrakenOS/Examples/Grating.py
```

### Comparing `KrakenOS-1.0.0.7/LICENSE.txt` & `KrakenOS-1.0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/README.md` & `KrakenOS-1.0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `KrakenOS-1.0.0.7/setup.py` & `KrakenOS-1.0.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='KrakenOS',
-    version='1.0.0.7',
+    version='1.0.0.9',
     packages=['KrakenOS', 'KrakenOS.AstroAtmosphere', 'KrakenOS.Cat', 'KrakenOS.Examples', 'KrakenOS.Docs'],
 
     install_requires=['pyvista','PyVTK','vtk','numpy','scipy','matplotlib', 'csv342', 'numba' ],
     package_data={'': ['LICENSE.txt', '../*.AGF', '../*.agf', '../*.stl', '../*.scad', '../*.pdf']},
     include_package_data=True,
     url='https://github.com/Garchupiter/Kraken-Optical-Simulator',
     license='GNU General Public License v3.0',
```

