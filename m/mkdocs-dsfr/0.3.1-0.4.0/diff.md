# Comparing `tmp/mkdocs_dsfr-0.3.1.tar.gz` & `tmp/mkdocs_dsfr-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_dsfr-0.3.1.tar", last modified: Mon Jul  3 13:34:12 2023, max compression
+gzip compressed data, was "mkdocs_dsfr-0.4.0.tar", last modified: Tue Jul  4 15:15:39 2023, max compression
```

## Comparing `mkdocs_dsfr-0.3.1.tar` & `mkdocs_dsfr-0.4.0.tar`

### file list

```diff
@@ -1,944 +1,944 @@
--rw-r--r--   0        0        0     1096 2023-05-31 09:02:27.963069 mkdocs_dsfr-0.3.1/LICENSE
--rw-r--r--   0        0        0      494 2023-06-30 15:05:52.158435 mkdocs_dsfr-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-05-31 09:02:27.964132 mkdocs_dsfr-0.3.1/dsfr/__init__.py
--rw-r--r--   0        0        0    16409 2023-06-02 13:12:07.563999 mkdocs_dsfr-0.3.1/dsfr/artwork/background/ovoid.svg
--rw-r--r--   0        0        0     3884 2023-06-02 13:12:07.437000 mkdocs_dsfr-0.3.1/dsfr/artwork/dark.svg
--rw-r--r--   0        0        0     4750 2023-06-02 13:12:07.526999 mkdocs_dsfr-0.3.1/dsfr/artwork/light.svg
--rw-r--r--   0        0        0     5712 2023-06-02 13:12:07.420000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/buildings/city-hall.svg
--rw-r--r--   0        0        0     6612 2023-06-02 13:12:07.459000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/buildings/factory.svg
--rw-r--r--   0        0        0     3564 2023-06-02 13:12:07.516000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/buildings/house.svg
--rw-r--r--   0        0        0    10932 2023-06-02 13:12:07.562999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/buildings/nuclear-plant.svg
--rw-r--r--   0        0        0     5534 2023-06-02 13:12:07.595999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/buildings/school.svg
--rw-r--r--   0        0        0     5409 2023-06-02 13:12:07.378999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/digital/application.svg
--rw-r--r--   0        0        0     4327 2023-06-02 13:12:07.390000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/digital/avatar.svg
--rw-r--r--   0        0        0     4158 2023-06-02 13:12:07.407999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/digital/calendar.svg
--rw-r--r--   0        0        0     4015 2023-06-02 13:12:07.426000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/digital/coding.svg
--rw-r--r--   0        0        0     5502 2023-06-02 13:12:07.437999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/digital/data-visualization.svg
--rw-r--r--   0        0        0     7230 2023-06-02 13:12:07.523999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/digital/internet.svg
--rw-r--r--   0        0        0     3993 2023-06-02 13:12:07.542000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/digital/mail-send.svg
--rw-r--r--   0        0        0     3191 2023-06-02 13:12:07.596999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/digital/search.svg
--rw-r--r--   0        0        0     4823 2023-06-02 13:12:07.430000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/document/contract.svg
--rw-r--r--   0        0        0     2599 2023-06-02 13:12:07.443000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/document/document-add.svg
--rw-r--r--   0        0        0     3905 2023-06-02 13:12:07.444000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/document/document-download.svg
--rw-r--r--   0        0        0     3201 2023-06-02 13:12:07.444000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/document/document-signature.svg
--rw-r--r--   0        0        0     2453 2023-06-02 13:12:07.444000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/document/document.svg
--rw-r--r--   0        0        0     4716 2023-06-02 13:12:07.448999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/document/driving-licence.svg
--rw-r--r--   0        0        0     4210 2023-06-02 13:12:07.559000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/document/national-identity-card.svg
--rw-r--r--   0        0        0     3572 2023-06-02 13:12:07.569999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/document/passport.svg
--rw-r--r--   0        0        0    10659 2023-06-02 13:12:07.625999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/document/tax-stamp.svg
--rw-r--r--   0        0        0     5360 2023-06-02 13:12:07.650000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/document/vehicle-registration.svg
--rw-r--r--   0        0        0     8630 2023-06-02 13:12:07.453999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/environment/environment.svg
--rw-r--r--   0        0        0     5177 2023-06-02 13:12:07.471999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/environment/food.svg
--rw-r--r--   0        0        0     6131 2023-06-02 13:12:07.503000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/environment/grocery.svg
--rw-r--r--   0        0        0    10973 2023-06-02 13:12:07.516999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/environment/human-cooperation.svg
--rw-r--r--   0        0        0     5704 2023-06-02 13:12:07.526999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/environment/leaf.svg
--rw-r--r--   0        0        0     2809 2023-06-02 13:12:07.555999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/environment/moon.svg
--rw-r--r--   0        0        0     4263 2023-06-02 13:12:07.558000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/environment/mountain.svg
--rw-r--r--   0        0        0     3555 2023-06-02 13:12:07.618999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/environment/sun.svg
--rw-r--r--   0        0        0     6161 2023-06-02 13:12:07.638000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/environment/tree.svg
--rw-r--r--   0        0        0     7177 2023-06-02 13:12:07.512000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/health/health.svg
--rw-r--r--   0        0        0     3577 2023-06-02 13:12:07.515000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/health/hospital.svg
--rw-r--r--   0        0        0     7720 2023-06-02 13:12:07.648999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/health/vaccine.svg
--rw-r--r--   0        0        0     8264 2023-06-02 13:12:07.653000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/health/virus.svg
--rw-r--r--   0        0        0     8682 2023-06-02 13:12:07.467000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/institutions/firefighter.svg
--rw-r--r--   0        0        0     5880 2023-06-02 13:12:07.484999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/institutions/gendarmerie.svg
--rw-r--r--   0        0        0     4778 2023-06-02 13:12:07.525000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/institutions/justice.svg
--rw-r--r--   0        0        0    16555 2023-06-02 13:12:07.553999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/institutions/money.svg
--rw-r--r--   0        0        0     8621 2023-06-02 13:12:07.578999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/institutions/police.svg
--rw-r--r--   0        0        0     7856 2023-06-02 13:12:07.398000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/leisure/book.svg
--rw-r--r--   0        0        0     4138 2023-06-02 13:12:07.427000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/leisure/community.svg
--rw-r--r--   0        0        0     6782 2023-06-02 13:12:07.434000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/leisure/culture.svg
--rw-r--r--   0        0        0     4973 2023-06-02 13:12:07.440999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/leisure/digital-art.svg
--rw-r--r--   0        0        0     6890 2023-06-02 13:12:07.565999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/leisure/paint.svg
--rw-r--r--   0        0        0     6799 2023-06-02 13:12:07.371999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/map/airport.svg
--rw-r--r--   0        0        0    15123 2023-06-02 13:12:07.533999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/map/location-france.svg
--rw-r--r--   0        0        0     4427 2023-06-02 13:12:07.538000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/map/luggage.svg
--rw-r--r--   0        0        0     7293 2023-06-02 13:12:07.543999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/map/map.svg
--rw-r--r--   0        0        0     2791 2023-06-02 13:12:07.430000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/system/connection-lost.svg
--rw-r--r--   0        0        0     2098 2023-06-02 13:12:07.456000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/system/error.svg
--rw-r--r--   0        0        0     3506 2023-06-02 13:12:07.520999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/system/information.svg
--rw-r--r--   0        0        0     4103 2023-06-02 13:12:07.561000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/system/notification.svg
--rw-r--r--   0        0        0     2592 2023-06-02 13:12:07.565000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/system/padlock.svg
--rw-r--r--   0        0        0     1985 2023-06-02 13:12:07.615999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/system/success.svg
--rw-r--r--   0        0        0    15162 2023-06-02 13:12:07.621999 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/system/system.svg
--rw-r--r--   0        0        0     4442 2023-06-02 13:12:07.628000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/system/technical-error.svg
--rw-r--r--   0        0        0     1577 2023-06-02 13:12:07.657000 mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/system/warning.svg
--rw-r--r--   0        0        0    15015 2023-06-02 13:12:07.621999 mkdocs_dsfr-0.3.1/dsfr/artwork/system.svg
--rw-r--r--   0        0        0    10383 2023-07-03 13:25:56.386252 mkdocs_dsfr-0.3.1/dsfr/base.html
--rw-r--r--   0        0        0     5366 2023-05-31 09:02:27.964627 mkdocs_dsfr-0.3.1/dsfr/css/theme.css
--rw-r--r--   0        0        0   137467 2023-07-03 13:33:47.318429 mkdocs_dsfr-0.3.1/dsfr/dsfr.min.css
--rw-r--r--   0        0        0    68681 2023-06-02 13:12:06.859999 mkdocs_dsfr-0.3.1/dsfr/dsfr.module.min.js
--rw-r--r--   0        0        0   218391 2023-06-02 13:12:06.865000 mkdocs_dsfr-0.3.1/dsfr/dsfr.nomodule.min.js
--rw-r--r--   0        0        0     3631 2023-06-02 13:12:07.177000 mkdocs_dsfr-0.3.1/dsfr/favicon/android-chrome-192x192.png
--rw-r--r--   0        0        0     9190 2023-06-02 13:12:07.177000 mkdocs_dsfr-0.3.1/dsfr/favicon/android-chrome-512x512.png
--rw-r--r--   0        0        0     3448 2023-06-02 13:12:07.177999 mkdocs_dsfr-0.3.1/dsfr/favicon/apple-touch-icon.png
--rw-r--r--   0        0        0     7406 2023-06-02 13:12:06.809999 mkdocs_dsfr-0.3.1/dsfr/favicon/favicon.ico
--rw-r--r--   0        0        0     6360 2023-06-02 13:12:07.460000 mkdocs_dsfr-0.3.1/dsfr/favicon/favicon.svg
--rw-r--r--   0        0        0      292 2023-06-02 13:12:07.661999 mkdocs_dsfr-0.3.1/dsfr/favicon/manifest.webmanifest
--rwxr-xr-x   0        0        0    52216 2023-06-02 13:12:07.664000 mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Bold.woff
--rwxr-xr-x   0        0        0    42092 2023-06-02 13:12:07.674999 mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Bold.woff2
--rwxr-xr-x   0        0        0    56436 2023-06-02 13:12:07.661999 mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Bold_Italic.woff
--rwxr-xr-x   0        0        0    45300 2023-06-02 13:12:07.674000 mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Bold_Italic.woff2
--rwxr-xr-x   0        0        0    50440 2023-06-02 13:12:07.665999 mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Light.woff
--rwxr-xr-x   0        0        0    41368 2023-06-02 13:12:07.677000 mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Light.woff2
--rwxr-xr-x   0        0        0    54492 2023-06-02 13:12:07.664999 mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Light_Italic.woff
--rwxr-xr-x   0        0        0    43916 2023-06-02 13:12:07.676000 mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Light_Italic.woff2
--rwxr-xr-x   0        0        0    51292 2023-06-02 13:12:07.667999 mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Medium.woff
--rwxr-xr-x   0        0        0    41940 2023-06-02 13:12:07.678999 mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Medium.woff2
--rwxr-xr-x   0        0        0    54680 2023-06-02 13:12:07.667000 mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Medium_Italic.woff
--rwxr-xr-x   0        0        0    44572 2023-06-02 13:12:07.677999 mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Medium_Italic.woff2
--rwxr-xr-x   0        0        0    51140 2023-06-02 13:12:07.670000 mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Regular.woff
--rwxr-xr-x   0        0        0    41328 2023-06-02 13:12:07.680999 mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Regular.woff2
--rwxr-xr-x   0        0        0    54328 2023-06-02 13:12:07.668999 mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Regular_Italic.woff
--rwxr-xr-x   0        0        0    44284 2023-06-02 13:12:07.680000 mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Regular_Italic.woff2
--rw-r--r--   0        0        0   114508 2023-06-02 13:12:07.671000 mkdocs_dsfr-0.3.1/dsfr/fonts/Spectral-ExtraBold.woff
--rw-r--r--   0        0        0    80368 2023-06-02 13:12:07.681999 mkdocs_dsfr-0.3.1/dsfr/fonts/Spectral-ExtraBold.woff2
--rw-r--r--   0        0        0   114016 2023-06-02 13:12:07.673000 mkdocs_dsfr-0.3.1/dsfr/fonts/Spectral-Regular.woff
--rw-r--r--   0        0        0    79472 2023-06-02 13:12:07.684000 mkdocs_dsfr-0.3.1/dsfr/fonts/Spectral-Regular.woff2
--rw-r--r--   0        0        0     3076 2023-06-30 14:51:49.052690 mkdocs_dsfr-0.3.1/dsfr/footer.html
--rw-r--r--   0        0        0     2213 2023-05-31 09:02:28.010420 mkdocs_dsfr-0.3.1/dsfr/header.html
--rw-r--r--   0        0        0      397 2023-06-02 13:12:07.378000 mkdocs_dsfr-0.3.1/dsfr/icons/buildings/ancient-gate-fill.svg
--rw-r--r--   0        0        0      789 2023-06-02 13:12:07.378000 mkdocs_dsfr-0.3.1/dsfr/icons/buildings/ancient-gate-line.svg
--rw-r--r--   0        0        0      280 2023-06-02 13:12:07.378000 mkdocs_dsfr-0.3.1/dsfr/icons/buildings/ancient-pavilion-fill.svg
--rw-r--r--   0        0        0      416 2023-06-02 13:12:07.378999 mkdocs_dsfr-0.3.1/dsfr/icons/buildings/ancient-pavilion-line.svg
--rw-r--r--   0        0        0      232 2023-06-02 13:12:07.392999 mkdocs_dsfr-0.3.1/dsfr/icons/buildings/bank-fill.svg
--rw-r--r--   0        0        0      262 2023-06-02 13:12:07.392999 mkdocs_dsfr-0.3.1/dsfr/icons/buildings/bank-line.svg
--rw-r--r--   0        0        0      204 2023-06-02 13:12:07.403000 mkdocs_dsfr-0.3.1/dsfr/icons/buildings/building-fill.svg
--rw-r--r--   0        0        0      225 2023-06-02 13:12:07.404000 mkdocs_dsfr-0.3.1/dsfr/icons/buildings/building-line.svg
--rw-r--r--   0        0        0      316 2023-06-02 13:12:07.427000 mkdocs_dsfr-0.3.1/dsfr/icons/buildings/community-fill.svg
--rw-r--r--   0        0        0      388 2023-06-02 13:12:07.427000 mkdocs_dsfr-0.3.1/dsfr/icons/buildings/community-line.svg
--rw-r--r--   0        0        0      232 2023-06-02 13:12:07.502000 mkdocs_dsfr-0.3.1/dsfr/icons/buildings/government-fill.svg
--rw-r--r--   0        0        0      227 2023-06-02 13:12:07.502000 mkdocs_dsfr-0.3.1/dsfr/icons/buildings/government-line.svg
--rw-r--r--   0        0        0      209 2023-06-02 13:12:07.513999 mkdocs_dsfr-0.3.1/dsfr/icons/buildings/home-4-fill.svg
--rw-r--r--   0        0        0      239 2023-06-02 13:12:07.513999 mkdocs_dsfr-0.3.1/dsfr/icons/buildings/home-4-line.svg
--rw-r--r--   0        0        0      212 2023-06-02 13:12:07.515000 mkdocs_dsfr-0.3.1/dsfr/icons/buildings/hospital-fill.svg
--rw-r--r--   0        0        0      228 2023-06-02 13:12:07.515000 mkdocs_dsfr-0.3.1/dsfr/icons/buildings/hospital-line.svg
--rw-r--r--   0        0        0      224 2023-06-02 13:12:07.516000 mkdocs_dsfr-0.3.1/dsfr/icons/buildings/hotel-fill.svg
--rw-r--r--   0        0        0      243 2023-06-02 13:12:07.516000 mkdocs_dsfr-0.3.1/dsfr/icons/buildings/hotel-line.svg
--rw-r--r--   0        0        0      437 2023-06-02 13:12:07.615000 mkdocs_dsfr-0.3.1/dsfr/icons/buildings/store-fill.svg
--rw-r--r--   0        0        0      546 2023-06-02 13:12:07.615000 mkdocs_dsfr-0.3.1/dsfr/icons/buildings/store-line.svg
--rw-r--r--   0        0        0      254 2023-06-02 13:12:07.380000 mkdocs_dsfr-0.3.1/dsfr/icons/business/archive-fill.svg
--rw-r--r--   0        0        0      288 2023-06-02 13:12:07.380000 mkdocs_dsfr-0.3.1/dsfr/icons/business/archive-line.svg
--rw-r--r--   0        0        0      330 2023-06-02 13:12:07.390000 mkdocs_dsfr-0.3.1/dsfr/icons/business/attachment-fill.svg
--rw-r--r--   0        0        0      241 2023-06-02 13:12:07.390000 mkdocs_dsfr-0.3.1/dsfr/icons/business/attachment-line.svg
--rw-r--r--   0        0        0      289 2023-06-02 13:12:07.391000 mkdocs_dsfr-0.3.1/dsfr/icons/business/award-fill.svg
--rw-r--r--   0        0        0      338 2023-06-02 13:12:07.391000 mkdocs_dsfr-0.3.1/dsfr/icons/business/award-line.svg
--rw-r--r--   0        0        0      218 2023-06-02 13:12:07.394000 mkdocs_dsfr-0.3.1/dsfr/icons/business/bar-chart-box-fill.svg
--rw-r--r--   0        0        0      234 2023-06-02 13:12:07.394000 mkdocs_dsfr-0.3.1/dsfr/icons/business/bar-chart-box-line.svg
--rw-r--r--   0        0        0      208 2023-06-02 13:12:07.398999 mkdocs_dsfr-0.3.1/dsfr/icons/business/bookmark-fill.svg
--rw-r--r--   0        0        0      242 2023-06-02 13:12:07.398999 mkdocs_dsfr-0.3.1/dsfr/icons/business/bookmark-line.svg
--rw-r--r--   0        0        0      253 2023-06-02 13:12:07.400000 mkdocs_dsfr-0.3.1/dsfr/icons/business/briefcase-fill.svg
--rw-r--r--   0        0        0      267 2023-06-02 13:12:07.400000 mkdocs_dsfr-0.3.1/dsfr/icons/business/briefcase-line.svg
--rw-r--r--   0        0        0      248 2023-06-02 13:12:07.404999 mkdocs_dsfr-0.3.1/dsfr/icons/business/calendar-2-fill.svg
--rw-r--r--   0        0        0      281 2023-06-02 13:12:07.405999 mkdocs_dsfr-0.3.1/dsfr/icons/business/calendar-2-line.svg
--rw-r--r--   0        0        0      218 2023-06-02 13:12:07.405999 mkdocs_dsfr-0.3.1/dsfr/icons/business/calendar-event-fill.svg
--rw-r--r--   0        0        0      251 2023-06-02 13:12:07.405999 mkdocs_dsfr-0.3.1/dsfr/icons/business/calendar-event-line.svg
--rw-r--r--   0        0        0      203 2023-06-02 13:12:07.407000 mkdocs_dsfr-0.3.1/dsfr/icons/business/calendar-fill.svg
--rw-r--r--   0        0        0      244 2023-06-02 13:12:07.407999 mkdocs_dsfr-0.3.1/dsfr/icons/business/calendar-line.svg
--rw-r--r--   0        0        0      254 2023-06-02 13:12:07.423000 mkdocs_dsfr-0.3.1/dsfr/icons/business/cloud-fill.svg
--rw-r--r--   0        0        0      356 2023-06-02 13:12:07.423000 mkdocs_dsfr-0.3.1/dsfr/icons/business/cloud-line.svg
--rw-r--r--   0        0        0      290 2023-06-02 13:12:07.431999 mkdocs_dsfr-0.3.1/dsfr/icons/business/copyright-fill.svg
--rw-r--r--   0        0        0      346 2023-06-02 13:12:07.431999 mkdocs_dsfr-0.3.1/dsfr/icons/business/copyright-line.svg
--rw-r--r--   0        0        0      341 2023-06-02 13:12:07.436000 mkdocs_dsfr-0.3.1/dsfr/icons/business/customer-service-fill.svg
--rw-r--r--   0        0        0      375 2023-06-02 13:12:07.436000 mkdocs_dsfr-0.3.1/dsfr/icons/business/customer-service-line.svg
--rw-r--r--   0        0        0      210 2023-06-02 13:12:07.469000 mkdocs_dsfr-0.3.1/dsfr/icons/business/flag-fill.svg
--rw-r--r--   0        0        0      255 2023-06-02 13:12:07.469000 mkdocs_dsfr-0.3.1/dsfr/icons/business/flag-line.svg
--rw-r--r--   0        0        0      540 2023-06-02 13:12:07.499000 mkdocs_dsfr-0.3.1/dsfr/icons/business/global-fill.svg
--rw-r--r--   0        0        0      607 2023-06-02 13:12:07.500000 mkdocs_dsfr-0.3.1/dsfr/icons/business/global-line.svg
--rw-r--r--   0        0        0      200 2023-06-02 13:12:07.529000 mkdocs_dsfr-0.3.1/dsfr/icons/business/line-chart-fill.svg
--rw-r--r--   0        0        0      218 2023-06-02 13:12:07.529000 mkdocs_dsfr-0.3.1/dsfr/icons/business/line-chart-line.svg
--rw-r--r--   0        0        0      409 2023-06-02 13:12:07.530999 mkdocs_dsfr-0.3.1/dsfr/icons/business/links-fill.svg
--rw-r--r--   0        0        0      418 2023-06-02 13:12:07.532000 mkdocs_dsfr-0.3.1/dsfr/icons/business/links-line.svg
--rw-r--r--   0        0        0      260 2023-06-02 13:12:07.539999 mkdocs_dsfr-0.3.1/dsfr/icons/business/mail-fill.svg
--rw-r--r--   0        0        0      247 2023-06-02 13:12:07.540999 mkdocs_dsfr-0.3.1/dsfr/icons/business/mail-line.svg
--rw-r--r--   0        0        0      318 2023-06-02 13:12:07.540999 mkdocs_dsfr-0.3.1/dsfr/icons/business/mail-open-fill.svg
--rw-r--r--   0        0        0      359 2023-06-02 13:12:07.540999 mkdocs_dsfr-0.3.1/dsfr/icons/business/mail-open-line.svg
--rw-r--r--   0        0        0      355 2023-06-02 13:12:07.546999 mkdocs_dsfr-0.3.1/dsfr/icons/business/medal-fill.svg
--rw-r--r--   0        0        0      389 2023-06-02 13:12:07.546999 mkdocs_dsfr-0.3.1/dsfr/icons/business/medal-line.svg
--rw-r--r--   0        0        0      248 2023-06-02 13:12:07.573999 mkdocs_dsfr-0.3.1/dsfr/icons/business/pie-chart-2-fill.svg
--rw-r--r--   0        0        0      378 2023-06-02 13:12:07.575000 mkdocs_dsfr-0.3.1/dsfr/icons/business/pie-chart-2-line.svg
--rw-r--r--   0        0        0      273 2023-06-02 13:12:07.575000 mkdocs_dsfr-0.3.1/dsfr/icons/business/pie-chart-box-fill.svg
--rw-r--r--   0        0        0      289 2023-06-02 13:12:07.575000 mkdocs_dsfr-0.3.1/dsfr/icons/business/pie-chart-box-line.svg
--rw-r--r--   0        0        0      256 2023-06-02 13:12:07.579999 mkdocs_dsfr-0.3.1/dsfr/icons/business/printer-fill.svg
--rw-r--r--   0        0        0      341 2023-06-02 13:12:07.579999 mkdocs_dsfr-0.3.1/dsfr/icons/business/printer-line.svg
--rw-r--r--   0        0        0      296 2023-06-02 13:12:07.581000 mkdocs_dsfr-0.3.1/dsfr/icons/business/profil-fill.svg
--rw-r--r--   0        0        0      312 2023-06-02 13:12:07.581000 mkdocs_dsfr-0.3.1/dsfr/icons/business/profil-line.svg
--rw-r--r--   0        0        0      356 2023-06-02 13:12:07.581000 mkdocs_dsfr-0.3.1/dsfr/icons/business/projector-2-fill.svg
--rw-r--r--   0        0        0      350 2023-06-02 13:12:07.582000 mkdocs_dsfr-0.3.1/dsfr/icons/business/projector-2-line.svg
--rw-r--r--   0        0        0      248 2023-06-02 13:12:07.598999 mkdocs_dsfr-0.3.1/dsfr/icons/business/send-plane-fill.svg
--rw-r--r--   0        0        0      301 2023-06-02 13:12:07.599999 mkdocs_dsfr-0.3.1/dsfr/icons/business/send-plane-line.svg
--rw-r--r--   0        0        0      226 2023-06-02 13:12:07.608000 mkdocs_dsfr-0.3.1/dsfr/icons/business/slideshow-fill.svg
--rw-r--r--   0        0        0      241 2023-06-02 13:12:07.608000 mkdocs_dsfr-0.3.1/dsfr/icons/business/slideshow-line.svg
--rw-r--r--   0        0        0      215 2023-06-02 13:12:07.657999 mkdocs_dsfr-0.3.1/dsfr/icons/business/window-fill.svg
--rw-r--r--   0        0        0      230 2023-06-02 13:12:07.658999 mkdocs_dsfr-0.3.1/dsfr/icons/business/window-line.svg
--rw-r--r--   0        0        0      199 2023-06-02 13:12:07.413000 mkdocs_dsfr-0.3.1/dsfr/icons/communication/chat-2-fill.svg
--rw-r--r--   0        0        0      237 2023-06-02 13:12:07.414000 mkdocs_dsfr-0.3.1/dsfr/icons/communication/chat-2-line.svg
--rw-r--r--   0        0        0      236 2023-06-02 13:12:07.414000 mkdocs_dsfr-0.3.1/dsfr/icons/communication/chat-3-fill.svg
--rw-r--r--   0        0        0      360 2023-06-02 13:12:07.414000 mkdocs_dsfr-0.3.1/dsfr/icons/communication/chat-3-line.svg
--rw-r--r--   0        0        0      256 2023-06-02 13:12:07.414999 mkdocs_dsfr-0.3.1/dsfr/icons/communication/chat-check-fill.svg
--rw-r--r--   0        0        0      283 2023-06-02 13:12:07.414999 mkdocs_dsfr-0.3.1/dsfr/icons/communication/chat-check-line.svg
--rw-r--r--   0        0        0      321 2023-06-02 13:12:07.414999 mkdocs_dsfr-0.3.1/dsfr/icons/communication/chat-delete-fill.svg
--rw-r--r--   0        0        0      348 2023-06-02 13:12:07.415999 mkdocs_dsfr-0.3.1/dsfr/icons/communication/chat-delete-line.svg
--rw-r--r--   0        0        0      243 2023-06-02 13:12:07.415999 mkdocs_dsfr-0.3.1/dsfr/icons/communication/chat-poll-fill.svg
--rw-r--r--   0        0        0      214 2023-06-02 13:12:07.415999 mkdocs_dsfr-0.3.1/dsfr/icons/communication/chat-poll-line.svg
--rw-r--r--   0        0        0      236 2023-06-02 13:12:07.441999 mkdocs_dsfr-0.3.1/dsfr/icons/communication/discuss-fill.svg
--rw-r--r--   0        0        0      282 2023-06-02 13:12:07.441999 mkdocs_dsfr-0.3.1/dsfr/icons/communication/discuss-line.svg
--rw-r--r--   0        0        0      201 2023-06-02 13:12:07.460000 mkdocs_dsfr-0.3.1/dsfr/icons/communication/feedback-fill.svg
--rw-r--r--   0        0        0      229 2023-06-02 13:12:07.460000 mkdocs_dsfr-0.3.1/dsfr/icons/communication/feedback-line.svg
--rw-r--r--   0        0        0      215 2023-06-02 13:12:07.549999 mkdocs_dsfr-0.3.1/dsfr/icons/communication/message-2-fill.svg
--rw-r--r--   0        0        0      245 2023-06-02 13:12:07.551000 mkdocs_dsfr-0.3.1/dsfr/icons/communication/message-2-line.svg
--rw-r--r--   0        0        0      231 2023-06-02 13:12:07.584000 mkdocs_dsfr-0.3.1/dsfr/icons/communication/question-answer-fill.svg
--rw-r--r--   0        0        0      260 2023-06-02 13:12:07.585000 mkdocs_dsfr-0.3.1/dsfr/icons/communication/question-answer-line.svg
--rw-r--r--   0        0        0      263 2023-06-02 13:12:07.585999 mkdocs_dsfr-0.3.1/dsfr/icons/communication/questionnaire-fill.svg
--rw-r--r--   0        0        0      327 2023-06-02 13:12:07.585999 mkdocs_dsfr-0.3.1/dsfr/icons/communication/questionnaire-line.svg
--rw-r--r--   0        0        0      206 2023-06-02 13:12:07.651000 mkdocs_dsfr-0.3.1/dsfr/icons/communication/video-chat-fill.svg
--rw-r--r--   0        0        0      234 2023-06-02 13:12:07.651000 mkdocs_dsfr-0.3.1/dsfr/icons/communication/video-chat-line.svg
--rw-r--r--   0        0        0      318 2023-06-02 13:12:07.391000 mkdocs_dsfr-0.3.1/dsfr/icons/design/ball-pen-fill.svg
--rw-r--r--   0        0        0      372 2023-06-02 13:12:07.391999 mkdocs_dsfr-0.3.1/dsfr/icons/design/ball-pen-line.svg
--rw-r--r--   0        0        0      252 2023-06-02 13:12:07.401000 mkdocs_dsfr-0.3.1/dsfr/icons/design/brush-3-fill.svg
--rw-r--r--   0        0        0      266 2023-06-02 13:12:07.401000 mkdocs_dsfr-0.3.1/dsfr/icons/design/brush-3-line.svg
--rw-r--r--   0        0        0      449 2023-06-02 13:12:07.401999 mkdocs_dsfr-0.3.1/dsfr/icons/design/brush-fill.svg
--rw-r--r--   0        0        0      689 2023-06-02 13:12:07.401999 mkdocs_dsfr-0.3.1/dsfr/icons/design/brush-line.svg
--rw-r--r--   0        0        0      195 2023-06-02 13:12:07.430999 mkdocs_dsfr-0.3.1/dsfr/icons/design/contrast-fill.svg
--rw-r--r--   0        0        0      230 2023-06-02 13:12:07.430999 mkdocs_dsfr-0.3.1/dsfr/icons/design/contrast-line.svg
--rw-r--r--   0        0        0      173 2023-06-02 13:12:07.431999 mkdocs_dsfr-0.3.1/dsfr/icons/design/crop-fill.svg
--rw-r--r--   0        0        0      184 2023-06-02 13:12:07.433000 mkdocs_dsfr-0.3.1/dsfr/icons/design/crop-line.svg
--rw-r--r--   0        0        0      399 2023-06-02 13:12:07.447000 mkdocs_dsfr-0.3.1/dsfr/icons/design/drag-move-2-fill.svg
--rw-r--r--   0        0        0      178 2023-06-02 13:12:07.447000 mkdocs_dsfr-0.3.1/dsfr/icons/design/drag-move-2-line.svg
--rw-r--r--   0        0        0      153 2023-06-02 13:12:07.448999 mkdocs_dsfr-0.3.1/dsfr/icons/design/drop-fill.svg
--rw-r--r--   0        0        0      190 2023-06-02 13:12:07.448999 mkdocs_dsfr-0.3.1/dsfr/icons/design/drop-line.svg
--rw-r--r--   0        0        0      275 2023-06-02 13:12:07.451999 mkdocs_dsfr-0.3.1/dsfr/icons/design/edit-box-fill.svg
--rw-r--r--   0        0        0      255 2023-06-02 13:12:07.451999 mkdocs_dsfr-0.3.1/dsfr/icons/design/edit-box-line.svg
--rw-r--r--   0        0        0      206 2023-06-02 13:12:07.453000 mkdocs_dsfr-0.3.1/dsfr/icons/design/edit-fill.svg
--rw-r--r--   0        0        0      258 2023-06-02 13:12:07.453000 mkdocs_dsfr-0.3.1/dsfr/icons/design/edit-line.svg
--rw-r--r--   0        0        0      266 2023-06-02 13:12:07.522000 mkdocs_dsfr-0.3.1/dsfr/icons/design/ink-bottle-fill.svg
--rw-r--r--   0        0        0      323 2023-06-02 13:12:07.522000 mkdocs_dsfr-0.3.1/dsfr/icons/design/ink-bottle-line.svg
--rw-r--r--   0        0        0      241 2023-06-02 13:12:07.525000 mkdocs_dsfr-0.3.1/dsfr/icons/design/layout-grid-fill.svg
--rw-r--r--   0        0        0      232 2023-06-02 13:12:07.526000 mkdocs_dsfr-0.3.1/dsfr/icons/design/layout-grid-line.svg
--rw-r--r--   0        0        0      401 2023-06-02 13:12:07.545000 mkdocs_dsfr-0.3.1/dsfr/icons/design/mark-pen-fill.svg
--rw-r--r--   0        0        0      503 2023-06-02 13:12:07.546000 mkdocs_dsfr-0.3.1/dsfr/icons/design/mark-pen-line.svg
--rw-r--r--   0        0        0      292 2023-06-02 13:12:07.565000 mkdocs_dsfr-0.3.1/dsfr/icons/design/paint-brush-fill.svg
--rw-r--r--   0        0        0      305 2023-06-02 13:12:07.565000 mkdocs_dsfr-0.3.1/dsfr/icons/design/paint-brush-line.svg
--rw-r--r--   0        0        0      339 2023-06-02 13:12:07.565999 mkdocs_dsfr-0.3.1/dsfr/icons/design/paint-fill.svg
--rw-r--r--   0        0        0      362 2023-06-02 13:12:07.565999 mkdocs_dsfr-0.3.1/dsfr/icons/design/paint-line.svg
--rw-r--r--   0        0        0      437 2023-06-02 13:12:07.566999 mkdocs_dsfr-0.3.1/dsfr/icons/design/palette-fill.svg
--rw-r--r--   0        0        0      584 2023-06-02 13:12:07.566999 mkdocs_dsfr-0.3.1/dsfr/icons/design/palette-line.svg
--rw-r--r--   0        0        0      386 2023-06-02 13:12:07.568000 mkdocs_dsfr-0.3.1/dsfr/icons/design/pantone-fill.svg
--rw-r--r--   0        0        0      505 2023-06-02 13:12:07.568000 mkdocs_dsfr-0.3.1/dsfr/icons/design/pantone-line.svg
--rw-r--r--   0        0        0      389 2023-06-02 13:12:07.571000 mkdocs_dsfr-0.3.1/dsfr/icons/design/pen-nib-fill.svg
--rw-r--r--   0        0        0      510 2023-06-02 13:12:07.572000 mkdocs_dsfr-0.3.1/dsfr/icons/design/pen-nib-line.svg
--rw-r--r--   0        0        0      254 2023-06-02 13:12:07.572000 mkdocs_dsfr-0.3.1/dsfr/icons/design/pencil-fill.svg
--rw-r--r--   0        0        0      310 2023-06-02 13:12:07.572999 mkdocs_dsfr-0.3.1/dsfr/icons/design/pencil-line.svg
--rw-r--r--   0        0        0      234 2023-06-02 13:12:07.572999 mkdocs_dsfr-0.3.1/dsfr/icons/design/pencil-ruler-fill.svg
--rw-r--r--   0        0        0      255 2023-06-02 13:12:07.572999 mkdocs_dsfr-0.3.1/dsfr/icons/design/pencil-ruler-line.svg
--rw-r--r--   0        0        0      302 2023-06-02 13:12:07.605999 mkdocs_dsfr-0.3.1/dsfr/icons/design/sip-fill.svg
--rw-r--r--   0        0        0      352 2023-06-02 13:12:07.607000 mkdocs_dsfr-0.3.1/dsfr/icons/design/sip-line.svg
--rw-r--r--   0        0        0      221 2023-06-02 13:12:07.622999 mkdocs_dsfr-0.3.1/dsfr/icons/design/table-fill.svg
--rw-r--r--   0        0        0      234 2023-06-02 13:12:07.624000 mkdocs_dsfr-0.3.1/dsfr/icons/design/table-line.svg
--rw-r--r--   0        0        0      500 2023-06-02 13:12:07.401999 mkdocs_dsfr-0.3.1/dsfr/icons/development/bug-fill.svg
--rw-r--r--   0        0        0      632 2023-06-02 13:12:07.403000 mkdocs_dsfr-0.3.1/dsfr/icons/development/bug-line.svg
--rw-r--r--   0        0        0      360 2023-06-02 13:12:07.424000 mkdocs_dsfr-0.3.1/dsfr/icons/development/code-box-fill.svg
--rw-r--r--   0        0        0      374 2023-06-02 13:12:07.424999 mkdocs_dsfr-0.3.1/dsfr/icons/development/code-box-line.svg
--rw-r--r--   0        0        0      281 2023-06-02 13:12:07.424999 mkdocs_dsfr-0.3.1/dsfr/icons/development/code-s-slash-line.svg
--rw-r--r--   0        0        0      197 2023-06-02 13:12:07.434999 mkdocs_dsfr-0.3.1/dsfr/icons/development/cursor-fill.svg
--rw-r--r--   0        0        0      283 2023-06-02 13:12:07.436000 mkdocs_dsfr-0.3.1/dsfr/icons/development/cursor-line.svg
--rw-r--r--   0        0        0      307 2023-06-02 13:12:07.490000 mkdocs_dsfr-0.3.1/dsfr/icons/development/git-branch-fill.svg
--rw-r--r--   0        0        0      425 2023-06-02 13:12:07.490999 mkdocs_dsfr-0.3.1/dsfr/icons/development/git-branch-line.svg
--rw-r--r--   0        0        0      187 2023-06-02 13:12:07.490999 mkdocs_dsfr-0.3.1/dsfr/icons/development/git-commit-fill.svg
--rw-r--r--   0        0        0      250 2023-06-02 13:12:07.494999 mkdocs_dsfr-0.3.1/dsfr/icons/development/git-commit-line.svg
--rw-r--r--   0        0        0      330 2023-06-02 13:12:07.494999 mkdocs_dsfr-0.3.1/dsfr/icons/development/git-merge-fill.svg
--rw-r--r--   0        0        0      455 2023-06-02 13:12:07.494999 mkdocs_dsfr-0.3.1/dsfr/icons/development/git-merge-line.svg
--rw-r--r--   0        0        0      233 2023-06-02 13:12:07.496000 mkdocs_dsfr-0.3.1/dsfr/icons/development/git-pull-request-fill.svg
--rw-r--r--   0        0        0      356 2023-06-02 13:12:07.496000 mkdocs_dsfr-0.3.1/dsfr/icons/development/git-pull-request-line.svg
--rw-r--r--   0        0        0      294 2023-06-02 13:12:07.496000 mkdocs_dsfr-0.3.1/dsfr/icons/development/git-repository-commits-fill.svg
--rw-r--r--   0        0        0      320 2023-06-02 13:12:07.496999 mkdocs_dsfr-0.3.1/dsfr/icons/development/git-repository-commits-line.svg
--rw-r--r--   0        0        0      285 2023-06-02 13:12:07.496999 mkdocs_dsfr-0.3.1/dsfr/icons/development/git-repository-fill.svg
--rw-r--r--   0        0        0      328 2023-06-02 13:12:07.496999 mkdocs_dsfr-0.3.1/dsfr/icons/development/git-repository-line.svg
--rw-r--r--   0        0        0      288 2023-06-02 13:12:07.497999 mkdocs_dsfr-0.3.1/dsfr/icons/development/git-repository-private-fill.svg
--rw-r--r--   0        0        0      304 2023-06-02 13:12:07.497999 mkdocs_dsfr-0.3.1/dsfr/icons/development/git-repository-private-line.svg
--rw-r--r--   0        0        0      260 2023-06-02 13:12:07.628999 mkdocs_dsfr-0.3.1/dsfr/icons/development/terminal-box-fill.svg
--rw-r--r--   0        0        0      287 2023-06-02 13:12:07.628999 mkdocs_dsfr-0.3.1/dsfr/icons/development/terminal-box-line.svg
--rw-r--r--   0        0        0      186 2023-06-02 13:12:07.630000 mkdocs_dsfr-0.3.1/dsfr/icons/development/terminal-line.svg
--rw-r--r--   0        0        0      230 2023-06-02 13:12:07.630000 mkdocs_dsfr-0.3.1/dsfr/icons/development/terminal-window-fill.svg
--rw-r--r--   0        0        0      245 2023-06-02 13:12:07.631000 mkdocs_dsfr-0.3.1/dsfr/icons/development/terminal-window-line.svg
--rw-r--r--   0        0        0      343 2023-06-02 13:12:07.395999 mkdocs_dsfr-0.3.1/dsfr/icons/device/bluetooth-fill.svg
--rw-r--r--   0        0        0      343 2023-06-02 13:12:07.395999 mkdocs_dsfr-0.3.1/dsfr/icons/device/bluetooth-line.svg
--rw-r--r--   0        0        0      256 2023-06-02 13:12:07.428999 mkdocs_dsfr-0.3.1/dsfr/icons/device/computer-fill.svg
--rw-r--r--   0        0        0      275 2023-06-02 13:12:07.428999 mkdocs_dsfr-0.3.1/dsfr/icons/device/computer-line.svg
--rw-r--r--   0        0        0      514 2023-06-02 13:12:07.437000 mkdocs_dsfr-0.3.1/dsfr/icons/device/dashboard-3-fill.svg
--rw-r--r--   0        0        0      552 2023-06-02 13:12:07.437999 mkdocs_dsfr-0.3.1/dsfr/icons/device/dashboard-3-line.svg
--rw-r--r--   0        0        0      266 2023-06-02 13:12:07.438999 mkdocs_dsfr-0.3.1/dsfr/icons/device/database-fill.svg
--rw-r--r--   0        0        0      296 2023-06-02 13:12:07.438999 mkdocs_dsfr-0.3.1/dsfr/icons/device/database-line.svg
--rw-r--r--   0        0        0      250 2023-06-02 13:12:07.440000 mkdocs_dsfr-0.3.1/dsfr/icons/device/device-fill.svg
--rw-r--r--   0        0        0      260 2023-06-02 13:12:07.440000 mkdocs_dsfr-0.3.1/dsfr/icons/device/device-line.svg
--rw-r--r--   0        0        0      206 2023-06-02 13:12:07.509000 mkdocs_dsfr-0.3.1/dsfr/icons/device/hard-drive-2-fill.svg
--rw-r--r--   0        0        0      222 2023-06-02 13:12:07.509000 mkdocs_dsfr-0.3.1/dsfr/icons/device/hard-drive-2-line.svg
--rw-r--r--   0        0        0      290 2023-06-02 13:12:07.539999 mkdocs_dsfr-0.3.1/dsfr/icons/device/mac-fill.svg
--rw-r--r--   0        0        0      288 2023-06-02 13:12:07.539999 mkdocs_dsfr-0.3.1/dsfr/icons/device/mac-line.svg
--rw-r--r--   0        0        0      485 2023-06-02 13:12:07.573999 mkdocs_dsfr-0.3.1/dsfr/icons/device/phone-fill.svg
--rw-r--r--   0        0        0      719 2023-06-02 13:12:07.573999 mkdocs_dsfr-0.3.1/dsfr/icons/device/phone-line.svg
--rw-r--r--   0        0        0      272 2023-06-02 13:12:07.582999 mkdocs_dsfr-0.3.1/dsfr/icons/device/qr-code-fill.svg
--rw-r--r--   0        0        0      315 2023-06-02 13:12:07.584000 mkdocs_dsfr-0.3.1/dsfr/icons/device/qr-code-line.svg
--rw-r--r--   0        0        0      229 2023-06-02 13:12:07.591000 mkdocs_dsfr-0.3.1/dsfr/icons/device/rss-fill.svg
--rw-r--r--   0        0        0      230 2023-06-02 13:12:07.592000 mkdocs_dsfr-0.3.1/dsfr/icons/device/rss-line.svg
--rw-r--r--   0        0        0      234 2023-06-02 13:12:07.592999 mkdocs_dsfr-0.3.1/dsfr/icons/device/save-3-fill.svg
--rw-r--r--   0        0        0      250 2023-06-02 13:12:07.594000 mkdocs_dsfr-0.3.1/dsfr/icons/device/save-3-line.svg
--rw-r--r--   0        0        0      195 2023-06-02 13:12:07.594000 mkdocs_dsfr-0.3.1/dsfr/icons/device/save-fill.svg
--rw-r--r--   0        0        0      219 2023-06-02 13:12:07.595000 mkdocs_dsfr-0.3.1/dsfr/icons/device/save-line.svg
--rw-r--r--   0        0        0      219 2023-06-02 13:12:07.599999 mkdocs_dsfr-0.3.1/dsfr/icons/device/server-fill.svg
--rw-r--r--   0        0        0      234 2023-06-02 13:12:07.601000 mkdocs_dsfr-0.3.1/dsfr/icons/device/server-line.svg
--rw-r--r--   0        0        0      208 2023-06-02 13:12:07.608999 mkdocs_dsfr-0.3.1/dsfr/icons/device/smartphone-fill.svg
--rw-r--r--   0        0        0      224 2023-06-02 13:12:07.608999 mkdocs_dsfr-0.3.1/dsfr/icons/device/smartphone-line.svg
--rw-r--r--   0        0        0      208 2023-06-02 13:12:07.624000 mkdocs_dsfr-0.3.1/dsfr/icons/device/tablet-fill.svg
--rw-r--r--   0        0        0      224 2023-06-02 13:12:07.625000 mkdocs_dsfr-0.3.1/dsfr/icons/device/tablet-line.svg
--rw-r--r--   0        0        0      285 2023-06-02 13:12:07.638999 mkdocs_dsfr-0.3.1/dsfr/icons/device/tv-fill.svg
--rw-r--r--   0        0        0      304 2023-06-02 13:12:07.640000 mkdocs_dsfr-0.3.1/dsfr/icons/device/tv-line.svg
--rw-r--r--   0        0        0      618 2023-06-02 13:12:07.657000 mkdocs_dsfr-0.3.1/dsfr/icons/device/wifi-fill.svg
--rw-r--r--   0        0        0      630 2023-06-02 13:12:07.657999 mkdocs_dsfr-0.3.1/dsfr/icons/device/wifi-line.svg
--rw-r--r--   0        0        0      233 2023-06-02 13:12:07.388000 mkdocs_dsfr-0.3.1/dsfr/icons/document/article-fill.svg
--rw-r--r--   0        0        0      249 2023-06-02 13:12:07.388999 mkdocs_dsfr-0.3.1/dsfr/icons/document/article-line.svg
--rw-r--r--   0        0        0      181 2023-06-02 13:12:07.397000 mkdocs_dsfr-0.3.1/dsfr/icons/document/book-2-fill.svg
--rw-r--r--   0        0        0      227 2023-06-02 13:12:07.397000 mkdocs_dsfr-0.3.1/dsfr/icons/document/book-2-line.svg
--rw-r--r--   0        0        0      226 2023-06-02 13:12:07.398000 mkdocs_dsfr-0.3.1/dsfr/icons/document/booklet-fill.svg
--rw-r--r--   0        0        0      242 2023-06-02 13:12:07.398999 mkdocs_dsfr-0.3.1/dsfr/icons/document/booklet-line.svg
--rw-r--r--   0        0        0      250 2023-06-02 13:12:07.421000 mkdocs_dsfr-0.3.1/dsfr/icons/document/clipboard-fill.svg
--rw-r--r--   0        0        0      274 2023-06-02 13:12:07.421000 mkdocs_dsfr-0.3.1/dsfr/icons/document/clipboard-line.svg
--rw-r--r--   0        0        0      317 2023-06-02 13:12:07.446000 mkdocs_dsfr-0.3.1/dsfr/icons/document/draft-fill.svg
--rw-r--r--   0        0        0      303 2023-06-02 13:12:07.447000 mkdocs_dsfr-0.3.1/dsfr/icons/document/draft-line.svg
--rw-r--r--   0        0        0      234 2023-06-02 13:12:07.460999 mkdocs_dsfr-0.3.1/dsfr/icons/document/file-add-fill.svg
--rw-r--r--   0        0        0      251 2023-06-02 13:12:07.460999 mkdocs_dsfr-0.3.1/dsfr/icons/document/file-add-line.svg
--rw-r--r--   0        0        0      227 2023-06-02 13:12:07.460999 mkdocs_dsfr-0.3.1/dsfr/icons/document/file-download-fill.svg
--rw-r--r--   0        0        0      245 2023-06-02 13:12:07.461999 mkdocs_dsfr-0.3.1/dsfr/icons/document/file-download-line.svg
--rw-r--r--   0        0        0      230 2023-06-02 13:12:07.461999 mkdocs_dsfr-0.3.1/dsfr/icons/document/file-fill.svg
--rw-r--r--   0        0        0      225 2023-06-02 13:12:07.463000 mkdocs_dsfr-0.3.1/dsfr/icons/document/file-line.svg
--rw-r--r--   0        0        0      255 2023-06-02 13:12:07.463000 mkdocs_dsfr-0.3.1/dsfr/icons/document/file-pdf-fill.svg
--rw-r--r--   0        0        0      273 2023-06-02 13:12:07.463000 mkdocs_dsfr-0.3.1/dsfr/icons/document/file-pdf-line.svg
--rw-r--r--   0        0        0      281 2023-06-02 13:12:07.463999 mkdocs_dsfr-0.3.1/dsfr/icons/document/file-text-fill.svg
--rw-r--r--   0        0        0      272 2023-06-02 13:12:07.463999 mkdocs_dsfr-0.3.1/dsfr/icons/document/file-text-line.svg
--rw-r--r--   0        0        0      198 2023-06-02 13:12:07.470000 mkdocs_dsfr-0.3.1/dsfr/icons/document/folder-2-fill.svg
--rw-r--r--   0        0        0      234 2023-06-02 13:12:07.470999 mkdocs_dsfr-0.3.1/dsfr/icons/document/folder-2-line.svg
--rw-r--r--   0        0        0      262 2023-06-02 13:12:07.559999 mkdocs_dsfr-0.3.1/dsfr/icons/document/newspaper-fill.svg
--rw-r--r--   0        0        0      290 2023-06-02 13:12:07.559999 mkdocs_dsfr-0.3.1/dsfr/icons/document/newspaper-line.svg
--rw-r--r--   0        0        0      292 2023-06-02 13:12:07.619999 mkdocs_dsfr-0.3.1/dsfr/icons/document/survey-fill.svg
--rw-r--r--   0        0        0      317 2023-06-02 13:12:07.619999 mkdocs_dsfr-0.3.1/dsfr/icons/document/survey-line.svg
--rw-r--r--   0        0        0      217 2023-06-02 13:12:07.635999 mkdocs_dsfr-0.3.1/dsfr/icons/document/todo-fill.svg
--rw-r--r--   0        0        0      250 2023-06-02 13:12:07.635999 mkdocs_dsfr-0.3.1/dsfr/icons/document/todo-line.svg
--rw-r--r--   0        0        0      250 2023-06-02 13:12:07.426000 mkdocs_dsfr-0.3.1/dsfr/icons/editor/code-view.svg
--rw-r--r--   0        0        0      250 2023-06-02 13:12:07.470999 mkdocs_dsfr-0.3.1/dsfr/icons/editor/font-size.svg
--rw-r--r--   0        0        0      314 2023-06-02 13:12:07.473999 mkdocs_dsfr-0.3.1/dsfr/icons/editor/fr--bold.svg
--rw-r--r--   0        0        0      160 2023-06-02 13:12:07.476000 mkdocs_dsfr-0.3.1/dsfr/icons/editor/fr--highlight.svg
--rw-r--r--   0        0        0      278 2023-06-02 13:12:07.477999 mkdocs_dsfr-0.3.1/dsfr/icons/editor/fr--quote-fill.svg
--rw-r--r--   0        0        0      344 2023-06-02 13:12:07.477999 mkdocs_dsfr-0.3.1/dsfr/icons/editor/fr--quote-line.svg
--rw-r--r--   0        0        0      223 2023-06-02 13:12:07.505000 mkdocs_dsfr-0.3.1/dsfr/icons/editor/h-1.svg
--rw-r--r--   0        0        0      387 2023-06-02 13:12:07.505000 mkdocs_dsfr-0.3.1/dsfr/icons/editor/h-2.svg
--rw-r--r--   0        0        0      542 2023-06-02 13:12:07.505000 mkdocs_dsfr-0.3.1/dsfr/icons/editor/h-3.svg
--rw-r--r--   0        0        0      268 2023-06-02 13:12:07.506000 mkdocs_dsfr-0.3.1/dsfr/icons/editor/h-4.svg
--rw-r--r--   0        0        0      393 2023-06-02 13:12:07.506999 mkdocs_dsfr-0.3.1/dsfr/icons/editor/h-5.svg
--rw-r--r--   0        0        0      538 2023-06-02 13:12:07.506999 mkdocs_dsfr-0.3.1/dsfr/icons/editor/h-6.svg
--rw-r--r--   0        0        0      298 2023-06-02 13:12:07.509000 mkdocs_dsfr-0.3.1/dsfr/icons/editor/hashtag.svg
--rw-r--r--   0        0        0      158 2023-06-02 13:12:07.525000 mkdocs_dsfr-0.3.1/dsfr/icons/editor/italic.svg
--rw-r--r--   0        0        0      468 2023-06-02 13:12:07.529999 mkdocs_dsfr-0.3.1/dsfr/icons/editor/link-unlink.svg
--rw-r--r--   0        0        0      408 2023-06-02 13:12:07.529999 mkdocs_dsfr-0.3.1/dsfr/icons/editor/link.svg
--rw-r--r--   0        0        0      246 2023-06-02 13:12:07.532000 mkdocs_dsfr-0.3.1/dsfr/icons/editor/list-ordered.svg
--rw-r--r--   0        0        0      275 2023-06-02 13:12:07.532999 mkdocs_dsfr-0.3.1/dsfr/icons/editor/list-unordered.svg
--rw-r--r--   0        0        0      341 2023-06-02 13:12:07.585999 mkdocs_dsfr-0.3.1/dsfr/icons/editor/question-mark.svg
--rw-r--r--   0        0        0      147 2023-06-02 13:12:07.599999 mkdocs_dsfr-0.3.1/dsfr/icons/editor/separator.svg
--rw-r--r--   0        0        0      151 2023-06-02 13:12:07.611000 mkdocs_dsfr-0.3.1/dsfr/icons/editor/space.svg
--rw-r--r--   0        0        0      317 2023-06-02 13:12:07.615999 mkdocs_dsfr-0.3.1/dsfr/icons/editor/subscript.svg
--rw-r--r--   0        0        0      315 2023-06-02 13:12:07.618999 mkdocs_dsfr-0.3.1/dsfr/icons/editor/superscript.svg
--rw-r--r--   0        0        0      263 2023-06-02 13:12:07.622999 mkdocs_dsfr-0.3.1/dsfr/icons/editor/table-2.svg
--rw-r--r--   0        0        0      505 2023-06-02 13:12:07.638000 mkdocs_dsfr-0.3.1/dsfr/icons/editor/translate-2.svg
--rw-r--r--   0        0        0      206 2023-06-02 13:12:07.391999 mkdocs_dsfr-0.3.1/dsfr/icons/finance/bank-card-fill.svg
--rw-r--r--   0        0        0      220 2023-06-02 13:12:07.392999 mkdocs_dsfr-0.3.1/dsfr/icons/finance/bank-card-line.svg
--rw-r--r--   0        0        0      277 2023-06-02 13:12:07.426000 mkdocs_dsfr-0.3.1/dsfr/icons/finance/coin-fill.svg
--rw-r--r--   0        0        0      393 2023-06-02 13:12:07.487999 mkdocs_dsfr-0.3.1/dsfr/icons/finance/gift-fill.svg
--rw-r--r--   0        0        0      406 2023-06-02 13:12:07.489000 mkdocs_dsfr-0.3.1/dsfr/icons/finance/gift-line.svg
--rw-r--r--   0        0        0      366 2023-06-02 13:12:07.552999 mkdocs_dsfr-0.3.1/dsfr/icons/finance/money-euro-box-fill.svg
--rw-r--r--   0        0        0      344 2023-06-02 13:12:07.552999 mkdocs_dsfr-0.3.1/dsfr/icons/finance/money-euro-box-line.svg
--rw-r--r--   0        0        0      365 2023-06-02 13:12:07.552999 mkdocs_dsfr-0.3.1/dsfr/icons/finance/money-euro-circle-fill.svg
--rw-r--r--   0        0        0      362 2023-06-02 13:12:07.553999 mkdocs_dsfr-0.3.1/dsfr/icons/finance/money-euro-circle-line.svg
--rw-r--r--   0        0        0      397 2023-06-02 13:12:07.598000 mkdocs_dsfr-0.3.1/dsfr/icons/finance/secure-payment-fill.svg
--rw-r--r--   0        0        0      427 2023-06-02 13:12:07.598000 mkdocs_dsfr-0.3.1/dsfr/icons/finance/secure-payment-line.svg
--rw-r--r--   0        0        0      348 2023-06-02 13:12:07.604000 mkdocs_dsfr-0.3.1/dsfr/icons/finance/shopping-bag-fill.svg
--rw-r--r--   0        0        0      282 2023-06-02 13:12:07.604000 mkdocs_dsfr-0.3.1/dsfr/icons/finance/shopping-bag-line.svg
--rw-r--r--   0        0        0      311 2023-06-02 13:12:07.605000 mkdocs_dsfr-0.3.1/dsfr/icons/finance/shopping-cart-2-fill.svg
--rw-r--r--   0        0        0      343 2023-06-02 13:12:07.605000 mkdocs_dsfr-0.3.1/dsfr/icons/finance/shopping-cart-2-line.svg
--rw-r--r--   0        0        0      200 2023-06-02 13:12:07.638000 mkdocs_dsfr-0.3.1/dsfr/icons/finance/trophy-fill.svg
--rw-r--r--   0        0        0      222 2023-06-02 13:12:07.638999 mkdocs_dsfr-0.3.1/dsfr/icons/finance/trophy-line.svg
--rw-r--r--   0        0        0      289 2023-06-02 13:12:07.410000 mkdocs_dsfr-0.3.1/dsfr/icons/health/capsule-fill.svg
--rw-r--r--   0        0        0      379 2023-06-02 13:12:07.410000 mkdocs_dsfr-0.3.1/dsfr/icons/health/capsule-line.svg
--rw-r--r--   0        0        0      336 2023-06-02 13:12:07.441999 mkdocs_dsfr-0.3.1/dsfr/icons/health/dislike-fill.svg
--rw-r--r--   0        0        0      543 2023-06-02 13:12:07.443000 mkdocs_dsfr-0.3.1/dsfr/icons/health/dislike-line.svg
--rw-r--r--   0        0        0      243 2023-06-02 13:12:07.444999 mkdocs_dsfr-0.3.1/dsfr/icons/health/dossier-fill.svg
--rw-r--r--   0        0        0      265 2023-06-02 13:12:07.444999 mkdocs_dsfr-0.3.1/dsfr/icons/health/dossier-line.svg
--rw-r--r--   0        0        0      269 2023-06-02 13:12:07.467999 mkdocs_dsfr-0.3.1/dsfr/icons/health/first-aid-kit-fill.svg
--rw-r--r--   0        0        0      283 2023-06-02 13:12:07.469000 mkdocs_dsfr-0.3.1/dsfr/icons/health/first-aid-kit-line.svg
--rw-r--r--   0        0        0      317 2023-06-02 13:12:07.507999 mkdocs_dsfr-0.3.1/dsfr/icons/health/hand-sanitizer-fill.svg
--rw-r--r--   0        0        0      359 2023-06-02 13:12:07.507999 mkdocs_dsfr-0.3.1/dsfr/icons/health/hand-sanitizer-line.svg
--rw-r--r--   0        0        0      258 2023-06-02 13:12:07.509999 mkdocs_dsfr-0.3.1/dsfr/icons/health/health-book-fill.svg
--rw-r--r--   0        0        0      273 2023-06-02 13:12:07.510999 mkdocs_dsfr-0.3.1/dsfr/icons/health/health-book-line.svg
--rw-r--r--   0        0        0      209 2023-06-02 13:12:07.512000 mkdocs_dsfr-0.3.1/dsfr/icons/health/heart-fill.svg
--rw-r--r--   0        0        0      365 2023-06-02 13:12:07.513000 mkdocs_dsfr-0.3.1/dsfr/icons/health/heart-line.svg
--rw-r--r--   0        0        0      331 2023-06-02 13:12:07.513000 mkdocs_dsfr-0.3.1/dsfr/icons/health/heart-pulse-fill.svg
--rw-r--r--   0        0        0      661 2023-06-02 13:12:07.513000 mkdocs_dsfr-0.3.1/dsfr/icons/health/heart-pulse-line.svg
--rw-r--r--   0        0        0      476 2023-06-02 13:12:07.538000 mkdocs_dsfr-0.3.1/dsfr/icons/health/lungs-fill.svg
--rw-r--r--   0        0        0      909 2023-06-02 13:12:07.539000 mkdocs_dsfr-0.3.1/dsfr/icons/health/lungs-line.svg
--rw-r--r--   0        0        0      241 2023-06-02 13:12:07.548000 mkdocs_dsfr-0.3.1/dsfr/icons/health/medicine-bottle-fill.svg
--rw-r--r--   0        0        0      293 2023-06-02 13:12:07.548000 mkdocs_dsfr-0.3.1/dsfr/icons/health/medicine-bottle-line.svg
--rw-r--r--   0        0        0      395 2023-06-02 13:12:07.548000 mkdocs_dsfr-0.3.1/dsfr/icons/health/mental-health-fill.svg
--rw-r--r--   0        0        0      503 2023-06-02 13:12:07.549000 mkdocs_dsfr-0.3.1/dsfr/icons/health/mental-health-line.svg
--rw-r--r--   0        0        0      519 2023-06-02 13:12:07.552000 mkdocs_dsfr-0.3.1/dsfr/icons/health/microscope-fill.svg
--rw-r--r--   0        0        0      618 2023-06-02 13:12:07.552000 mkdocs_dsfr-0.3.1/dsfr/icons/health/microscope-line.svg
--rw-r--r--   0        0        0      370 2023-06-02 13:12:07.582000 mkdocs_dsfr-0.3.1/dsfr/icons/health/psychotherapy-fill.svg
--rw-r--r--   0        0        0      504 2023-06-02 13:12:07.582999 mkdocs_dsfr-0.3.1/dsfr/icons/health/psychotherapy-line.svg
--rw-r--r--   0        0        0      181 2023-06-02 13:12:07.582999 mkdocs_dsfr-0.3.1/dsfr/icons/health/pulse-line.svg
--rw-r--r--   0        0        0      311 2023-06-02 13:12:07.612999 mkdocs_dsfr-0.3.1/dsfr/icons/health/stethoscope-fill.svg
--rw-r--r--   0        0        0      346 2023-06-02 13:12:07.614000 mkdocs_dsfr-0.3.1/dsfr/icons/health/stethoscope-line.svg
--rw-r--r--   0        0        0      446 2023-06-02 13:12:07.618999 mkdocs_dsfr-0.3.1/dsfr/icons/health/surgical-mask-fill.svg
--rw-r--r--   0        0        0      567 2023-06-02 13:12:07.619999 mkdocs_dsfr-0.3.1/dsfr/icons/health/surgical-mask-line.svg
--rw-r--r--   0        0        0      466 2023-06-02 13:12:07.621000 mkdocs_dsfr-0.3.1/dsfr/icons/health/syringe-fill.svg
--rw-r--r--   0        0        0      486 2023-06-02 13:12:07.621000 mkdocs_dsfr-0.3.1/dsfr/icons/health/syringe-line.svg
--rw-r--r--   0        0        0      237 2023-06-02 13:12:07.631000 mkdocs_dsfr-0.3.1/dsfr/icons/health/test-tube-fill.svg
--rw-r--r--   0        0        0      264 2023-06-02 13:12:07.631000 mkdocs_dsfr-0.3.1/dsfr/icons/health/test-tube-line.svg
--rw-r--r--   0        0        0      484 2023-06-02 13:12:07.631999 mkdocs_dsfr-0.3.1/dsfr/icons/health/thermometer-fill.svg
--rw-r--r--   0        0        0      576 2023-06-02 13:12:07.631999 mkdocs_dsfr-0.3.1/dsfr/icons/health/thermometer-line.svg
--rw-r--r--   0        0        0     1055 2023-06-02 13:12:07.651999 mkdocs_dsfr-0.3.1/dsfr/icons/health/virus-fill.svg
--rw-r--r--   0        0        0     1112 2023-06-02 13:12:07.653000 mkdocs_dsfr-0.3.1/dsfr/icons/health/virus-line.svg
--rw-r--r--   0        0        0      552 2023-06-02 13:12:07.418999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/chrome-fill.svg
--rw-r--r--   0        0        0      594 2023-06-02 13:12:07.418999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/chrome-line.svg
--rw-r--r--   0        0        0      591 2023-06-02 13:12:07.450999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/edge-fill.svg
--rw-r--r--   0        0        0      411 2023-06-02 13:12:07.450999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/edge-line.svg
--rw-r--r--   0        0        0      368 2023-06-02 13:12:07.457999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/facebook-circle-fill.svg
--rw-r--r--   0        0        0      458 2023-06-02 13:12:07.459000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/facebook-circle-line.svg
--rw-r--r--   0        0        0      708 2023-06-02 13:12:07.467000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/firefox-fill.svg
--rw-r--r--   0        0        0     1003 2023-06-02 13:12:07.467999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/firefox-line.svg
--rw-r--r--   0        0        0      685 2023-06-02 13:12:07.474999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/fr--dailymotion-fill.svg
--rw-r--r--   0        0        0      806 2023-06-02 13:12:07.474999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/fr--dailymotion-line.svg
--rw-r--r--   0        0        0      561 2023-06-02 13:12:07.480000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/fr--tiktok-fill.svg
--rw-r--r--   0        0        0      428 2023-06-02 13:12:07.480000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/fr--tiktok-line.svg
--rw-r--r--   0        0        0      790 2023-06-02 13:12:07.497999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/github-fill.svg
--rw-r--r--   0        0        0     1485 2023-06-02 13:12:07.499000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/github-line.svg
--rw-r--r--   0        0        0      530 2023-06-02 13:12:07.500999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/google-fill.svg
--rw-r--r--   0        0        0      371 2023-06-02 13:12:07.500999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/google-line.svg
--rw-r--r--   0        0        0      965 2023-06-02 13:12:07.516999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/ie-fill.svg
--rw-r--r--   0        0        0      796 2023-06-02 13:12:07.517999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/ie-line.svg
--rw-r--r--   0        0        0      917 2023-06-02 13:12:07.523000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/instagram-fill.svg
--rw-r--r--   0        0        0     2014 2023-06-02 13:12:07.523000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/instagram-line.svg
--rw-r--r--   0        0        0      552 2023-06-02 13:12:07.530999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/linkedin-box-fill.svg
--rw-r--r--   0        0        0      366 2023-06-02 13:12:07.530999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/linkedin-box-line.svg
--rw-r--r--   0        0        0      948 2023-06-02 13:12:07.546000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/mastodon-fill.svg
--rw-r--r--   0        0        0     1259 2023-06-02 13:12:07.546999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/mastodon-line.svg
--rw-r--r--   0        0        0      202 2023-06-02 13:12:07.562000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/npmjs-fill.svg
--rw-r--r--   0        0        0      220 2023-06-02 13:12:07.562000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/npmjs-line.svg
--rw-r--r--   0        0        0      331 2023-06-02 13:12:07.588000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/remixicon-fill.svg
--rw-r--r--   0        0        0      391 2023-06-02 13:12:07.588999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/remixicon-line.svg
--rw-r--r--   0        0        0      972 2023-06-02 13:12:07.592000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/safari-fill.svg
--rw-r--r--   0        0        0      574 2023-06-02 13:12:07.592000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/safari-line.svg
--rw-r--r--   0        0        0     1133 2023-06-02 13:12:07.607000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/slack-fill.svg
--rw-r--r--   0        0        0      514 2023-06-02 13:12:07.607000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/slack-line.svg
--rw-r--r--   0        0        0     1494 2023-06-02 13:12:07.609999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/snapchat-fill.svg
--rw-r--r--   0        0        0     1848 2023-06-02 13:12:07.611000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/snapchat-line.svg
--rw-r--r--   0        0        0      398 2023-06-02 13:12:07.628000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/telegram-fill.svg
--rw-r--r--   0        0        0      440 2023-06-02 13:12:07.628999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/telegram-line.svg
--rw-r--r--   0        0        0      332 2023-06-02 13:12:07.640000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/twitch-fill.svg
--rw-r--r--   0        0        0      241 2023-06-02 13:12:07.641000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/twitch-line.svg
--rw-r--r--   0        0        0      586 2023-06-02 13:12:07.641000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/twitter-fill.svg
--rw-r--r--   0        0        0      690 2023-06-02 13:12:07.641999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/twitter-line.svg
--rw-r--r--   0        0        0      726 2023-06-02 13:12:07.651999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/vimeo-fill.svg
--rw-r--r--   0        0        0     1001 2023-06-02 13:12:07.651999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/vimeo-line.svg
--rw-r--r--   0        0        0      178 2023-06-02 13:12:07.655999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/vuejs-fill.svg
--rw-r--r--   0        0        0      198 2023-06-02 13:12:07.657000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/vuejs-line.svg
--rw-r--r--   0        0        0      418 2023-06-02 13:12:07.658999 mkdocs_dsfr-0.3.1/dsfr/icons/logo/youtube-fill.svg
--rw-r--r--   0        0        0      899 2023-06-02 13:12:07.660000 mkdocs_dsfr-0.3.1/dsfr/icons/logo/youtube-line.svg
--rw-r--r--   0        0        0      385 2023-06-02 13:12:07.377000 mkdocs_dsfr-0.3.1/dsfr/icons/map/anchor-fill.svg
--rw-r--r--   0        0        0      350 2023-06-02 13:12:07.377000 mkdocs_dsfr-0.3.1/dsfr/icons/map/anchor-line.svg
--rw-r--r--   0        0        0      359 2023-06-02 13:12:07.394000 mkdocs_dsfr-0.3.1/dsfr/icons/map/bike-fill.svg
--rw-r--r--   0        0        0      359 2023-06-02 13:12:07.394999 mkdocs_dsfr-0.3.1/dsfr/icons/map/bike-line.svg
--rw-r--r--   0        0        0      284 2023-06-02 13:12:07.404000 mkdocs_dsfr-0.3.1/dsfr/icons/map/bus-fill.svg
--rw-r--r--   0        0        0      299 2023-06-02 13:12:07.404999 mkdocs_dsfr-0.3.1/dsfr/icons/map/bus-line.svg
--rw-r--r--   0        0        0      372 2023-06-02 13:12:07.411000 mkdocs_dsfr-0.3.1/dsfr/icons/map/car-fill.svg
--rw-r--r--   0        0        0      387 2023-06-02 13:12:07.411000 mkdocs_dsfr-0.3.1/dsfr/icons/map/car-line.svg
--rw-r--r--   0        0        0      317 2023-06-02 13:12:07.411999 mkdocs_dsfr-0.3.1/dsfr/icons/map/caravan-fill.svg
--rw-r--r--   0        0        0      383 2023-06-02 13:12:07.411999 mkdocs_dsfr-0.3.1/dsfr/icons/map/caravan-line.svg
--rw-r--r--   0        0        0      253 2023-06-02 13:12:07.411999 mkdocs_dsfr-0.3.1/dsfr/icons/map/charging-pile-2-fill.svg
--rw-r--r--   0        0        0      265 2023-06-02 13:12:07.413000 mkdocs_dsfr-0.3.1/dsfr/icons/map/charging-pile-2-line.svg
--rw-r--r--   0        0        0      246 2023-06-02 13:12:07.427999 mkdocs_dsfr-0.3.1/dsfr/icons/map/compass-3-fill.svg
--rw-r--r--   0        0        0      281 2023-06-02 13:12:07.427999 mkdocs_dsfr-0.3.1/dsfr/icons/map/compass-3-line.svg
--rw-r--r--   0        0        0      222 2023-06-02 13:12:07.434000 mkdocs_dsfr-0.3.1/dsfr/icons/map/cup-fill.svg
--rw-r--r--   0        0        0      264 2023-06-02 13:12:07.434999 mkdocs_dsfr-0.3.1/dsfr/icons/map/cup-line.svg
--rw-r--r--   0        0        0      945 2023-06-02 13:12:07.450000 mkdocs_dsfr-0.3.1/dsfr/icons/map/earth-fill.svg
--rw-r--r--   0        0        0      905 2023-06-02 13:12:07.450000 mkdocs_dsfr-0.3.1/dsfr/icons/map/earth-line.svg
--rw-r--r--   0        0        0     2305 2023-06-02 13:12:07.480999 mkdocs_dsfr-0.3.1/dsfr/icons/map/france-fill.svg
--rw-r--r--   0        0        0     4459 2023-06-02 13:12:07.482000 mkdocs_dsfr-0.3.1/dsfr/icons/map/france-line.svg
--rw-r--r--   0        0        0      303 2023-06-02 13:12:07.483000 mkdocs_dsfr-0.3.1/dsfr/icons/map/gas-station-fill.svg
--rw-r--r--   0        0        0      318 2023-06-02 13:12:07.483999 mkdocs_dsfr-0.3.1/dsfr/icons/map/gas-station-line.svg
--rw-r--r--   0        0        0      179 2023-06-02 13:12:07.500000 mkdocs_dsfr-0.3.1/dsfr/icons/map/goblet-fill.svg
--rw-r--r--   0        0        0      208 2023-06-02 13:12:07.500000 mkdocs_dsfr-0.3.1/dsfr/icons/map/goblet-line.svg
--rw-r--r--   0        0        0      214 2023-06-02 13:12:07.542000 mkdocs_dsfr-0.3.1/dsfr/icons/map/map-pin-2-fill.svg
--rw-r--r--   0        0        0      280 2023-06-02 13:12:07.542999 mkdocs_dsfr-0.3.1/dsfr/icons/map/map-pin-2-line.svg
--rw-r--r--   0        0        0      277 2023-06-02 13:12:07.542999 mkdocs_dsfr-0.3.1/dsfr/icons/map/map-pin-user-fill.svg
--rw-r--r--   0        0        0      363 2023-06-02 13:12:07.543999 mkdocs_dsfr-0.3.1/dsfr/icons/map/map-pin-user-line.svg
--rw-r--r--   0        0        0      378 2023-06-02 13:12:07.556999 mkdocs_dsfr-0.3.1/dsfr/icons/map/motorbike-fill.svg
--rw-r--r--   0        0        0      447 2023-06-02 13:12:07.558000 mkdocs_dsfr-0.3.1/dsfr/icons/map/motorbike-line.svg
--rw-r--r--   0        0        0      256 2023-06-02 13:12:07.569000 mkdocs_dsfr-0.3.1/dsfr/icons/map/passport-fill.svg
--rw-r--r--   0        0        0      272 2023-06-02 13:12:07.569999 mkdocs_dsfr-0.3.1/dsfr/icons/map/passport-line.svg
--rw-r--r--   0        0        0      221 2023-06-02 13:12:07.588999 mkdocs_dsfr-0.3.1/dsfr/icons/map/restaurant-fill.svg
--rw-r--r--   0        0        0      257 2023-06-02 13:12:07.588999 mkdocs_dsfr-0.3.1/dsfr/icons/map/restaurant-line.svg
--rw-r--r--   0        0        0      381 2023-06-02 13:12:07.589999 mkdocs_dsfr-0.3.1/dsfr/icons/map/road-map-fill.svg
--rw-r--r--   0        0        0      405 2023-06-02 13:12:07.591000 mkdocs_dsfr-0.3.1/dsfr/icons/map/road-map-line.svg
--rw-r--r--   0        0        0      278 2023-06-02 13:12:07.592999 mkdocs_dsfr-0.3.1/dsfr/icons/map/sailboat-fill.svg
--rw-r--r--   0        0        0      333 2023-06-02 13:12:07.592999 mkdocs_dsfr-0.3.1/dsfr/icons/map/sailboat-line.svg
--rw-r--r--   0        0        0      580 2023-06-02 13:12:07.602999 mkdocs_dsfr-0.3.1/dsfr/icons/map/ship-2-fill.svg
--rw-r--r--   0        0        0      562 2023-06-02 13:12:07.604000 mkdocs_dsfr-0.3.1/dsfr/icons/map/ship-2-line.svg
--rw-r--r--   0        0        0      351 2023-06-02 13:12:07.605000 mkdocs_dsfr-0.3.1/dsfr/icons/map/signal-tower-fill.svg
--rw-r--r--   0        0        0      348 2023-06-02 13:12:07.605999 mkdocs_dsfr-0.3.1/dsfr/icons/map/signal-tower-line.svg
--rw-r--r--   0        0        0      271 2023-06-02 13:12:07.617000 mkdocs_dsfr-0.3.1/dsfr/icons/map/suitcase-2-fill.svg
--rw-r--r--   0        0        0      286 2023-06-02 13:12:07.617000 mkdocs_dsfr-0.3.1/dsfr/icons/map/suitcase-2-line.svg
--rw-r--r--   0        0        0      374 2023-06-02 13:12:07.625999 mkdocs_dsfr-0.3.1/dsfr/icons/map/taxi-fill.svg
--rw-r--r--   0        0        0      386 2023-06-02 13:12:07.627000 mkdocs_dsfr-0.3.1/dsfr/icons/map/taxi-line.svg
--rw-r--r--   0        0        0      251 2023-06-02 13:12:07.637000 mkdocs_dsfr-0.3.1/dsfr/icons/map/train-fill.svg
--rw-r--r--   0        0        0      293 2023-06-02 13:12:07.637000 mkdocs_dsfr-0.3.1/dsfr/icons/map/train-line.svg
--rw-r--r--   0        0        0      160 2023-06-02 13:12:07.375999 mkdocs_dsfr-0.3.1/dsfr/icons/media/align-left.svg
--rw-r--r--   0        0        0      253 2023-06-02 13:12:07.408999 mkdocs_dsfr-0.3.1/dsfr/icons/media/camera-fill.svg
--rw-r--r--   0        0        0      311 2023-06-02 13:12:07.408999 mkdocs_dsfr-0.3.1/dsfr/icons/media/camera-line.svg
--rw-r--r--   0        0        0      294 2023-06-02 13:12:07.420000 mkdocs_dsfr-0.3.1/dsfr/icons/media/clapperboard-fill.svg
--rw-r--r--   0        0        0      312 2023-06-02 13:12:07.421000 mkdocs_dsfr-0.3.1/dsfr/icons/media/clapperboard-line.svg
--rw-r--r--   0        0        0      334 2023-06-02 13:12:07.453999 mkdocs_dsfr-0.3.1/dsfr/icons/media/equalizer-fill.svg
--rw-r--r--   0        0        0      505 2023-06-02 13:12:07.454999 mkdocs_dsfr-0.3.1/dsfr/icons/media/equalizer-line.svg
--rw-r--r--   0        0        0      340 2023-06-02 13:12:07.463999 mkdocs_dsfr-0.3.1/dsfr/icons/media/film-fill.svg
--rw-r--r--   0        0        0      355 2023-06-02 13:12:07.464999 mkdocs_dsfr-0.3.1/dsfr/icons/media/film-line.svg
--rw-r--r--   0        0        0      184 2023-06-02 13:12:07.482000 mkdocs_dsfr-0.3.1/dsfr/icons/media/fullscreen-line.svg
--rw-r--r--   0        0        0      388 2023-06-02 13:12:07.483000 mkdocs_dsfr-0.3.1/dsfr/icons/media/gallery-fill.svg
--rw-r--r--   0        0        0      466 2023-06-02 13:12:07.483000 mkdocs_dsfr-0.3.1/dsfr/icons/media/gallery-line.svg
--rw-r--r--   0        0        0      261 2023-06-02 13:12:07.509999 mkdocs_dsfr-0.3.1/dsfr/icons/media/headphone-fill.svg
--rw-r--r--   0        0        0      300 2023-06-02 13:12:07.509999 mkdocs_dsfr-0.3.1/dsfr/icons/media/headphone-line.svg
--rw-r--r--   0        0        0      394 2023-06-02 13:12:07.517999 mkdocs_dsfr-0.3.1/dsfr/icons/media/image-add-fill.svg
--rw-r--r--   0        0        0      316 2023-06-02 13:12:07.519000 mkdocs_dsfr-0.3.1/dsfr/icons/media/image-add-line.svg
--rw-r--r--   0        0        0      398 2023-06-02 13:12:07.519000 mkdocs_dsfr-0.3.1/dsfr/icons/media/image-edit-fill.svg
--rw-r--r--   0        0        0      415 2023-06-02 13:12:07.519000 mkdocs_dsfr-0.3.1/dsfr/icons/media/image-edit-line.svg
--rw-r--r--   0        0        0      307 2023-06-02 13:12:07.519999 mkdocs_dsfr-0.3.1/dsfr/icons/media/image-fill.svg
--rw-r--r--   0        0        0      334 2023-06-02 13:12:07.519999 mkdocs_dsfr-0.3.1/dsfr/icons/media/image-line.svg
--rw-r--r--   0        0        0      394 2023-06-02 13:12:07.532999 mkdocs_dsfr-0.3.1/dsfr/icons/media/live-fill.svg
--rw-r--r--   0        0        0      408 2023-06-02 13:12:07.532999 mkdocs_dsfr-0.3.1/dsfr/icons/media/live-line.svg
--rw-r--r--   0        0        0      269 2023-06-02 13:12:07.551000 mkdocs_dsfr-0.3.1/dsfr/icons/media/mic-fill.svg
--rw-r--r--   0        0        0      320 2023-06-02 13:12:07.551000 mkdocs_dsfr-0.3.1/dsfr/icons/media/mic-line.svg
--rw-r--r--   0        0        0      158 2023-06-02 13:12:07.559000 mkdocs_dsfr-0.3.1/dsfr/icons/media/music-2-fill.svg
--rw-r--r--   0        0        0      226 2023-06-02 13:12:07.559000 mkdocs_dsfr-0.3.1/dsfr/icons/media/music-2-line.svg
--rw-r--r--   0        0        0      154 2023-06-02 13:12:07.559999 mkdocs_dsfr-0.3.1/dsfr/icons/media/notification-3-fill.svg
--rw-r--r--   0        0        0      208 2023-06-02 13:12:07.561000 mkdocs_dsfr-0.3.1/dsfr/icons/media/notification-3-line.svg
--rw-r--r--   0        0        0      201 2023-06-02 13:12:07.571000 mkdocs_dsfr-0.3.1/dsfr/icons/media/pause-circle-fill.svg
--rw-r--r--   0        0        0      236 2023-06-02 13:12:07.571000 mkdocs_dsfr-0.3.1/dsfr/icons/media/pause-circle-line.svg
--rw-r--r--   0        0        0      281 2023-06-02 13:12:07.578000 mkdocs_dsfr-0.3.1/dsfr/icons/media/play-circle-fill.svg
--rw-r--r--   0        0        0      313 2023-06-02 13:12:07.578000 mkdocs_dsfr-0.3.1/dsfr/icons/media/play-circle-line.svg
--rw-r--r--   0        0        0      186 2023-06-02 13:12:07.614000 mkdocs_dsfr-0.3.1/dsfr/icons/media/stop-circle-fill.svg
--rw-r--r--   0        0        0      221 2023-06-02 13:12:07.614000 mkdocs_dsfr-0.3.1/dsfr/icons/media/stop-circle-line.svg
--rw-r--r--   0        0        0      403 2023-06-02 13:12:07.654000 mkdocs_dsfr-0.3.1/dsfr/icons/media/volume-down-fill.svg
--rw-r--r--   0        0        0      489 2023-06-02 13:12:07.654000 mkdocs_dsfr-0.3.1/dsfr/icons/media/volume-down-line.svg
--rw-r--r--   0        0        0      407 2023-06-02 13:12:07.654999 mkdocs_dsfr-0.3.1/dsfr/icons/media/volume-mute-fill.svg
--rw-r--r--   0        0        0      490 2023-06-02 13:12:07.654999 mkdocs_dsfr-0.3.1/dsfr/icons/media/volume-mute-line.svg
--rw-r--r--   0        0        0      551 2023-06-02 13:12:07.654999 mkdocs_dsfr-0.3.1/dsfr/icons/media/volume-up-fill.svg
--rw-r--r--   0        0        0      630 2023-06-02 13:12:07.655999 mkdocs_dsfr-0.3.1/dsfr/icons/media/volume-up-line.svg
--rw-r--r--   0        0        0      334 2023-06-02 13:12:07.526000 mkdocs_dsfr-0.3.1/dsfr/icons/others/leaf-fill.svg
--rw-r--r--   0        0        0      467 2023-06-02 13:12:07.526999 mkdocs_dsfr-0.3.1/dsfr/icons/others/leaf-line.svg
--rw-r--r--   0        0        0      253 2023-06-02 13:12:07.528000 mkdocs_dsfr-0.3.1/dsfr/icons/others/lightbulb-fill.svg
--rw-r--r--   0        0        0      406 2023-06-02 13:12:07.528000 mkdocs_dsfr-0.3.1/dsfr/icons/others/lightbulb-line.svg
--rw-r--r--   0        0        0      277 2023-06-02 13:12:07.575999 mkdocs_dsfr-0.3.1/dsfr/icons/others/plant-fill.svg
--rw-r--r--   0        0        0      362 2023-06-02 13:12:07.576999 mkdocs_dsfr-0.3.1/dsfr/icons/others/plant-line.svg
--rw-r--r--   0        0        0      573 2023-06-02 13:12:07.586999 mkdocs_dsfr-0.3.1/dsfr/icons/others/recycle-fill.svg
--rw-r--r--   0        0        0      558 2023-06-02 13:12:07.586999 mkdocs_dsfr-0.3.1/dsfr/icons/others/recycle-line.svg
--rw-r--r--   0        0        0      454 2023-06-02 13:12:07.595000 mkdocs_dsfr-0.3.1/dsfr/icons/others/scales-3-fill.svg
--rw-r--r--   0        0        0      552 2023-06-02 13:12:07.595999 mkdocs_dsfr-0.3.1/dsfr/icons/others/scales-3-line.svg
--rw-r--r--   0        0        0      258 2023-06-02 13:12:07.598000 mkdocs_dsfr-0.3.1/dsfr/icons/others/seedling-fill.svg
--rw-r--r--   0        0        0      326 2023-06-02 13:12:07.598999 mkdocs_dsfr-0.3.1/dsfr/icons/others/seedling-line.svg
--rw-r--r--   0        0        0      232 2023-06-02 13:12:07.641999 mkdocs_dsfr-0.3.1/dsfr/icons/others/umbrella-fill.svg
--rw-r--r--   0        0        0      315 2023-06-02 13:12:07.641999 mkdocs_dsfr-0.3.1/dsfr/icons/others/umbrella-line.svg
--rw-r--r--   0        0        0      209 2023-06-02 13:12:07.369999 mkdocs_dsfr-0.3.1/dsfr/icons/system/add-circle-fill.svg
--rw-r--r--   0        0        0      260 2023-06-02 13:12:07.371000 mkdocs_dsfr-0.3.1/dsfr/icons/system/add-circle-line.svg
--rw-r--r--   0        0        0      136 2023-06-02 13:12:07.371000 mkdocs_dsfr-0.3.1/dsfr/icons/system/add-line.svg
--rw-r--r--   0        0        0      319 2023-06-02 13:12:07.372999 mkdocs_dsfr-0.3.1/dsfr/icons/system/alarm-warning-fill.svg
--rw-r--r--   0        0        0      360 2023-06-02 13:12:07.374000 mkdocs_dsfr-0.3.1/dsfr/icons/system/alarm-warning-line.svg
--rw-r--r--   0        0        0      224 2023-06-02 13:12:07.374000 mkdocs_dsfr-0.3.1/dsfr/icons/system/alert-fill.svg
--rw-r--r--   0        0        0      257 2023-06-02 13:12:07.375000 mkdocs_dsfr-0.3.1/dsfr/icons/system/alert-line.svg
--rw-r--r--   0        0        0      127 2023-06-02 13:12:07.380000 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-down-fill.svg
--rw-r--r--   0        0        0      188 2023-06-02 13:12:07.381000 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-down-line.svg
--rw-r--r--   0        0        0      120 2023-06-02 13:12:07.381000 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-down-s-fill.svg
--rw-r--r--   0        0        0      173 2023-06-02 13:12:07.381000 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-down-s-line.svg
--rw-r--r--   0        0        0      159 2023-06-02 13:12:07.381999 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-go-back-fill.svg
--rw-r--r--   0        0        0      213 2023-06-02 13:12:07.382999 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-go-back-line.svg
--rw-r--r--   0        0        0      161 2023-06-02 13:12:07.382999 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-go-forward-fill.svg
--rw-r--r--   0        0        0      218 2023-06-02 13:12:07.382999 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-go-forward-line.svg
--rw-r--r--   0        0        0      128 2023-06-02 13:12:07.382999 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-left-fill.svg
--rw-r--r--   0        0        0      184 2023-06-02 13:12:07.384000 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-left-line.svg
--rw-r--r--   0        0        0      119 2023-06-02 13:12:07.384000 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-left-s-fill.svg
--rw-r--r--   0        0        0      173 2023-06-02 13:12:07.384999 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-left-s-line.svg
--rw-r--r--   0        0        0      128 2023-06-02 13:12:07.384999 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-right-fill.svg
--rw-r--r--   0        0        0      189 2023-06-02 13:12:07.384999 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-right-line.svg
--rw-r--r--   0        0        0      118 2023-06-02 13:12:07.385999 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-right-s-fill.svg
--rw-r--r--   0        0        0      175 2023-06-02 13:12:07.385999 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-right-s-line.svg
--rw-r--r--   0        0        0      197 2023-06-02 13:12:07.385999 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-right-up-line.svg
--rw-r--r--   0        0        0      129 2023-06-02 13:12:07.387000 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-up-fill.svg
--rw-r--r--   0        0        0      186 2023-06-02 13:12:07.387000 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-up-line.svg
--rw-r--r--   0        0        0      117 2023-06-02 13:12:07.387000 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-up-s-fill.svg
--rw-r--r--   0        0        0      173 2023-06-02 13:12:07.388000 mkdocs_dsfr-0.3.1/dsfr/icons/system/arrow-up-s-line.svg
--rw-r--r--   0        0        0      177 2023-06-02 13:12:07.417000 mkdocs_dsfr-0.3.1/dsfr/icons/system/check-line.svg
--rw-r--r--   0        0        0      252 2023-06-02 13:12:07.417000 mkdocs_dsfr-0.3.1/dsfr/icons/system/checkbox-circle-fill.svg
--rw-r--r--   0        0        0      288 2023-06-02 13:12:07.417999 mkdocs_dsfr-0.3.1/dsfr/icons/system/checkbox-circle-line.svg
--rw-r--r--   0        0        0      252 2023-06-02 13:12:07.417999 mkdocs_dsfr-0.3.1/dsfr/icons/system/checkbox-fill.svg
--rw-r--r--   0        0        0      288 2023-06-02 13:12:07.417999 mkdocs_dsfr-0.3.1/dsfr/icons/system/checkbox-line.svg
--rw-r--r--   0        0        0      321 2023-06-02 13:12:07.421999 mkdocs_dsfr-0.3.1/dsfr/icons/system/close-circle-fill.svg
--rw-r--r--   0        0        0      342 2023-06-02 13:12:07.421999 mkdocs_dsfr-0.3.1/dsfr/icons/system/close-circle-line.svg
--rw-r--r--   0        0        0      210 2023-06-02 13:12:07.421999 mkdocs_dsfr-0.3.1/dsfr/icons/system/close-line.svg
--rw-r--r--   0        0        0      189 2023-06-02 13:12:07.438999 mkdocs_dsfr-0.3.1/dsfr/icons/system/delete-bin-fill.svg
--rw-r--r--   0        0        0      203 2023-06-02 13:12:07.440000 mkdocs_dsfr-0.3.1/dsfr/icons/system/delete-bin-line.svg
--rw-r--r--   0        0        0      142 2023-06-02 13:12:07.446000 mkdocs_dsfr-0.3.1/dsfr/icons/system/download-fill.svg
--rw-r--r--   0        0        0      198 2023-06-02 13:12:07.446000 mkdocs_dsfr-0.3.1/dsfr/icons/system/download-line.svg
--rw-r--r--   0        0        0      203 2023-06-02 13:12:07.454999 mkdocs_dsfr-0.3.1/dsfr/icons/system/error-warning-fill.svg
--rw-r--r--   0        0        0      238 2023-06-02 13:12:07.454999 mkdocs_dsfr-0.3.1/dsfr/icons/system/error-warning-line.svg
--rw-r--r--   0        0        0      228 2023-06-02 13:12:07.456000 mkdocs_dsfr-0.3.1/dsfr/icons/system/external-link-fill.svg
--rw-r--r--   0        0        0      230 2023-06-02 13:12:07.456000 mkdocs_dsfr-0.3.1/dsfr/icons/system/external-link-line.svg
--rw-r--r--   0        0        0      281 2023-06-02 13:12:07.457000 mkdocs_dsfr-0.3.1/dsfr/icons/system/eye-fill.svg
--rw-r--r--   0        0        0      380 2023-06-02 13:12:07.457000 mkdocs_dsfr-0.3.1/dsfr/icons/system/eye-line.svg
--rw-r--r--   0        0        0      481 2023-06-02 13:12:07.457000 mkdocs_dsfr-0.3.1/dsfr/icons/system/eye-off-fill.svg
--rw-r--r--   0        0        0      678 2023-06-02 13:12:07.457999 mkdocs_dsfr-0.3.1/dsfr/icons/system/eye-off-line.svg
--rw-r--r--   0        0        0      136 2023-06-02 13:12:07.464999 mkdocs_dsfr-0.3.1/dsfr/icons/system/filter-fill.svg
--rw-r--r--   0        0        0      187 2023-06-02 13:12:07.466000 mkdocs_dsfr-0.3.1/dsfr/icons/system/filter-line.svg
--rw-r--r--   0        0        0      196 2023-06-02 13:12:07.471999 mkdocs_dsfr-0.3.1/dsfr/icons/system/fr--arrow-left-s-first-line.svg
--rw-r--r--   0        0        0      197 2023-06-02 13:12:07.471999 mkdocs_dsfr-0.3.1/dsfr/icons/system/fr--arrow-left-s-line-double.svg
--rw-r--r--   0        0        0      377 2023-06-02 13:12:07.473000 mkdocs_dsfr-0.3.1/dsfr/icons/system/fr--arrow-right-down-circle-fill.svg
--rw-r--r--   0        0        0      201 2023-06-02 13:12:07.473000 mkdocs_dsfr-0.3.1/dsfr/icons/system/fr--arrow-right-s-last-line.svg
--rw-r--r--   0        0        0      201 2023-06-02 13:12:07.473000 mkdocs_dsfr-0.3.1/dsfr/icons/system/fr--arrow-right-s-line-double.svg
--rw-r--r--   0        0        0      377 2023-06-02 13:12:07.473999 mkdocs_dsfr-0.3.1/dsfr/icons/system/fr--arrow-right-up-circle-fill.svg
--rw-r--r--   0        0        0      327 2023-06-02 13:12:07.473999 mkdocs_dsfr-0.3.1/dsfr/icons/system/fr--capslock-line.svg
--rw-r--r--   0        0        0      329 2023-06-02 13:12:07.474999 mkdocs_dsfr-0.3.1/dsfr/icons/system/fr--equal-circle-fill.svg
--rw-r--r--   0        0        0      260 2023-06-02 13:12:07.476000 mkdocs_dsfr-0.3.1/dsfr/icons/system/fr--error-fill.svg
--rw-r--r--   0        0        0      309 2023-06-02 13:12:07.476000 mkdocs_dsfr-0.3.1/dsfr/icons/system/fr--error-line.svg
--rw-r--r--   0        0        0      237 2023-06-02 13:12:07.476999 mkdocs_dsfr-0.3.1/dsfr/icons/system/fr--info-fill.svg
--rw-r--r--   0        0        0      328 2023-06-02 13:12:07.476999 mkdocs_dsfr-0.3.1/dsfr/icons/system/fr--info-line.svg
--rw-r--r--   0        0        0      253 2023-06-02 13:12:07.477999 mkdocs_dsfr-0.3.1/dsfr/icons/system/fr--success-fill.svg
--rw-r--r--   0        0        0      289 2023-06-02 13:12:07.479000 mkdocs_dsfr-0.3.1/dsfr/icons/system/fr--success-line.svg
--rw-r--r--   0        0        0      482 2023-06-02 13:12:07.479000 mkdocs_dsfr-0.3.1/dsfr/icons/system/fr--theme-fill.svg
--rw-r--r--   0        0        0      225 2023-06-02 13:12:07.480999 mkdocs_dsfr-0.3.1/dsfr/icons/system/fr--warning-fill.svg
--rw-r--r--   0        0        0      258 2023-06-02 13:12:07.480999 mkdocs_dsfr-0.3.1/dsfr/icons/system/fr--warning-line.svg
--rw-r--r--   0        0        0      205 2023-06-02 13:12:07.520999 mkdocs_dsfr-0.3.1/dsfr/icons/system/information-fill.svg
--rw-r--r--   0        0        0      239 2023-06-02 13:12:07.520999 mkdocs_dsfr-0.3.1/dsfr/icons/system/information-line.svg
--rw-r--r--   0        0        0      238 2023-06-02 13:12:07.535000 mkdocs_dsfr-0.3.1/dsfr/icons/system/lock-fill.svg
--rw-r--r--   0        0        0      252 2023-06-02 13:12:07.535000 mkdocs_dsfr-0.3.1/dsfr/icons/system/lock-line.svg
--rw-r--r--   0        0        0      252 2023-06-02 13:12:07.536000 mkdocs_dsfr-0.3.1/dsfr/icons/system/lock-unlock-fill.svg
--rw-r--r--   0        0        0      268 2023-06-02 13:12:07.536000 mkdocs_dsfr-0.3.1/dsfr/icons/system/lock-unlock-line.svg
--rw-r--r--   0        0        0      197 2023-06-02 13:12:07.536999 mkdocs_dsfr-0.3.1/dsfr/icons/system/logout-box-r-fill.svg
--rw-r--r--   0        0        0      219 2023-06-02 13:12:07.538000 mkdocs_dsfr-0.3.1/dsfr/icons/system/logout-box-r-line.svg
--rw-r--r--   0        0        0      145 2023-06-02 13:12:07.549000 mkdocs_dsfr-0.3.1/dsfr/icons/system/menu-2-fill.svg
--rw-r--r--   0        0        0      145 2023-06-02 13:12:07.549999 mkdocs_dsfr-0.3.1/dsfr/icons/system/menu-fill.svg
--rw-r--r--   0        0        0      248 2023-06-02 13:12:07.555999 mkdocs_dsfr-0.3.1/dsfr/icons/system/more-fill.svg
--rw-r--r--   0        0        0      348 2023-06-02 13:12:07.555999 mkdocs_dsfr-0.3.1/dsfr/icons/system/more-line.svg
--rw-r--r--   0        0        0      220 2023-06-02 13:12:07.561000 mkdocs_dsfr-0.3.1/dsfr/icons/system/notification-badge-fill.svg
--rw-r--r--   0        0        0      288 2023-06-02 13:12:07.561000 mkdocs_dsfr-0.3.1/dsfr/icons/system/notification-badge-line.svg
--rw-r--r--   0        0        0      311 2023-06-02 13:12:07.585000 mkdocs_dsfr-0.3.1/dsfr/icons/system/question-fill.svg
--rw-r--r--   0        0        0      325 2023-06-02 13:12:07.585000 mkdocs_dsfr-0.3.1/dsfr/icons/system/question-line.svg
--rw-r--r--   0        0        0      280 2023-06-02 13:12:07.586999 mkdocs_dsfr-0.3.1/dsfr/icons/system/refresh-fill.svg
--rw-r--r--   0        0        0      244 2023-06-02 13:12:07.588000 mkdocs_dsfr-0.3.1/dsfr/icons/system/refresh-line.svg
--rw-r--r--   0        0        0      247 2023-06-02 13:12:07.596999 mkdocs_dsfr-0.3.1/dsfr/icons/system/search-fill.svg
--rw-r--r--   0        0        0      382 2023-06-02 13:12:07.596999 mkdocs_dsfr-0.3.1/dsfr/icons/system/search-line.svg
--rw-r--r--   0        0        0      864 2023-06-02 13:12:07.601000 mkdocs_dsfr-0.3.1/dsfr/icons/system/settings-5-fill.svg
--rw-r--r--   0        0        0     1599 2023-06-02 13:12:07.601999 mkdocs_dsfr-0.3.1/dsfr/icons/system/settings-5-line.svg
--rw-r--r--   0        0        0      241 2023-06-02 13:12:07.601999 mkdocs_dsfr-0.3.1/dsfr/icons/system/shield-fill.svg
--rw-r--r--   0        0        0      332 2023-06-02 13:12:07.601999 mkdocs_dsfr-0.3.1/dsfr/icons/system/shield-line.svg
--rw-r--r--   0        0        0      217 2023-06-02 13:12:07.611999 mkdocs_dsfr-0.3.1/dsfr/icons/system/star-fill.svg
--rw-r--r--   0        0        0      333 2023-06-02 13:12:07.611999 mkdocs_dsfr-0.3.1/dsfr/icons/system/star-line.svg
--rw-r--r--   0        0        0      203 2023-06-02 13:12:07.611999 mkdocs_dsfr-0.3.1/dsfr/icons/system/star-s-fill.svg
--rw-r--r--   0        0        0      325 2023-06-02 13:12:07.612999 mkdocs_dsfr-0.3.1/dsfr/icons/system/star-s-line.svg
--rw-r--r--   0        0        0      117 2023-06-02 13:12:07.615999 mkdocs_dsfr-0.3.1/dsfr/icons/system/subtract-line.svg
--rw-r--r--   0        0        0      341 2023-06-02 13:12:07.631999 mkdocs_dsfr-0.3.1/dsfr/icons/system/thumb-down-fill.svg
--rw-r--r--   0        0        0      442 2023-06-02 13:12:07.632999 mkdocs_dsfr-0.3.1/dsfr/icons/system/thumb-down-line.svg
--rw-r--r--   0        0        0      340 2023-06-02 13:12:07.632999 mkdocs_dsfr-0.3.1/dsfr/icons/system/thumb-up-fill.svg
--rw-r--r--   0        0        0      459 2023-06-02 13:12:07.634000 mkdocs_dsfr-0.3.1/dsfr/icons/system/thumb-up-line.svg
--rw-r--r--   0        0        0      193 2023-06-02 13:12:07.634000 mkdocs_dsfr-0.3.1/dsfr/icons/system/time-fill.svg
--rw-r--r--   0        0        0      226 2023-06-02 13:12:07.634000 mkdocs_dsfr-0.3.1/dsfr/icons/system/time-line.svg
--rw-r--r--   0        0        0      201 2023-06-02 13:12:07.634999 mkdocs_dsfr-0.3.1/dsfr/icons/system/timer-fill.svg
--rw-r--r--   0        0        0      236 2023-06-02 13:12:07.634999 mkdocs_dsfr-0.3.1/dsfr/icons/system/timer-line.svg
--rw-r--r--   0        0        0      180 2023-06-02 13:12:07.642999 mkdocs_dsfr-0.3.1/dsfr/icons/system/upload-2-fill.svg
--rw-r--r--   0        0        0      180 2023-06-02 13:12:07.642999 mkdocs_dsfr-0.3.1/dsfr/icons/system/upload-2-line.svg
--rw-r--r--   0        0        0      144 2023-06-02 13:12:07.644000 mkdocs_dsfr-0.3.1/dsfr/icons/system/upload-fill.svg
--rw-r--r--   0        0        0      206 2023-06-02 13:12:07.644000 mkdocs_dsfr-0.3.1/dsfr/icons/system/upload-line.svg
--rw-r--r--   0        0        0      279 2023-06-02 13:12:07.660000 mkdocs_dsfr-0.3.1/dsfr/icons/system/zoom-in-fill.svg
--rw-r--r--   0        0        0      407 2023-06-02 13:12:07.660000 mkdocs_dsfr-0.3.1/dsfr/icons/system/zoom-in-line.svg
--rw-r--r--   0        0        0      260 2023-06-02 13:12:07.661000 mkdocs_dsfr-0.3.1/dsfr/icons/system/zoom-out-fill.svg
--rw-r--r--   0        0        0      388 2023-06-02 13:12:07.661000 mkdocs_dsfr-0.3.1/dsfr/icons/system/zoom-out-line.svg
--rw-r--r--   0        0        0      337 2023-06-02 13:12:07.368999 mkdocs_dsfr-0.3.1/dsfr/icons/user/account-circle-fill.svg
--rw-r--r--   0        0        0      462 2023-06-02 13:12:07.368999 mkdocs_dsfr-0.3.1/dsfr/icons/user/account-circle-line.svg
--rw-r--r--   0        0        0      383 2023-06-02 13:12:07.368999 mkdocs_dsfr-0.3.1/dsfr/icons/user/account-pin-circle-fill.svg
--rw-r--r--   0        0        0      575 2023-06-02 13:12:07.369999 mkdocs_dsfr-0.3.1/dsfr/icons/user/account-pin-circle-line.svg
--rw-r--r--   0        0        0      279 2023-06-02 13:12:07.371000 mkdocs_dsfr-0.3.1/dsfr/icons/user/admin-fill.svg
--rw-r--r--   0        0        0      349 2023-06-02 13:12:07.371999 mkdocs_dsfr-0.3.1/dsfr/icons/user/admin-line.svg
--rw-r--r--   0        0        0      357 2023-06-02 13:12:07.503000 mkdocs_dsfr-0.3.1/dsfr/icons/user/group-fill.svg
--rw-r--r--   0        0        0      462 2023-06-02 13:12:07.503999 mkdocs_dsfr-0.3.1/dsfr/icons/user/group-line.svg
--rw-r--r--   0        0        0      279 2023-06-02 13:12:07.568000 mkdocs_dsfr-0.3.1/dsfr/icons/user/parent-fill.svg
--rw-r--r--   0        0        0      413 2023-06-02 13:12:07.569000 mkdocs_dsfr-0.3.1/dsfr/icons/user/parent-line.svg
--rw-r--r--   0        0        0      424 2023-06-02 13:12:07.627000 mkdocs_dsfr-0.3.1/dsfr/icons/user/team-fill.svg
--rw-r--r--   0        0        0      750 2023-06-02 13:12:07.628000 mkdocs_dsfr-0.3.1/dsfr/icons/user/team-line.svg
--rw-r--r--   0        0        0      235 2023-06-02 13:12:07.644000 mkdocs_dsfr-0.3.1/dsfr/icons/user/user-add-fill.svg
--rw-r--r--   0        0        0      316 2023-06-02 13:12:07.644999 mkdocs_dsfr-0.3.1/dsfr/icons/user/user-add-line.svg
--rw-r--r--   0        0        0      186 2023-06-02 13:12:07.644999 mkdocs_dsfr-0.3.1/dsfr/icons/user/user-fill.svg
--rw-r--r--   0        0        0      314 2023-06-02 13:12:07.645999 mkdocs_dsfr-0.3.1/dsfr/icons/user/user-heart-fill.svg
--rw-r--r--   0        0        0      439 2023-06-02 13:12:07.645999 mkdocs_dsfr-0.3.1/dsfr/icons/user/user-heart-line.svg
--rw-r--r--   0        0        0      275 2023-06-02 13:12:07.647000 mkdocs_dsfr-0.3.1/dsfr/icons/user/user-line.svg
--rw-r--r--   0        0        0      314 2023-06-02 13:12:07.647000 mkdocs_dsfr-0.3.1/dsfr/icons/user/user-search-fill.svg
--rw-r--r--   0        0        0      384 2023-06-02 13:12:07.647000 mkdocs_dsfr-0.3.1/dsfr/icons/user/user-search-line.svg
--rw-r--r--   0        0        0      529 2023-06-02 13:12:07.648000 mkdocs_dsfr-0.3.1/dsfr/icons/user/user-setting-fill.svg
--rw-r--r--   0        0        0      462 2023-06-02 13:12:07.648000 mkdocs_dsfr-0.3.1/dsfr/icons/user/user-setting-line.svg
--rw-r--r--   0        0        0      298 2023-06-02 13:12:07.648000 mkdocs_dsfr-0.3.1/dsfr/icons/user/user-star-fill.svg
--rw-r--r--   0        0        0      367 2023-06-02 13:12:07.648999 mkdocs_dsfr-0.3.1/dsfr/icons/user/user-star-line.svg
--rw-r--r--   0        0        0      167 2023-06-02 13:12:07.424000 mkdocs_dsfr-0.3.1/dsfr/icons/weather/cloudy-2-fill.svg
--rw-r--r--   0        0        0      291 2023-06-02 13:12:07.424000 mkdocs_dsfr-0.3.1/dsfr/icons/weather/cloudy-2-line.svg
--rw-r--r--   0        0        0      128 2023-06-02 13:12:07.470000 mkdocs_dsfr-0.3.1/dsfr/icons/weather/flashlight-fill.svg
--rw-r--r--   0        0        0      172 2023-06-02 13:12:07.470000 mkdocs_dsfr-0.3.1/dsfr/icons/weather/flashlight-line.svg
--rw-r--r--   0        0        0      226 2023-06-02 13:12:07.555000 mkdocs_dsfr-0.3.1/dsfr/icons/weather/moon-fill.svg
--rw-r--r--   0        0        0      286 2023-06-02 13:12:07.555000 mkdocs_dsfr-0.3.1/dsfr/icons/weather/moon-line.svg
--rw-r--r--   0        0        0      449 2023-06-02 13:12:07.618000 mkdocs_dsfr-0.3.1/dsfr/icons/weather/sun-fill.svg
--rw-r--r--   0        0        0      482 2023-06-02 13:12:07.618000 mkdocs_dsfr-0.3.1/dsfr/icons/weather/sun-line.svg
--rw-r--r--   0        0        0     1221 2023-05-31 09:02:28.010861 mkdocs_dsfr-0.3.1/dsfr/js/base.js
--rw-r--r--   0        0        0    58073 2023-05-31 09:02:28.011124 mkdocs_dsfr-0.3.1/dsfr/js/bootstrap.min.js
--rw-r--r--   0        0        0    93107 2023-05-31 09:02:28.011514 mkdocs_dsfr-0.3.1/dsfr/js/jquery-1.10.2.min.js
--rw-r--r--   0        0        0     1553 2023-05-31 09:02:28.011584 mkdocs_dsfr-0.3.1/dsfr/lateral.html
--rw-r--r--   0        0        0       25 2023-05-31 09:02:28.011646 mkdocs_dsfr-0.3.1/dsfr/main.html
--rw-r--r--   0        0        0      174 2023-05-31 09:02:28.011702 mkdocs_dsfr-0.3.1/dsfr/mkdocs_theme.yml
--rw-r--r--   0        0        0     1068 2023-05-31 09:02:28.011760 mkdocs_dsfr-0.3.1/dsfr/nav.html
--rw-r--r--   0        0        0      743 2023-05-31 09:02:28.011819 mkdocs_dsfr-0.3.1/dsfr/prev-next-nav.html
--rw-r--r--   0        0        0      575 2023-05-31 09:02:28.011878 mkdocs_dsfr-0.3.1/dsfr/search.html
--rw-r--r--   0        0        0        0 2023-05-31 09:05:29.657662 mkdocs_dsfr-0.3.1/dsfr/tabs.html
--rw-r--r--   0        0        0      748 2023-06-02 13:12:07.173000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/README.md
--rw-r--r--   0        0        0      794 2023-06-02 13:12:07.171000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/README.md
--rw-r--r--   0        0        0     8218 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.css
--rw-r--r--   0        0        0    18287 2023-06-02 13:12:07.059999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.css.map
--rw-r--r--   0        0        0     3542 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.css
--rw-r--r--   0        0        0     8457 2023-06-02 13:12:07.059999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.css.map
--rw-r--r--   0        0        0     3036 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.min.css
--rw-r--r--   0        0        0     8332 2023-06-02 13:12:07.059999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.min.css.map
--rw-r--r--   0        0        0     4916 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.main.css
--rw-r--r--   0        0        0    12037 2023-06-02 13:12:07.059999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.main.css.map
--rw-r--r--   0        0        0     4370 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.main.min.css
--rw-r--r--   0        0        0    11358 2023-06-02 13:12:07.059999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.main.min.css.map
--rw-r--r--   0        0        0     7178 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.min.css
--rw-r--r--   0        0        0    17475 2023-06-02 13:12:07.061000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.min.css.map
--rw-r--r--   0        0        0      788 2023-06-02 13:12:07.171000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/README.md
--rw-r--r--   0        0        0    22912 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.css
--rw-r--r--   0        0        0    36228 2023-06-02 13:12:07.061000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.css.map
--rw-r--r--   0        0        0     9504 2023-06-02 13:12:06.515000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.legacy.css
--rw-r--r--   0        0        0    15589 2023-06-02 13:12:07.061000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.legacy.css.map
--rw-r--r--   0        0        0     8088 2023-06-02 13:12:06.515000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.legacy.min.css
--rw-r--r--   0        0        0    15215 2023-06-02 13:12:07.061000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.legacy.min.css.map
--rw-r--r--   0        0        0    13648 2023-06-02 13:12:06.515000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.main.css
--rw-r--r--   0        0        0    22829 2023-06-02 13:12:07.062000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.main.css.map
--rw-r--r--   0        0        0    12243 2023-06-02 13:12:06.515000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.main.min.css
--rw-r--r--   0        0        0    21852 2023-06-02 13:12:07.062000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.main.min.css.map
--rw-r--r--   0        0        0    20103 2023-06-02 13:12:06.516000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.min.css
--rw-r--r--   0        0        0    34868 2023-06-02 13:12:07.062000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.min.css.map
--rw-r--r--   0        0        0      818 2023-06-02 13:12:07.171000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/README.md
--rw-r--r--   0        0        0     8770 2023-06-02 13:12:06.516000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.css
--rw-r--r--   0        0        0    18782 2023-06-02 13:12:07.062000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.css.map
--rw-r--r--   0        0        0     3786 2023-06-02 13:12:06.516000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.legacy.css
--rw-r--r--   0        0        0     8627 2023-06-02 13:12:07.062000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.legacy.css.map
--rw-r--r--   0        0        0     3272 2023-06-02 13:12:06.516000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.legacy.min.css
--rw-r--r--   0        0        0     8500 2023-06-02 13:12:07.062000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.legacy.min.css.map
--rw-r--r--   0        0        0     5224 2023-06-02 13:12:06.516000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.main.css
--rw-r--r--   0        0        0    12366 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.main.css.map
--rw-r--r--   0        0        0     4674 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.main.min.css
--rw-r--r--   0        0        0    11670 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.main.min.css.map
--rw-r--r--   0        0        0     7718 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.min.css
--rw-r--r--   0        0        0    17951 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.min.css.map
--rw-r--r--   0        0        0      776 2023-06-02 13:12:07.171000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/README.md
--rw-r--r--   0        0        0    15237 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.css
--rw-r--r--   0        0        0    26942 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.css.map
--rw-r--r--   0        0        0     6494 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.legacy.css
--rw-r--r--   0        0        0    12000 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.legacy.css.map
--rw-r--r--   0        0        0     5504 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.legacy.min.css
--rw-r--r--   0        0        0    11743 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.legacy.min.css.map
--rw-r--r--   0        0        0     8983 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.main.css
--rw-r--r--   0        0        0    17146 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.main.css.map
--rw-r--r--   0        0        0     8000 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.main.min.css
--rw-r--r--   0        0        0    16324 2023-06-02 13:12:07.063999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.main.min.css.map
--rw-r--r--   0        0        0    13276 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.min.css
--rw-r--r--   0        0        0    25855 2023-06-02 13:12:07.063999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.min.css.map
--rw-r--r--   0        0        0      806 2023-06-02 13:12:07.171000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/README.md
--rw-r--r--   0        0        0    10584 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.css
--rw-r--r--   0        0        0    20888 2023-06-02 13:12:07.063999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.css.map
--rw-r--r--   0        0        0     4556 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.legacy.css
--rw-r--r--   0        0        0     9503 2023-06-02 13:12:07.063999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.legacy.css.map
--rw-r--r--   0        0        0     3954 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.legacy.min.css
--rw-r--r--   0        0        0     9352 2023-06-02 13:12:07.063999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.legacy.min.css.map
--rw-r--r--   0        0        0     6268 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.main.css
--rw-r--r--   0        0        0    13594 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.main.css.map
--rw-r--r--   0        0        0     5638 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.main.min.css
--rw-r--r--   0        0        0    12876 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.main.min.css.map
--rw-r--r--   0        0        0     9364 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.min.css
--rw-r--r--   0        0        0    20011 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.min.css.map
--rw-r--r--   0        0        0      776 2023-06-02 13:12:07.171000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/README.md
--rw-r--r--   0        0        0    13498 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.css
--rw-r--r--   0        0        0    24915 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.css.map
--rw-r--r--   0        0        0     5696 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.legacy.css
--rw-r--r--   0        0        0    11099 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.legacy.css.map
--rw-r--r--   0        0        0     4810 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.legacy.min.css
--rw-r--r--   0        0        0    10870 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.legacy.min.css.map
--rw-r--r--   0        0        0     8042 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.main.css
--rw-r--r--   0        0        0    16020 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.main.css.map
--rw-r--r--   0        0        0     7132 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.main.min.css
--rw-r--r--   0        0        0    15219 2023-06-02 13:12:07.065999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.main.min.css.map
--rw-r--r--   0        0        0    11714 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.min.css
--rw-r--r--   0        0        0    23877 2023-06-02 13:12:07.065999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.min.css.map
--rw-r--r--   0        0        0      788 2023-06-02 13:12:07.171999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/README.md
--rw-r--r--   0        0        0    12044 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.css
--rw-r--r--   0        0        0    23019 2023-06-02 13:12:07.065999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.css.map
--rw-r--r--   0        0        0     5060 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.legacy.css
--rw-r--r--   0        0        0    10303 2023-06-02 13:12:07.065999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.legacy.css.map
--rw-r--r--   0        0        0     4306 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.legacy.min.css
--rw-r--r--   0        0        0    10110 2023-06-02 13:12:07.065999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.legacy.min.css.map
--rw-r--r--   0        0        0     7224 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.main.css
--rw-r--r--   0        0        0    14922 2023-06-02 13:12:07.066999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.main.css.map
--rw-r--r--   0        0        0     6434 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.main.min.css
--rw-r--r--   0        0        0    14157 2023-06-02 13:12:07.066999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.main.min.css.map
--rw-r--r--   0        0        0    10512 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.min.css
--rw-r--r--   0        0        0    22053 2023-06-02 13:12:07.066999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.min.css.map
--rw-r--r--   0        0        0      776 2023-06-02 13:12:07.171999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/README.md
--rw-r--r--   0        0        0    10188 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.css
--rw-r--r--   0        0        0    21006 2023-06-02 13:12:07.066999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.css.map
--rw-r--r--   0        0        0     4282 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.legacy.css
--rw-r--r--   0        0        0     9470 2023-06-02 13:12:07.066999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.legacy.css.map
--rw-r--r--   0        0        0     3576 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.legacy.min.css
--rw-r--r--   0        0        0     9290 2023-06-02 13:12:07.068000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.legacy.min.css.map
--rw-r--r--   0        0        0     6146 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.main.css
--rw-r--r--   0        0        0    13740 2023-06-02 13:12:07.068000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.main.css.map
--rw-r--r--   0        0        0     5396 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.main.min.css
--rw-r--r--   0        0        0    12995 2023-06-02 13:12:07.068000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.main.min.css.map
--rw-r--r--   0        0        0     8744 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.min.css
--rw-r--r--   0        0        0    20073 2023-06-02 13:12:07.068000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.min.css.map
--rw-r--r--   0        0        0      782 2023-06-02 13:12:07.171999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/README.md
--rw-r--r--   0        0        0     6775 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.css
--rw-r--r--   0        0        0    16388 2023-06-02 13:12:07.068000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.css.map
--rw-r--r--   0        0        0     2988 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.legacy.css
--rw-r--r--   0        0        0     7688 2023-06-02 13:12:07.069000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.legacy.css.map
--rw-r--r--   0        0        0     2584 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.legacy.min.css
--rw-r--r--   0        0        0     7591 2023-06-02 13:12:07.069000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.legacy.min.css.map
--rw-r--r--   0        0        0     4027 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.main.css
--rw-r--r--   0        0        0    10905 2023-06-02 13:12:07.069000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.main.css.map
--rw-r--r--   0        0        0     3577 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.main.min.css
--rw-r--r--   0        0        0    10262 2023-06-02 13:12:07.069000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.main.min.css.map
--rw-r--r--   0        0        0     5933 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.min.css
--rw-r--r--   0        0        0    15640 2023-06-02 13:12:07.069000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.min.css.map
--rw-r--r--   0        0        0      776 2023-06-02 13:12:07.171999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/README.md
--rw-r--r--   0        0        0    14367 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.css
--rw-r--r--   0        0        0    25626 2023-06-02 13:12:07.069000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.css.map
--rw-r--r--   0        0        0     6168 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.legacy.css
--rw-r--r--   0        0        0    11461 2023-06-02 13:12:07.069999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.legacy.css.map
--rw-r--r--   0        0        0     5280 2023-06-02 13:12:06.520999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.legacy.min.css
--rw-r--r--   0        0        0    11232 2023-06-02 13:12:07.069999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.legacy.min.css.map
--rw-r--r--   0        0        0     8439 2023-06-02 13:12:06.520999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.main.css
--rw-r--r--   0        0        0    16369 2023-06-02 13:12:07.069999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.main.css.map
--rw-r--r--   0        0        0     7549 2023-06-02 13:12:06.520999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.main.min.css
--rw-r--r--   0        0        0    15575 2023-06-02 13:12:07.069999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.main.min.css.map
--rw-r--r--   0        0        0    12601 2023-06-02 13:12:06.520999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.min.css
--rw-r--r--   0        0        0    24595 2023-06-02 13:12:07.069999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.min.css.map
--rw-r--r--   0        0        0      764 2023-06-02 13:12:07.171999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/README.md
--rw-r--r--   0        0        0    24122 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.css
--rw-r--r--   0        0        0    38165 2023-06-02 13:12:07.069999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.css.map
--rw-r--r--   0        0        0     9746 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.legacy.css
--rw-r--r--   0        0        0    16087 2023-06-02 13:12:07.071000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.legacy.css.map
--rw-r--r--   0        0        0     8200 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.legacy.min.css
--rw-r--r--   0        0        0    15676 2023-06-02 13:12:07.071000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.legacy.min.css.map
--rw-r--r--   0        0        0    14616 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.main.css
--rw-r--r--   0        0        0    24218 2023-06-02 13:12:07.071000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.main.css.map
--rw-r--r--   0        0        0    13026 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.main.min.css
--rw-r--r--   0        0        0    23185 2023-06-02 13:12:07.071000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.main.min.css.map
--rw-r--r--   0        0        0    20998 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.min.css
--rw-r--r--   0        0        0    36712 2023-06-02 13:12:07.071000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.min.css.map
--rw-r--r--   0        0        0      758 2023-06-02 13:12:07.171999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/README.md
--rw-r--r--   0        0        0    17550 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.css
--rw-r--r--   0        0        0    29852 2023-06-02 13:12:07.072000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.css.map
--rw-r--r--   0        0        0     7456 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.legacy.css
--rw-r--r--   0        0        0    13177 2023-06-02 13:12:07.072000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.legacy.css.map
--rw-r--r--   0        0        0     6298 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.legacy.min.css
--rw-r--r--   0        0        0    12874 2023-06-02 13:12:07.072000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.legacy.min.css.map
--rw-r--r--   0        0        0    10334 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.main.css
--rw-r--r--   0        0        0    18876 2023-06-02 13:12:07.072000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.main.css.map
--rw-r--r--   0        0        0     9184 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.main.min.css
--rw-r--r--   0        0        0    18000 2023-06-02 13:12:07.072999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.main.min.css.map
--rw-r--r--   0        0        0    15254 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.min.css
--rw-r--r--   0        0        0    28665 2023-06-02 13:12:07.072999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.min.css.map
--rw-r--r--   0        0        0      770 2023-06-02 13:12:07.173000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/README.md
--rw-r--r--   0        0        0    19301 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.css
--rw-r--r--   0        0        0    31920 2023-06-02 13:12:07.072999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.css.map
--rw-r--r--   0        0        0     7999 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.legacy.css
--rw-r--r--   0        0        0    13839 2023-06-02 13:12:07.072999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.legacy.css.map
--rw-r--r--   0        0        0     6785 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.legacy.min.css
--rw-r--r--   0        0        0    13520 2023-06-02 13:12:07.072999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.legacy.min.css.map
--rw-r--r--   0        0        0    11542 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.main.css
--rw-r--r--   0        0        0    20284 2023-06-02 13:12:07.073999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.main.css.map
--rw-r--r--   0        0        0    10312 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.main.min.css
--rw-r--r--   0        0        0    19374 2023-06-02 13:12:07.073999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.main.min.css.map
--rw-r--r--   0        0        0    16869 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.min.css
--rw-r--r--   0        0        0    30683 2023-06-02 13:12:07.073999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.min.css.map
--rw-r--r--   0        0        0      776 2023-06-02 13:12:07.173000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/README.md
--rw-r--r--   0        0        0     5250 2023-06-02 13:12:06.523999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.css
--rw-r--r--   0        0        0    14634 2023-06-02 13:12:07.073999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.css.map
--rw-r--r--   0        0        0     2350 2023-06-02 13:12:06.523999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.legacy.css
--rw-r--r--   0        0        0     6968 2023-06-02 13:12:07.073999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.legacy.css.map
--rw-r--r--   0        0        0     2012 2023-06-02 13:12:06.523999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.legacy.min.css
--rw-r--r--   0        0        0     6889 2023-06-02 13:12:07.075000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.legacy.min.css.map
--rw-r--r--   0        0        0     3140 2023-06-02 13:12:06.523999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.main.css
--rw-r--r--   0        0        0     9870 2023-06-02 13:12:07.075000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.main.css.map
--rw-r--r--   0        0        0     2750 2023-06-02 13:12:06.523999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.main.min.css
--rw-r--r--   0        0        0     9251 2023-06-02 13:12:07.075000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.main.min.css.map
--rw-r--r--   0        0        0     4534 2023-06-02 13:12:06.523999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.min.css
--rw-r--r--   0        0        0    13928 2023-06-02 13:12:07.075000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.min.css.map
--rw-r--r--   0        0        0      776 2023-06-02 13:12:07.173000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/README.md
--rw-r--r--   0        0        0    61210 2023-06-02 13:12:06.525000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.css
--rw-r--r--   0        0        0    83686 2023-06-02 13:12:07.075999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.css.map
--rw-r--r--   0        0        0    24507 2023-06-02 13:12:06.525000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.legacy.css
--rw-r--r--   0        0        0    33766 2023-06-02 13:12:07.075999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.legacy.css.map
--rw-r--r--   0        0        0    20773 2023-06-02 13:12:06.525000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.legacy.min.css
--rw-r--r--   0        0        0    32754 2023-06-02 13:12:07.075999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.legacy.min.css.map
--rw-r--r--   0        0        0    36943 2023-06-02 13:12:06.525000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.main.css
--rw-r--r--   0        0        0    51783 2023-06-02 13:12:07.075999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.main.css.map
--rw-r--r--   0        0        0    33240 2023-06-02 13:12:06.525000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.main.min.css
--rw-r--r--   0        0        0    50018 2023-06-02 13:12:07.076999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.main.min.css.map
--rw-r--r--   0        0        0    53785 2023-06-02 13:12:06.525000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.min.css
--rw-r--r--   0        0        0    80902 2023-06-02 13:12:07.076999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.min.css.map
--rw-r--r--   0        0        0      764 2023-06-02 13:12:07.173000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/README.md
--rw-r--r--   0        0        0    10694 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.css
--rw-r--r--   0        0        0    21349 2023-06-02 13:12:07.076999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.css.map
--rw-r--r--   0        0        0     4602 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.legacy.css
--rw-r--r--   0        0        0     9729 2023-06-02 13:12:07.078000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.legacy.css.map
--rw-r--r--   0        0        0     3920 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.legacy.min.css
--rw-r--r--   0        0        0     9556 2023-06-02 13:12:07.078000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.legacy.min.css.map
--rw-r--r--   0        0        0     6332 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.main.css
--rw-r--r--   0        0        0    13822 2023-06-02 13:12:07.078000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.main.css.map
--rw-r--r--   0        0        0     5622 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.main.min.css
--rw-r--r--   0        0        0    13097 2023-06-02 13:12:07.078000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.main.min.css.map
--rw-r--r--   0        0        0     9314 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.min.css
--rw-r--r--   0        0        0    20443 2023-06-02 13:12:07.078999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.min.css.map
--rw-r--r--   0        0        0      782 2023-06-02 13:12:07.173000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/README.md
--rw-r--r--   0        0        0     3858 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.css
--rw-r--r--   0        0        0    13024 2023-06-02 13:12:07.078999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.css.map
--rw-r--r--   0        0        0     1726 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.legacy.css
--rw-r--r--   0        0        0     6315 2023-06-02 13:12:07.078999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.legacy.css.map
--rw-r--r--   0        0        0     1484 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.legacy.min.css
--rw-r--r--   0        0        0     6262 2023-06-02 13:12:07.078999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.legacy.min.css.map
--rw-r--r--   0        0        0     2372 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.main.css
--rw-r--r--   0        0        0     8914 2023-06-02 13:12:07.078999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.main.css.map
--rw-r--r--   0        0        0     2062 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.main.min.css
--rw-r--r--   0        0        0     8320 2023-06-02 13:12:07.079999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.main.min.css.map
--rw-r--r--   0        0        0     3318 2023-06-02 13:12:06.526999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.min.css
--rw-r--r--   0        0        0    12369 2023-06-02 13:12:07.079999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.min.css.map
--rw-r--r--   0        0        0   252525 2023-06-02 13:12:06.528000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.css
--rw-r--r--   0        0        0   338301 2023-06-02 13:12:07.081000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.css.map
--rw-r--r--   0        0        0   103243 2023-06-02 13:12:06.528000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.legacy.css
--rw-r--r--   0        0        0   134266 2023-06-02 13:12:07.081000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.legacy.css.map
--rw-r--r--   0        0        0    87075 2023-06-02 13:12:06.528000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.legacy.min.css
--rw-r--r--   0        0        0   129807 2023-06-02 13:12:07.082000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.legacy.min.css.map
--rw-r--r--   0        0        0   149522 2023-06-02 13:12:06.529000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.main.css
--rw-r--r--   0        0        0   204422 2023-06-02 13:12:07.082999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.main.css.map
--rw-r--r--   0        0        0   133091 2023-06-02 13:12:06.529000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.main.min.css
--rw-r--r--   0        0        0   190288 2023-06-02 13:12:07.082999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.main.min.css.map
--rw-r--r--   0        0        0   219938 2023-06-02 13:12:06.529999 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.min.css
--rw-r--r--   0        0        0   318184 2023-06-02 13:12:07.084000 mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.min.css.map
--rw-r--r--   0        0        0      583 2023-07-03 13:34:12.938063 mkdocs_dsfr-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      891 1970-01-01 00:00:00.000000 mkdocs_dsfr-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-05-31 09:02:27.963069 mkdocs_dsfr-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2532 2023-07-04 15:14:45.683720 mkdocs_dsfr-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 09:02:27.964132 mkdocs_dsfr-0.4.0/dsfr/__init__.py
+-rw-r--r--   0        0        0    16409 2023-06-02 13:12:07.563999 mkdocs_dsfr-0.4.0/dsfr/artwork/background/ovoid.svg
+-rw-r--r--   0        0        0     3884 2023-06-02 13:12:07.437000 mkdocs_dsfr-0.4.0/dsfr/artwork/dark.svg
+-rw-r--r--   0        0        0     4750 2023-06-02 13:12:07.526999 mkdocs_dsfr-0.4.0/dsfr/artwork/light.svg
+-rw-r--r--   0        0        0     5712 2023-06-02 13:12:07.420000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/buildings/city-hall.svg
+-rw-r--r--   0        0        0     6612 2023-06-02 13:12:07.459000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/buildings/factory.svg
+-rw-r--r--   0        0        0     3564 2023-06-02 13:12:07.516000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/buildings/house.svg
+-rw-r--r--   0        0        0    10932 2023-06-02 13:12:07.562999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/buildings/nuclear-plant.svg
+-rw-r--r--   0        0        0     5534 2023-06-02 13:12:07.595999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/buildings/school.svg
+-rw-r--r--   0        0        0     5409 2023-06-02 13:12:07.378999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/digital/application.svg
+-rw-r--r--   0        0        0     4327 2023-06-02 13:12:07.390000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/digital/avatar.svg
+-rw-r--r--   0        0        0     4158 2023-06-02 13:12:07.407999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/digital/calendar.svg
+-rw-r--r--   0        0        0     4015 2023-06-02 13:12:07.426000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/digital/coding.svg
+-rw-r--r--   0        0        0     5502 2023-06-02 13:12:07.437999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/digital/data-visualization.svg
+-rw-r--r--   0        0        0     7230 2023-06-02 13:12:07.523999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/digital/internet.svg
+-rw-r--r--   0        0        0     3993 2023-06-02 13:12:07.542000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/digital/mail-send.svg
+-rw-r--r--   0        0        0     3191 2023-06-02 13:12:07.596999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/digital/search.svg
+-rw-r--r--   0        0        0     4823 2023-06-02 13:12:07.430000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/document/contract.svg
+-rw-r--r--   0        0        0     2599 2023-06-02 13:12:07.443000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/document/document-add.svg
+-rw-r--r--   0        0        0     3905 2023-06-02 13:12:07.444000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/document/document-download.svg
+-rw-r--r--   0        0        0     3201 2023-06-02 13:12:07.444000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/document/document-signature.svg
+-rw-r--r--   0        0        0     2453 2023-06-02 13:12:07.444000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/document/document.svg
+-rw-r--r--   0        0        0     4716 2023-06-02 13:12:07.448999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/document/driving-licence.svg
+-rw-r--r--   0        0        0     4210 2023-06-02 13:12:07.559000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/document/national-identity-card.svg
+-rw-r--r--   0        0        0     3572 2023-06-02 13:12:07.569999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/document/passport.svg
+-rw-r--r--   0        0        0    10659 2023-06-02 13:12:07.625999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/document/tax-stamp.svg
+-rw-r--r--   0        0        0     5360 2023-06-02 13:12:07.650000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/document/vehicle-registration.svg
+-rw-r--r--   0        0        0     8630 2023-06-02 13:12:07.453999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/environment/environment.svg
+-rw-r--r--   0        0        0     5177 2023-06-02 13:12:07.471999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/environment/food.svg
+-rw-r--r--   0        0        0     6131 2023-06-02 13:12:07.503000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/environment/grocery.svg
+-rw-r--r--   0        0        0    10973 2023-06-02 13:12:07.516999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/environment/human-cooperation.svg
+-rw-r--r--   0        0        0     5704 2023-06-02 13:12:07.526999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/environment/leaf.svg
+-rw-r--r--   0        0        0     2809 2023-06-02 13:12:07.555999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/environment/moon.svg
+-rw-r--r--   0        0        0     4263 2023-06-02 13:12:07.558000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/environment/mountain.svg
+-rw-r--r--   0        0        0     3555 2023-06-02 13:12:07.618999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/environment/sun.svg
+-rw-r--r--   0        0        0     6161 2023-06-02 13:12:07.638000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/environment/tree.svg
+-rw-r--r--   0        0        0     7177 2023-06-02 13:12:07.512000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/health/health.svg
+-rw-r--r--   0        0        0     3577 2023-06-02 13:12:07.515000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/health/hospital.svg
+-rw-r--r--   0        0        0     7720 2023-06-02 13:12:07.648999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/health/vaccine.svg
+-rw-r--r--   0        0        0     8264 2023-06-02 13:12:07.653000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/health/virus.svg
+-rw-r--r--   0        0        0     8682 2023-06-02 13:12:07.467000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/institutions/firefighter.svg
+-rw-r--r--   0        0        0     5880 2023-06-02 13:12:07.484999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/institutions/gendarmerie.svg
+-rw-r--r--   0        0        0     4778 2023-06-02 13:12:07.525000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/institutions/justice.svg
+-rw-r--r--   0        0        0    16555 2023-06-02 13:12:07.553999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/institutions/money.svg
+-rw-r--r--   0        0        0     8621 2023-06-02 13:12:07.578999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/institutions/police.svg
+-rw-r--r--   0        0        0     7856 2023-06-02 13:12:07.398000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/leisure/book.svg
+-rw-r--r--   0        0        0     4138 2023-06-02 13:12:07.427000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/leisure/community.svg
+-rw-r--r--   0        0        0     6782 2023-06-02 13:12:07.434000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/leisure/culture.svg
+-rw-r--r--   0        0        0     4973 2023-06-02 13:12:07.440999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/leisure/digital-art.svg
+-rw-r--r--   0        0        0     6890 2023-06-02 13:12:07.565999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/leisure/paint.svg
+-rw-r--r--   0        0        0     6799 2023-06-02 13:12:07.371999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/map/airport.svg
+-rw-r--r--   0        0        0    15123 2023-06-02 13:12:07.533999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/map/location-france.svg
+-rw-r--r--   0        0        0     4427 2023-06-02 13:12:07.538000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/map/luggage.svg
+-rw-r--r--   0        0        0     7293 2023-06-02 13:12:07.543999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/map/map.svg
+-rw-r--r--   0        0        0     2791 2023-06-02 13:12:07.430000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/system/connection-lost.svg
+-rw-r--r--   0        0        0     2098 2023-06-02 13:12:07.456000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/system/error.svg
+-rw-r--r--   0        0        0     3506 2023-06-02 13:12:07.520999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/system/information.svg
+-rw-r--r--   0        0        0     4103 2023-06-02 13:12:07.561000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/system/notification.svg
+-rw-r--r--   0        0        0     2592 2023-06-02 13:12:07.565000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/system/padlock.svg
+-rw-r--r--   0        0        0     1985 2023-06-02 13:12:07.615999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/system/success.svg
+-rw-r--r--   0        0        0    15162 2023-06-02 13:12:07.621999 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/system/system.svg
+-rw-r--r--   0        0        0     4442 2023-06-02 13:12:07.628000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/system/technical-error.svg
+-rw-r--r--   0        0        0     1577 2023-06-02 13:12:07.657000 mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/system/warning.svg
+-rw-r--r--   0        0        0    15015 2023-06-02 13:12:07.621999 mkdocs_dsfr-0.4.0/dsfr/artwork/system.svg
+-rw-r--r--   0        0        0    10383 2023-07-03 13:25:56.386252 mkdocs_dsfr-0.4.0/dsfr/base.html
+-rw-r--r--   0        0        0     5366 2023-05-31 09:02:27.964627 mkdocs_dsfr-0.4.0/dsfr/css/theme.css
+-rw-r--r--   0        0        0   137003 2023-07-04 15:15:30.610871 mkdocs_dsfr-0.4.0/dsfr/dsfr.min.css
+-rw-r--r--   0        0        0    68681 2023-06-02 13:12:06.859999 mkdocs_dsfr-0.4.0/dsfr/dsfr.module.min.js
+-rw-r--r--   0        0        0   218391 2023-06-02 13:12:06.865000 mkdocs_dsfr-0.4.0/dsfr/dsfr.nomodule.min.js
+-rw-r--r--   0        0        0     3631 2023-06-02 13:12:07.177000 mkdocs_dsfr-0.4.0/dsfr/favicon/android-chrome-192x192.png
+-rw-r--r--   0        0        0     9190 2023-06-02 13:12:07.177000 mkdocs_dsfr-0.4.0/dsfr/favicon/android-chrome-512x512.png
+-rw-r--r--   0        0        0     3448 2023-06-02 13:12:07.177999 mkdocs_dsfr-0.4.0/dsfr/favicon/apple-touch-icon.png
+-rw-r--r--   0        0        0     7406 2023-06-02 13:12:06.809999 mkdocs_dsfr-0.4.0/dsfr/favicon/favicon.ico
+-rw-r--r--   0        0        0     6360 2023-06-02 13:12:07.460000 mkdocs_dsfr-0.4.0/dsfr/favicon/favicon.svg
+-rw-r--r--   0        0        0      292 2023-06-02 13:12:07.661999 mkdocs_dsfr-0.4.0/dsfr/favicon/manifest.webmanifest
+-rwxr-xr-x   0        0        0    52216 2023-06-02 13:12:07.664000 mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Bold.woff
+-rwxr-xr-x   0        0        0    42092 2023-06-02 13:12:07.674999 mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Bold.woff2
+-rwxr-xr-x   0        0        0    56436 2023-06-02 13:12:07.661999 mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Bold_Italic.woff
+-rwxr-xr-x   0        0        0    45300 2023-06-02 13:12:07.674000 mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Bold_Italic.woff2
+-rwxr-xr-x   0        0        0    50440 2023-06-02 13:12:07.665999 mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Light.woff
+-rwxr-xr-x   0        0        0    41368 2023-06-02 13:12:07.677000 mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Light.woff2
+-rwxr-xr-x   0        0        0    54492 2023-06-02 13:12:07.664999 mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Light_Italic.woff
+-rwxr-xr-x   0        0        0    43916 2023-06-02 13:12:07.676000 mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Light_Italic.woff2
+-rwxr-xr-x   0        0        0    51292 2023-06-02 13:12:07.667999 mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Medium.woff
+-rwxr-xr-x   0        0        0    41940 2023-06-02 13:12:07.678999 mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Medium.woff2
+-rwxr-xr-x   0        0        0    54680 2023-06-02 13:12:07.667000 mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Medium_Italic.woff
+-rwxr-xr-x   0        0        0    44572 2023-06-02 13:12:07.677999 mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Medium_Italic.woff2
+-rwxr-xr-x   0        0        0    51140 2023-06-02 13:12:07.670000 mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Regular.woff
+-rwxr-xr-x   0        0        0    41328 2023-06-02 13:12:07.680999 mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Regular.woff2
+-rwxr-xr-x   0        0        0    54328 2023-06-02 13:12:07.668999 mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Regular_Italic.woff
+-rwxr-xr-x   0        0        0    44284 2023-06-02 13:12:07.680000 mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Regular_Italic.woff2
+-rw-r--r--   0        0        0   114508 2023-06-02 13:12:07.671000 mkdocs_dsfr-0.4.0/dsfr/fonts/Spectral-ExtraBold.woff
+-rw-r--r--   0        0        0    80368 2023-06-02 13:12:07.681999 mkdocs_dsfr-0.4.0/dsfr/fonts/Spectral-ExtraBold.woff2
+-rw-r--r--   0        0        0   114016 2023-06-02 13:12:07.673000 mkdocs_dsfr-0.4.0/dsfr/fonts/Spectral-Regular.woff
+-rw-r--r--   0        0        0    79472 2023-06-02 13:12:07.684000 mkdocs_dsfr-0.4.0/dsfr/fonts/Spectral-Regular.woff2
+-rw-r--r--   0        0        0     2531 2023-07-04 15:12:54.172701 mkdocs_dsfr-0.4.0/dsfr/footer.html
+-rw-r--r--   0        0        0     2235 2023-07-04 15:12:54.173271 mkdocs_dsfr-0.4.0/dsfr/header.html
+-rw-r--r--   0        0        0      397 2023-06-02 13:12:07.378000 mkdocs_dsfr-0.4.0/dsfr/icons/buildings/ancient-gate-fill.svg
+-rw-r--r--   0        0        0      789 2023-06-02 13:12:07.378000 mkdocs_dsfr-0.4.0/dsfr/icons/buildings/ancient-gate-line.svg
+-rw-r--r--   0        0        0      280 2023-06-02 13:12:07.378000 mkdocs_dsfr-0.4.0/dsfr/icons/buildings/ancient-pavilion-fill.svg
+-rw-r--r--   0        0        0      416 2023-06-02 13:12:07.378999 mkdocs_dsfr-0.4.0/dsfr/icons/buildings/ancient-pavilion-line.svg
+-rw-r--r--   0        0        0      232 2023-06-02 13:12:07.392999 mkdocs_dsfr-0.4.0/dsfr/icons/buildings/bank-fill.svg
+-rw-r--r--   0        0        0      262 2023-06-02 13:12:07.392999 mkdocs_dsfr-0.4.0/dsfr/icons/buildings/bank-line.svg
+-rw-r--r--   0        0        0      204 2023-06-02 13:12:07.403000 mkdocs_dsfr-0.4.0/dsfr/icons/buildings/building-fill.svg
+-rw-r--r--   0        0        0      225 2023-06-02 13:12:07.404000 mkdocs_dsfr-0.4.0/dsfr/icons/buildings/building-line.svg
+-rw-r--r--   0        0        0      316 2023-06-02 13:12:07.427000 mkdocs_dsfr-0.4.0/dsfr/icons/buildings/community-fill.svg
+-rw-r--r--   0        0        0      388 2023-06-02 13:12:07.427000 mkdocs_dsfr-0.4.0/dsfr/icons/buildings/community-line.svg
+-rw-r--r--   0        0        0      232 2023-06-02 13:12:07.502000 mkdocs_dsfr-0.4.0/dsfr/icons/buildings/government-fill.svg
+-rw-r--r--   0        0        0      227 2023-06-02 13:12:07.502000 mkdocs_dsfr-0.4.0/dsfr/icons/buildings/government-line.svg
+-rw-r--r--   0        0        0      209 2023-06-02 13:12:07.513999 mkdocs_dsfr-0.4.0/dsfr/icons/buildings/home-4-fill.svg
+-rw-r--r--   0        0        0      239 2023-06-02 13:12:07.513999 mkdocs_dsfr-0.4.0/dsfr/icons/buildings/home-4-line.svg
+-rw-r--r--   0        0        0      212 2023-06-02 13:12:07.515000 mkdocs_dsfr-0.4.0/dsfr/icons/buildings/hospital-fill.svg
+-rw-r--r--   0        0        0      228 2023-06-02 13:12:07.515000 mkdocs_dsfr-0.4.0/dsfr/icons/buildings/hospital-line.svg
+-rw-r--r--   0        0        0      224 2023-06-02 13:12:07.516000 mkdocs_dsfr-0.4.0/dsfr/icons/buildings/hotel-fill.svg
+-rw-r--r--   0        0        0      243 2023-06-02 13:12:07.516000 mkdocs_dsfr-0.4.0/dsfr/icons/buildings/hotel-line.svg
+-rw-r--r--   0        0        0      437 2023-06-02 13:12:07.615000 mkdocs_dsfr-0.4.0/dsfr/icons/buildings/store-fill.svg
+-rw-r--r--   0        0        0      546 2023-06-02 13:12:07.615000 mkdocs_dsfr-0.4.0/dsfr/icons/buildings/store-line.svg
+-rw-r--r--   0        0        0      254 2023-06-02 13:12:07.380000 mkdocs_dsfr-0.4.0/dsfr/icons/business/archive-fill.svg
+-rw-r--r--   0        0        0      288 2023-06-02 13:12:07.380000 mkdocs_dsfr-0.4.0/dsfr/icons/business/archive-line.svg
+-rw-r--r--   0        0        0      330 2023-06-02 13:12:07.390000 mkdocs_dsfr-0.4.0/dsfr/icons/business/attachment-fill.svg
+-rw-r--r--   0        0        0      241 2023-06-02 13:12:07.390000 mkdocs_dsfr-0.4.0/dsfr/icons/business/attachment-line.svg
+-rw-r--r--   0        0        0      289 2023-06-02 13:12:07.391000 mkdocs_dsfr-0.4.0/dsfr/icons/business/award-fill.svg
+-rw-r--r--   0        0        0      338 2023-06-02 13:12:07.391000 mkdocs_dsfr-0.4.0/dsfr/icons/business/award-line.svg
+-rw-r--r--   0        0        0      218 2023-06-02 13:12:07.394000 mkdocs_dsfr-0.4.0/dsfr/icons/business/bar-chart-box-fill.svg
+-rw-r--r--   0        0        0      234 2023-06-02 13:12:07.394000 mkdocs_dsfr-0.4.0/dsfr/icons/business/bar-chart-box-line.svg
+-rw-r--r--   0        0        0      208 2023-06-02 13:12:07.398999 mkdocs_dsfr-0.4.0/dsfr/icons/business/bookmark-fill.svg
+-rw-r--r--   0        0        0      242 2023-06-02 13:12:07.398999 mkdocs_dsfr-0.4.0/dsfr/icons/business/bookmark-line.svg
+-rw-r--r--   0        0        0      253 2023-06-02 13:12:07.400000 mkdocs_dsfr-0.4.0/dsfr/icons/business/briefcase-fill.svg
+-rw-r--r--   0        0        0      267 2023-06-02 13:12:07.400000 mkdocs_dsfr-0.4.0/dsfr/icons/business/briefcase-line.svg
+-rw-r--r--   0        0        0      248 2023-06-02 13:12:07.404999 mkdocs_dsfr-0.4.0/dsfr/icons/business/calendar-2-fill.svg
+-rw-r--r--   0        0        0      281 2023-06-02 13:12:07.405999 mkdocs_dsfr-0.4.0/dsfr/icons/business/calendar-2-line.svg
+-rw-r--r--   0        0        0      218 2023-06-02 13:12:07.405999 mkdocs_dsfr-0.4.0/dsfr/icons/business/calendar-event-fill.svg
+-rw-r--r--   0        0        0      251 2023-06-02 13:12:07.405999 mkdocs_dsfr-0.4.0/dsfr/icons/business/calendar-event-line.svg
+-rw-r--r--   0        0        0      203 2023-06-02 13:12:07.407000 mkdocs_dsfr-0.4.0/dsfr/icons/business/calendar-fill.svg
+-rw-r--r--   0        0        0      244 2023-06-02 13:12:07.407999 mkdocs_dsfr-0.4.0/dsfr/icons/business/calendar-line.svg
+-rw-r--r--   0        0        0      254 2023-06-02 13:12:07.423000 mkdocs_dsfr-0.4.0/dsfr/icons/business/cloud-fill.svg
+-rw-r--r--   0        0        0      356 2023-06-02 13:12:07.423000 mkdocs_dsfr-0.4.0/dsfr/icons/business/cloud-line.svg
+-rw-r--r--   0        0        0      290 2023-06-02 13:12:07.431999 mkdocs_dsfr-0.4.0/dsfr/icons/business/copyright-fill.svg
+-rw-r--r--   0        0        0      346 2023-06-02 13:12:07.431999 mkdocs_dsfr-0.4.0/dsfr/icons/business/copyright-line.svg
+-rw-r--r--   0        0        0      341 2023-06-02 13:12:07.436000 mkdocs_dsfr-0.4.0/dsfr/icons/business/customer-service-fill.svg
+-rw-r--r--   0        0        0      375 2023-06-02 13:12:07.436000 mkdocs_dsfr-0.4.0/dsfr/icons/business/customer-service-line.svg
+-rw-r--r--   0        0        0      210 2023-06-02 13:12:07.469000 mkdocs_dsfr-0.4.0/dsfr/icons/business/flag-fill.svg
+-rw-r--r--   0        0        0      255 2023-06-02 13:12:07.469000 mkdocs_dsfr-0.4.0/dsfr/icons/business/flag-line.svg
+-rw-r--r--   0        0        0      540 2023-06-02 13:12:07.499000 mkdocs_dsfr-0.4.0/dsfr/icons/business/global-fill.svg
+-rw-r--r--   0        0        0      607 2023-06-02 13:12:07.500000 mkdocs_dsfr-0.4.0/dsfr/icons/business/global-line.svg
+-rw-r--r--   0        0        0      200 2023-06-02 13:12:07.529000 mkdocs_dsfr-0.4.0/dsfr/icons/business/line-chart-fill.svg
+-rw-r--r--   0        0        0      218 2023-06-02 13:12:07.529000 mkdocs_dsfr-0.4.0/dsfr/icons/business/line-chart-line.svg
+-rw-r--r--   0        0        0      409 2023-06-02 13:12:07.530999 mkdocs_dsfr-0.4.0/dsfr/icons/business/links-fill.svg
+-rw-r--r--   0        0        0      418 2023-06-02 13:12:07.532000 mkdocs_dsfr-0.4.0/dsfr/icons/business/links-line.svg
+-rw-r--r--   0        0        0      260 2023-06-02 13:12:07.539999 mkdocs_dsfr-0.4.0/dsfr/icons/business/mail-fill.svg
+-rw-r--r--   0        0        0      247 2023-06-02 13:12:07.540999 mkdocs_dsfr-0.4.0/dsfr/icons/business/mail-line.svg
+-rw-r--r--   0        0        0      318 2023-06-02 13:12:07.540999 mkdocs_dsfr-0.4.0/dsfr/icons/business/mail-open-fill.svg
+-rw-r--r--   0        0        0      359 2023-06-02 13:12:07.540999 mkdocs_dsfr-0.4.0/dsfr/icons/business/mail-open-line.svg
+-rw-r--r--   0        0        0      355 2023-06-02 13:12:07.546999 mkdocs_dsfr-0.4.0/dsfr/icons/business/medal-fill.svg
+-rw-r--r--   0        0        0      389 2023-06-02 13:12:07.546999 mkdocs_dsfr-0.4.0/dsfr/icons/business/medal-line.svg
+-rw-r--r--   0        0        0      248 2023-06-02 13:12:07.573999 mkdocs_dsfr-0.4.0/dsfr/icons/business/pie-chart-2-fill.svg
+-rw-r--r--   0        0        0      378 2023-06-02 13:12:07.575000 mkdocs_dsfr-0.4.0/dsfr/icons/business/pie-chart-2-line.svg
+-rw-r--r--   0        0        0      273 2023-06-02 13:12:07.575000 mkdocs_dsfr-0.4.0/dsfr/icons/business/pie-chart-box-fill.svg
+-rw-r--r--   0        0        0      289 2023-06-02 13:12:07.575000 mkdocs_dsfr-0.4.0/dsfr/icons/business/pie-chart-box-line.svg
+-rw-r--r--   0        0        0      256 2023-06-02 13:12:07.579999 mkdocs_dsfr-0.4.0/dsfr/icons/business/printer-fill.svg
+-rw-r--r--   0        0        0      341 2023-06-02 13:12:07.579999 mkdocs_dsfr-0.4.0/dsfr/icons/business/printer-line.svg
+-rw-r--r--   0        0        0      296 2023-06-02 13:12:07.581000 mkdocs_dsfr-0.4.0/dsfr/icons/business/profil-fill.svg
+-rw-r--r--   0        0        0      312 2023-06-02 13:12:07.581000 mkdocs_dsfr-0.4.0/dsfr/icons/business/profil-line.svg
+-rw-r--r--   0        0        0      356 2023-06-02 13:12:07.581000 mkdocs_dsfr-0.4.0/dsfr/icons/business/projector-2-fill.svg
+-rw-r--r--   0        0        0      350 2023-06-02 13:12:07.582000 mkdocs_dsfr-0.4.0/dsfr/icons/business/projector-2-line.svg
+-rw-r--r--   0        0        0      248 2023-06-02 13:12:07.598999 mkdocs_dsfr-0.4.0/dsfr/icons/business/send-plane-fill.svg
+-rw-r--r--   0        0        0      301 2023-06-02 13:12:07.599999 mkdocs_dsfr-0.4.0/dsfr/icons/business/send-plane-line.svg
+-rw-r--r--   0        0        0      226 2023-06-02 13:12:07.608000 mkdocs_dsfr-0.4.0/dsfr/icons/business/slideshow-fill.svg
+-rw-r--r--   0        0        0      241 2023-06-02 13:12:07.608000 mkdocs_dsfr-0.4.0/dsfr/icons/business/slideshow-line.svg
+-rw-r--r--   0        0        0      215 2023-06-02 13:12:07.657999 mkdocs_dsfr-0.4.0/dsfr/icons/business/window-fill.svg
+-rw-r--r--   0        0        0      230 2023-06-02 13:12:07.658999 mkdocs_dsfr-0.4.0/dsfr/icons/business/window-line.svg
+-rw-r--r--   0        0        0      199 2023-06-02 13:12:07.413000 mkdocs_dsfr-0.4.0/dsfr/icons/communication/chat-2-fill.svg
+-rw-r--r--   0        0        0      237 2023-06-02 13:12:07.414000 mkdocs_dsfr-0.4.0/dsfr/icons/communication/chat-2-line.svg
+-rw-r--r--   0        0        0      236 2023-06-02 13:12:07.414000 mkdocs_dsfr-0.4.0/dsfr/icons/communication/chat-3-fill.svg
+-rw-r--r--   0        0        0      360 2023-06-02 13:12:07.414000 mkdocs_dsfr-0.4.0/dsfr/icons/communication/chat-3-line.svg
+-rw-r--r--   0        0        0      256 2023-06-02 13:12:07.414999 mkdocs_dsfr-0.4.0/dsfr/icons/communication/chat-check-fill.svg
+-rw-r--r--   0        0        0      283 2023-06-02 13:12:07.414999 mkdocs_dsfr-0.4.0/dsfr/icons/communication/chat-check-line.svg
+-rw-r--r--   0        0        0      321 2023-06-02 13:12:07.414999 mkdocs_dsfr-0.4.0/dsfr/icons/communication/chat-delete-fill.svg
+-rw-r--r--   0        0        0      348 2023-06-02 13:12:07.415999 mkdocs_dsfr-0.4.0/dsfr/icons/communication/chat-delete-line.svg
+-rw-r--r--   0        0        0      243 2023-06-02 13:12:07.415999 mkdocs_dsfr-0.4.0/dsfr/icons/communication/chat-poll-fill.svg
+-rw-r--r--   0        0        0      214 2023-06-02 13:12:07.415999 mkdocs_dsfr-0.4.0/dsfr/icons/communication/chat-poll-line.svg
+-rw-r--r--   0        0        0      236 2023-06-02 13:12:07.441999 mkdocs_dsfr-0.4.0/dsfr/icons/communication/discuss-fill.svg
+-rw-r--r--   0        0        0      282 2023-06-02 13:12:07.441999 mkdocs_dsfr-0.4.0/dsfr/icons/communication/discuss-line.svg
+-rw-r--r--   0        0        0      201 2023-06-02 13:12:07.460000 mkdocs_dsfr-0.4.0/dsfr/icons/communication/feedback-fill.svg
+-rw-r--r--   0        0        0      229 2023-06-02 13:12:07.460000 mkdocs_dsfr-0.4.0/dsfr/icons/communication/feedback-line.svg
+-rw-r--r--   0        0        0      215 2023-06-02 13:12:07.549999 mkdocs_dsfr-0.4.0/dsfr/icons/communication/message-2-fill.svg
+-rw-r--r--   0        0        0      245 2023-06-02 13:12:07.551000 mkdocs_dsfr-0.4.0/dsfr/icons/communication/message-2-line.svg
+-rw-r--r--   0        0        0      231 2023-06-02 13:12:07.584000 mkdocs_dsfr-0.4.0/dsfr/icons/communication/question-answer-fill.svg
+-rw-r--r--   0        0        0      260 2023-06-02 13:12:07.585000 mkdocs_dsfr-0.4.0/dsfr/icons/communication/question-answer-line.svg
+-rw-r--r--   0        0        0      263 2023-06-02 13:12:07.585999 mkdocs_dsfr-0.4.0/dsfr/icons/communication/questionnaire-fill.svg
+-rw-r--r--   0        0        0      327 2023-06-02 13:12:07.585999 mkdocs_dsfr-0.4.0/dsfr/icons/communication/questionnaire-line.svg
+-rw-r--r--   0        0        0      206 2023-06-02 13:12:07.651000 mkdocs_dsfr-0.4.0/dsfr/icons/communication/video-chat-fill.svg
+-rw-r--r--   0        0        0      234 2023-06-02 13:12:07.651000 mkdocs_dsfr-0.4.0/dsfr/icons/communication/video-chat-line.svg
+-rw-r--r--   0        0        0      318 2023-06-02 13:12:07.391000 mkdocs_dsfr-0.4.0/dsfr/icons/design/ball-pen-fill.svg
+-rw-r--r--   0        0        0      372 2023-06-02 13:12:07.391999 mkdocs_dsfr-0.4.0/dsfr/icons/design/ball-pen-line.svg
+-rw-r--r--   0        0        0      252 2023-06-02 13:12:07.401000 mkdocs_dsfr-0.4.0/dsfr/icons/design/brush-3-fill.svg
+-rw-r--r--   0        0        0      266 2023-06-02 13:12:07.401000 mkdocs_dsfr-0.4.0/dsfr/icons/design/brush-3-line.svg
+-rw-r--r--   0        0        0      449 2023-06-02 13:12:07.401999 mkdocs_dsfr-0.4.0/dsfr/icons/design/brush-fill.svg
+-rw-r--r--   0        0        0      689 2023-06-02 13:12:07.401999 mkdocs_dsfr-0.4.0/dsfr/icons/design/brush-line.svg
+-rw-r--r--   0        0        0      195 2023-06-02 13:12:07.430999 mkdocs_dsfr-0.4.0/dsfr/icons/design/contrast-fill.svg
+-rw-r--r--   0        0        0      230 2023-06-02 13:12:07.430999 mkdocs_dsfr-0.4.0/dsfr/icons/design/contrast-line.svg
+-rw-r--r--   0        0        0      173 2023-06-02 13:12:07.431999 mkdocs_dsfr-0.4.0/dsfr/icons/design/crop-fill.svg
+-rw-r--r--   0        0        0      184 2023-06-02 13:12:07.433000 mkdocs_dsfr-0.4.0/dsfr/icons/design/crop-line.svg
+-rw-r--r--   0        0        0      399 2023-06-02 13:12:07.447000 mkdocs_dsfr-0.4.0/dsfr/icons/design/drag-move-2-fill.svg
+-rw-r--r--   0        0        0      178 2023-06-02 13:12:07.447000 mkdocs_dsfr-0.4.0/dsfr/icons/design/drag-move-2-line.svg
+-rw-r--r--   0        0        0      153 2023-06-02 13:12:07.448999 mkdocs_dsfr-0.4.0/dsfr/icons/design/drop-fill.svg
+-rw-r--r--   0        0        0      190 2023-06-02 13:12:07.448999 mkdocs_dsfr-0.4.0/dsfr/icons/design/drop-line.svg
+-rw-r--r--   0        0        0      275 2023-06-02 13:12:07.451999 mkdocs_dsfr-0.4.0/dsfr/icons/design/edit-box-fill.svg
+-rw-r--r--   0        0        0      255 2023-06-02 13:12:07.451999 mkdocs_dsfr-0.4.0/dsfr/icons/design/edit-box-line.svg
+-rw-r--r--   0        0        0      206 2023-06-02 13:12:07.453000 mkdocs_dsfr-0.4.0/dsfr/icons/design/edit-fill.svg
+-rw-r--r--   0        0        0      258 2023-06-02 13:12:07.453000 mkdocs_dsfr-0.4.0/dsfr/icons/design/edit-line.svg
+-rw-r--r--   0        0        0      266 2023-06-02 13:12:07.522000 mkdocs_dsfr-0.4.0/dsfr/icons/design/ink-bottle-fill.svg
+-rw-r--r--   0        0        0      323 2023-06-02 13:12:07.522000 mkdocs_dsfr-0.4.0/dsfr/icons/design/ink-bottle-line.svg
+-rw-r--r--   0        0        0      241 2023-06-02 13:12:07.525000 mkdocs_dsfr-0.4.0/dsfr/icons/design/layout-grid-fill.svg
+-rw-r--r--   0        0        0      232 2023-06-02 13:12:07.526000 mkdocs_dsfr-0.4.0/dsfr/icons/design/layout-grid-line.svg
+-rw-r--r--   0        0        0      401 2023-06-02 13:12:07.545000 mkdocs_dsfr-0.4.0/dsfr/icons/design/mark-pen-fill.svg
+-rw-r--r--   0        0        0      503 2023-06-02 13:12:07.546000 mkdocs_dsfr-0.4.0/dsfr/icons/design/mark-pen-line.svg
+-rw-r--r--   0        0        0      292 2023-06-02 13:12:07.565000 mkdocs_dsfr-0.4.0/dsfr/icons/design/paint-brush-fill.svg
+-rw-r--r--   0        0        0      305 2023-06-02 13:12:07.565000 mkdocs_dsfr-0.4.0/dsfr/icons/design/paint-brush-line.svg
+-rw-r--r--   0        0        0      339 2023-06-02 13:12:07.565999 mkdocs_dsfr-0.4.0/dsfr/icons/design/paint-fill.svg
+-rw-r--r--   0        0        0      362 2023-06-02 13:12:07.565999 mkdocs_dsfr-0.4.0/dsfr/icons/design/paint-line.svg
+-rw-r--r--   0        0        0      437 2023-06-02 13:12:07.566999 mkdocs_dsfr-0.4.0/dsfr/icons/design/palette-fill.svg
+-rw-r--r--   0        0        0      584 2023-06-02 13:12:07.566999 mkdocs_dsfr-0.4.0/dsfr/icons/design/palette-line.svg
+-rw-r--r--   0        0        0      386 2023-06-02 13:12:07.568000 mkdocs_dsfr-0.4.0/dsfr/icons/design/pantone-fill.svg
+-rw-r--r--   0        0        0      505 2023-06-02 13:12:07.568000 mkdocs_dsfr-0.4.0/dsfr/icons/design/pantone-line.svg
+-rw-r--r--   0        0        0      389 2023-06-02 13:12:07.571000 mkdocs_dsfr-0.4.0/dsfr/icons/design/pen-nib-fill.svg
+-rw-r--r--   0        0        0      510 2023-06-02 13:12:07.572000 mkdocs_dsfr-0.4.0/dsfr/icons/design/pen-nib-line.svg
+-rw-r--r--   0        0        0      254 2023-06-02 13:12:07.572000 mkdocs_dsfr-0.4.0/dsfr/icons/design/pencil-fill.svg
+-rw-r--r--   0        0        0      310 2023-06-02 13:12:07.572999 mkdocs_dsfr-0.4.0/dsfr/icons/design/pencil-line.svg
+-rw-r--r--   0        0        0      234 2023-06-02 13:12:07.572999 mkdocs_dsfr-0.4.0/dsfr/icons/design/pencil-ruler-fill.svg
+-rw-r--r--   0        0        0      255 2023-06-02 13:12:07.572999 mkdocs_dsfr-0.4.0/dsfr/icons/design/pencil-ruler-line.svg
+-rw-r--r--   0        0        0      302 2023-06-02 13:12:07.605999 mkdocs_dsfr-0.4.0/dsfr/icons/design/sip-fill.svg
+-rw-r--r--   0        0        0      352 2023-06-02 13:12:07.607000 mkdocs_dsfr-0.4.0/dsfr/icons/design/sip-line.svg
+-rw-r--r--   0        0        0      221 2023-06-02 13:12:07.622999 mkdocs_dsfr-0.4.0/dsfr/icons/design/table-fill.svg
+-rw-r--r--   0        0        0      234 2023-06-02 13:12:07.624000 mkdocs_dsfr-0.4.0/dsfr/icons/design/table-line.svg
+-rw-r--r--   0        0        0      500 2023-06-02 13:12:07.401999 mkdocs_dsfr-0.4.0/dsfr/icons/development/bug-fill.svg
+-rw-r--r--   0        0        0      632 2023-06-02 13:12:07.403000 mkdocs_dsfr-0.4.0/dsfr/icons/development/bug-line.svg
+-rw-r--r--   0        0        0      360 2023-06-02 13:12:07.424000 mkdocs_dsfr-0.4.0/dsfr/icons/development/code-box-fill.svg
+-rw-r--r--   0        0        0      374 2023-06-02 13:12:07.424999 mkdocs_dsfr-0.4.0/dsfr/icons/development/code-box-line.svg
+-rw-r--r--   0        0        0      281 2023-06-02 13:12:07.424999 mkdocs_dsfr-0.4.0/dsfr/icons/development/code-s-slash-line.svg
+-rw-r--r--   0        0        0      197 2023-06-02 13:12:07.434999 mkdocs_dsfr-0.4.0/dsfr/icons/development/cursor-fill.svg
+-rw-r--r--   0        0        0      283 2023-06-02 13:12:07.436000 mkdocs_dsfr-0.4.0/dsfr/icons/development/cursor-line.svg
+-rw-r--r--   0        0        0      307 2023-06-02 13:12:07.490000 mkdocs_dsfr-0.4.0/dsfr/icons/development/git-branch-fill.svg
+-rw-r--r--   0        0        0      425 2023-06-02 13:12:07.490999 mkdocs_dsfr-0.4.0/dsfr/icons/development/git-branch-line.svg
+-rw-r--r--   0        0        0      187 2023-06-02 13:12:07.490999 mkdocs_dsfr-0.4.0/dsfr/icons/development/git-commit-fill.svg
+-rw-r--r--   0        0        0      250 2023-06-02 13:12:07.494999 mkdocs_dsfr-0.4.0/dsfr/icons/development/git-commit-line.svg
+-rw-r--r--   0        0        0      330 2023-06-02 13:12:07.494999 mkdocs_dsfr-0.4.0/dsfr/icons/development/git-merge-fill.svg
+-rw-r--r--   0        0        0      455 2023-06-02 13:12:07.494999 mkdocs_dsfr-0.4.0/dsfr/icons/development/git-merge-line.svg
+-rw-r--r--   0        0        0      233 2023-06-02 13:12:07.496000 mkdocs_dsfr-0.4.0/dsfr/icons/development/git-pull-request-fill.svg
+-rw-r--r--   0        0        0      356 2023-06-02 13:12:07.496000 mkdocs_dsfr-0.4.0/dsfr/icons/development/git-pull-request-line.svg
+-rw-r--r--   0        0        0      294 2023-06-02 13:12:07.496000 mkdocs_dsfr-0.4.0/dsfr/icons/development/git-repository-commits-fill.svg
+-rw-r--r--   0        0        0      320 2023-06-02 13:12:07.496999 mkdocs_dsfr-0.4.0/dsfr/icons/development/git-repository-commits-line.svg
+-rw-r--r--   0        0        0      285 2023-06-02 13:12:07.496999 mkdocs_dsfr-0.4.0/dsfr/icons/development/git-repository-fill.svg
+-rw-r--r--   0        0        0      328 2023-06-02 13:12:07.496999 mkdocs_dsfr-0.4.0/dsfr/icons/development/git-repository-line.svg
+-rw-r--r--   0        0        0      288 2023-06-02 13:12:07.497999 mkdocs_dsfr-0.4.0/dsfr/icons/development/git-repository-private-fill.svg
+-rw-r--r--   0        0        0      304 2023-06-02 13:12:07.497999 mkdocs_dsfr-0.4.0/dsfr/icons/development/git-repository-private-line.svg
+-rw-r--r--   0        0        0      260 2023-06-02 13:12:07.628999 mkdocs_dsfr-0.4.0/dsfr/icons/development/terminal-box-fill.svg
+-rw-r--r--   0        0        0      287 2023-06-02 13:12:07.628999 mkdocs_dsfr-0.4.0/dsfr/icons/development/terminal-box-line.svg
+-rw-r--r--   0        0        0      186 2023-06-02 13:12:07.630000 mkdocs_dsfr-0.4.0/dsfr/icons/development/terminal-line.svg
+-rw-r--r--   0        0        0      230 2023-06-02 13:12:07.630000 mkdocs_dsfr-0.4.0/dsfr/icons/development/terminal-window-fill.svg
+-rw-r--r--   0        0        0      245 2023-06-02 13:12:07.631000 mkdocs_dsfr-0.4.0/dsfr/icons/development/terminal-window-line.svg
+-rw-r--r--   0        0        0      343 2023-06-02 13:12:07.395999 mkdocs_dsfr-0.4.0/dsfr/icons/device/bluetooth-fill.svg
+-rw-r--r--   0        0        0      343 2023-06-02 13:12:07.395999 mkdocs_dsfr-0.4.0/dsfr/icons/device/bluetooth-line.svg
+-rw-r--r--   0        0        0      256 2023-06-02 13:12:07.428999 mkdocs_dsfr-0.4.0/dsfr/icons/device/computer-fill.svg
+-rw-r--r--   0        0        0      275 2023-06-02 13:12:07.428999 mkdocs_dsfr-0.4.0/dsfr/icons/device/computer-line.svg
+-rw-r--r--   0        0        0      514 2023-06-02 13:12:07.437000 mkdocs_dsfr-0.4.0/dsfr/icons/device/dashboard-3-fill.svg
+-rw-r--r--   0        0        0      552 2023-06-02 13:12:07.437999 mkdocs_dsfr-0.4.0/dsfr/icons/device/dashboard-3-line.svg
+-rw-r--r--   0        0        0      266 2023-06-02 13:12:07.438999 mkdocs_dsfr-0.4.0/dsfr/icons/device/database-fill.svg
+-rw-r--r--   0        0        0      296 2023-06-02 13:12:07.438999 mkdocs_dsfr-0.4.0/dsfr/icons/device/database-line.svg
+-rw-r--r--   0        0        0      250 2023-06-02 13:12:07.440000 mkdocs_dsfr-0.4.0/dsfr/icons/device/device-fill.svg
+-rw-r--r--   0        0        0      260 2023-06-02 13:12:07.440000 mkdocs_dsfr-0.4.0/dsfr/icons/device/device-line.svg
+-rw-r--r--   0        0        0      206 2023-06-02 13:12:07.509000 mkdocs_dsfr-0.4.0/dsfr/icons/device/hard-drive-2-fill.svg
+-rw-r--r--   0        0        0      222 2023-06-02 13:12:07.509000 mkdocs_dsfr-0.4.0/dsfr/icons/device/hard-drive-2-line.svg
+-rw-r--r--   0        0        0      290 2023-06-02 13:12:07.539999 mkdocs_dsfr-0.4.0/dsfr/icons/device/mac-fill.svg
+-rw-r--r--   0        0        0      288 2023-06-02 13:12:07.539999 mkdocs_dsfr-0.4.0/dsfr/icons/device/mac-line.svg
+-rw-r--r--   0        0        0      485 2023-06-02 13:12:07.573999 mkdocs_dsfr-0.4.0/dsfr/icons/device/phone-fill.svg
+-rw-r--r--   0        0        0      719 2023-06-02 13:12:07.573999 mkdocs_dsfr-0.4.0/dsfr/icons/device/phone-line.svg
+-rw-r--r--   0        0        0      272 2023-06-02 13:12:07.582999 mkdocs_dsfr-0.4.0/dsfr/icons/device/qr-code-fill.svg
+-rw-r--r--   0        0        0      315 2023-06-02 13:12:07.584000 mkdocs_dsfr-0.4.0/dsfr/icons/device/qr-code-line.svg
+-rw-r--r--   0        0        0      229 2023-06-02 13:12:07.591000 mkdocs_dsfr-0.4.0/dsfr/icons/device/rss-fill.svg
+-rw-r--r--   0        0        0      230 2023-06-02 13:12:07.592000 mkdocs_dsfr-0.4.0/dsfr/icons/device/rss-line.svg
+-rw-r--r--   0        0        0      234 2023-06-02 13:12:07.592999 mkdocs_dsfr-0.4.0/dsfr/icons/device/save-3-fill.svg
+-rw-r--r--   0        0        0      250 2023-06-02 13:12:07.594000 mkdocs_dsfr-0.4.0/dsfr/icons/device/save-3-line.svg
+-rw-r--r--   0        0        0      195 2023-06-02 13:12:07.594000 mkdocs_dsfr-0.4.0/dsfr/icons/device/save-fill.svg
+-rw-r--r--   0        0        0      219 2023-06-02 13:12:07.595000 mkdocs_dsfr-0.4.0/dsfr/icons/device/save-line.svg
+-rw-r--r--   0        0        0      219 2023-06-02 13:12:07.599999 mkdocs_dsfr-0.4.0/dsfr/icons/device/server-fill.svg
+-rw-r--r--   0        0        0      234 2023-06-02 13:12:07.601000 mkdocs_dsfr-0.4.0/dsfr/icons/device/server-line.svg
+-rw-r--r--   0        0        0      208 2023-06-02 13:12:07.608999 mkdocs_dsfr-0.4.0/dsfr/icons/device/smartphone-fill.svg
+-rw-r--r--   0        0        0      224 2023-06-02 13:12:07.608999 mkdocs_dsfr-0.4.0/dsfr/icons/device/smartphone-line.svg
+-rw-r--r--   0        0        0      208 2023-06-02 13:12:07.624000 mkdocs_dsfr-0.4.0/dsfr/icons/device/tablet-fill.svg
+-rw-r--r--   0        0        0      224 2023-06-02 13:12:07.625000 mkdocs_dsfr-0.4.0/dsfr/icons/device/tablet-line.svg
+-rw-r--r--   0        0        0      285 2023-06-02 13:12:07.638999 mkdocs_dsfr-0.4.0/dsfr/icons/device/tv-fill.svg
+-rw-r--r--   0        0        0      304 2023-06-02 13:12:07.640000 mkdocs_dsfr-0.4.0/dsfr/icons/device/tv-line.svg
+-rw-r--r--   0        0        0      618 2023-06-02 13:12:07.657000 mkdocs_dsfr-0.4.0/dsfr/icons/device/wifi-fill.svg
+-rw-r--r--   0        0        0      630 2023-06-02 13:12:07.657999 mkdocs_dsfr-0.4.0/dsfr/icons/device/wifi-line.svg
+-rw-r--r--   0        0        0      233 2023-06-02 13:12:07.388000 mkdocs_dsfr-0.4.0/dsfr/icons/document/article-fill.svg
+-rw-r--r--   0        0        0      249 2023-06-02 13:12:07.388999 mkdocs_dsfr-0.4.0/dsfr/icons/document/article-line.svg
+-rw-r--r--   0        0        0      181 2023-06-02 13:12:07.397000 mkdocs_dsfr-0.4.0/dsfr/icons/document/book-2-fill.svg
+-rw-r--r--   0        0        0      227 2023-06-02 13:12:07.397000 mkdocs_dsfr-0.4.0/dsfr/icons/document/book-2-line.svg
+-rw-r--r--   0        0        0      226 2023-06-02 13:12:07.398000 mkdocs_dsfr-0.4.0/dsfr/icons/document/booklet-fill.svg
+-rw-r--r--   0        0        0      242 2023-06-02 13:12:07.398999 mkdocs_dsfr-0.4.0/dsfr/icons/document/booklet-line.svg
+-rw-r--r--   0        0        0      250 2023-06-02 13:12:07.421000 mkdocs_dsfr-0.4.0/dsfr/icons/document/clipboard-fill.svg
+-rw-r--r--   0        0        0      274 2023-06-02 13:12:07.421000 mkdocs_dsfr-0.4.0/dsfr/icons/document/clipboard-line.svg
+-rw-r--r--   0        0        0      317 2023-06-02 13:12:07.446000 mkdocs_dsfr-0.4.0/dsfr/icons/document/draft-fill.svg
+-rw-r--r--   0        0        0      303 2023-06-02 13:12:07.447000 mkdocs_dsfr-0.4.0/dsfr/icons/document/draft-line.svg
+-rw-r--r--   0        0        0      234 2023-06-02 13:12:07.460999 mkdocs_dsfr-0.4.0/dsfr/icons/document/file-add-fill.svg
+-rw-r--r--   0        0        0      251 2023-06-02 13:12:07.460999 mkdocs_dsfr-0.4.0/dsfr/icons/document/file-add-line.svg
+-rw-r--r--   0        0        0      227 2023-06-02 13:12:07.460999 mkdocs_dsfr-0.4.0/dsfr/icons/document/file-download-fill.svg
+-rw-r--r--   0        0        0      245 2023-06-02 13:12:07.461999 mkdocs_dsfr-0.4.0/dsfr/icons/document/file-download-line.svg
+-rw-r--r--   0        0        0      230 2023-06-02 13:12:07.461999 mkdocs_dsfr-0.4.0/dsfr/icons/document/file-fill.svg
+-rw-r--r--   0        0        0      225 2023-06-02 13:12:07.463000 mkdocs_dsfr-0.4.0/dsfr/icons/document/file-line.svg
+-rw-r--r--   0        0        0      255 2023-06-02 13:12:07.463000 mkdocs_dsfr-0.4.0/dsfr/icons/document/file-pdf-fill.svg
+-rw-r--r--   0        0        0      273 2023-06-02 13:12:07.463000 mkdocs_dsfr-0.4.0/dsfr/icons/document/file-pdf-line.svg
+-rw-r--r--   0        0        0      281 2023-06-02 13:12:07.463999 mkdocs_dsfr-0.4.0/dsfr/icons/document/file-text-fill.svg
+-rw-r--r--   0        0        0      272 2023-06-02 13:12:07.463999 mkdocs_dsfr-0.4.0/dsfr/icons/document/file-text-line.svg
+-rw-r--r--   0        0        0      198 2023-06-02 13:12:07.470000 mkdocs_dsfr-0.4.0/dsfr/icons/document/folder-2-fill.svg
+-rw-r--r--   0        0        0      234 2023-06-02 13:12:07.470999 mkdocs_dsfr-0.4.0/dsfr/icons/document/folder-2-line.svg
+-rw-r--r--   0        0        0      262 2023-06-02 13:12:07.559999 mkdocs_dsfr-0.4.0/dsfr/icons/document/newspaper-fill.svg
+-rw-r--r--   0        0        0      290 2023-06-02 13:12:07.559999 mkdocs_dsfr-0.4.0/dsfr/icons/document/newspaper-line.svg
+-rw-r--r--   0        0        0      292 2023-06-02 13:12:07.619999 mkdocs_dsfr-0.4.0/dsfr/icons/document/survey-fill.svg
+-rw-r--r--   0        0        0      317 2023-06-02 13:12:07.619999 mkdocs_dsfr-0.4.0/dsfr/icons/document/survey-line.svg
+-rw-r--r--   0        0        0      217 2023-06-02 13:12:07.635999 mkdocs_dsfr-0.4.0/dsfr/icons/document/todo-fill.svg
+-rw-r--r--   0        0        0      250 2023-06-02 13:12:07.635999 mkdocs_dsfr-0.4.0/dsfr/icons/document/todo-line.svg
+-rw-r--r--   0        0        0      250 2023-06-02 13:12:07.426000 mkdocs_dsfr-0.4.0/dsfr/icons/editor/code-view.svg
+-rw-r--r--   0        0        0      250 2023-06-02 13:12:07.470999 mkdocs_dsfr-0.4.0/dsfr/icons/editor/font-size.svg
+-rw-r--r--   0        0        0      314 2023-06-02 13:12:07.473999 mkdocs_dsfr-0.4.0/dsfr/icons/editor/fr--bold.svg
+-rw-r--r--   0        0        0      160 2023-06-02 13:12:07.476000 mkdocs_dsfr-0.4.0/dsfr/icons/editor/fr--highlight.svg
+-rw-r--r--   0        0        0      278 2023-06-02 13:12:07.477999 mkdocs_dsfr-0.4.0/dsfr/icons/editor/fr--quote-fill.svg
+-rw-r--r--   0        0        0      344 2023-06-02 13:12:07.477999 mkdocs_dsfr-0.4.0/dsfr/icons/editor/fr--quote-line.svg
+-rw-r--r--   0        0        0      223 2023-06-02 13:12:07.505000 mkdocs_dsfr-0.4.0/dsfr/icons/editor/h-1.svg
+-rw-r--r--   0        0        0      387 2023-06-02 13:12:07.505000 mkdocs_dsfr-0.4.0/dsfr/icons/editor/h-2.svg
+-rw-r--r--   0        0        0      542 2023-06-02 13:12:07.505000 mkdocs_dsfr-0.4.0/dsfr/icons/editor/h-3.svg
+-rw-r--r--   0        0        0      268 2023-06-02 13:12:07.506000 mkdocs_dsfr-0.4.0/dsfr/icons/editor/h-4.svg
+-rw-r--r--   0        0        0      393 2023-06-02 13:12:07.506999 mkdocs_dsfr-0.4.0/dsfr/icons/editor/h-5.svg
+-rw-r--r--   0        0        0      538 2023-06-02 13:12:07.506999 mkdocs_dsfr-0.4.0/dsfr/icons/editor/h-6.svg
+-rw-r--r--   0        0        0      298 2023-06-02 13:12:07.509000 mkdocs_dsfr-0.4.0/dsfr/icons/editor/hashtag.svg
+-rw-r--r--   0        0        0      158 2023-06-02 13:12:07.525000 mkdocs_dsfr-0.4.0/dsfr/icons/editor/italic.svg
+-rw-r--r--   0        0        0      468 2023-06-02 13:12:07.529999 mkdocs_dsfr-0.4.0/dsfr/icons/editor/link-unlink.svg
+-rw-r--r--   0        0        0      408 2023-06-02 13:12:07.529999 mkdocs_dsfr-0.4.0/dsfr/icons/editor/link.svg
+-rw-r--r--   0        0        0      246 2023-06-02 13:12:07.532000 mkdocs_dsfr-0.4.0/dsfr/icons/editor/list-ordered.svg
+-rw-r--r--   0        0        0      275 2023-06-02 13:12:07.532999 mkdocs_dsfr-0.4.0/dsfr/icons/editor/list-unordered.svg
+-rw-r--r--   0        0        0      341 2023-06-02 13:12:07.585999 mkdocs_dsfr-0.4.0/dsfr/icons/editor/question-mark.svg
+-rw-r--r--   0        0        0      147 2023-06-02 13:12:07.599999 mkdocs_dsfr-0.4.0/dsfr/icons/editor/separator.svg
+-rw-r--r--   0        0        0      151 2023-06-02 13:12:07.611000 mkdocs_dsfr-0.4.0/dsfr/icons/editor/space.svg
+-rw-r--r--   0        0        0      317 2023-06-02 13:12:07.615999 mkdocs_dsfr-0.4.0/dsfr/icons/editor/subscript.svg
+-rw-r--r--   0        0        0      315 2023-06-02 13:12:07.618999 mkdocs_dsfr-0.4.0/dsfr/icons/editor/superscript.svg
+-rw-r--r--   0        0        0      263 2023-06-02 13:12:07.622999 mkdocs_dsfr-0.4.0/dsfr/icons/editor/table-2.svg
+-rw-r--r--   0        0        0      505 2023-06-02 13:12:07.638000 mkdocs_dsfr-0.4.0/dsfr/icons/editor/translate-2.svg
+-rw-r--r--   0        0        0      206 2023-06-02 13:12:07.391999 mkdocs_dsfr-0.4.0/dsfr/icons/finance/bank-card-fill.svg
+-rw-r--r--   0        0        0      220 2023-06-02 13:12:07.392999 mkdocs_dsfr-0.4.0/dsfr/icons/finance/bank-card-line.svg
+-rw-r--r--   0        0        0      277 2023-06-02 13:12:07.426000 mkdocs_dsfr-0.4.0/dsfr/icons/finance/coin-fill.svg
+-rw-r--r--   0        0        0      393 2023-06-02 13:12:07.487999 mkdocs_dsfr-0.4.0/dsfr/icons/finance/gift-fill.svg
+-rw-r--r--   0        0        0      406 2023-06-02 13:12:07.489000 mkdocs_dsfr-0.4.0/dsfr/icons/finance/gift-line.svg
+-rw-r--r--   0        0        0      366 2023-06-02 13:12:07.552999 mkdocs_dsfr-0.4.0/dsfr/icons/finance/money-euro-box-fill.svg
+-rw-r--r--   0        0        0      344 2023-06-02 13:12:07.552999 mkdocs_dsfr-0.4.0/dsfr/icons/finance/money-euro-box-line.svg
+-rw-r--r--   0        0        0      365 2023-06-02 13:12:07.552999 mkdocs_dsfr-0.4.0/dsfr/icons/finance/money-euro-circle-fill.svg
+-rw-r--r--   0        0        0      362 2023-06-02 13:12:07.553999 mkdocs_dsfr-0.4.0/dsfr/icons/finance/money-euro-circle-line.svg
+-rw-r--r--   0        0        0      397 2023-06-02 13:12:07.598000 mkdocs_dsfr-0.4.0/dsfr/icons/finance/secure-payment-fill.svg
+-rw-r--r--   0        0        0      427 2023-06-02 13:12:07.598000 mkdocs_dsfr-0.4.0/dsfr/icons/finance/secure-payment-line.svg
+-rw-r--r--   0        0        0      348 2023-06-02 13:12:07.604000 mkdocs_dsfr-0.4.0/dsfr/icons/finance/shopping-bag-fill.svg
+-rw-r--r--   0        0        0      282 2023-06-02 13:12:07.604000 mkdocs_dsfr-0.4.0/dsfr/icons/finance/shopping-bag-line.svg
+-rw-r--r--   0        0        0      311 2023-06-02 13:12:07.605000 mkdocs_dsfr-0.4.0/dsfr/icons/finance/shopping-cart-2-fill.svg
+-rw-r--r--   0        0        0      343 2023-06-02 13:12:07.605000 mkdocs_dsfr-0.4.0/dsfr/icons/finance/shopping-cart-2-line.svg
+-rw-r--r--   0        0        0      200 2023-06-02 13:12:07.638000 mkdocs_dsfr-0.4.0/dsfr/icons/finance/trophy-fill.svg
+-rw-r--r--   0        0        0      222 2023-06-02 13:12:07.638999 mkdocs_dsfr-0.4.0/dsfr/icons/finance/trophy-line.svg
+-rw-r--r--   0        0        0      289 2023-06-02 13:12:07.410000 mkdocs_dsfr-0.4.0/dsfr/icons/health/capsule-fill.svg
+-rw-r--r--   0        0        0      379 2023-06-02 13:12:07.410000 mkdocs_dsfr-0.4.0/dsfr/icons/health/capsule-line.svg
+-rw-r--r--   0        0        0      336 2023-06-02 13:12:07.441999 mkdocs_dsfr-0.4.0/dsfr/icons/health/dislike-fill.svg
+-rw-r--r--   0        0        0      543 2023-06-02 13:12:07.443000 mkdocs_dsfr-0.4.0/dsfr/icons/health/dislike-line.svg
+-rw-r--r--   0        0        0      243 2023-06-02 13:12:07.444999 mkdocs_dsfr-0.4.0/dsfr/icons/health/dossier-fill.svg
+-rw-r--r--   0        0        0      265 2023-06-02 13:12:07.444999 mkdocs_dsfr-0.4.0/dsfr/icons/health/dossier-line.svg
+-rw-r--r--   0        0        0      269 2023-06-02 13:12:07.467999 mkdocs_dsfr-0.4.0/dsfr/icons/health/first-aid-kit-fill.svg
+-rw-r--r--   0        0        0      283 2023-06-02 13:12:07.469000 mkdocs_dsfr-0.4.0/dsfr/icons/health/first-aid-kit-line.svg
+-rw-r--r--   0        0        0      317 2023-06-02 13:12:07.507999 mkdocs_dsfr-0.4.0/dsfr/icons/health/hand-sanitizer-fill.svg
+-rw-r--r--   0        0        0      359 2023-06-02 13:12:07.507999 mkdocs_dsfr-0.4.0/dsfr/icons/health/hand-sanitizer-line.svg
+-rw-r--r--   0        0        0      258 2023-06-02 13:12:07.509999 mkdocs_dsfr-0.4.0/dsfr/icons/health/health-book-fill.svg
+-rw-r--r--   0        0        0      273 2023-06-02 13:12:07.510999 mkdocs_dsfr-0.4.0/dsfr/icons/health/health-book-line.svg
+-rw-r--r--   0        0        0      209 2023-06-02 13:12:07.512000 mkdocs_dsfr-0.4.0/dsfr/icons/health/heart-fill.svg
+-rw-r--r--   0        0        0      365 2023-06-02 13:12:07.513000 mkdocs_dsfr-0.4.0/dsfr/icons/health/heart-line.svg
+-rw-r--r--   0        0        0      331 2023-06-02 13:12:07.513000 mkdocs_dsfr-0.4.0/dsfr/icons/health/heart-pulse-fill.svg
+-rw-r--r--   0        0        0      661 2023-06-02 13:12:07.513000 mkdocs_dsfr-0.4.0/dsfr/icons/health/heart-pulse-line.svg
+-rw-r--r--   0        0        0      476 2023-06-02 13:12:07.538000 mkdocs_dsfr-0.4.0/dsfr/icons/health/lungs-fill.svg
+-rw-r--r--   0        0        0      909 2023-06-02 13:12:07.539000 mkdocs_dsfr-0.4.0/dsfr/icons/health/lungs-line.svg
+-rw-r--r--   0        0        0      241 2023-06-02 13:12:07.548000 mkdocs_dsfr-0.4.0/dsfr/icons/health/medicine-bottle-fill.svg
+-rw-r--r--   0        0        0      293 2023-06-02 13:12:07.548000 mkdocs_dsfr-0.4.0/dsfr/icons/health/medicine-bottle-line.svg
+-rw-r--r--   0        0        0      395 2023-06-02 13:12:07.548000 mkdocs_dsfr-0.4.0/dsfr/icons/health/mental-health-fill.svg
+-rw-r--r--   0        0        0      503 2023-06-02 13:12:07.549000 mkdocs_dsfr-0.4.0/dsfr/icons/health/mental-health-line.svg
+-rw-r--r--   0        0        0      519 2023-06-02 13:12:07.552000 mkdocs_dsfr-0.4.0/dsfr/icons/health/microscope-fill.svg
+-rw-r--r--   0        0        0      618 2023-06-02 13:12:07.552000 mkdocs_dsfr-0.4.0/dsfr/icons/health/microscope-line.svg
+-rw-r--r--   0        0        0      370 2023-06-02 13:12:07.582000 mkdocs_dsfr-0.4.0/dsfr/icons/health/psychotherapy-fill.svg
+-rw-r--r--   0        0        0      504 2023-06-02 13:12:07.582999 mkdocs_dsfr-0.4.0/dsfr/icons/health/psychotherapy-line.svg
+-rw-r--r--   0        0        0      181 2023-06-02 13:12:07.582999 mkdocs_dsfr-0.4.0/dsfr/icons/health/pulse-line.svg
+-rw-r--r--   0        0        0      311 2023-06-02 13:12:07.612999 mkdocs_dsfr-0.4.0/dsfr/icons/health/stethoscope-fill.svg
+-rw-r--r--   0        0        0      346 2023-06-02 13:12:07.614000 mkdocs_dsfr-0.4.0/dsfr/icons/health/stethoscope-line.svg
+-rw-r--r--   0        0        0      446 2023-06-02 13:12:07.618999 mkdocs_dsfr-0.4.0/dsfr/icons/health/surgical-mask-fill.svg
+-rw-r--r--   0        0        0      567 2023-06-02 13:12:07.619999 mkdocs_dsfr-0.4.0/dsfr/icons/health/surgical-mask-line.svg
+-rw-r--r--   0        0        0      466 2023-06-02 13:12:07.621000 mkdocs_dsfr-0.4.0/dsfr/icons/health/syringe-fill.svg
+-rw-r--r--   0        0        0      486 2023-06-02 13:12:07.621000 mkdocs_dsfr-0.4.0/dsfr/icons/health/syringe-line.svg
+-rw-r--r--   0        0        0      237 2023-06-02 13:12:07.631000 mkdocs_dsfr-0.4.0/dsfr/icons/health/test-tube-fill.svg
+-rw-r--r--   0        0        0      264 2023-06-02 13:12:07.631000 mkdocs_dsfr-0.4.0/dsfr/icons/health/test-tube-line.svg
+-rw-r--r--   0        0        0      484 2023-06-02 13:12:07.631999 mkdocs_dsfr-0.4.0/dsfr/icons/health/thermometer-fill.svg
+-rw-r--r--   0        0        0      576 2023-06-02 13:12:07.631999 mkdocs_dsfr-0.4.0/dsfr/icons/health/thermometer-line.svg
+-rw-r--r--   0        0        0     1055 2023-06-02 13:12:07.651999 mkdocs_dsfr-0.4.0/dsfr/icons/health/virus-fill.svg
+-rw-r--r--   0        0        0     1112 2023-06-02 13:12:07.653000 mkdocs_dsfr-0.4.0/dsfr/icons/health/virus-line.svg
+-rw-r--r--   0        0        0      552 2023-06-02 13:12:07.418999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/chrome-fill.svg
+-rw-r--r--   0        0        0      594 2023-06-02 13:12:07.418999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/chrome-line.svg
+-rw-r--r--   0        0        0      591 2023-06-02 13:12:07.450999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/edge-fill.svg
+-rw-r--r--   0        0        0      411 2023-06-02 13:12:07.450999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/edge-line.svg
+-rw-r--r--   0        0        0      368 2023-06-02 13:12:07.457999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/facebook-circle-fill.svg
+-rw-r--r--   0        0        0      458 2023-06-02 13:12:07.459000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/facebook-circle-line.svg
+-rw-r--r--   0        0        0      708 2023-06-02 13:12:07.467000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/firefox-fill.svg
+-rw-r--r--   0        0        0     1003 2023-06-02 13:12:07.467999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/firefox-line.svg
+-rw-r--r--   0        0        0      685 2023-06-02 13:12:07.474999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/fr--dailymotion-fill.svg
+-rw-r--r--   0        0        0      806 2023-06-02 13:12:07.474999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/fr--dailymotion-line.svg
+-rw-r--r--   0        0        0      561 2023-06-02 13:12:07.480000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/fr--tiktok-fill.svg
+-rw-r--r--   0        0        0      428 2023-06-02 13:12:07.480000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/fr--tiktok-line.svg
+-rw-r--r--   0        0        0      790 2023-06-02 13:12:07.497999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/github-fill.svg
+-rw-r--r--   0        0        0     1485 2023-06-02 13:12:07.499000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/github-line.svg
+-rw-r--r--   0        0        0      530 2023-06-02 13:12:07.500999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/google-fill.svg
+-rw-r--r--   0        0        0      371 2023-06-02 13:12:07.500999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/google-line.svg
+-rw-r--r--   0        0        0      965 2023-06-02 13:12:07.516999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/ie-fill.svg
+-rw-r--r--   0        0        0      796 2023-06-02 13:12:07.517999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/ie-line.svg
+-rw-r--r--   0        0        0      917 2023-06-02 13:12:07.523000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/instagram-fill.svg
+-rw-r--r--   0        0        0     2014 2023-06-02 13:12:07.523000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/instagram-line.svg
+-rw-r--r--   0        0        0      552 2023-06-02 13:12:07.530999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/linkedin-box-fill.svg
+-rw-r--r--   0        0        0      366 2023-06-02 13:12:07.530999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/linkedin-box-line.svg
+-rw-r--r--   0        0        0      948 2023-06-02 13:12:07.546000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/mastodon-fill.svg
+-rw-r--r--   0        0        0     1259 2023-06-02 13:12:07.546999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/mastodon-line.svg
+-rw-r--r--   0        0        0      202 2023-06-02 13:12:07.562000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/npmjs-fill.svg
+-rw-r--r--   0        0        0      220 2023-06-02 13:12:07.562000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/npmjs-line.svg
+-rw-r--r--   0        0        0      331 2023-06-02 13:12:07.588000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/remixicon-fill.svg
+-rw-r--r--   0        0        0      391 2023-06-02 13:12:07.588999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/remixicon-line.svg
+-rw-r--r--   0        0        0      972 2023-06-02 13:12:07.592000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/safari-fill.svg
+-rw-r--r--   0        0        0      574 2023-06-02 13:12:07.592000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/safari-line.svg
+-rw-r--r--   0        0        0     1133 2023-06-02 13:12:07.607000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/slack-fill.svg
+-rw-r--r--   0        0        0      514 2023-06-02 13:12:07.607000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/slack-line.svg
+-rw-r--r--   0        0        0     1494 2023-06-02 13:12:07.609999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/snapchat-fill.svg
+-rw-r--r--   0        0        0     1848 2023-06-02 13:12:07.611000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/snapchat-line.svg
+-rw-r--r--   0        0        0      398 2023-06-02 13:12:07.628000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/telegram-fill.svg
+-rw-r--r--   0        0        0      440 2023-06-02 13:12:07.628999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/telegram-line.svg
+-rw-r--r--   0        0        0      332 2023-06-02 13:12:07.640000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/twitch-fill.svg
+-rw-r--r--   0        0        0      241 2023-06-02 13:12:07.641000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/twitch-line.svg
+-rw-r--r--   0        0        0      586 2023-06-02 13:12:07.641000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/twitter-fill.svg
+-rw-r--r--   0        0        0      690 2023-06-02 13:12:07.641999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/twitter-line.svg
+-rw-r--r--   0        0        0      726 2023-06-02 13:12:07.651999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/vimeo-fill.svg
+-rw-r--r--   0        0        0     1001 2023-06-02 13:12:07.651999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/vimeo-line.svg
+-rw-r--r--   0        0        0      178 2023-06-02 13:12:07.655999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/vuejs-fill.svg
+-rw-r--r--   0        0        0      198 2023-06-02 13:12:07.657000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/vuejs-line.svg
+-rw-r--r--   0        0        0      418 2023-06-02 13:12:07.658999 mkdocs_dsfr-0.4.0/dsfr/icons/logo/youtube-fill.svg
+-rw-r--r--   0        0        0      899 2023-06-02 13:12:07.660000 mkdocs_dsfr-0.4.0/dsfr/icons/logo/youtube-line.svg
+-rw-r--r--   0        0        0      385 2023-06-02 13:12:07.377000 mkdocs_dsfr-0.4.0/dsfr/icons/map/anchor-fill.svg
+-rw-r--r--   0        0        0      350 2023-06-02 13:12:07.377000 mkdocs_dsfr-0.4.0/dsfr/icons/map/anchor-line.svg
+-rw-r--r--   0        0        0      359 2023-06-02 13:12:07.394000 mkdocs_dsfr-0.4.0/dsfr/icons/map/bike-fill.svg
+-rw-r--r--   0        0        0      359 2023-06-02 13:12:07.394999 mkdocs_dsfr-0.4.0/dsfr/icons/map/bike-line.svg
+-rw-r--r--   0        0        0      284 2023-06-02 13:12:07.404000 mkdocs_dsfr-0.4.0/dsfr/icons/map/bus-fill.svg
+-rw-r--r--   0        0        0      299 2023-06-02 13:12:07.404999 mkdocs_dsfr-0.4.0/dsfr/icons/map/bus-line.svg
+-rw-r--r--   0        0        0      372 2023-06-02 13:12:07.411000 mkdocs_dsfr-0.4.0/dsfr/icons/map/car-fill.svg
+-rw-r--r--   0        0        0      387 2023-06-02 13:12:07.411000 mkdocs_dsfr-0.4.0/dsfr/icons/map/car-line.svg
+-rw-r--r--   0        0        0      317 2023-06-02 13:12:07.411999 mkdocs_dsfr-0.4.0/dsfr/icons/map/caravan-fill.svg
+-rw-r--r--   0        0        0      383 2023-06-02 13:12:07.411999 mkdocs_dsfr-0.4.0/dsfr/icons/map/caravan-line.svg
+-rw-r--r--   0        0        0      253 2023-06-02 13:12:07.411999 mkdocs_dsfr-0.4.0/dsfr/icons/map/charging-pile-2-fill.svg
+-rw-r--r--   0        0        0      265 2023-06-02 13:12:07.413000 mkdocs_dsfr-0.4.0/dsfr/icons/map/charging-pile-2-line.svg
+-rw-r--r--   0        0        0      246 2023-06-02 13:12:07.427999 mkdocs_dsfr-0.4.0/dsfr/icons/map/compass-3-fill.svg
+-rw-r--r--   0        0        0      281 2023-06-02 13:12:07.427999 mkdocs_dsfr-0.4.0/dsfr/icons/map/compass-3-line.svg
+-rw-r--r--   0        0        0      222 2023-06-02 13:12:07.434000 mkdocs_dsfr-0.4.0/dsfr/icons/map/cup-fill.svg
+-rw-r--r--   0        0        0      264 2023-06-02 13:12:07.434999 mkdocs_dsfr-0.4.0/dsfr/icons/map/cup-line.svg
+-rw-r--r--   0        0        0      945 2023-06-02 13:12:07.450000 mkdocs_dsfr-0.4.0/dsfr/icons/map/earth-fill.svg
+-rw-r--r--   0        0        0      905 2023-06-02 13:12:07.450000 mkdocs_dsfr-0.4.0/dsfr/icons/map/earth-line.svg
+-rw-r--r--   0        0        0     2305 2023-06-02 13:12:07.480999 mkdocs_dsfr-0.4.0/dsfr/icons/map/france-fill.svg
+-rw-r--r--   0        0        0     4459 2023-06-02 13:12:07.482000 mkdocs_dsfr-0.4.0/dsfr/icons/map/france-line.svg
+-rw-r--r--   0        0        0      303 2023-06-02 13:12:07.483000 mkdocs_dsfr-0.4.0/dsfr/icons/map/gas-station-fill.svg
+-rw-r--r--   0        0        0      318 2023-06-02 13:12:07.483999 mkdocs_dsfr-0.4.0/dsfr/icons/map/gas-station-line.svg
+-rw-r--r--   0        0        0      179 2023-06-02 13:12:07.500000 mkdocs_dsfr-0.4.0/dsfr/icons/map/goblet-fill.svg
+-rw-r--r--   0        0        0      208 2023-06-02 13:12:07.500000 mkdocs_dsfr-0.4.0/dsfr/icons/map/goblet-line.svg
+-rw-r--r--   0        0        0      214 2023-06-02 13:12:07.542000 mkdocs_dsfr-0.4.0/dsfr/icons/map/map-pin-2-fill.svg
+-rw-r--r--   0        0        0      280 2023-06-02 13:12:07.542999 mkdocs_dsfr-0.4.0/dsfr/icons/map/map-pin-2-line.svg
+-rw-r--r--   0        0        0      277 2023-06-02 13:12:07.542999 mkdocs_dsfr-0.4.0/dsfr/icons/map/map-pin-user-fill.svg
+-rw-r--r--   0        0        0      363 2023-06-02 13:12:07.543999 mkdocs_dsfr-0.4.0/dsfr/icons/map/map-pin-user-line.svg
+-rw-r--r--   0        0        0      378 2023-06-02 13:12:07.556999 mkdocs_dsfr-0.4.0/dsfr/icons/map/motorbike-fill.svg
+-rw-r--r--   0        0        0      447 2023-06-02 13:12:07.558000 mkdocs_dsfr-0.4.0/dsfr/icons/map/motorbike-line.svg
+-rw-r--r--   0        0        0      256 2023-06-02 13:12:07.569000 mkdocs_dsfr-0.4.0/dsfr/icons/map/passport-fill.svg
+-rw-r--r--   0        0        0      272 2023-06-02 13:12:07.569999 mkdocs_dsfr-0.4.0/dsfr/icons/map/passport-line.svg
+-rw-r--r--   0        0        0      221 2023-06-02 13:12:07.588999 mkdocs_dsfr-0.4.0/dsfr/icons/map/restaurant-fill.svg
+-rw-r--r--   0        0        0      257 2023-06-02 13:12:07.588999 mkdocs_dsfr-0.4.0/dsfr/icons/map/restaurant-line.svg
+-rw-r--r--   0        0        0      381 2023-06-02 13:12:07.589999 mkdocs_dsfr-0.4.0/dsfr/icons/map/road-map-fill.svg
+-rw-r--r--   0        0        0      405 2023-06-02 13:12:07.591000 mkdocs_dsfr-0.4.0/dsfr/icons/map/road-map-line.svg
+-rw-r--r--   0        0        0      278 2023-06-02 13:12:07.592999 mkdocs_dsfr-0.4.0/dsfr/icons/map/sailboat-fill.svg
+-rw-r--r--   0        0        0      333 2023-06-02 13:12:07.592999 mkdocs_dsfr-0.4.0/dsfr/icons/map/sailboat-line.svg
+-rw-r--r--   0        0        0      580 2023-06-02 13:12:07.602999 mkdocs_dsfr-0.4.0/dsfr/icons/map/ship-2-fill.svg
+-rw-r--r--   0        0        0      562 2023-06-02 13:12:07.604000 mkdocs_dsfr-0.4.0/dsfr/icons/map/ship-2-line.svg
+-rw-r--r--   0        0        0      351 2023-06-02 13:12:07.605000 mkdocs_dsfr-0.4.0/dsfr/icons/map/signal-tower-fill.svg
+-rw-r--r--   0        0        0      348 2023-06-02 13:12:07.605999 mkdocs_dsfr-0.4.0/dsfr/icons/map/signal-tower-line.svg
+-rw-r--r--   0        0        0      271 2023-06-02 13:12:07.617000 mkdocs_dsfr-0.4.0/dsfr/icons/map/suitcase-2-fill.svg
+-rw-r--r--   0        0        0      286 2023-06-02 13:12:07.617000 mkdocs_dsfr-0.4.0/dsfr/icons/map/suitcase-2-line.svg
+-rw-r--r--   0        0        0      374 2023-06-02 13:12:07.625999 mkdocs_dsfr-0.4.0/dsfr/icons/map/taxi-fill.svg
+-rw-r--r--   0        0        0      386 2023-06-02 13:12:07.627000 mkdocs_dsfr-0.4.0/dsfr/icons/map/taxi-line.svg
+-rw-r--r--   0        0        0      251 2023-06-02 13:12:07.637000 mkdocs_dsfr-0.4.0/dsfr/icons/map/train-fill.svg
+-rw-r--r--   0        0        0      293 2023-06-02 13:12:07.637000 mkdocs_dsfr-0.4.0/dsfr/icons/map/train-line.svg
+-rw-r--r--   0        0        0      160 2023-06-02 13:12:07.375999 mkdocs_dsfr-0.4.0/dsfr/icons/media/align-left.svg
+-rw-r--r--   0        0        0      253 2023-06-02 13:12:07.408999 mkdocs_dsfr-0.4.0/dsfr/icons/media/camera-fill.svg
+-rw-r--r--   0        0        0      311 2023-06-02 13:12:07.408999 mkdocs_dsfr-0.4.0/dsfr/icons/media/camera-line.svg
+-rw-r--r--   0        0        0      294 2023-06-02 13:12:07.420000 mkdocs_dsfr-0.4.0/dsfr/icons/media/clapperboard-fill.svg
+-rw-r--r--   0        0        0      312 2023-06-02 13:12:07.421000 mkdocs_dsfr-0.4.0/dsfr/icons/media/clapperboard-line.svg
+-rw-r--r--   0        0        0      334 2023-06-02 13:12:07.453999 mkdocs_dsfr-0.4.0/dsfr/icons/media/equalizer-fill.svg
+-rw-r--r--   0        0        0      505 2023-06-02 13:12:07.454999 mkdocs_dsfr-0.4.0/dsfr/icons/media/equalizer-line.svg
+-rw-r--r--   0        0        0      340 2023-06-02 13:12:07.463999 mkdocs_dsfr-0.4.0/dsfr/icons/media/film-fill.svg
+-rw-r--r--   0        0        0      355 2023-06-02 13:12:07.464999 mkdocs_dsfr-0.4.0/dsfr/icons/media/film-line.svg
+-rw-r--r--   0        0        0      184 2023-06-02 13:12:07.482000 mkdocs_dsfr-0.4.0/dsfr/icons/media/fullscreen-line.svg
+-rw-r--r--   0        0        0      388 2023-06-02 13:12:07.483000 mkdocs_dsfr-0.4.0/dsfr/icons/media/gallery-fill.svg
+-rw-r--r--   0        0        0      466 2023-06-02 13:12:07.483000 mkdocs_dsfr-0.4.0/dsfr/icons/media/gallery-line.svg
+-rw-r--r--   0        0        0      261 2023-06-02 13:12:07.509999 mkdocs_dsfr-0.4.0/dsfr/icons/media/headphone-fill.svg
+-rw-r--r--   0        0        0      300 2023-06-02 13:12:07.509999 mkdocs_dsfr-0.4.0/dsfr/icons/media/headphone-line.svg
+-rw-r--r--   0        0        0      394 2023-06-02 13:12:07.517999 mkdocs_dsfr-0.4.0/dsfr/icons/media/image-add-fill.svg
+-rw-r--r--   0        0        0      316 2023-06-02 13:12:07.519000 mkdocs_dsfr-0.4.0/dsfr/icons/media/image-add-line.svg
+-rw-r--r--   0        0        0      398 2023-06-02 13:12:07.519000 mkdocs_dsfr-0.4.0/dsfr/icons/media/image-edit-fill.svg
+-rw-r--r--   0        0        0      415 2023-06-02 13:12:07.519000 mkdocs_dsfr-0.4.0/dsfr/icons/media/image-edit-line.svg
+-rw-r--r--   0        0        0      307 2023-06-02 13:12:07.519999 mkdocs_dsfr-0.4.0/dsfr/icons/media/image-fill.svg
+-rw-r--r--   0        0        0      334 2023-06-02 13:12:07.519999 mkdocs_dsfr-0.4.0/dsfr/icons/media/image-line.svg
+-rw-r--r--   0        0        0      394 2023-06-02 13:12:07.532999 mkdocs_dsfr-0.4.0/dsfr/icons/media/live-fill.svg
+-rw-r--r--   0        0        0      408 2023-06-02 13:12:07.532999 mkdocs_dsfr-0.4.0/dsfr/icons/media/live-line.svg
+-rw-r--r--   0        0        0      269 2023-06-02 13:12:07.551000 mkdocs_dsfr-0.4.0/dsfr/icons/media/mic-fill.svg
+-rw-r--r--   0        0        0      320 2023-06-02 13:12:07.551000 mkdocs_dsfr-0.4.0/dsfr/icons/media/mic-line.svg
+-rw-r--r--   0        0        0      158 2023-06-02 13:12:07.559000 mkdocs_dsfr-0.4.0/dsfr/icons/media/music-2-fill.svg
+-rw-r--r--   0        0        0      226 2023-06-02 13:12:07.559000 mkdocs_dsfr-0.4.0/dsfr/icons/media/music-2-line.svg
+-rw-r--r--   0        0        0      154 2023-06-02 13:12:07.559999 mkdocs_dsfr-0.4.0/dsfr/icons/media/notification-3-fill.svg
+-rw-r--r--   0        0        0      208 2023-06-02 13:12:07.561000 mkdocs_dsfr-0.4.0/dsfr/icons/media/notification-3-line.svg
+-rw-r--r--   0        0        0      201 2023-06-02 13:12:07.571000 mkdocs_dsfr-0.4.0/dsfr/icons/media/pause-circle-fill.svg
+-rw-r--r--   0        0        0      236 2023-06-02 13:12:07.571000 mkdocs_dsfr-0.4.0/dsfr/icons/media/pause-circle-line.svg
+-rw-r--r--   0        0        0      281 2023-06-02 13:12:07.578000 mkdocs_dsfr-0.4.0/dsfr/icons/media/play-circle-fill.svg
+-rw-r--r--   0        0        0      313 2023-06-02 13:12:07.578000 mkdocs_dsfr-0.4.0/dsfr/icons/media/play-circle-line.svg
+-rw-r--r--   0        0        0      186 2023-06-02 13:12:07.614000 mkdocs_dsfr-0.4.0/dsfr/icons/media/stop-circle-fill.svg
+-rw-r--r--   0        0        0      221 2023-06-02 13:12:07.614000 mkdocs_dsfr-0.4.0/dsfr/icons/media/stop-circle-line.svg
+-rw-r--r--   0        0        0      403 2023-06-02 13:12:07.654000 mkdocs_dsfr-0.4.0/dsfr/icons/media/volume-down-fill.svg
+-rw-r--r--   0        0        0      489 2023-06-02 13:12:07.654000 mkdocs_dsfr-0.4.0/dsfr/icons/media/volume-down-line.svg
+-rw-r--r--   0        0        0      407 2023-06-02 13:12:07.654999 mkdocs_dsfr-0.4.0/dsfr/icons/media/volume-mute-fill.svg
+-rw-r--r--   0        0        0      490 2023-06-02 13:12:07.654999 mkdocs_dsfr-0.4.0/dsfr/icons/media/volume-mute-line.svg
+-rw-r--r--   0        0        0      551 2023-06-02 13:12:07.654999 mkdocs_dsfr-0.4.0/dsfr/icons/media/volume-up-fill.svg
+-rw-r--r--   0        0        0      630 2023-06-02 13:12:07.655999 mkdocs_dsfr-0.4.0/dsfr/icons/media/volume-up-line.svg
+-rw-r--r--   0        0        0      334 2023-06-02 13:12:07.526000 mkdocs_dsfr-0.4.0/dsfr/icons/others/leaf-fill.svg
+-rw-r--r--   0        0        0      467 2023-06-02 13:12:07.526999 mkdocs_dsfr-0.4.0/dsfr/icons/others/leaf-line.svg
+-rw-r--r--   0        0        0      253 2023-06-02 13:12:07.528000 mkdocs_dsfr-0.4.0/dsfr/icons/others/lightbulb-fill.svg
+-rw-r--r--   0        0        0      406 2023-06-02 13:12:07.528000 mkdocs_dsfr-0.4.0/dsfr/icons/others/lightbulb-line.svg
+-rw-r--r--   0        0        0      277 2023-06-02 13:12:07.575999 mkdocs_dsfr-0.4.0/dsfr/icons/others/plant-fill.svg
+-rw-r--r--   0        0        0      362 2023-06-02 13:12:07.576999 mkdocs_dsfr-0.4.0/dsfr/icons/others/plant-line.svg
+-rw-r--r--   0        0        0      573 2023-06-02 13:12:07.586999 mkdocs_dsfr-0.4.0/dsfr/icons/others/recycle-fill.svg
+-rw-r--r--   0        0        0      558 2023-06-02 13:12:07.586999 mkdocs_dsfr-0.4.0/dsfr/icons/others/recycle-line.svg
+-rw-r--r--   0        0        0      454 2023-06-02 13:12:07.595000 mkdocs_dsfr-0.4.0/dsfr/icons/others/scales-3-fill.svg
+-rw-r--r--   0        0        0      552 2023-06-02 13:12:07.595999 mkdocs_dsfr-0.4.0/dsfr/icons/others/scales-3-line.svg
+-rw-r--r--   0        0        0      258 2023-06-02 13:12:07.598000 mkdocs_dsfr-0.4.0/dsfr/icons/others/seedling-fill.svg
+-rw-r--r--   0        0        0      326 2023-06-02 13:12:07.598999 mkdocs_dsfr-0.4.0/dsfr/icons/others/seedling-line.svg
+-rw-r--r--   0        0        0      232 2023-06-02 13:12:07.641999 mkdocs_dsfr-0.4.0/dsfr/icons/others/umbrella-fill.svg
+-rw-r--r--   0        0        0      315 2023-06-02 13:12:07.641999 mkdocs_dsfr-0.4.0/dsfr/icons/others/umbrella-line.svg
+-rw-r--r--   0        0        0      209 2023-06-02 13:12:07.369999 mkdocs_dsfr-0.4.0/dsfr/icons/system/add-circle-fill.svg
+-rw-r--r--   0        0        0      260 2023-06-02 13:12:07.371000 mkdocs_dsfr-0.4.0/dsfr/icons/system/add-circle-line.svg
+-rw-r--r--   0        0        0      136 2023-06-02 13:12:07.371000 mkdocs_dsfr-0.4.0/dsfr/icons/system/add-line.svg
+-rw-r--r--   0        0        0      319 2023-06-02 13:12:07.372999 mkdocs_dsfr-0.4.0/dsfr/icons/system/alarm-warning-fill.svg
+-rw-r--r--   0        0        0      360 2023-06-02 13:12:07.374000 mkdocs_dsfr-0.4.0/dsfr/icons/system/alarm-warning-line.svg
+-rw-r--r--   0        0        0      224 2023-06-02 13:12:07.374000 mkdocs_dsfr-0.4.0/dsfr/icons/system/alert-fill.svg
+-rw-r--r--   0        0        0      257 2023-06-02 13:12:07.375000 mkdocs_dsfr-0.4.0/dsfr/icons/system/alert-line.svg
+-rw-r--r--   0        0        0      127 2023-06-02 13:12:07.380000 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-down-fill.svg
+-rw-r--r--   0        0        0      188 2023-06-02 13:12:07.381000 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-down-line.svg
+-rw-r--r--   0        0        0      120 2023-06-02 13:12:07.381000 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-down-s-fill.svg
+-rw-r--r--   0        0        0      173 2023-06-02 13:12:07.381000 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-down-s-line.svg
+-rw-r--r--   0        0        0      159 2023-06-02 13:12:07.381999 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-go-back-fill.svg
+-rw-r--r--   0        0        0      213 2023-06-02 13:12:07.382999 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-go-back-line.svg
+-rw-r--r--   0        0        0      161 2023-06-02 13:12:07.382999 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-go-forward-fill.svg
+-rw-r--r--   0        0        0      218 2023-06-02 13:12:07.382999 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-go-forward-line.svg
+-rw-r--r--   0        0        0      128 2023-06-02 13:12:07.382999 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-left-fill.svg
+-rw-r--r--   0        0        0      184 2023-06-02 13:12:07.384000 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-left-line.svg
+-rw-r--r--   0        0        0      119 2023-06-02 13:12:07.384000 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-left-s-fill.svg
+-rw-r--r--   0        0        0      173 2023-06-02 13:12:07.384999 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-left-s-line.svg
+-rw-r--r--   0        0        0      128 2023-06-02 13:12:07.384999 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-right-fill.svg
+-rw-r--r--   0        0        0      189 2023-06-02 13:12:07.384999 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-right-line.svg
+-rw-r--r--   0        0        0      118 2023-06-02 13:12:07.385999 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-right-s-fill.svg
+-rw-r--r--   0        0        0      175 2023-06-02 13:12:07.385999 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-right-s-line.svg
+-rw-r--r--   0        0        0      197 2023-06-02 13:12:07.385999 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-right-up-line.svg
+-rw-r--r--   0        0        0      129 2023-06-02 13:12:07.387000 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-up-fill.svg
+-rw-r--r--   0        0        0      186 2023-06-02 13:12:07.387000 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-up-line.svg
+-rw-r--r--   0        0        0      117 2023-06-02 13:12:07.387000 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-up-s-fill.svg
+-rw-r--r--   0        0        0      173 2023-06-02 13:12:07.388000 mkdocs_dsfr-0.4.0/dsfr/icons/system/arrow-up-s-line.svg
+-rw-r--r--   0        0        0      177 2023-06-02 13:12:07.417000 mkdocs_dsfr-0.4.0/dsfr/icons/system/check-line.svg
+-rw-r--r--   0        0        0      252 2023-06-02 13:12:07.417000 mkdocs_dsfr-0.4.0/dsfr/icons/system/checkbox-circle-fill.svg
+-rw-r--r--   0        0        0      288 2023-06-02 13:12:07.417999 mkdocs_dsfr-0.4.0/dsfr/icons/system/checkbox-circle-line.svg
+-rw-r--r--   0        0        0      252 2023-06-02 13:12:07.417999 mkdocs_dsfr-0.4.0/dsfr/icons/system/checkbox-fill.svg
+-rw-r--r--   0        0        0      288 2023-06-02 13:12:07.417999 mkdocs_dsfr-0.4.0/dsfr/icons/system/checkbox-line.svg
+-rw-r--r--   0        0        0      321 2023-06-02 13:12:07.421999 mkdocs_dsfr-0.4.0/dsfr/icons/system/close-circle-fill.svg
+-rw-r--r--   0        0        0      342 2023-06-02 13:12:07.421999 mkdocs_dsfr-0.4.0/dsfr/icons/system/close-circle-line.svg
+-rw-r--r--   0        0        0      210 2023-06-02 13:12:07.421999 mkdocs_dsfr-0.4.0/dsfr/icons/system/close-line.svg
+-rw-r--r--   0        0        0      189 2023-06-02 13:12:07.438999 mkdocs_dsfr-0.4.0/dsfr/icons/system/delete-bin-fill.svg
+-rw-r--r--   0        0        0      203 2023-06-02 13:12:07.440000 mkdocs_dsfr-0.4.0/dsfr/icons/system/delete-bin-line.svg
+-rw-r--r--   0        0        0      142 2023-06-02 13:12:07.446000 mkdocs_dsfr-0.4.0/dsfr/icons/system/download-fill.svg
+-rw-r--r--   0        0        0      198 2023-06-02 13:12:07.446000 mkdocs_dsfr-0.4.0/dsfr/icons/system/download-line.svg
+-rw-r--r--   0        0        0      203 2023-06-02 13:12:07.454999 mkdocs_dsfr-0.4.0/dsfr/icons/system/error-warning-fill.svg
+-rw-r--r--   0        0        0      238 2023-06-02 13:12:07.454999 mkdocs_dsfr-0.4.0/dsfr/icons/system/error-warning-line.svg
+-rw-r--r--   0        0        0      228 2023-06-02 13:12:07.456000 mkdocs_dsfr-0.4.0/dsfr/icons/system/external-link-fill.svg
+-rw-r--r--   0        0        0      230 2023-06-02 13:12:07.456000 mkdocs_dsfr-0.4.0/dsfr/icons/system/external-link-line.svg
+-rw-r--r--   0        0        0      281 2023-06-02 13:12:07.457000 mkdocs_dsfr-0.4.0/dsfr/icons/system/eye-fill.svg
+-rw-r--r--   0        0        0      380 2023-06-02 13:12:07.457000 mkdocs_dsfr-0.4.0/dsfr/icons/system/eye-line.svg
+-rw-r--r--   0        0        0      481 2023-06-02 13:12:07.457000 mkdocs_dsfr-0.4.0/dsfr/icons/system/eye-off-fill.svg
+-rw-r--r--   0        0        0      678 2023-06-02 13:12:07.457999 mkdocs_dsfr-0.4.0/dsfr/icons/system/eye-off-line.svg
+-rw-r--r--   0        0        0      136 2023-06-02 13:12:07.464999 mkdocs_dsfr-0.4.0/dsfr/icons/system/filter-fill.svg
+-rw-r--r--   0        0        0      187 2023-06-02 13:12:07.466000 mkdocs_dsfr-0.4.0/dsfr/icons/system/filter-line.svg
+-rw-r--r--   0        0        0      196 2023-06-02 13:12:07.471999 mkdocs_dsfr-0.4.0/dsfr/icons/system/fr--arrow-left-s-first-line.svg
+-rw-r--r--   0        0        0      197 2023-06-02 13:12:07.471999 mkdocs_dsfr-0.4.0/dsfr/icons/system/fr--arrow-left-s-line-double.svg
+-rw-r--r--   0        0        0      377 2023-06-02 13:12:07.473000 mkdocs_dsfr-0.4.0/dsfr/icons/system/fr--arrow-right-down-circle-fill.svg
+-rw-r--r--   0        0        0      201 2023-06-02 13:12:07.473000 mkdocs_dsfr-0.4.0/dsfr/icons/system/fr--arrow-right-s-last-line.svg
+-rw-r--r--   0        0        0      201 2023-06-02 13:12:07.473000 mkdocs_dsfr-0.4.0/dsfr/icons/system/fr--arrow-right-s-line-double.svg
+-rw-r--r--   0        0        0      377 2023-06-02 13:12:07.473999 mkdocs_dsfr-0.4.0/dsfr/icons/system/fr--arrow-right-up-circle-fill.svg
+-rw-r--r--   0        0        0      327 2023-06-02 13:12:07.473999 mkdocs_dsfr-0.4.0/dsfr/icons/system/fr--capslock-line.svg
+-rw-r--r--   0        0        0      329 2023-06-02 13:12:07.474999 mkdocs_dsfr-0.4.0/dsfr/icons/system/fr--equal-circle-fill.svg
+-rw-r--r--   0        0        0      260 2023-06-02 13:12:07.476000 mkdocs_dsfr-0.4.0/dsfr/icons/system/fr--error-fill.svg
+-rw-r--r--   0        0        0      309 2023-06-02 13:12:07.476000 mkdocs_dsfr-0.4.0/dsfr/icons/system/fr--error-line.svg
+-rw-r--r--   0        0        0      237 2023-06-02 13:12:07.476999 mkdocs_dsfr-0.4.0/dsfr/icons/system/fr--info-fill.svg
+-rw-r--r--   0        0        0      328 2023-06-02 13:12:07.476999 mkdocs_dsfr-0.4.0/dsfr/icons/system/fr--info-line.svg
+-rw-r--r--   0        0        0      253 2023-06-02 13:12:07.477999 mkdocs_dsfr-0.4.0/dsfr/icons/system/fr--success-fill.svg
+-rw-r--r--   0        0        0      289 2023-06-02 13:12:07.479000 mkdocs_dsfr-0.4.0/dsfr/icons/system/fr--success-line.svg
+-rw-r--r--   0        0        0      482 2023-06-02 13:12:07.479000 mkdocs_dsfr-0.4.0/dsfr/icons/system/fr--theme-fill.svg
+-rw-r--r--   0        0        0      225 2023-06-02 13:12:07.480999 mkdocs_dsfr-0.4.0/dsfr/icons/system/fr--warning-fill.svg
+-rw-r--r--   0        0        0      258 2023-06-02 13:12:07.480999 mkdocs_dsfr-0.4.0/dsfr/icons/system/fr--warning-line.svg
+-rw-r--r--   0        0        0      205 2023-06-02 13:12:07.520999 mkdocs_dsfr-0.4.0/dsfr/icons/system/information-fill.svg
+-rw-r--r--   0        0        0      239 2023-06-02 13:12:07.520999 mkdocs_dsfr-0.4.0/dsfr/icons/system/information-line.svg
+-rw-r--r--   0        0        0      238 2023-06-02 13:12:07.535000 mkdocs_dsfr-0.4.0/dsfr/icons/system/lock-fill.svg
+-rw-r--r--   0        0        0      252 2023-06-02 13:12:07.535000 mkdocs_dsfr-0.4.0/dsfr/icons/system/lock-line.svg
+-rw-r--r--   0        0        0      252 2023-06-02 13:12:07.536000 mkdocs_dsfr-0.4.0/dsfr/icons/system/lock-unlock-fill.svg
+-rw-r--r--   0        0        0      268 2023-06-02 13:12:07.536000 mkdocs_dsfr-0.4.0/dsfr/icons/system/lock-unlock-line.svg
+-rw-r--r--   0        0        0      197 2023-06-02 13:12:07.536999 mkdocs_dsfr-0.4.0/dsfr/icons/system/logout-box-r-fill.svg
+-rw-r--r--   0        0        0      219 2023-06-02 13:12:07.538000 mkdocs_dsfr-0.4.0/dsfr/icons/system/logout-box-r-line.svg
+-rw-r--r--   0        0        0      145 2023-06-02 13:12:07.549000 mkdocs_dsfr-0.4.0/dsfr/icons/system/menu-2-fill.svg
+-rw-r--r--   0        0        0      145 2023-06-02 13:12:07.549999 mkdocs_dsfr-0.4.0/dsfr/icons/system/menu-fill.svg
+-rw-r--r--   0        0        0      248 2023-06-02 13:12:07.555999 mkdocs_dsfr-0.4.0/dsfr/icons/system/more-fill.svg
+-rw-r--r--   0        0        0      348 2023-06-02 13:12:07.555999 mkdocs_dsfr-0.4.0/dsfr/icons/system/more-line.svg
+-rw-r--r--   0        0        0      220 2023-06-02 13:12:07.561000 mkdocs_dsfr-0.4.0/dsfr/icons/system/notification-badge-fill.svg
+-rw-r--r--   0        0        0      288 2023-06-02 13:12:07.561000 mkdocs_dsfr-0.4.0/dsfr/icons/system/notification-badge-line.svg
+-rw-r--r--   0        0        0      311 2023-06-02 13:12:07.585000 mkdocs_dsfr-0.4.0/dsfr/icons/system/question-fill.svg
+-rw-r--r--   0        0        0      325 2023-06-02 13:12:07.585000 mkdocs_dsfr-0.4.0/dsfr/icons/system/question-line.svg
+-rw-r--r--   0        0        0      280 2023-06-02 13:12:07.586999 mkdocs_dsfr-0.4.0/dsfr/icons/system/refresh-fill.svg
+-rw-r--r--   0        0        0      244 2023-06-02 13:12:07.588000 mkdocs_dsfr-0.4.0/dsfr/icons/system/refresh-line.svg
+-rw-r--r--   0        0        0      247 2023-06-02 13:12:07.596999 mkdocs_dsfr-0.4.0/dsfr/icons/system/search-fill.svg
+-rw-r--r--   0        0        0      382 2023-06-02 13:12:07.596999 mkdocs_dsfr-0.4.0/dsfr/icons/system/search-line.svg
+-rw-r--r--   0        0        0      864 2023-06-02 13:12:07.601000 mkdocs_dsfr-0.4.0/dsfr/icons/system/settings-5-fill.svg
+-rw-r--r--   0        0        0     1599 2023-06-02 13:12:07.601999 mkdocs_dsfr-0.4.0/dsfr/icons/system/settings-5-line.svg
+-rw-r--r--   0        0        0      241 2023-06-02 13:12:07.601999 mkdocs_dsfr-0.4.0/dsfr/icons/system/shield-fill.svg
+-rw-r--r--   0        0        0      332 2023-06-02 13:12:07.601999 mkdocs_dsfr-0.4.0/dsfr/icons/system/shield-line.svg
+-rw-r--r--   0        0        0      217 2023-06-02 13:12:07.611999 mkdocs_dsfr-0.4.0/dsfr/icons/system/star-fill.svg
+-rw-r--r--   0        0        0      333 2023-06-02 13:12:07.611999 mkdocs_dsfr-0.4.0/dsfr/icons/system/star-line.svg
+-rw-r--r--   0        0        0      203 2023-06-02 13:12:07.611999 mkdocs_dsfr-0.4.0/dsfr/icons/system/star-s-fill.svg
+-rw-r--r--   0        0        0      325 2023-06-02 13:12:07.612999 mkdocs_dsfr-0.4.0/dsfr/icons/system/star-s-line.svg
+-rw-r--r--   0        0        0      117 2023-06-02 13:12:07.615999 mkdocs_dsfr-0.4.0/dsfr/icons/system/subtract-line.svg
+-rw-r--r--   0        0        0      341 2023-06-02 13:12:07.631999 mkdocs_dsfr-0.4.0/dsfr/icons/system/thumb-down-fill.svg
+-rw-r--r--   0        0        0      442 2023-06-02 13:12:07.632999 mkdocs_dsfr-0.4.0/dsfr/icons/system/thumb-down-line.svg
+-rw-r--r--   0        0        0      340 2023-06-02 13:12:07.632999 mkdocs_dsfr-0.4.0/dsfr/icons/system/thumb-up-fill.svg
+-rw-r--r--   0        0        0      459 2023-06-02 13:12:07.634000 mkdocs_dsfr-0.4.0/dsfr/icons/system/thumb-up-line.svg
+-rw-r--r--   0        0        0      193 2023-06-02 13:12:07.634000 mkdocs_dsfr-0.4.0/dsfr/icons/system/time-fill.svg
+-rw-r--r--   0        0        0      226 2023-06-02 13:12:07.634000 mkdocs_dsfr-0.4.0/dsfr/icons/system/time-line.svg
+-rw-r--r--   0        0        0      201 2023-06-02 13:12:07.634999 mkdocs_dsfr-0.4.0/dsfr/icons/system/timer-fill.svg
+-rw-r--r--   0        0        0      236 2023-06-02 13:12:07.634999 mkdocs_dsfr-0.4.0/dsfr/icons/system/timer-line.svg
+-rw-r--r--   0        0        0      180 2023-06-02 13:12:07.642999 mkdocs_dsfr-0.4.0/dsfr/icons/system/upload-2-fill.svg
+-rw-r--r--   0        0        0      180 2023-06-02 13:12:07.642999 mkdocs_dsfr-0.4.0/dsfr/icons/system/upload-2-line.svg
+-rw-r--r--   0        0        0      144 2023-06-02 13:12:07.644000 mkdocs_dsfr-0.4.0/dsfr/icons/system/upload-fill.svg
+-rw-r--r--   0        0        0      206 2023-06-02 13:12:07.644000 mkdocs_dsfr-0.4.0/dsfr/icons/system/upload-line.svg
+-rw-r--r--   0        0        0      279 2023-06-02 13:12:07.660000 mkdocs_dsfr-0.4.0/dsfr/icons/system/zoom-in-fill.svg
+-rw-r--r--   0        0        0      407 2023-06-02 13:12:07.660000 mkdocs_dsfr-0.4.0/dsfr/icons/system/zoom-in-line.svg
+-rw-r--r--   0        0        0      260 2023-06-02 13:12:07.661000 mkdocs_dsfr-0.4.0/dsfr/icons/system/zoom-out-fill.svg
+-rw-r--r--   0        0        0      388 2023-06-02 13:12:07.661000 mkdocs_dsfr-0.4.0/dsfr/icons/system/zoom-out-line.svg
+-rw-r--r--   0        0        0      337 2023-06-02 13:12:07.368999 mkdocs_dsfr-0.4.0/dsfr/icons/user/account-circle-fill.svg
+-rw-r--r--   0        0        0      462 2023-06-02 13:12:07.368999 mkdocs_dsfr-0.4.0/dsfr/icons/user/account-circle-line.svg
+-rw-r--r--   0        0        0      383 2023-06-02 13:12:07.368999 mkdocs_dsfr-0.4.0/dsfr/icons/user/account-pin-circle-fill.svg
+-rw-r--r--   0        0        0      575 2023-06-02 13:12:07.369999 mkdocs_dsfr-0.4.0/dsfr/icons/user/account-pin-circle-line.svg
+-rw-r--r--   0        0        0      279 2023-06-02 13:12:07.371000 mkdocs_dsfr-0.4.0/dsfr/icons/user/admin-fill.svg
+-rw-r--r--   0        0        0      349 2023-06-02 13:12:07.371999 mkdocs_dsfr-0.4.0/dsfr/icons/user/admin-line.svg
+-rw-r--r--   0        0        0      357 2023-06-02 13:12:07.503000 mkdocs_dsfr-0.4.0/dsfr/icons/user/group-fill.svg
+-rw-r--r--   0        0        0      462 2023-06-02 13:12:07.503999 mkdocs_dsfr-0.4.0/dsfr/icons/user/group-line.svg
+-rw-r--r--   0        0        0      279 2023-06-02 13:12:07.568000 mkdocs_dsfr-0.4.0/dsfr/icons/user/parent-fill.svg
+-rw-r--r--   0        0        0      413 2023-06-02 13:12:07.569000 mkdocs_dsfr-0.4.0/dsfr/icons/user/parent-line.svg
+-rw-r--r--   0        0        0      424 2023-06-02 13:12:07.627000 mkdocs_dsfr-0.4.0/dsfr/icons/user/team-fill.svg
+-rw-r--r--   0        0        0      750 2023-06-02 13:12:07.628000 mkdocs_dsfr-0.4.0/dsfr/icons/user/team-line.svg
+-rw-r--r--   0        0        0      235 2023-06-02 13:12:07.644000 mkdocs_dsfr-0.4.0/dsfr/icons/user/user-add-fill.svg
+-rw-r--r--   0        0        0      316 2023-06-02 13:12:07.644999 mkdocs_dsfr-0.4.0/dsfr/icons/user/user-add-line.svg
+-rw-r--r--   0        0        0      186 2023-06-02 13:12:07.644999 mkdocs_dsfr-0.4.0/dsfr/icons/user/user-fill.svg
+-rw-r--r--   0        0        0      314 2023-06-02 13:12:07.645999 mkdocs_dsfr-0.4.0/dsfr/icons/user/user-heart-fill.svg
+-rw-r--r--   0        0        0      439 2023-06-02 13:12:07.645999 mkdocs_dsfr-0.4.0/dsfr/icons/user/user-heart-line.svg
+-rw-r--r--   0        0        0      275 2023-06-02 13:12:07.647000 mkdocs_dsfr-0.4.0/dsfr/icons/user/user-line.svg
+-rw-r--r--   0        0        0      314 2023-06-02 13:12:07.647000 mkdocs_dsfr-0.4.0/dsfr/icons/user/user-search-fill.svg
+-rw-r--r--   0        0        0      384 2023-06-02 13:12:07.647000 mkdocs_dsfr-0.4.0/dsfr/icons/user/user-search-line.svg
+-rw-r--r--   0        0        0      529 2023-06-02 13:12:07.648000 mkdocs_dsfr-0.4.0/dsfr/icons/user/user-setting-fill.svg
+-rw-r--r--   0        0        0      462 2023-06-02 13:12:07.648000 mkdocs_dsfr-0.4.0/dsfr/icons/user/user-setting-line.svg
+-rw-r--r--   0        0        0      298 2023-06-02 13:12:07.648000 mkdocs_dsfr-0.4.0/dsfr/icons/user/user-star-fill.svg
+-rw-r--r--   0        0        0      367 2023-06-02 13:12:07.648999 mkdocs_dsfr-0.4.0/dsfr/icons/user/user-star-line.svg
+-rw-r--r--   0        0        0      167 2023-06-02 13:12:07.424000 mkdocs_dsfr-0.4.0/dsfr/icons/weather/cloudy-2-fill.svg
+-rw-r--r--   0        0        0      291 2023-06-02 13:12:07.424000 mkdocs_dsfr-0.4.0/dsfr/icons/weather/cloudy-2-line.svg
+-rw-r--r--   0        0        0      128 2023-06-02 13:12:07.470000 mkdocs_dsfr-0.4.0/dsfr/icons/weather/flashlight-fill.svg
+-rw-r--r--   0        0        0      172 2023-06-02 13:12:07.470000 mkdocs_dsfr-0.4.0/dsfr/icons/weather/flashlight-line.svg
+-rw-r--r--   0        0        0      226 2023-06-02 13:12:07.555000 mkdocs_dsfr-0.4.0/dsfr/icons/weather/moon-fill.svg
+-rw-r--r--   0        0        0      286 2023-06-02 13:12:07.555000 mkdocs_dsfr-0.4.0/dsfr/icons/weather/moon-line.svg
+-rw-r--r--   0        0        0      449 2023-06-02 13:12:07.618000 mkdocs_dsfr-0.4.0/dsfr/icons/weather/sun-fill.svg
+-rw-r--r--   0        0        0      482 2023-06-02 13:12:07.618000 mkdocs_dsfr-0.4.0/dsfr/icons/weather/sun-line.svg
+-rw-r--r--   0        0        0     1221 2023-05-31 09:02:28.010861 mkdocs_dsfr-0.4.0/dsfr/js/base.js
+-rw-r--r--   0        0        0    58073 2023-05-31 09:02:28.011124 mkdocs_dsfr-0.4.0/dsfr/js/bootstrap.min.js
+-rw-r--r--   0        0        0    93107 2023-05-31 09:02:28.011514 mkdocs_dsfr-0.4.0/dsfr/js/jquery-1.10.2.min.js
+-rw-r--r--   0        0        0     1553 2023-05-31 09:02:28.011584 mkdocs_dsfr-0.4.0/dsfr/lateral.html
+-rw-r--r--   0        0        0       25 2023-05-31 09:02:28.011646 mkdocs_dsfr-0.4.0/dsfr/main.html
+-rw-r--r--   0        0        0      174 2023-05-31 09:02:28.011702 mkdocs_dsfr-0.4.0/dsfr/mkdocs_theme.yml
+-rw-r--r--   0        0        0     1068 2023-05-31 09:02:28.011760 mkdocs_dsfr-0.4.0/dsfr/nav.html
+-rw-r--r--   0        0        0      743 2023-05-31 09:02:28.011819 mkdocs_dsfr-0.4.0/dsfr/prev-next-nav.html
+-rw-r--r--   0        0        0      575 2023-05-31 09:02:28.011878 mkdocs_dsfr-0.4.0/dsfr/search.html
+-rw-r--r--   0        0        0        0 2023-05-31 09:05:29.657662 mkdocs_dsfr-0.4.0/dsfr/tabs.html
+-rw-r--r--   0        0        0      748 2023-06-02 13:12:07.173000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/README.md
+-rw-r--r--   0        0        0      794 2023-06-02 13:12:07.171000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/README.md
+-rw-r--r--   0        0        0     8218 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.css
+-rw-r--r--   0        0        0    18287 2023-06-02 13:12:07.059999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.css.map
+-rw-r--r--   0        0        0     3542 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.css
+-rw-r--r--   0        0        0     8457 2023-06-02 13:12:07.059999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.css.map
+-rw-r--r--   0        0        0     3036 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.min.css
+-rw-r--r--   0        0        0     8332 2023-06-02 13:12:07.059999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.min.css.map
+-rw-r--r--   0        0        0     4916 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.main.css
+-rw-r--r--   0        0        0    12037 2023-06-02 13:12:07.059999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.main.css.map
+-rw-r--r--   0        0        0     4370 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.main.min.css
+-rw-r--r--   0        0        0    11358 2023-06-02 13:12:07.059999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.main.min.css.map
+-rw-r--r--   0        0        0     7178 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.min.css
+-rw-r--r--   0        0        0    17475 2023-06-02 13:12:07.061000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.min.css.map
+-rw-r--r--   0        0        0      788 2023-06-02 13:12:07.171000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/README.md
+-rw-r--r--   0        0        0    22912 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.css
+-rw-r--r--   0        0        0    36228 2023-06-02 13:12:07.061000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.css.map
+-rw-r--r--   0        0        0     9504 2023-06-02 13:12:06.515000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.legacy.css
+-rw-r--r--   0        0        0    15589 2023-06-02 13:12:07.061000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.legacy.css.map
+-rw-r--r--   0        0        0     8088 2023-06-02 13:12:06.515000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.legacy.min.css
+-rw-r--r--   0        0        0    15215 2023-06-02 13:12:07.061000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.legacy.min.css.map
+-rw-r--r--   0        0        0    13648 2023-06-02 13:12:06.515000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.main.css
+-rw-r--r--   0        0        0    22829 2023-06-02 13:12:07.062000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.main.css.map
+-rw-r--r--   0        0        0    12243 2023-06-02 13:12:06.515000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.main.min.css
+-rw-r--r--   0        0        0    21852 2023-06-02 13:12:07.062000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.main.min.css.map
+-rw-r--r--   0        0        0    20103 2023-06-02 13:12:06.516000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.min.css
+-rw-r--r--   0        0        0    34868 2023-06-02 13:12:07.062000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.min.css.map
+-rw-r--r--   0        0        0      818 2023-06-02 13:12:07.171000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/README.md
+-rw-r--r--   0        0        0     8770 2023-06-02 13:12:06.516000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.css
+-rw-r--r--   0        0        0    18782 2023-06-02 13:12:07.062000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.css.map
+-rw-r--r--   0        0        0     3786 2023-06-02 13:12:06.516000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.legacy.css
+-rw-r--r--   0        0        0     8627 2023-06-02 13:12:07.062000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.legacy.css.map
+-rw-r--r--   0        0        0     3272 2023-06-02 13:12:06.516000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.legacy.min.css
+-rw-r--r--   0        0        0     8500 2023-06-02 13:12:07.062000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.legacy.min.css.map
+-rw-r--r--   0        0        0     5224 2023-06-02 13:12:06.516000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.main.css
+-rw-r--r--   0        0        0    12366 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.main.css.map
+-rw-r--r--   0        0        0     4674 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.main.min.css
+-rw-r--r--   0        0        0    11670 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.main.min.css.map
+-rw-r--r--   0        0        0     7718 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.min.css
+-rw-r--r--   0        0        0    17951 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.min.css.map
+-rw-r--r--   0        0        0      776 2023-06-02 13:12:07.171000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/README.md
+-rw-r--r--   0        0        0    15237 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.css
+-rw-r--r--   0        0        0    26942 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.css.map
+-rw-r--r--   0        0        0     6494 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.legacy.css
+-rw-r--r--   0        0        0    12000 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.legacy.css.map
+-rw-r--r--   0        0        0     5504 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.legacy.min.css
+-rw-r--r--   0        0        0    11743 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.legacy.min.css.map
+-rw-r--r--   0        0        0     8983 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.main.css
+-rw-r--r--   0        0        0    17146 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.main.css.map
+-rw-r--r--   0        0        0     8000 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.main.min.css
+-rw-r--r--   0        0        0    16324 2023-06-02 13:12:07.063999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.main.min.css.map
+-rw-r--r--   0        0        0    13276 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.min.css
+-rw-r--r--   0        0        0    25855 2023-06-02 13:12:07.063999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.min.css.map
+-rw-r--r--   0        0        0      806 2023-06-02 13:12:07.171000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/README.md
+-rw-r--r--   0        0        0    10584 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.css
+-rw-r--r--   0        0        0    20888 2023-06-02 13:12:07.063999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.css.map
+-rw-r--r--   0        0        0     4556 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.legacy.css
+-rw-r--r--   0        0        0     9503 2023-06-02 13:12:07.063999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.legacy.css.map
+-rw-r--r--   0        0        0     3954 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.legacy.min.css
+-rw-r--r--   0        0        0     9352 2023-06-02 13:12:07.063999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.legacy.min.css.map
+-rw-r--r--   0        0        0     6268 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.main.css
+-rw-r--r--   0        0        0    13594 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.main.css.map
+-rw-r--r--   0        0        0     5638 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.main.min.css
+-rw-r--r--   0        0        0    12876 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.main.min.css.map
+-rw-r--r--   0        0        0     9364 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.min.css
+-rw-r--r--   0        0        0    20011 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.min.css.map
+-rw-r--r--   0        0        0      776 2023-06-02 13:12:07.171000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/README.md
+-rw-r--r--   0        0        0    13498 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.css
+-rw-r--r--   0        0        0    24915 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.css.map
+-rw-r--r--   0        0        0     5696 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.legacy.css
+-rw-r--r--   0        0        0    11099 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.legacy.css.map
+-rw-r--r--   0        0        0     4810 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.legacy.min.css
+-rw-r--r--   0        0        0    10870 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.legacy.min.css.map
+-rw-r--r--   0        0        0     8042 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.main.css
+-rw-r--r--   0        0        0    16020 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.main.css.map
+-rw-r--r--   0        0        0     7132 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.main.min.css
+-rw-r--r--   0        0        0    15219 2023-06-02 13:12:07.065999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.main.min.css.map
+-rw-r--r--   0        0        0    11714 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.min.css
+-rw-r--r--   0        0        0    23877 2023-06-02 13:12:07.065999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.min.css.map
+-rw-r--r--   0        0        0      788 2023-06-02 13:12:07.171999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/README.md
+-rw-r--r--   0        0        0    12044 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.css
+-rw-r--r--   0        0        0    23019 2023-06-02 13:12:07.065999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.css.map
+-rw-r--r--   0        0        0     5060 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.legacy.css
+-rw-r--r--   0        0        0    10303 2023-06-02 13:12:07.065999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.legacy.css.map
+-rw-r--r--   0        0        0     4306 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.legacy.min.css
+-rw-r--r--   0        0        0    10110 2023-06-02 13:12:07.065999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.legacy.min.css.map
+-rw-r--r--   0        0        0     7224 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.main.css
+-rw-r--r--   0        0        0    14922 2023-06-02 13:12:07.066999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.main.css.map
+-rw-r--r--   0        0        0     6434 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.main.min.css
+-rw-r--r--   0        0        0    14157 2023-06-02 13:12:07.066999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.main.min.css.map
+-rw-r--r--   0        0        0    10512 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.min.css
+-rw-r--r--   0        0        0    22053 2023-06-02 13:12:07.066999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.min.css.map
+-rw-r--r--   0        0        0      776 2023-06-02 13:12:07.171999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/README.md
+-rw-r--r--   0        0        0    10188 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.css
+-rw-r--r--   0        0        0    21006 2023-06-02 13:12:07.066999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.css.map
+-rw-r--r--   0        0        0     4282 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.legacy.css
+-rw-r--r--   0        0        0     9470 2023-06-02 13:12:07.066999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.legacy.css.map
+-rw-r--r--   0        0        0     3576 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.legacy.min.css
+-rw-r--r--   0        0        0     9290 2023-06-02 13:12:07.068000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.legacy.min.css.map
+-rw-r--r--   0        0        0     6146 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.main.css
+-rw-r--r--   0        0        0    13740 2023-06-02 13:12:07.068000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.main.css.map
+-rw-r--r--   0        0        0     5396 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.main.min.css
+-rw-r--r--   0        0        0    12995 2023-06-02 13:12:07.068000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.main.min.css.map
+-rw-r--r--   0        0        0     8744 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.min.css
+-rw-r--r--   0        0        0    20073 2023-06-02 13:12:07.068000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.min.css.map
+-rw-r--r--   0        0        0      782 2023-06-02 13:12:07.171999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/README.md
+-rw-r--r--   0        0        0     6775 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.css
+-rw-r--r--   0        0        0    16388 2023-06-02 13:12:07.068000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.css.map
+-rw-r--r--   0        0        0     2988 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.legacy.css
+-rw-r--r--   0        0        0     7688 2023-06-02 13:12:07.069000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.legacy.css.map
+-rw-r--r--   0        0        0     2584 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.legacy.min.css
+-rw-r--r--   0        0        0     7591 2023-06-02 13:12:07.069000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.legacy.min.css.map
+-rw-r--r--   0        0        0     4027 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.main.css
+-rw-r--r--   0        0        0    10905 2023-06-02 13:12:07.069000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.main.css.map
+-rw-r--r--   0        0        0     3577 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.main.min.css
+-rw-r--r--   0        0        0    10262 2023-06-02 13:12:07.069000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.main.min.css.map
+-rw-r--r--   0        0        0     5933 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.min.css
+-rw-r--r--   0        0        0    15640 2023-06-02 13:12:07.069000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.min.css.map
+-rw-r--r--   0        0        0      776 2023-06-02 13:12:07.171999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/README.md
+-rw-r--r--   0        0        0    14367 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.css
+-rw-r--r--   0        0        0    25626 2023-06-02 13:12:07.069000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.css.map
+-rw-r--r--   0        0        0     6168 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.legacy.css
+-rw-r--r--   0        0        0    11461 2023-06-02 13:12:07.069999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.legacy.css.map
+-rw-r--r--   0        0        0     5280 2023-06-02 13:12:06.520999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.legacy.min.css
+-rw-r--r--   0        0        0    11232 2023-06-02 13:12:07.069999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.legacy.min.css.map
+-rw-r--r--   0        0        0     8439 2023-06-02 13:12:06.520999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.main.css
+-rw-r--r--   0        0        0    16369 2023-06-02 13:12:07.069999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.main.css.map
+-rw-r--r--   0        0        0     7549 2023-06-02 13:12:06.520999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.main.min.css
+-rw-r--r--   0        0        0    15575 2023-06-02 13:12:07.069999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.main.min.css.map
+-rw-r--r--   0        0        0    12601 2023-06-02 13:12:06.520999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.min.css
+-rw-r--r--   0        0        0    24595 2023-06-02 13:12:07.069999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.min.css.map
+-rw-r--r--   0        0        0      764 2023-06-02 13:12:07.171999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/README.md
+-rw-r--r--   0        0        0    24122 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.css
+-rw-r--r--   0        0        0    38165 2023-06-02 13:12:07.069999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.css.map
+-rw-r--r--   0        0        0     9746 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.legacy.css
+-rw-r--r--   0        0        0    16087 2023-06-02 13:12:07.071000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.legacy.css.map
+-rw-r--r--   0        0        0     8200 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.legacy.min.css
+-rw-r--r--   0        0        0    15676 2023-06-02 13:12:07.071000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.legacy.min.css.map
+-rw-r--r--   0        0        0    14616 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.main.css
+-rw-r--r--   0        0        0    24218 2023-06-02 13:12:07.071000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.main.css.map
+-rw-r--r--   0        0        0    13026 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.main.min.css
+-rw-r--r--   0        0        0    23185 2023-06-02 13:12:07.071000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.main.min.css.map
+-rw-r--r--   0        0        0    20998 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.min.css
+-rw-r--r--   0        0        0    36712 2023-06-02 13:12:07.071000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.min.css.map
+-rw-r--r--   0        0        0      758 2023-06-02 13:12:07.171999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/README.md
+-rw-r--r--   0        0        0    17550 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.css
+-rw-r--r--   0        0        0    29852 2023-06-02 13:12:07.072000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.css.map
+-rw-r--r--   0        0        0     7456 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.legacy.css
+-rw-r--r--   0        0        0    13177 2023-06-02 13:12:07.072000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.legacy.css.map
+-rw-r--r--   0        0        0     6298 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.legacy.min.css
+-rw-r--r--   0        0        0    12874 2023-06-02 13:12:07.072000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.legacy.min.css.map
+-rw-r--r--   0        0        0    10334 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.main.css
+-rw-r--r--   0        0        0    18876 2023-06-02 13:12:07.072000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.main.css.map
+-rw-r--r--   0        0        0     9184 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.main.min.css
+-rw-r--r--   0        0        0    18000 2023-06-02 13:12:07.072999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.main.min.css.map
+-rw-r--r--   0        0        0    15254 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.min.css
+-rw-r--r--   0        0        0    28665 2023-06-02 13:12:07.072999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.min.css.map
+-rw-r--r--   0        0        0      770 2023-06-02 13:12:07.173000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/README.md
+-rw-r--r--   0        0        0    19301 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.css
+-rw-r--r--   0        0        0    31920 2023-06-02 13:12:07.072999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.css.map
+-rw-r--r--   0        0        0     7999 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.legacy.css
+-rw-r--r--   0        0        0    13839 2023-06-02 13:12:07.072999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.legacy.css.map
+-rw-r--r--   0        0        0     6785 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.legacy.min.css
+-rw-r--r--   0        0        0    13520 2023-06-02 13:12:07.072999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.legacy.min.css.map
+-rw-r--r--   0        0        0    11542 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.main.css
+-rw-r--r--   0        0        0    20284 2023-06-02 13:12:07.073999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.main.css.map
+-rw-r--r--   0        0        0    10312 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.main.min.css
+-rw-r--r--   0        0        0    19374 2023-06-02 13:12:07.073999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.main.min.css.map
+-rw-r--r--   0        0        0    16869 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.min.css
+-rw-r--r--   0        0        0    30683 2023-06-02 13:12:07.073999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.min.css.map
+-rw-r--r--   0        0        0      776 2023-06-02 13:12:07.173000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/README.md
+-rw-r--r--   0        0        0     5250 2023-06-02 13:12:06.523999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.css
+-rw-r--r--   0        0        0    14634 2023-06-02 13:12:07.073999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.css.map
+-rw-r--r--   0        0        0     2350 2023-06-02 13:12:06.523999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.legacy.css
+-rw-r--r--   0        0        0     6968 2023-06-02 13:12:07.073999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.legacy.css.map
+-rw-r--r--   0        0        0     2012 2023-06-02 13:12:06.523999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.legacy.min.css
+-rw-r--r--   0        0        0     6889 2023-06-02 13:12:07.075000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.legacy.min.css.map
+-rw-r--r--   0        0        0     3140 2023-06-02 13:12:06.523999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.main.css
+-rw-r--r--   0        0        0     9870 2023-06-02 13:12:07.075000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.main.css.map
+-rw-r--r--   0        0        0     2750 2023-06-02 13:12:06.523999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.main.min.css
+-rw-r--r--   0        0        0     9251 2023-06-02 13:12:07.075000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.main.min.css.map
+-rw-r--r--   0        0        0     4534 2023-06-02 13:12:06.523999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.min.css
+-rw-r--r--   0        0        0    13928 2023-06-02 13:12:07.075000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.min.css.map
+-rw-r--r--   0        0        0      776 2023-06-02 13:12:07.173000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/README.md
+-rw-r--r--   0        0        0    61210 2023-06-02 13:12:06.525000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.css
+-rw-r--r--   0        0        0    83686 2023-06-02 13:12:07.075999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.css.map
+-rw-r--r--   0        0        0    24507 2023-06-02 13:12:06.525000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.legacy.css
+-rw-r--r--   0        0        0    33766 2023-06-02 13:12:07.075999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.legacy.css.map
+-rw-r--r--   0        0        0    20773 2023-06-02 13:12:06.525000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.legacy.min.css
+-rw-r--r--   0        0        0    32754 2023-06-02 13:12:07.075999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.legacy.min.css.map
+-rw-r--r--   0        0        0    36943 2023-06-02 13:12:06.525000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.main.css
+-rw-r--r--   0        0        0    51783 2023-06-02 13:12:07.075999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.main.css.map
+-rw-r--r--   0        0        0    33240 2023-06-02 13:12:06.525000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.main.min.css
+-rw-r--r--   0        0        0    50018 2023-06-02 13:12:07.076999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.main.min.css.map
+-rw-r--r--   0        0        0    53785 2023-06-02 13:12:06.525000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.min.css
+-rw-r--r--   0        0        0    80902 2023-06-02 13:12:07.076999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.min.css.map
+-rw-r--r--   0        0        0      764 2023-06-02 13:12:07.173000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/README.md
+-rw-r--r--   0        0        0    10694 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.css
+-rw-r--r--   0        0        0    21349 2023-06-02 13:12:07.076999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.css.map
+-rw-r--r--   0        0        0     4602 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.legacy.css
+-rw-r--r--   0        0        0     9729 2023-06-02 13:12:07.078000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.legacy.css.map
+-rw-r--r--   0        0        0     3920 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.legacy.min.css
+-rw-r--r--   0        0        0     9556 2023-06-02 13:12:07.078000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.legacy.min.css.map
+-rw-r--r--   0        0        0     6332 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.main.css
+-rw-r--r--   0        0        0    13822 2023-06-02 13:12:07.078000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.main.css.map
+-rw-r--r--   0        0        0     5622 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.main.min.css
+-rw-r--r--   0        0        0    13097 2023-06-02 13:12:07.078000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.main.min.css.map
+-rw-r--r--   0        0        0     9314 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.min.css
+-rw-r--r--   0        0        0    20443 2023-06-02 13:12:07.078999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.min.css.map
+-rw-r--r--   0        0        0      782 2023-06-02 13:12:07.173000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/README.md
+-rw-r--r--   0        0        0     3858 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.css
+-rw-r--r--   0        0        0    13024 2023-06-02 13:12:07.078999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.css.map
+-rw-r--r--   0        0        0     1726 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.legacy.css
+-rw-r--r--   0        0        0     6315 2023-06-02 13:12:07.078999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.legacy.css.map
+-rw-r--r--   0        0        0     1484 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.legacy.min.css
+-rw-r--r--   0        0        0     6262 2023-06-02 13:12:07.078999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.legacy.min.css.map
+-rw-r--r--   0        0        0     2372 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.main.css
+-rw-r--r--   0        0        0     8914 2023-06-02 13:12:07.078999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.main.css.map
+-rw-r--r--   0        0        0     2062 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.main.min.css
+-rw-r--r--   0        0        0     8320 2023-06-02 13:12:07.079999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.main.min.css.map
+-rw-r--r--   0        0        0     3318 2023-06-02 13:12:06.526999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.min.css
+-rw-r--r--   0        0        0    12369 2023-06-02 13:12:07.079999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.min.css.map
+-rw-r--r--   0        0        0   252525 2023-06-02 13:12:06.528000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.css
+-rw-r--r--   0        0        0   338301 2023-06-02 13:12:07.081000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.css.map
+-rw-r--r--   0        0        0   103243 2023-06-02 13:12:06.528000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.legacy.css
+-rw-r--r--   0        0        0   134266 2023-06-02 13:12:07.081000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.legacy.css.map
+-rw-r--r--   0        0        0    87075 2023-06-02 13:12:06.528000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.legacy.min.css
+-rw-r--r--   0        0        0   129807 2023-06-02 13:12:07.082000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.legacy.min.css.map
+-rw-r--r--   0        0        0   149522 2023-06-02 13:12:06.529000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.main.css
+-rw-r--r--   0        0        0   204422 2023-06-02 13:12:07.082999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.main.css.map
+-rw-r--r--   0        0        0   133091 2023-06-02 13:12:06.529000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.main.min.css
+-rw-r--r--   0        0        0   190288 2023-06-02 13:12:07.082999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.main.min.css.map
+-rw-r--r--   0        0        0   219938 2023-06-02 13:12:06.529999 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.min.css
+-rw-r--r--   0        0        0   318184 2023-06-02 13:12:07.084000 mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.min.css.map
+-rw-r--r--   0        0        0      583 2023-07-04 15:15:39.347533 mkdocs_dsfr-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2929 1970-01-01 00:00:00.000000 mkdocs_dsfr-0.4.0/PKG-INFO
```

### Comparing `mkdocs_dsfr-0.3.1/LICENSE` & `mkdocs_dsfr-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/background/ovoid.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/background/ovoid.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/dark.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/dark.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/light.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/light.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/buildings/city-hall.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/buildings/city-hall.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/buildings/factory.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/buildings/factory.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/buildings/house.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/buildings/house.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/buildings/nuclear-plant.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/buildings/nuclear-plant.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/buildings/school.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/buildings/school.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/digital/application.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/digital/application.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/digital/avatar.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/digital/avatar.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/digital/calendar.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/digital/calendar.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/digital/coding.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/digital/coding.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/digital/data-visualization.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/digital/data-visualization.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/digital/internet.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/digital/internet.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/digital/mail-send.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/digital/mail-send.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/digital/search.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/digital/search.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/document/contract.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/document/contract.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/document/document-add.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/document/document-add.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/document/document-download.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/document/document-download.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/document/document-signature.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/document/document-signature.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/document/document.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/document/document.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/document/driving-licence.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/document/driving-licence.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/document/national-identity-card.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/document/national-identity-card.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/document/passport.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/document/passport.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/document/tax-stamp.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/document/tax-stamp.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/document/vehicle-registration.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/document/vehicle-registration.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/environment/environment.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/environment/environment.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/environment/food.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/environment/food.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/environment/grocery.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/environment/grocery.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/environment/human-cooperation.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/environment/human-cooperation.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/environment/leaf.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/environment/leaf.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/environment/moon.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/environment/moon.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/environment/mountain.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/environment/mountain.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/environment/sun.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/environment/sun.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/environment/tree.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/environment/tree.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/health/health.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/health/health.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/health/hospital.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/health/hospital.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/health/vaccine.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/health/vaccine.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/health/virus.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/health/virus.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/institutions/firefighter.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/institutions/firefighter.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/institutions/gendarmerie.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/institutions/gendarmerie.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/institutions/justice.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/institutions/justice.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/institutions/money.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/institutions/money.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/institutions/police.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/institutions/police.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/leisure/book.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/leisure/book.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/leisure/community.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/leisure/community.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/leisure/culture.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/leisure/culture.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/leisure/digital-art.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/leisure/digital-art.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/leisure/paint.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/leisure/paint.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/map/airport.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/map/airport.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/map/location-france.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/map/location-france.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/map/luggage.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/map/luggage.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/map/map.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/map/map.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/system/connection-lost.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/system/connection-lost.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/system/error.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/system/error.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/system/information.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/system/information.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/system/notification.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/system/notification.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/system/padlock.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/system/padlock.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/system/success.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/system/success.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/system/system.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/system/system.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/system/technical-error.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/system/technical-error.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/pictograms/system/warning.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/pictograms/system/warning.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/artwork/system.svg` & `mkdocs_dsfr-0.4.0/dsfr/artwork/system.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/base.html` & `mkdocs_dsfr-0.4.0/dsfr/base.html`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/css/theme.css` & `mkdocs_dsfr-0.4.0/dsfr/css/theme.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/dsfr.min.css` & `mkdocs_dsfr-0.4.0/dsfr/dsfr.min.css`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 @charset "UTF-8";
 /*!
  * DSFR v1.9.3 | SPDX-License-Identifier: MIT | License-Filename: LICENSE.md | restricted use (see terms and conditions)
- */a{--hover-tint:var(--idle);--active-tint:var(--active);color:inherit;text-decoration:none}:root{--underline-max-width:100%;--underline-hover-width:0;--underline-idle-width:var(--underline-max-width);--underline-x:calc(var(--underline-max-width)*0);--underline-thickness:max(1px,0.0625em);--underline-img:linear-gradient(0deg,currentColor,currentColor);--external-link-content:"";--ul-type:disc;--ol-type:decimal;--ul-start:1rem;--ol-start:1.5rem;--xl-block:0.5rem;--li-bottom:0.25rem;--xl-base:1em;--ol-content:counters(li-counter,".") ".  ";--text-spacing:0 0 1.5rem;--title-spacing:0 0 1.5rem;--display-spacing:0 0 2rem;--background-default-grey:var(--grey-1000-50);--background-default-grey-hover:var(--grey-1000-50-hover);--background-default-grey-active:var(--grey-1000-50-active);--background-alt-grey:var(--grey-975-75);--background-alt-grey-hover:var(--grey-975-75-hover);--background-alt-grey-active:var(--grey-975-75-active);--background-alt-blue-france:var(--blue-france-975-75);--background-alt-blue-france-hover:var(--blue-france-975-75-hover);--background-alt-blue-france-active:var(--blue-france-975-75-active);--background-alt-red-marianne:var(--red-marianne-975-75);--background-alt-red-marianne-hover:var(--red-marianne-975-75-hover);--background-alt-red-marianne-active:var(--red-marianne-975-75-active);--background-alt-green-tilleul-verveine:var(--green-tilleul-verveine-975-75);--background-alt-green-tilleul-verveine-hover:var(--green-tilleul-verveine-975-75-hover);--background-alt-green-tilleul-verveine-active:var(--green-tilleul-verveine-975-75-active);--background-alt-green-bourgeon:var(--green-bourgeon-975-75);--background-alt-green-bourgeon-hover:var(--green-bourgeon-975-75-hover);--background-alt-green-bourgeon-active:var(--green-bourgeon-975-75-active);--background-alt-green-emeraude:var(--green-emeraude-975-75);--background-alt-green-emeraude-hover:var(--green-emeraude-975-75-hover);--background-alt-green-emeraude-active:var(--green-emeraude-975-75-active);--background-alt-green-menthe:var(--green-menthe-975-75);--background-alt-green-menthe-hover:var(--green-menthe-975-75-hover);--background-alt-green-menthe-active:var(--green-menthe-975-75-active);--background-alt-green-archipel:var(--green-archipel-975-75);--background-alt-green-archipel-hover:var(--green-archipel-975-75-hover);--background-alt-green-archipel-active:var(--green-archipel-975-75-active);--background-alt-blue-ecume:var(--blue-ecume-975-75);--background-alt-blue-ecume-hover:var(--blue-ecume-975-75-hover);--background-alt-blue-ecume-active:var(--blue-ecume-975-75-active);--background-alt-blue-cumulus:var(--blue-cumulus-975-75);--background-alt-blue-cumulus-hover:var(--blue-cumulus-975-75-hover);--background-alt-blue-cumulus-active:var(--blue-cumulus-975-75-active);--background-alt-purple-glycine:var(--purple-glycine-975-75);--background-alt-purple-glycine-hover:var(--purple-glycine-975-75-hover);--background-alt-purple-glycine-active:var(--purple-glycine-975-75-active);--background-alt-pink-macaron:var(--pink-macaron-975-75);--background-alt-pink-macaron-hover:var(--pink-macaron-975-75-hover);--background-alt-pink-macaron-active:var(--pink-macaron-975-75-active);--background-alt-pink-tuile:var(--pink-tuile-975-75);--background-alt-pink-tuile-hover:var(--pink-tuile-975-75-hover);--background-alt-pink-tuile-active:var(--pink-tuile-975-75-active);--background-alt-yellow-tournesol:var(--yellow-tournesol-975-75);--background-alt-yellow-tournesol-hover:var(--yellow-tournesol-975-75-hover);--background-alt-yellow-tournesol-active:var(--yellow-tournesol-975-75-active);--background-alt-yellow-moutarde:var(--yellow-moutarde-975-75);--background-alt-yellow-moutarde-hover:var(--yellow-moutarde-975-75-hover);--background-alt-yellow-moutarde-active:var(--yellow-moutarde-975-75-active);--background-alt-orange-terre-battue:var(--orange-terre-battue-975-75);--background-alt-orange-terre-battue-hover:var(--orange-terre-battue-975-75-hover);--background-alt-orange-terre-battue-active:var(--orange-terre-battue-975-75-active);--background-alt-brown-cafe-creme:var(--brown-cafe-creme-975-75);--background-alt-brown-cafe-creme-hover:var(--brown-cafe-creme-975-75-hover);--background-alt-brown-cafe-creme-active:var(--brown-cafe-creme-975-75-active);--background-alt-brown-caramel:var(--brown-caramel-975-75);--background-alt-brown-caramel-hover:var(--brown-caramel-975-75-hover);--background-alt-brown-caramel-active:var(--brown-caramel-975-75-active);--background-alt-brown-opera:var(--brown-opera-975-75);--background-alt-brown-opera-hover:var(--brown-opera-975-75-hover);--background-alt-brown-opera-active:var(--brown-opera-975-75-active);--background-alt-beige-gris-galet:var(--beige-gris-galet-975-75);--background-alt-beige-gris-galet-hover:var(--beige-gris-galet-975-75-hover);--background-alt-beige-gris-galet-active:var(--beige-gris-galet-975-75-active);--background-contrast-grey:var(--grey-950-100);--background-contrast-grey-hover:var(--grey-950-100-hover);--background-contrast-grey-active:var(--grey-950-100-active);--background-contrast-blue-france:var(--blue-france-950-100);--background-contrast-blue-france-hover:var(--blue-france-950-100-hover);--background-contrast-blue-france-active:var(--blue-france-950-100-active);--background-contrast-red-marianne:var(--red-marianne-950-100);--background-contrast-red-marianne-hover:var(--red-marianne-950-100-hover);--background-contrast-red-marianne-active:var(--red-marianne-950-100-active);--background-contrast-green-tilleul-verveine:var(--green-tilleul-verveine-950-100);--background-contrast-green-tilleul-verveine-hover:var(--green-tilleul-verveine-950-100-hover);--background-contrast-green-tilleul-verveine-active:var(--green-tilleul-verveine-950-100-active);--background-contrast-green-bourgeon:var(--green-bourgeon-950-100);--background-contrast-green-bourgeon-hover:var(--green-bourgeon-950-100-hover);--background-contrast-green-bourgeon-active:var(--green-bourgeon-950-100-active);--background-contrast-green-emeraude:var(--green-emeraude-950-100);--background-contrast-green-emeraude-hover:var(--green-emeraude-950-100-hover);--background-contrast-green-emeraude-active:var(--green-emeraude-950-100-active);--background-contrast-green-menthe:var(--green-menthe-950-100);--background-contrast-green-menthe-hover:var(--green-menthe-950-100-hover);--background-contrast-green-menthe-active:var(--green-menthe-950-100-active);--background-contrast-green-archipel:var(--green-archipel-950-100);--background-contrast-green-archipel-hover:var(--green-archipel-950-100-hover);--background-contrast-green-archipel-active:var(--green-archipel-950-100-active);--background-contrast-blue-ecume:var(--blue-ecume-950-100);--background-contrast-blue-ecume-hover:var(--blue-ecume-950-100-hover);--background-contrast-blue-ecume-active:var(--blue-ecume-950-100-active);--background-contrast-blue-cumulus:var(--blue-cumulus-950-100);--background-contrast-blue-cumulus-hover:var(--blue-cumulus-950-100-hover);--background-contrast-blue-cumulus-active:var(--blue-cumulus-950-100-active);--background-contrast-purple-glycine:var(--purple-glycine-950-100);--background-contrast-purple-glycine-hover:var(--purple-glycine-950-100-hover);--background-contrast-purple-glycine-active:var(--purple-glycine-950-100-active);--background-contrast-pink-macaron:var(--pink-macaron-950-100);--background-contrast-pink-macaron-hover:var(--pink-macaron-950-100-hover);--background-contrast-pink-macaron-active:var(--pink-macaron-950-100-active);--background-contrast-pink-tuile:var(--pink-tuile-950-100);--background-contrast-pink-tuile-hover:var(--pink-tuile-950-100-hover);--background-contrast-pink-tuile-active:var(--pink-tuile-950-100-active);--background-contrast-yellow-tournesol:var(--yellow-tournesol-950-100);--background-contrast-yellow-tournesol-hover:var(--yellow-tournesol-950-100-hover);--background-contrast-yellow-tournesol-active:var(--yellow-tournesol-950-100-active);--background-contrast-yellow-moutarde:var(--yellow-moutarde-950-100);--background-contrast-yellow-moutarde-hover:var(--yellow-moutarde-950-100-hover);--background-contrast-yellow-moutarde-active:var(--yellow-moutarde-950-100-active);--background-contrast-orange-terre-battue:var(--orange-terre-battue-950-100);--background-contrast-orange-terre-battue-hover:var(--orange-terre-battue-950-100-hover);--background-contrast-orange-terre-battue-active:var(--orange-terre-battue-950-100-active);--background-contrast-brown-cafe-creme:var(--brown-cafe-creme-950-100);--background-contrast-brown-cafe-creme-hover:var(--brown-cafe-creme-950-100-hover);--background-contrast-brown-cafe-creme-active:var(--brown-cafe-creme-950-100-active);--background-contrast-brown-caramel:var(--brown-caramel-950-100);--background-contrast-brown-caramel-hover:var(--brown-caramel-950-100-hover);--background-contrast-brown-caramel-active:var(--brown-caramel-950-100-active);--background-contrast-brown-opera:var(--brown-opera-950-100);--background-contrast-brown-opera-hover:var(--brown-opera-950-100-hover);--background-contrast-brown-opera-active:var(--brown-opera-950-100-active);--background-contrast-beige-gris-galet:var(--beige-gris-galet-950-100);--background-contrast-beige-gris-galet-hover:var(--beige-gris-galet-950-100-hover);--background-contrast-beige-gris-galet-active:var(--beige-gris-galet-950-100-active);--background-contrast-info:var(--info-950-100);--background-contrast-info-hover:var(--info-950-100-hover);--background-contrast-info-active:var(--info-950-100-active);--background-contrast-success:var(--success-950-100);--background-contrast-success-hover:var(--success-950-100-hover);--background-contrast-success-active:var(--success-950-100-active);--background-contrast-warning:var(--warning-950-100);--background-contrast-warning-hover:var(--warning-950-100-hover);--background-contrast-warning-active:var(--warning-950-100-active);--background-contrast-error:var(--error-950-100);--background-contrast-error-hover:var(--error-950-100-hover);--background-contrast-error-active:var(--error-950-100-active);--background-flat-grey:var(--grey-200-850);--background-flat-info:var(--info-425-625);--background-flat-success:var(--success-425-625);--background-flat-warning:var(--warning-425-625);--background-flat-error:var(--error-425-625);--background-action-high-blue-france:var(--blue-france-sun-113-625);--background-action-high-blue-france-hover:var(--blue-france-sun-113-625-hover);--background-action-high-blue-france-active:var(--blue-france-sun-113-625-active);--background-action-high-red-marianne:var(--red-marianne-425-625);--background-action-high-red-marianne-hover:var(--red-marianne-425-625-hover);--background-action-high-red-marianne-active:var(--red-marianne-425-625-active);--background-action-high-green-tilleul-verveine:var(--green-tilleul-verveine-sun-418-moon-817);--background-action-high-green-tilleul-verveine-hover:var(--green-tilleul-verveine-sun-418-moon-817-hover);--background-action-high-green-tilleul-verveine-active:var(--green-tilleul-verveine-sun-418-moon-817-active);--background-action-high-green-bourgeon:var(--green-bourgeon-sun-425-moon-759);--background-action-high-green-bourgeon-hover:var(--green-bourgeon-sun-425-moon-759-hover);--background-action-high-green-bourgeon-active:var(--green-bourgeon-sun-425-moon-759-active);--background-action-high-green-emeraude:var(--green-emeraude-sun-425-moon-753);--background-action-high-green-emeraude-hover:var(--green-emeraude-sun-425-moon-753-hover);--background-action-high-green-emeraude-active:var(--green-emeraude-sun-425-moon-753-active);--background-action-high-green-menthe:var(--green-menthe-sun-373-moon-652);--background-action-high-green-menthe-hover:var(--green-menthe-sun-373-moon-652-hover);--background-action-high-green-menthe-active:var(--green-menthe-sun-373-moon-652-active);--background-action-high-green-archipel:var(--green-archipel-sun-391-moon-716);--background-action-high-green-archipel-hover:var(--green-archipel-sun-391-moon-716-hover);--background-action-high-green-archipel-active:var(--green-archipel-sun-391-moon-716-active);--background-action-high-blue-ecume:var(--blue-ecume-sun-247-moon-675);--background-action-high-blue-ecume-hover:var(--blue-ecume-sun-247-moon-675-hover);--background-action-high-blue-ecume-active:var(--blue-ecume-sun-247-moon-675-active);--background-action-high-blue-cumulus:var(--blue-cumulus-sun-368-moon-732);--background-action-high-blue-cumulus-hover:var(--blue-cumulus-sun-368-moon-732-hover);--background-action-high-blue-cumulus-active:var(--blue-cumulus-sun-368-moon-732-active);--background-action-high-purple-glycine:var(--purple-glycine-sun-319-moon-630);--background-action-high-purple-glycine-hover:var(--purple-glycine-sun-319-moon-630-hover);--background-action-high-purple-glycine-active:var(--purple-glycine-sun-319-moon-630-active);--background-action-high-pink-macaron:var(--pink-macaron-sun-406-moon-833);--background-action-high-pink-macaron-hover:var(--pink-macaron-sun-406-moon-833-hover);--background-action-high-pink-macaron-active:var(--pink-macaron-sun-406-moon-833-active);--background-action-high-pink-tuile:var(--pink-tuile-sun-425-moon-750);--background-action-high-pink-tuile-hover:var(--pink-tuile-sun-425-moon-750-hover);--background-action-high-pink-tuile-active:var(--pink-tuile-sun-425-moon-750-active);--background-action-high-yellow-tournesol:var(--yellow-tournesol-sun-407-moon-922);--background-action-high-yellow-tournesol-hover:var(--yellow-tournesol-sun-407-moon-922-hover);--background-action-high-yellow-tournesol-active:var(--yellow-tournesol-sun-407-moon-922-active);--background-action-high-yellow-moutarde:var(--yellow-moutarde-sun-348-moon-860);--background-action-high-yellow-moutarde-hover:var(--yellow-moutarde-sun-348-moon-860-hover);--background-action-high-yellow-moutarde-active:var(--yellow-moutarde-sun-348-moon-860-active);--background-action-high-orange-terre-battue:var(--orange-terre-battue-sun-370-moon-672);--background-action-high-orange-terre-battue-hover:var(--orange-terre-battue-sun-370-moon-672-hover);--background-action-high-orange-terre-battue-active:var(--orange-terre-battue-sun-370-moon-672-active);--background-action-high-brown-cafe-creme:var(--brown-cafe-creme-sun-383-moon-885);--background-action-high-brown-cafe-creme-hover:var(--brown-cafe-creme-sun-383-moon-885-hover);--background-action-high-brown-cafe-creme-active:var(--brown-cafe-creme-sun-383-moon-885-active);--background-action-high-brown-caramel:var(--brown-caramel-sun-425-moon-901);--background-action-high-brown-caramel-hover:var(--brown-caramel-sun-425-moon-901-hover);--background-action-high-brown-caramel-active:var(--brown-caramel-sun-425-moon-901-active);--background-action-high-brown-opera:var(--brown-opera-sun-395-moon-820);--background-action-high-brown-opera-hover:var(--brown-opera-sun-395-moon-820-hover);--background-action-high-brown-opera-active:var(--brown-opera-sun-395-moon-820-active);--background-action-high-beige-gris-galet:var(--beige-gris-galet-sun-407-moon-821);--background-action-high-beige-gris-galet-hover:var(--beige-gris-galet-sun-407-moon-821-hover);--background-action-high-beige-gris-galet-active:var(--beige-gris-galet-sun-407-moon-821-active);--background-action-high-info:var(--info-425-625);--background-action-high-info-hover:var(--info-425-625-hover);--background-action-high-info-active:var(--info-425-625-active);--background-action-high-success:var(--success-425-625);--background-action-high-success-hover:var(--success-425-625-hover);--background-action-high-success-active:var(--success-425-625-active);--background-action-high-warning:var(--warning-425-625);--background-action-high-warning-hover:var(--warning-425-625-hover);--background-action-high-warning-active:var(--warning-425-625-active);--background-action-high-error:var(--error-425-625);--background-action-high-error-hover:var(--error-425-625-hover);--background-action-high-error-active:var(--error-425-625-active);--background-action-low-blue-france:var(--blue-france-925-125);--background-action-low-blue-france-hover:var(--blue-france-925-125-hover);--background-action-low-blue-france-active:var(--blue-france-925-125-active);--background-action-low-red-marianne:var(--red-marianne-925-125);--background-action-low-red-marianne-hover:var(--red-marianne-925-125-hover);--background-action-low-red-marianne-active:var(--red-marianne-925-125-active);--background-action-low-green-tilleul-verveine:var(--green-tilleul-verveine-925-125);--background-action-low-green-tilleul-verveine-hover:var(--green-tilleul-verveine-925-125-hover);--background-action-low-green-tilleul-verveine-active:var(--green-tilleul-verveine-925-125-active);--background-action-low-green-bourgeon:var(--green-bourgeon-925-125);--background-action-low-green-bourgeon-hover:var(--green-bourgeon-925-125-hover);--background-action-low-green-bourgeon-active:var(--green-bourgeon-925-125-active);--background-action-low-green-emeraude:var(--green-emeraude-925-125);--background-action-low-green-emeraude-hover:var(--green-emeraude-925-125-hover);--background-action-low-green-emeraude-active:var(--green-emeraude-925-125-active);--background-action-low-green-menthe:var(--green-menthe-925-125);--background-action-low-green-menthe-hover:var(--green-menthe-925-125-hover);--background-action-low-green-menthe-active:var(--green-menthe-925-125-active);--background-action-low-green-archipel:var(--green-archipel-925-125);--background-action-low-green-archipel-hover:var(--green-archipel-925-125-hover);--background-action-low-green-archipel-active:var(--green-archipel-925-125-active);--background-action-low-blue-ecume:var(--blue-ecume-925-125);--background-action-low-blue-ecume-hover:var(--blue-ecume-925-125-hover);--background-action-low-blue-ecume-active:var(--blue-ecume-925-125-active);--background-action-low-blue-cumulus:var(--blue-cumulus-925-125);--background-action-low-blue-cumulus-hover:var(--blue-cumulus-925-125-hover);--background-action-low-blue-cumulus-active:var(--blue-cumulus-925-125-active);--background-action-low-purple-glycine:var(--purple-glycine-925-125);--background-action-low-purple-glycine-hover:var(--purple-glycine-925-125-hover);--background-action-low-purple-glycine-active:var(--purple-glycine-925-125-active);--background-action-low-pink-macaron:var(--pink-macaron-925-125);--background-action-low-pink-macaron-hover:var(--pink-macaron-925-125-hover);--background-action-low-pink-macaron-active:var(--pink-macaron-925-125-active);--background-action-low-pink-tuile:var(--pink-tuile-925-125);--background-action-low-pink-tuile-hover:var(--pink-tuile-925-125-hover);--background-action-low-pink-tuile-active:var(--pink-tuile-925-125-active);--background-action-low-yellow-tournesol:var(--yellow-tournesol-925-125);--background-action-low-yellow-tournesol-hover:var(--yellow-tournesol-925-125-hover);--background-action-low-yellow-tournesol-active:var(--yellow-tournesol-925-125-active);--background-action-low-yellow-moutarde:var(--yellow-moutarde-925-125);--background-action-low-yellow-moutarde-hover:var(--yellow-moutarde-925-125-hover);--background-action-low-yellow-moutarde-active:var(--yellow-moutarde-925-125-active);--background-action-low-orange-terre-battue:var(--orange-terre-battue-925-125);--background-action-low-orange-terre-battue-hover:var(--orange-terre-battue-925-125-hover);--background-action-low-orange-terre-battue-active:var(--orange-terre-battue-925-125-active);--background-action-low-brown-cafe-creme:var(--brown-cafe-creme-925-125);--background-action-low-brown-cafe-creme-hover:var(--brown-cafe-creme-925-125-hover);--background-action-low-brown-cafe-creme-active:var(--brown-cafe-creme-925-125-active);--background-action-low-brown-caramel:var(--brown-caramel-925-125);--background-action-low-brown-caramel-hover:var(--brown-caramel-925-125-hover);--background-action-low-brown-caramel-active:var(--brown-caramel-925-125-active);--background-action-low-brown-opera:var(--brown-opera-925-125);--background-action-low-brown-opera-hover:var(--brown-opera-925-125-hover);--background-action-low-brown-opera-active:var(--brown-opera-925-125-active);--background-action-low-beige-gris-galet:var(--beige-gris-galet-925-125);--background-action-low-beige-gris-galet-hover:var(--beige-gris-galet-925-125-hover);--background-action-low-beige-gris-galet-active:var(--beige-gris-galet-925-125-active);--background-active-blue-france:var(--blue-france-sun-113-625);--background-active-blue-france-hover:var(--blue-france-sun-113-625-hover);--background-active-blue-france-active:var(--blue-france-sun-113-625-active);--background-active-red-marianne:var(--red-marianne-425-625);--background-active-red-marianne-hover:var(--red-marianne-425-625-hover);--background-active-red-marianne-active:var(--red-marianne-425-625-active);--background-open-blue-france:var(--blue-france-925-125);--background-open-blue-france-hover:var(--blue-france-925-125-hover);--background-open-blue-france-active:var(--blue-france-925-125-active);--background-open-red-marianne:var(--red-marianne-925-125);--background-open-red-marianne-hover:var(--red-marianne-925-125-hover);--background-open-red-marianne-active:var(--red-marianne-925-125-active);--background-disabled-grey:var(--grey-925-125);--background-raised-grey:var(--grey-1000-75);--background-raised-grey-hover:var(--grey-1000-75-hover);--background-raised-grey-active:var(--grey-1000-75-active);--background-overlap-grey:var(--grey-1000-100);--background-overlap-grey-hover:var(--grey-1000-100-hover);--background-overlap-grey-active:var(--grey-1000-100-active);--background-lifted-grey:var(--grey-1000-75);--background-lifted-grey-hover:var(--grey-1000-75-hover);--background-lifted-grey-active:var(--grey-1000-75-active);--background-alt-raised-grey:var(--grey-975-100);--background-alt-raised-grey-hover:var(--grey-975-100-hover);--background-alt-raised-grey-active:var(--grey-975-100-active);--background-alt-overlap-grey:var(--grey-975-125);--background-alt-overlap-grey-hover:var(--grey-975-125-hover);--background-alt-overlap-grey-active:var(--grey-975-125-active);--background-contrast-raised-grey:var(--grey-950-125);--background-contrast-raised-grey-hover:var(--grey-950-125-hover);--background-contrast-raised-grey-active:var(--grey-950-125-active);--background-contrast-overlap-grey:var(--grey-950-150);--background-contrast-overlap-grey-hover:var(--grey-950-150-hover);--background-contrast-overlap-grey-active:var(--grey-950-150-active);--text-default-grey:var(--grey-200-850);--text-default-info:var(--info-425-625);--text-default-success:var(--success-425-625);--text-default-warning:var(--warning-425-625);--text-default-error:var(--error-425-625);--text-action-high-grey:var(--grey-50-1000);--text-action-high-blue-france:var(--blue-france-sun-113-625);--text-action-high-red-marianne:var(--red-marianne-425-625);--text-action-high-green-tilleul-verveine:var(--green-tilleul-verveine-sun-418-moon-817);--text-action-high-green-bourgeon:var(--green-bourgeon-sun-425-moon-759);--text-action-high-green-emeraude:var(--green-emeraude-sun-425-moon-753);--text-action-high-green-menthe:var(--green-menthe-sun-373-moon-652);--text-action-high-green-archipel:var(--green-archipel-sun-391-moon-716);--text-action-high-blue-ecume:var(--blue-ecume-sun-247-moon-675);--text-action-high-blue-cumulus:var(--blue-cumulus-sun-368-moon-732);--text-action-high-purple-glycine:var(--purple-glycine-sun-319-moon-630);--text-action-high-pink-macaron:var(--pink-macaron-sun-406-moon-833);--text-action-high-pink-tuile:var(--pink-tuile-sun-425-moon-750);--text-action-high-yellow-tournesol:var(--yellow-tournesol-sun-407-moon-922);--text-action-high-yellow-moutarde:var(--yellow-moutarde-sun-348-moon-860);--text-action-high-orange-terre-battue:var(--orange-terre-battue-sun-370-moon-672);--text-action-high-brown-cafe-creme:var(--brown-cafe-creme-sun-383-moon-885);--text-action-high-brown-caramel:var(--brown-caramel-sun-425-moon-901);--text-action-high-brown-opera:var(--brown-opera-sun-395-moon-820);--text-action-high-beige-gris-galet:var(--beige-gris-galet-sun-407-moon-821);--text-title-grey:var(--grey-50-1000);--text-title-blue-france:var(--blue-france-sun-113-625);--text-title-red-marianne:var(--red-marianne-425-625);--text-label-grey:var(--grey-50-1000);--text-label-blue-france:var(--blue-france-sun-113-625);--text-label-red-marianne:var(--red-marianne-425-625);--text-label-green-tilleul-verveine:var(--green-tilleul-verveine-sun-418-moon-817);--text-label-green-bourgeon:var(--green-bourgeon-sun-425-moon-759);--text-label-green-emeraude:var(--green-emeraude-sun-425-moon-753);--text-label-green-menthe:var(--green-menthe-sun-373-moon-652);--text-label-green-archipel:var(--green-archipel-sun-391-moon-716);--text-label-blue-ecume:var(--blue-ecume-sun-247-moon-675);--text-label-blue-cumulus:var(--blue-cumulus-sun-368-moon-732);--text-label-purple-glycine:var(--purple-glycine-sun-319-moon-630);--text-label-pink-macaron:var(--pink-macaron-sun-406-moon-833);--text-label-pink-tuile:var(--pink-tuile-sun-425-moon-750);--text-label-yellow-tournesol:var(--yellow-tournesol-sun-407-moon-922);--text-label-yellow-moutarde:var(--yellow-moutarde-sun-348-moon-860);--text-label-orange-terre-battue:var(--orange-terre-battue-sun-370-moon-672);--text-label-brown-cafe-creme:var(--brown-cafe-creme-sun-383-moon-885);--text-label-brown-caramel:var(--brown-caramel-sun-425-moon-901);--text-label-brown-opera:var(--brown-opera-sun-395-moon-820);--text-label-beige-gris-galet:var(--beige-gris-galet-sun-407-moon-821);--text-active-grey:var(--grey-50-1000);--text-active-blue-france:var(--blue-france-sun-113-625);--text-active-red-marianne:var(--red-marianne-425-625);--text-mention-grey:var(--grey-425-625);--text-inverted-grey:var(--grey-1000-50);--text-inverted-blue-france:var(--blue-france-975-sun-113);--text-inverted-red-marianne:var(--red-marianne-975-75);--text-inverted-info:var(--info-975-75);--text-inverted-success:var(--success-975-75);--text-inverted-warning:var(--warning-975-75);--text-inverted-error:var(--error-975-75);--text-inverted-green-tilleul-verveine:var(--green-tilleul-verveine-975-75);--text-inverted-green-bourgeon:var(--green-bourgeon-975-75);--text-inverted-green-emeraude:var(--green-emeraude-975-75);--text-inverted-green-menthe:var(--green-menthe-975-75);--text-inverted-green-archipel:var(--green-archipel-975-75);--text-inverted-blue-ecume:var(--blue-ecume-975-75);--text-inverted-blue-cumulus:var(--blue-cumulus-975-75);--text-inverted-purple-glycine:var(--purple-glycine-975-75);--text-inverted-pink-macaron:var(--pink-macaron-975-75);--text-inverted-pink-tuile:var(--pink-tuile-975-75);--text-inverted-yellow-tournesol:var(--yellow-tournesol-975-75);--text-inverted-yellow-moutarde:var(--yellow-moutarde-975-75);--text-inverted-orange-terre-battue:var(--orange-terre-battue-975-75);--text-inverted-brown-cafe-creme:var(--brown-cafe-creme-975-75);--text-inverted-brown-caramel:var(--brown-caramel-975-75);--text-inverted-brown-opera:var(--brown-opera-975-75);--text-inverted-beige-gris-galet:var(--beige-gris-galet-975-75);--text-disabled-grey:var(--grey-625-425);--border-default-grey:var(--grey-900-175);--border-default-blue-france:var(--blue-france-main-525);--border-default-red-marianne:var(--red-marianne-main-472);--border-default-green-tilleul-verveine:var(--green-tilleul-verveine-main-707);--border-default-green-bourgeon:var(--green-bourgeon-main-640);--border-default-green-emeraude:var(--green-emeraude-main-632);--border-default-green-menthe:var(--green-menthe-main-548);--border-default-green-archipel:var(--green-archipel-main-557);--border-default-blue-ecume:var(--blue-ecume-main-400);--border-default-blue-cumulus:var(--blue-cumulus-main-526);--border-default-purple-glycine:var(--purple-glycine-main-494);--border-default-pink-macaron:var(--pink-macaron-main-689);--border-default-pink-tuile:var(--pink-tuile-main-556);--border-default-yellow-tournesol:var(--yellow-tournesol-main-731);--border-default-yellow-moutarde:var(--yellow-moutarde-main-679);--border-default-orange-terre-battue:var(--orange-terre-battue-main-645);--border-default-brown-cafe-creme:var(--brown-cafe-creme-main-782);--border-default-brown-caramel:var(--brown-caramel-main-648);--border-default-brown-opera:var(--brown-opera-main-680);--border-default-beige-gris-galet:var(--beige-gris-galet-main-702);--border-active-blue-france:var(--blue-france-sun-113-625);--border-active-red-marianne:var(--red-marianne-425-625);--border-action-high-grey:var(--grey-50-1000);--border-action-high-blue-france:var(--blue-france-sun-113-625);--border-action-high-red-marianne:var(--red-marianne-425-625);--border-action-high-info:var(--info-425-625);--border-action-high-success:var(--success-425-625);--border-action-high-warning:var(--warning-425-625);--border-action-high-error:var(--error-425-625);--border-action-low-blue-france:var(--blue-france-850-200);--border-action-low-red-marianne:var(--red-marianne-850-200);--border-action-low-green-tilleul-verveine:var(--green-tilleul-verveine-850-200);--border-action-low-green-bourgeon:var(--green-bourgeon-850-200);--border-action-low-green-emeraude:var(--green-emeraude-850-200);--border-action-low-green-menthe:var(--green-menthe-850-200);--border-action-low-green-archipel:var(--green-archipel-850-200);--border-action-low-blue-ecume:var(--blue-ecume-850-200);--border-action-low-blue-cumulus:var(--blue-cumulus-850-200);--border-action-low-purple-glycine:var(--purple-glycine-850-200);--border-action-low-pink-macaron:var(--pink-macaron-850-200);--border-action-low-pink-tuile:var(--pink-tuile-850-200);--border-action-low-yellow-tournesol:var(--yellow-tournesol-850-200);--border-action-low-yellow-moutarde:var(--yellow-moutarde-850-200);--border-action-low-orange-terre-battue:var(--orange-terre-battue-850-200);--border-action-low-brown-cafe-creme:var(--brown-cafe-creme-850-200);--border-action-low-brown-caramel:var(--brown-caramel-850-200);--border-action-low-brown-opera:var(--brown-opera-850-200);--border-action-low-beige-gris-galet:var(--beige-gris-galet-850-200);--border-open-blue-france:var(--blue-france-925-125);--border-open-red-marianne:var(--red-marianne-925-125);--border-plain-grey:var(--grey-200-850);--border-plain-blue-france:var(--blue-france-sun-113-625);--border-plain-red-marianne:var(--red-marianne-425-625);--border-plain-info:var(--info-425-625);--border-plain-success:var(--success-425-625);--border-plain-warning:var(--warning-425-625);--border-plain-error:var(--error-425-625);--border-plain-green-tilleul-verveine:var(--green-tilleul-verveine-sun-418-moon-817);--border-plain-green-bourgeon:var(--green-bourgeon-sun-425-moon-759);--border-plain-green-emeraude:var(--green-emeraude-sun-425-moon-753);--border-plain-green-menthe:var(--green-menthe-sun-373-moon-652);--border-plain-green-archipel:var(--green-archipel-sun-391-moon-716);--border-plain-blue-ecume:var(--blue-ecume-sun-247-moon-675);--border-plain-blue-cumulus:var(--blue-cumulus-sun-368-moon-732);--border-plain-purple-glycine:var(--purple-glycine-sun-319-moon-630);--border-plain-pink-macaron:var(--pink-macaron-sun-406-moon-833);--border-plain-pink-tuile:var(--pink-tuile-sun-425-moon-750);--border-plain-yellow-tournesol:var(--yellow-tournesol-sun-407-moon-922);--border-plain-yellow-moutarde:var(--yellow-moutarde-sun-348-moon-860);--border-plain-orange-terre-battue:var(--orange-terre-battue-sun-370-moon-672);--border-plain-brown-cafe-creme:var(--brown-cafe-creme-sun-383-moon-885);--border-plain-brown-caramel:var(--brown-caramel-sun-425-moon-901);--border-plain-brown-opera:var(--brown-opera-sun-395-moon-820);--border-plain-beige-gris-galet:var(--beige-gris-galet-sun-407-moon-821);--border-disabled-grey:var(--grey-925-125);--artwork-major-blue-france:var(--blue-france-sun-113-625);--artwork-major-blue-france-hover:var(--blue-france-sun-113-625-hover);--artwork-major-blue-france-active:var(--blue-france-sun-113-625-active);--artwork-major-red-marianne:var(--red-marianne-425-625);--artwork-major-red-marianne-hover:var(--red-marianne-425-625-hover);--artwork-major-red-marianne-active:var(--red-marianne-425-625-active);--artwork-major-green-tilleul-verveine:var(--green-tilleul-verveine-sun-418-moon-817);--artwork-major-green-tilleul-verveine-hover:var(--green-tilleul-verveine-sun-418-moon-817-hover);--artwork-major-green-tilleul-verveine-active:var(--green-tilleul-verveine-sun-418-moon-817-active);--artwork-major-green-bourgeon:var(--green-bourgeon-sun-425-moon-759);--artwork-major-green-bourgeon-hover:var(--green-bourgeon-sun-425-moon-759-hover);--artwork-major-green-bourgeon-active:var(--green-bourgeon-sun-425-moon-759-active);--artwork-major-green-emeraude:var(--green-emeraude-sun-425-moon-753);--artwork-major-green-emeraude-hover:var(--green-emeraude-sun-425-moon-753-hover);--artwork-major-green-emeraude-active:var(--green-emeraude-sun-425-moon-753-active);--artwork-major-green-menthe:var(--green-menthe-sun-373-moon-652);--artwork-major-green-menthe-hover:var(--green-menthe-sun-373-moon-652-hover);--artwork-major-green-menthe-active:var(--green-menthe-sun-373-moon-652-active);--artwork-major-green-archipel:var(--green-archipel-sun-391-moon-716);--artwork-major-green-archipel-hover:var(--green-archipel-sun-391-moon-716-hover);--artwork-major-green-archipel-active:var(--green-archipel-sun-391-moon-716-active);--artwork-major-blue-ecume:var(--blue-ecume-sun-247-moon-675);--artwork-major-blue-ecume-hover:var(--blue-ecume-sun-247-moon-675-hover);--artwork-major-blue-ecume-active:var(--blue-ecume-sun-247-moon-675-active);--artwork-major-blue-cumulus:var(--blue-cumulus-sun-368-moon-732);--artwork-major-blue-cumulus-hover:var(--blue-cumulus-sun-368-moon-732-hover);--artwork-major-blue-cumulus-active:var(--blue-cumulus-sun-368-moon-732-active);--artwork-major-purple-glycine:var(--purple-glycine-sun-319-moon-630);--artwork-major-purple-glycine-hover:var(--purple-glycine-sun-319-moon-630-hover);--artwork-major-purple-glycine-active:var(--purple-glycine-sun-319-moon-630-active);--artwork-major-pink-macaron:var(--pink-macaron-sun-406-moon-833);--artwork-major-pink-macaron-hover:var(--pink-macaron-sun-406-moon-833-hover);--artwork-major-pink-macaron-active:var(--pink-macaron-sun-406-moon-833-active);--artwork-major-pink-tuile:var(--pink-tuile-sun-425-moon-750);--artwork-major-pink-tuile-hover:var(--pink-tuile-sun-425-moon-750-hover);--artwork-major-pink-tuile-active:var(--pink-tuile-sun-425-moon-750-active);--artwork-major-yellow-tournesol:var(--yellow-tournesol-sun-407-moon-922);--artwork-major-yellow-tournesol-hover:var(--yellow-tournesol-sun-407-moon-922-hover);--artwork-major-yellow-tournesol-active:var(--yellow-tournesol-sun-407-moon-922-active);--artwork-major-yellow-moutarde:var(--yellow-moutarde-sun-348-moon-860);--artwork-major-yellow-moutarde-hover:var(--yellow-moutarde-sun-348-moon-860-hover);--artwork-major-yellow-moutarde-active:var(--yellow-moutarde-sun-348-moon-860-active);--artwork-major-orange-terre-battue:var(--orange-terre-battue-sun-370-moon-672);--artwork-major-orange-terre-battue-hover:var(--orange-terre-battue-sun-370-moon-672-hover);--artwork-major-orange-terre-battue-active:var(--orange-terre-battue-sun-370-moon-672-active);--artwork-major-brown-cafe-creme:var(--brown-cafe-creme-sun-383-moon-885);--artwork-major-brown-cafe-creme-hover:var(--brown-cafe-creme-sun-383-moon-885-hover);--artwork-major-brown-cafe-creme-active:var(--brown-cafe-creme-sun-383-moon-885-active);--artwork-major-brown-caramel:var(--brown-caramel-sun-425-moon-901);--artwork-major-brown-caramel-hover:var(--brown-caramel-sun-425-moon-901-hover);--artwork-major-brown-caramel-active:var(--brown-caramel-sun-425-moon-901-active);--artwork-major-brown-opera:var(--brown-opera-sun-395-moon-820);--artwork-major-brown-opera-hover:var(--brown-opera-sun-395-moon-820-hover);--artwork-major-brown-opera-active:var(--brown-opera-sun-395-moon-820-active);--artwork-major-beige-gris-galet:var(--beige-gris-galet-sun-407-moon-821);--artwork-major-beige-gris-galet-hover:var(--beige-gris-galet-sun-407-moon-821-hover);--artwork-major-beige-gris-galet-active:var(--beige-gris-galet-sun-407-moon-821-active);--artwork-minor-blue-france:var(--blue-france-main-525);--artwork-minor-red-marianne:var(--red-marianne-main-472);--artwork-minor-green-tilleul-verveine:var(--green-tilleul-verveine-main-707);--artwork-minor-green-bourgeon:var(--green-bourgeon-main-640);--artwork-minor-green-emeraude:var(--green-emeraude-main-632);--artwork-minor-green-menthe:var(--green-menthe-main-548);--artwork-minor-green-archipel:var(--green-archipel-main-557);--artwork-minor-blue-ecume:var(--blue-ecume-main-400);--artwork-minor-blue-cumulus:var(--blue-cumulus-main-526);--artwork-minor-purple-glycine:var(--purple-glycine-main-494);--artwork-minor-pink-macaron:var(--pink-macaron-main-689);--artwork-minor-pink-tuile:var(--pink-tuile-main-556);--artwork-minor-yellow-tournesol:var(--yellow-tournesol-main-731);--artwork-minor-yellow-moutarde:var(--yellow-moutarde-main-679);--artwork-minor-orange-terre-battue:var(--orange-terre-battue-main-645);--artwork-minor-brown-cafe-creme:var(--brown-cafe-creme-main-782);--artwork-minor-brown-caramel:var(--brown-caramel-main-648);--artwork-minor-brown-opera:var(--brown-opera-main-680);--artwork-minor-beige-gris-galet:var(--beige-gris-galet-main-702);--artwork-decorative-grey:var(--grey-950-100);--artwork-decorative-blue-france:var(--blue-france-950-100);--artwork-decorative-red-marianne:var(--red-marianne-950-100);--artwork-decorative-green-tilleul-verveine:var(--green-tilleul-verveine-950-100);--artwork-decorative-green-bourgeon:var(--green-bourgeon-950-100);--artwork-decorative-green-emeraude:var(--green-emeraude-950-100);--artwork-decorative-green-menthe:var(--green-menthe-950-100);--artwork-decorative-green-archipel:var(--green-archipel-950-100);--artwork-decorative-blue-ecume:var(--blue-ecume-950-100);--artwork-decorative-blue-cumulus:var(--blue-cumulus-950-100);--artwork-decorative-purple-glycine:var(--purple-glycine-950-100);--artwork-decorative-pink-macaron:var(--pink-macaron-950-100);--artwork-decorative-pink-tuile:var(--pink-tuile-950-100);--artwork-decorative-yellow-tournesol:var(--yellow-tournesol-950-100);--artwork-decorative-yellow-moutarde:var(--yellow-moutarde-950-100);--artwork-decorative-orange-terre-battue:var(--orange-terre-battue-950-100);--artwork-decorative-brown-cafe-creme:var(--brown-cafe-creme-950-100);--artwork-decorative-brown-caramel:var(--brown-caramel-950-100);--artwork-decorative-brown-opera:var(--brown-opera-950-100);--artwork-decorative-beige-gris-galet:var(--beige-gris-galet-950-100);--artwork-background-grey:var(--grey-975-75);--artwork-background-blue-france:var(--blue-france-975-75);--artwork-background-red-marianne:var(--red-marianne-975-75);--artwork-background-green-tilleul-verveine:var(--green-tilleul-verveine-975-75);--artwork-background-green-bourgeon:var(--green-bourgeon-975-75);--artwork-background-green-emeraude:var(--green-emeraude-975-75);--artwork-background-green-menthe:var(--green-menthe-975-75);--artwork-background-green-archipel:var(--green-archipel-975-75);--artwork-background-blue-ecume:var(--blue-ecume-975-75);--artwork-background-blue-cumulus:var(--blue-cumulus-975-75);--artwork-background-purple-glycine:var(--purple-glycine-975-75);--artwork-background-pink-macaron:var(--pink-macaron-975-75);--artwork-background-pink-tuile:var(--pink-tuile-975-75);--artwork-background-yellow-tournesol:var(--yellow-tournesol-975-75);--artwork-background-yellow-moutarde:var(--yellow-moutarde-975-75);--artwork-background-orange-terre-battue:var(--orange-terre-battue-975-75);--artwork-background-brown-cafe-creme:var(--brown-cafe-creme-975-75);--artwork-background-brown-caramel:var(--brown-caramel-975-75);--artwork-background-brown-opera:var(--brown-opera-975-75);--artwork-background-beige-gris-galet:var(--beige-gris-galet-975-75);--artwork-motif-grey:var(--grey-925-125);--artwork-motif-blue-france:var(--blue-france-925-125);--artwork-motif-red-marianne:var(--red-marianne-925-125);--artwork-motif-green-tilleul-verveine:var(--green-tilleul-verveine-925-125);--artwork-motif-green-bourgeon:var(--green-bourgeon-925-125);--artwork-motif-green-emeraude:var(--green-emeraude-925-125);--artwork-motif-green-menthe:var(--green-menthe-925-125);--artwork-motif-green-archipel:var(--green-archipel-925-125);--artwork-motif-blue-ecume:var(--blue-ecume-925-125);--artwork-motif-blue-cumulus:var(--blue-cumulus-925-125);--artwork-motif-purple-glycine:var(--purple-glycine-925-125);--artwork-motif-pink-macaron:var(--pink-macaron-925-125);--artwork-motif-pink-tuile:var(--pink-tuile-925-125);--artwork-motif-yellow-tournesol:var(--yellow-tournesol-925-125);--artwork-motif-yellow-moutarde:var(--yellow-moutarde-925-125);--artwork-motif-orange-terre-battue:var(--orange-terre-battue-925-125);--artwork-motif-brown-cafe-creme:var(--brown-cafe-creme-925-125);--artwork-motif-brown-caramel:var(--brown-caramel-925-125);--artwork-motif-brown-opera:var(--brown-opera-925-125);--artwork-motif-beige-gris-galet:var(--beige-gris-galet-925-125);--grey-1000-50:#fff;--grey-1000-50-hover:#f6f6f6;--grey-1000-50-active:#ededed;--grey-975-75:#f6f6f6;--grey-975-75-hover:#dfdfdf;--grey-975-75-active:#cfcfcf;--grey-950-100:#eee;--grey-950-100-hover:#d2d2d2;--grey-950-100-active:#c1c1c1;--grey-200-850:#3a3a3a;--grey-925-125:#e5e5e5;--grey-1000-75:#fff;--grey-1000-75-hover:#f6f6f6;--grey-1000-75-active:#ededed;--grey-1000-100:#fff;--grey-1000-100-hover:#f6f6f6;--grey-1000-100-active:#ededed;--grey-975-100:#f6f6f6;--grey-975-100-hover:#dfdfdf;--grey-975-100-active:#cfcfcf;--grey-975-125:#f6f6f6;--grey-975-125-hover:#dfdfdf;--grey-975-125-active:#cfcfcf;--grey-950-125:#eee;--grey-950-125-hover:#d2d2d2;--grey-950-125-active:#c1c1c1;--grey-950-150:#eee;--grey-950-150-hover:#d2d2d2;--grey-950-150-active:#c1c1c1;--grey-50-1000:#161616;--grey-425-625:#666;--grey-625-425:#929292;--grey-900-175:#ddd;--blue-france-975-75:#f5f5fe;--blue-france-975-75-hover:#dcdcfc;--blue-france-975-75-active:#cbcbfa;--blue-france-950-100:#ececfe;--blue-france-950-100-hover:#cecefc;--blue-france-950-100-active:#bbbbfc;--blue-france-sun-113-625:#000091;--blue-france-sun-113-625-hover:#1212ff;--blue-france-sun-113-625-active:#2323ff;--blue-france-925-125:#e3e3fd;--blue-france-925-125-hover:#c1c1fb;--blue-france-925-125-active:#adadf9;--blue-france-975-sun-113:#f5f5fe;--blue-france-main-525:#6a6af4;--blue-france-850-200:#cacafb;--red-marianne-975-75:#fef4f4;--red-marianne-975-75-hover:#fcd7d7;--red-marianne-975-75-active:#fac4c4;--red-marianne-950-100:#fee9e9;--red-marianne-950-100-hover:#fdc5c5;--red-marianne-950-100-active:#fcafaf;--red-marianne-425-625:#c9191e;--red-marianne-425-625-hover:#f93f42;--red-marianne-425-625-active:#f95a5c;--red-marianne-925-125:#fddede;--red-marianne-925-125-hover:#fbb6b6;--red-marianne-925-125-active:#fa9e9e;--red-marianne-main-472:#e1000f;--red-marianne-850-200:#fcbfbf;--info-950-100:#e8edff;--info-950-100-hover:#c2d1ff;--info-950-100-active:#a9bfff;--info-425-625:#0063cb;--info-425-625-hover:#3b87ff;--info-425-625-active:#6798ff;--info-975-75:#f4f6ff;--success-950-100:#b8fec9;--success-950-100-hover:#46fd89;--success-950-100-active:#34eb7b;--success-425-625:#18753c;--success-425-625-hover:#27a959;--success-425-625-active:#2fc368;--success-975-75:#dffee6;--warning-950-100:#ffe9e6;--warning-950-100-hover:#ffc6bd;--warning-950-100-active:#ffb0a2;--warning-425-625:#b34000;--warning-425-625-hover:#ff6218;--warning-425-625-active:#ff7a55;--warning-975-75:#fff4f3;--error-950-100:#ffe9e9;--error-950-100-hover:#ffc5c5;--error-950-100-active:#ffafaf;--error-425-625:#ce0500;--error-425-625-hover:#ff2725;--error-425-625-active:#ff4140;--error-975-75:#fff4f4;--green-tilleul-verveine-975-75:#fef7da;--green-tilleul-verveine-975-75-hover:#fce552;--green-tilleul-verveine-975-75-active:#ebd54c;--green-tilleul-verveine-950-100:#fceeac;--green-tilleul-verveine-950-100-hover:#e8d45c;--green-tilleul-verveine-950-100-active:#d4c254;--green-tilleul-verveine-sun-418-moon-817:#66673d;--green-tilleul-verveine-sun-418-moon-817-hover:#929359;--green-tilleul-verveine-sun-418-moon-817-active:#a7a967;--green-tilleul-verveine-925-125:#fbe769;--green-tilleul-verveine-925-125-hover:#d7c655;--green-tilleul-verveine-925-125-active:#c2b24c;--green-tilleul-verveine-main-707:#b7a73f;--green-tilleul-verveine-850-200:#e2cf58;--green-bourgeon-975-75:#e6feda;--green-bourgeon-975-75-hover:#a7fc62;--green-bourgeon-975-75-active:#98ed4d;--green-bourgeon-950-100:#c9fcac;--green-bourgeon-950-100-hover:#9ae95d;--green-bourgeon-950-100-active:#8dd555;--green-bourgeon-sun-425-moon-759:#447049;--green-bourgeon-sun-425-moon-759-hover:#639f6a;--green-bourgeon-sun-425-moon-759-active:#72b77a;--green-bourgeon-925-125:#a9fb68;--green-bourgeon-925-125-hover:#8ed654;--green-bourgeon-925-125-active:#7fc04b;--green-bourgeon-main-640:#68a532;--green-bourgeon-850-200:#95e257;--green-emeraude-975-75:#e3fdeb;--green-emeraude-975-75-hover:#94f9b9;--green-emeraude-975-75-active:#6df1a3;--green-emeraude-950-100:#c3fad5;--green-emeraude-950-100-hover:#77eda5;--green-emeraude-950-100-active:#6dd897;--green-emeraude-sun-425-moon-753:#297254;--green-emeraude-sun-425-moon-753-hover:#3ea47a;--green-emeraude-sun-425-moon-753-active:#49bc8d;--green-emeraude-925-125:#9ef9be;--green-emeraude-925-125-hover:#69df97;--green-emeraude-925-125-active:#5ec988;--green-emeraude-main-632:#00a95f;--green-emeraude-850-200:#6fe49d;--green-menthe-975-75:#dffdf7;--green-menthe-975-75-hover:#84f9e7;--green-menthe-975-75-active:#70ebd8;--green-menthe-950-100:#bafaee;--green-menthe-950-100-hover:#79e7d5;--green-menthe-950-100-active:#6fd3c3;--green-menthe-sun-373-moon-652:#37635f;--green-menthe-sun-373-moon-652-hover:#53918c;--green-menthe-sun-373-moon-652-active:#62a9a2;--green-menthe-925-125:#8bf8e7;--green-menthe-925-125-hover:#6ed5c5;--green-menthe-925-125-active:#62bfb1;--green-menthe-main-548:#009081;--green-menthe-850-200:#73e0cf;--green-archipel-975-75:#e5fbfd;--green-archipel-975-75-hover:#99f2f8;--green-archipel-975-75-active:#73e9f0;--green-archipel-950-100:#c7f6fc;--green-archipel-950-100-hover:#64ecf8;--green-archipel-950-100-active:#5bd8e3;--green-archipel-sun-391-moon-716:#006a6f;--green-archipel-sun-391-moon-716-hover:#009fa7;--green-archipel-sun-391-moon-716-active:#00bbc3;--green-archipel-925-125:#a6f2fa;--green-archipel-925-125-hover:#62dbe5;--green-archipel-925-125-active:#58c5cf;--green-archipel-main-557:#009099;--green-archipel-850-200:#60e0eb;--blue-ecume-975-75:#f4f6fe;--blue-ecume-975-75-hover:#d7dffb;--blue-ecume-975-75-active:#c3cffa;--blue-ecume-950-100:#e9edfe;--blue-ecume-950-100-hover:#c5d0fc;--blue-ecume-950-100-active:#adbffc;--blue-ecume-sun-247-moon-675:#2f4077;--blue-ecume-sun-247-moon-675-hover:#4e68bb;--blue-ecume-sun-247-moon-675-active:#667dcf;--blue-ecume-925-125:#dee5fd;--blue-ecume-925-125-hover:#b4c5fb;--blue-ecume-925-125-active:#99b3f9;--blue-ecume-main-400:#465f9d;--blue-ecume-850-200:#bfccfb;--blue-cumulus-975-75:#f3f6fe;--blue-cumulus-975-75-hover:#d3dffc;--blue-cumulus-975-75-active:#bed0fa;--blue-cumulus-950-100:#e6eefe;--blue-cumulus-950-100-hover:#bcd3fc;--blue-cumulus-950-100-active:#9fc3fc;--blue-cumulus-sun-368-moon-732:#3558a2;--blue-cumulus-sun-368-moon-732-hover:#5982e0;--blue-cumulus-sun-368-moon-732-active:#7996e6;--blue-cumulus-925-125:#dae6fd;--blue-cumulus-925-125-hover:#a9c8fb;--blue-cumulus-925-125-active:#8ab8f9;--blue-cumulus-main-526:#417dc4;--blue-cumulus-850-200:#b6cffb;--purple-glycine-975-75:#fef3fd;--purple-glycine-975-75-hover:#fcd4f8;--purple-glycine-975-75-active:#fabff5;--purple-glycine-950-100:#fee7fc;--purple-glycine-950-100-hover:#fdc0f8;--purple-glycine-950-100-active:#fca8f6;--purple-glycine-sun-319-moon-630:#6e445a;--purple-glycine-sun-319-moon-630-hover:#a66989;--purple-glycine-sun-319-moon-630-active:#bb7f9e;--purple-glycine-925-125:#fddbfa;--purple-glycine-925-125-hover:#fbaff5;--purple-glycine-925-125-active:#fa96f2;--purple-glycine-main-494:#a558a0;--purple-glycine-850-200:#fbb8f6;--pink-macaron-975-75:#fef4f2;--pink-macaron-975-75-hover:#fcd8d0;--pink-macaron-975-75-active:#fac5b8;--pink-macaron-950-100:#fee9e6;--pink-macaron-950-100-hover:#fdc6bd;--pink-macaron-950-100-active:#fcb0a2;--pink-macaron-sun-406-moon-833:#8d533e;--pink-macaron-sun-406-moon-833-hover:#ca795c;--pink-macaron-sun-406-moon-833-active:#e08e73;--pink-macaron-925-125:#fddfda;--pink-macaron-925-125-hover:#fbb8ab;--pink-macaron-925-125-active:#faa18d;--pink-macaron-main-689:#e18b76;--pink-macaron-850-200:#fcc0b4;--pink-tuile-975-75:#fef4f3;--pink-tuile-975-75-hover:#fcd7d3;--pink-tuile-975-75-active:#fac4be;--pink-tuile-950-100:#fee9e7;--pink-tuile-950-100-hover:#fdc6c0;--pink-tuile-950-100-active:#fcb0a7;--pink-tuile-sun-425-moon-750:#a94645;--pink-tuile-sun-425-moon-750-hover:#d5706f;--pink-tuile-sun-425-moon-750-active:#da8a89;--pink-tuile-925-125:#fddfdb;--pink-tuile-925-125-hover:#fbb8ad;--pink-tuile-925-125-active:#faa191;--pink-tuile-main-556:#ce614a;--pink-tuile-850-200:#fcbfb7;--yellow-tournesol-975-75:#fef6e3;--yellow-tournesol-975-75-hover:#fce086;--yellow-tournesol-975-75-active:#f5d24b;--yellow-tournesol-950-100:#feecc2;--yellow-tournesol-950-100-hover:#fbd335;--yellow-tournesol-950-100-active:#e6c130;--yellow-tournesol-sun-407-moon-922:#716043;--yellow-tournesol-sun-407-moon-922-hover:#a28a62;--yellow-tournesol-sun-407-moon-922-active:#ba9f72;--yellow-tournesol-925-125:#fde39c;--yellow-tournesol-925-125-hover:#e9c53b;--yellow-tournesol-925-125-active:#d3b235;--yellow-tournesol-main-731:#c8aa39;--yellow-tournesol-850-200:#efcb3a;--yellow-moutarde-975-75:#fef5e8;--yellow-moutarde-975-75-hover:#fcdca3;--yellow-moutarde-975-75-active:#fbcd64;--yellow-moutarde-950-100:#feebd0;--yellow-moutarde-950-100-hover:#fdcd6d;--yellow-moutarde-950-100-active:#f4be30;--yellow-moutarde-sun-348-moon-860:#695240;--yellow-moutarde-sun-348-moon-860-hover:#9b7b61;--yellow-moutarde-sun-348-moon-860-active:#b58f72;--yellow-moutarde-925-125:#fde2b5;--yellow-moutarde-925-125-hover:#f6c43c;--yellow-moutarde-925-125-active:#dfb135;--yellow-moutarde-main-679:#c3992a;--yellow-moutarde-850-200:#fcc63a;--orange-terre-battue-975-75:#fef4f2;--orange-terre-battue-975-75-hover:#fcd8d0;--orange-terre-battue-975-75-active:#fac5b8;--orange-terre-battue-950-100:#fee9e5;--orange-terre-battue-950-100-hover:#fdc6ba;--orange-terre-battue-950-100-active:#fcb09e;--orange-terre-battue-sun-370-moon-672:#755348;--orange-terre-battue-sun-370-moon-672-hover:#ab7b6b;--orange-terre-battue-sun-370-moon-672-active:#c68f7d;--orange-terre-battue-925-125:#fddfd8;--orange-terre-battue-925-125-hover:#fbb8a5;--orange-terre-battue-925-125-active:#faa184;--orange-terre-battue-main-645:#e4794a;--orange-terre-battue-850-200:#fcc0b0;--brown-cafe-creme-975-75:#fbf6ed;--brown-cafe-creme-975-75-hover:#f2deb6;--brown-cafe-creme-975-75-active:#eacf91;--brown-cafe-creme-950-100:#f7ecdb;--brown-cafe-creme-950-100-hover:#edce94;--brown-cafe-creme-950-100-active:#dabd84;--brown-cafe-creme-sun-383-moon-885:#685c48;--brown-cafe-creme-sun-383-moon-885-hover:#97866a;--brown-cafe-creme-sun-383-moon-885-active:#ae9b7b;--brown-cafe-creme-925-125:#f4e3c7;--brown-cafe-creme-925-125-hover:#e1c386;--brown-cafe-creme-925-125-active:#ccb078;--brown-cafe-creme-main-782:#d1b781;--brown-cafe-creme-850-200:#e7ca8e;--brown-caramel-975-75:#fbf5f2;--brown-caramel-975-75-hover:#f1dbcf;--brown-caramel-975-75-active:#ecc9b5;--brown-caramel-950-100:#f7ebe5;--brown-caramel-950-100-hover:#eccbb9;--brown-caramel-950-100-active:#e6b79a;--brown-caramel-sun-425-moon-901:#845d48;--brown-caramel-sun-425-moon-901-hover:#bb8568;--brown-caramel-sun-425-moon-901-active:#d69978;--brown-caramel-925-125:#f3e2d9;--brown-caramel-925-125-hover:#e7bea6;--brown-caramel-925-125-active:#e1a982;--brown-caramel-main-648:#c08c65;--brown-caramel-850-200:#eac7b2;--brown-opera-975-75:#fbf5f2;--brown-opera-975-75-hover:#f1dbcf;--brown-opera-975-75-active:#ecc9b5;--brown-opera-950-100:#f7ece4;--brown-opera-950-100-hover:#eccdb3;--brown-opera-950-100-active:#e6ba90;--brown-opera-sun-395-moon-820:#745b47;--brown-opera-sun-395-moon-820-hover:#a78468;--brown-opera-sun-395-moon-820-active:#c09979;--brown-opera-925-125:#f3e2d7;--brown-opera-925-125-hover:#e7bfa0;--brown-opera-925-125-active:#deaa7e;--brown-opera-main-680:#bd987a;--brown-opera-850-200:#eac7ad;--beige-gris-galet-975-75:#f9f6f2;--beige-gris-galet-975-75-hover:#eadecd;--beige-gris-galet-975-75-active:#e1ceb1;--beige-gris-galet-950-100:#f3ede5;--beige-gris-galet-950-100-hover:#e1d0b5;--beige-gris-galet-950-100-active:#d1bea2;--beige-gris-galet-sun-407-moon-821:#6a6156;--beige-gris-galet-sun-407-moon-821-hover:#988b7c;--beige-gris-galet-sun-407-moon-821-active:#afa08f;--beige-gris-galet-925-125:#eee4d9;--beige-gris-galet-925-125-hover:#dbc3a4;--beige-gris-galet-925-125-active:#c6b094;--beige-gris-galet-main-702:#aea397;--beige-gris-galet-850-200:#e0cab0;--ground:0;--shadow-color:rgba(0,0,18,.16);--raised-shadow:0 1px 3px var(--shadow-color);--overlap-shadow:0 2px 6px var(--shadow-color);--lifted-shadow:0 3px 9px var(--shadow-color);box-sizing:border-box}[href]{background-image:var(--underline-img),var(--underline-img);background-position:var(--underline-x) 100%,var(--underline-x) calc(100% - var(--underline-thickness));background-repeat:no-repeat,no-repeat;background-size:var(--underline-hover-width) calc(var(--underline-thickness)*2),var(--underline-idle-width) var(--underline-thickness);transition:background-size 0s}[target=_blank]:after,[target=_blank][class*=" fr-fi-"]:after,[target=_blank][class^=fr-fi-]:after{--icon-size:1rem;background-color:currentColor;content:var(--external-link-content);display:inline-block;flex:0 0 auto;height:var(--icon-size);margin-left:.25rem;-webkit-mask-image:url(icons/system/external-link-line.svg);mask-image:url(icons/system/external-link-line.svg);-webkit-mask-size:100% 100%;mask-size:100% 100%;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}button{border:none;color:inherit;font-family:inherit}button,input,select{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:transparent;margin:0}input,select{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;-webkit-text-size-adjust:100%;border:0;border-radius:0;font-family:Marianne,arial,sans-serif;text-rendering:optimizeLegibility}input[type=radio]{-webkit-appearance:auto;-moz-appearance:auto;appearance:auto}a,button,input,input[type=button],input[type=image],input[type=radio]+label:before,select{outline-color:#0a76f6;outline-offset:2px;outline-width:2px}a:focus,button:focus,input:focus,input[type=button]:focus,input[type=image]:focus,input[type=radio]:focus+label:before,select:focus{outline-style:solid}a:focus:not(:focus-visible),button:focus:not(:focus-visible),input:focus:not(:focus-visible),input[type=button]:focus:not(:focus-visible),input[type=image]:focus:not(:focus-visible),input[type=radio]:focus:not(:focus-visible)+label:before,select:focus:not(:focus-visible){outline-style:none}a:focus-visible,button:focus-visible,input:focus-visible,input[type=button]:focus-visible,input[type=image]:focus-visible,input[type=radio]:focus-visible+label:before,select:focus-visible{outline-style:solid}button,input[type=button],input[type=image]{--hover-tint:var(--hover);--active-tint:var(--active)}a,button,input[type=button],input[type=file],input[type=image],input[type=radio],input[type=radio]+label,select{cursor:pointer}a:not([href]),button:disabled,input:disabled,input[type=button]:disabled,input[type=file]:disabled,input[type=image]:disabled,input[type=radio]:disabled,input[type=radio]:disabled+label,select:disabled{cursor:not-allowed}a:not([href]),button:disabled,input:disabled,input[type=radio]:disabled,input[type=radio]:disabled+label{color:var(--text-disabled-grey);opacity:1}.fr-enlarge-link{position:relative}.fr-enlarge-link a{background-image:none;outline-width:0}.fr-enlarge-link a:before{bottom:0;content:"";display:block;height:100%;left:0;outline-color:inherit;outline-offset:2px;outline-style:inherit;outline-width:2px;position:absolute;right:0;top:0;width:100%;z-index:1}@font-face{font-display:swap;font-family:Marianne;font-style:normal;font-weight:300;src:url(fonts/Marianne-Light.woff2) format("woff2"),url(fonts/Marianne-Light.woff) format("woff")}@font-face{font-display:swap;font-family:Marianne;font-style:italic;font-weight:300;src:url(fonts/Marianne-Light_Italic.woff2) format("woff2"),url(fonts/Marianne-Light_Italic.woff) format("woff")}@font-face{font-display:swap;font-family:Marianne;font-style:normal;font-weight:400;src:url(fonts/Marianne-Regular.woff2) format("woff2"),url(fonts/Marianne-Regular.woff) format("woff")}@font-face{font-display:swap;font-family:Marianne;font-style:italic;font-weight:400;src:url(fonts/Marianne-Regular_Italic.woff2) format("woff2"),url(fonts/Marianne-Regular_Italic.woff) format("woff")}@font-face{font-display:swap;font-family:Marianne;font-style:normal;font-weight:500;src:url(fonts/Marianne-Medium.woff2) format("woff2"),url(fonts/Marianne-Medium.woff) format("woff")}@font-face{font-display:swap;font-family:Marianne;font-style:italic;font-weight:500;src:url(fonts/Marianne-Medium_Italic.woff2) format("woff2"),url(fonts/Marianne-Medium_Italic.woff) format("woff")}@font-face{font-display:swap;font-family:Marianne;font-style:normal;font-weight:700;src:url(fonts/Marianne-Bold.woff2) format("woff2"),url(fonts/Marianne-Bold.woff) format("woff")}@font-face{font-display:swap;font-family:Marianne;font-style:italic;font-weight:700;src:url(fonts/Marianne-Bold_Italic.woff2) format("woff2"),url(fonts/Marianne-Bold_Italic.woff) format("woff")}@font-face{font-display:swap;font-family:Spectral;font-style:normal;font-weight:400;src:url(fonts/Spectral-Regular.woff2) format("woff2"),url(fonts/Spectral-Regular.woff) format("woff")}@font-face{font-display:swap;font-family:Spectral;font-style:normal;font-weight:900;src:url(fonts/Spectral-ExtraBold.woff2) format("woff2"),url(fonts/Spectral-ExtraBold.woff) format("woff")}h3{font-size:1.5rem;line-height:2rem}h2,h3{font-weight:700;margin:var(--title-spacing)}h2{font-size:1.75rem;line-height:2.25rem}h1{font-size:2rem;font-weight:700;line-height:2.5rem;margin:var(--title-spacing)}p{font-size:1rem;line-height:1.5rem;margin:var(--text-spacing)}ul{--xl-size:var(--xl-base);margin:0;margin-block-end:var(--xl-block);margin-block-start:var(--xl-block);padding:0}ul{list-style-type:var(--ul-type);padding-inline-start:var(--ul-start)}ul>li::marker{font-size:calc(var(--xl-size)*.9)}li{--xl-base:calc(var(--xl-size)*0.9);padding-bottom:var(--li-bottom)}.fr-text--regular{font-weight:400!important}*,:after,:before{box-sizing:inherit}body{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;-webkit-text-size-adjust:100%;--idle:transparent;--hover:var(--background-default-grey-hover);--active:var(--background-default-grey-active);background-color:var(--background-default-grey);color:var(--text-default-grey);font-family:Marianne,arial,sans-serif;font-size:1rem;line-height:1.5rem;margin:0;padding:0;text-rendering:optimizeLegibility}[class*=" fr-fi-"]:after,[class*=" fr-fi-"]:before,[class^=fr-fi-]:after,[class^=fr-fi-]:before{--icon-size:1.5rem;background-color:currentColor;display:inline-block;flex:0 0 auto;height:var(--icon-size);-webkit-mask-size:100% 100%;mask-size:100% 100%;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}[class*=" fr-fi-"]:before,[class^=fr-fi-]:before{content:""}hr{background-image:linear-gradient(0deg,var(--border-default-grey),var(--border-default-grey));background-position:0 0;background-repeat:no-repeat;background-size:100% 1px;border:0;display:block;margin:0;padding:var(--text-spacing)}.fr-grid-row{display:flex;flex-wrap:wrap;margin:0;padding:0}.fr-grid-row--center{justify-content:center}.fr-container{margin-left:auto;margin-right:auto;padding-left:1rem;padding-right:1rem;width:100%}.fr-container--fluid{max-width:none;overflow:hidden;padding-left:0;padding-right:0}.fr-col-12{flex:0 0 100%;max-width:100%;width:100%}.fr-collapse{--collapse-max-height:0;--collapse:-99999px;--collapser:"";max-height:0;max-height:var(--collapse-max-height);overflow:hidden;transition:visibility .3s}.fr-collapse:before{content:"";content:var(--collapser);display:block;margin-top:0;transition:margin-top .3s}.fr-collapse:not(.fr-collapse--expanded){visibility:hidden}.fr-collapse:not(.fr-collapse--expanded):before{margin-top:-99999px;margin-top:var(--collapse)}.fr-mb-0-5v{margin-bottom:.125rem!important}.fr-mx-auto{margin-left:auto}.fr-mx-auto{margin-right:auto}.fr-py-12v{padding-top:3rem!important}.fr-py-12v{padding-bottom:3rem!important}:root[data-fr-theme=dark]{--shadow-color:rgba(0,0,18,.32);--grey-1000-50:#161616;--grey-1000-50-hover:#343434;--grey-1000-50-active:#474747;--grey-975-75:#1e1e1e;--grey-975-75-hover:#3f3f3f;--grey-975-75-active:#525252;--grey-950-100:#242424;--grey-950-100-hover:#474747;--grey-950-100-active:#5b5b5b;--grey-200-850:#cecece;--grey-925-125:#2a2a2a;--grey-1000-75:#1e1e1e;--grey-1000-75-hover:#3f3f3f;--grey-1000-75-active:#525252;--grey-1000-100:#242424;--grey-1000-100-hover:#474747;--grey-1000-100-active:#5b5b5b;--grey-975-100:#242424;--grey-975-100-hover:#474747;--grey-975-100-active:#5b5b5b;--grey-975-125:#2a2a2a;--grey-975-125-hover:#4e4e4e;--grey-975-125-active:#636363;--grey-950-125:#2a2a2a;--grey-950-125-hover:#4e4e4e;--grey-950-125-active:#636363;--grey-950-150:#2f2f2f;--grey-950-150-hover:#545454;--grey-950-150-active:#696969;--grey-50-1000:#fff;--grey-425-625:#929292;--grey-625-425:#666;--grey-900-175:#353535;--blue-france-975-75:#1b1b35;--blue-france-975-75-hover:#3a3a68;--blue-france-975-75-active:#4d4d83;--blue-france-950-100:#21213f;--blue-france-950-100-hover:#424275;--blue-france-950-100-active:#56568c;--blue-france-sun-113-625:#8585f6;--blue-france-sun-113-625-hover:#b1b1f9;--blue-france-sun-113-625-active:#c6c6fb;--blue-france-925-125:#272747;--blue-france-925-125-hover:#4a4a7d;--blue-france-925-125-active:#5e5e90;--blue-france-975-sun-113:#000091;--blue-france-main-525:#6a6af4;--blue-france-850-200:#313178;--red-marianne-975-75:#2b1919;--red-marianne-975-75-hover:#573737;--red-marianne-975-75-active:#704848;--red-marianne-950-100:#331f1f;--red-marianne-950-100-hover:#613f3f;--red-marianne-950-100-active:#7b5151;--red-marianne-425-625:#f95c5e;--red-marianne-425-625-hover:#fa9293;--red-marianne-425-625-active:#fbabac;--red-marianne-925-125:#3b2424;--red-marianne-925-125-hover:#6b4545;--red-marianne-925-125-active:#865757;--red-marianne-main-472:#e1000f;--red-marianne-850-200:#5e2a2b;--info-950-100:#1d2437;--info-950-100-hover:#3b4767;--info-950-100-active:#4c5b83;--info-425-625:#518fff;--info-425-625-hover:#98b4ff;--info-425-625-active:#b4c7ff;--info-975-75:#171d2e;--success-950-100:#19271d;--success-950-100-hover:#344c3b;--success-950-100-active:#44624d;--success-425-625:#27a658;--success-425-625-hover:#36d975;--success-425-625-active:#3df183;--success-975-75:#142117;--warning-950-100:#361e19;--warning-950-100-hover:#663d35;--warning-950-100-active:#824f44;--warning-425-625:#fc5d00;--warning-425-625-hover:#ff8c73;--warning-425-625-active:#ffa595;--warning-975-75:#2d1814;--error-950-100:#391c1c;--error-950-100-hover:#6c3a3a;--error-950-100-active:#894b4b;--error-425-625:#ff5655;--error-425-625-hover:#ff8c8c;--error-425-625-active:#ffa6a6;--error-975-75:#301717;--green-tilleul-verveine-975-75:#201e14;--green-tilleul-verveine-975-75-hover:#433f2e;--green-tilleul-verveine-975-75-active:#57533d;--green-tilleul-verveine-950-100:#272419;--green-tilleul-verveine-950-100-hover:#4c4734;--green-tilleul-verveine-950-100-active:#615b44;--green-tilleul-verveine-sun-418-moon-817:#d8c634;--green-tilleul-verveine-sun-418-moon-817-hover:#fee943;--green-tilleul-verveine-sun-418-moon-817-active:#fef1ab;--green-tilleul-verveine-925-125:#2d2a1d;--green-tilleul-verveine-925-125-hover:#534f39;--green-tilleul-verveine-925-125-active:#696349;--green-tilleul-verveine-main-707:#b7a73f;--green-tilleul-verveine-850-200:#3f3a20;--green-bourgeon-975-75:#182014;--green-bourgeon-975-75-hover:#35432e;--green-bourgeon-975-75-active:#46573d;--green-bourgeon-950-100:#1e2719;--green-bourgeon-950-100-hover:#3d4c34;--green-bourgeon-950-100-active:#4e6144;--green-bourgeon-sun-425-moon-759:#99c221;--green-bourgeon-sun-425-moon-759-hover:#baec2a;--green-bourgeon-sun-425-moon-759-active:#c9fd2e;--green-bourgeon-925-125:#232d1d;--green-bourgeon-925-125-hover:#435339;--green-bourgeon-925-125-active:#556949;--green-bourgeon-main-640:#68a532;--green-bourgeon-850-200:#2a401a;--green-emeraude-975-75:#142018;--green-emeraude-975-75-hover:#2e4335;--green-emeraude-975-75-active:#3d5846;--green-emeraude-950-100:#19271e;--green-emeraude-950-100-hover:#344c3d;--green-emeraude-950-100-active:#44624f;--green-emeraude-sun-425-moon-753:#34cb6a;--green-emeraude-sun-425-moon-753-hover:#42fb84;--green-emeraude-sun-425-moon-753-active:#80fda3;--green-emeraude-925-125:#1e2e23;--green-emeraude-925-125-hover:#3b5543;--green-emeraude-925-125-active:#4b6b55;--green-emeraude-main-632:#00a95f;--green-emeraude-850-200:#21402c;--green-menthe-975-75:#15201e;--green-menthe-975-75-hover:#30433f;--green-menthe-975-75-active:#3f5753;--green-menthe-950-100:#1a2624;--green-menthe-950-100-hover:#364b47;--green-menthe-950-100-active:#46605b;--green-menthe-sun-373-moon-652:#21ab8e;--green-menthe-sun-373-moon-652-hover:#2eddb8;--green-menthe-sun-373-moon-652-active:#34f4cc;--green-menthe-925-125:#1f2d2a;--green-menthe-925-125-hover:#3c534e;--green-menthe-925-125-active:#4d6963;--green-menthe-main-548:#009081;--green-menthe-850-200:#223f3a;--green-archipel-975-75:#152021;--green-archipel-975-75-hover:#2f4345;--green-archipel-975-75-active:#3f5759;--green-archipel-950-100:#1a2628;--green-archipel-950-100-hover:#364a4e;--green-archipel-950-100-active:#465f63;--green-archipel-sun-391-moon-716:#34bab5;--green-archipel-sun-391-moon-716-hover:#43e9e2;--green-archipel-sun-391-moon-716-active:#4cfdf6;--green-archipel-925-125:#1f2c2e;--green-archipel-925-125-hover:#3c5255;--green-archipel-925-125-active:#4d676b;--green-archipel-main-557:#009099;--green-archipel-850-200:#233e41;--blue-ecume-975-75:#171d2f;--blue-ecume-975-75-hover:#333e5e;--blue-ecume-975-75-active:#445179;--blue-ecume-950-100:#1d2437;--blue-ecume-950-100-hover:#3b4767;--blue-ecume-950-100-active:#4c5b83;--blue-ecume-sun-247-moon-675:#869ece;--blue-ecume-sun-247-moon-675-hover:#b8c5e2;--blue-ecume-sun-247-moon-675-active:#ced6ea;--blue-ecume-925-125:#222940;--blue-ecume-925-125-hover:#424d73;--blue-ecume-925-125-active:#536190;--blue-ecume-main-400:#465f9d;--blue-ecume-850-200:#273962;--blue-cumulus-975-75:#171e2b;--blue-cumulus-975-75-hover:#333f56;--blue-cumulus-975-75-active:#43536f;--blue-cumulus-950-100:#1c2433;--blue-cumulus-950-100-hover:#3a4761;--blue-cumulus-950-100-active:#4a5b7b;--blue-cumulus-sun-368-moon-732:#7ab1e8;--blue-cumulus-sun-368-moon-732-hover:#bad2f2;--blue-cumulus-sun-368-moon-732-active:#d2e2f6;--blue-cumulus-925-125:#212a3a;--blue-cumulus-925-125-hover:#404f69;--blue-cumulus-925-125-active:#516384;--blue-cumulus-main-526:#417dc4;--blue-cumulus-850-200:#263b58;--purple-glycine-975-75:#251a24;--purple-glycine-975-75-hover:#4c394a;--purple-glycine-975-75-active:#634a60;--purple-glycine-950-100:#2c202b;--purple-glycine-950-100-hover:#554053;--purple-glycine-950-100-active:#6c536a;--purple-glycine-sun-319-moon-630:#ce70cc;--purple-glycine-sun-319-moon-630-hover:#dfa4dd;--purple-glycine-sun-319-moon-630-active:#e7bbe6;--purple-glycine-925-125:#332632;--purple-glycine-925-125-hover:#5d485c;--purple-glycine-925-125-active:#755b73;--purple-glycine-main-494:#a558a0;--purple-glycine-850-200:#502e4d;--pink-macaron-975-75:#261b19;--pink-macaron-975-75-hover:#4e3a37;--pink-macaron-975-75-active:#654c48;--pink-macaron-950-100:#2e211f;--pink-macaron-950-100-hover:#58423f;--pink-macaron-950-100-active:#705551;--pink-macaron-sun-406-moon-833:#ffb7ae;--pink-macaron-sun-406-moon-833-hover:#ffe0dc;--pink-macaron-sun-406-moon-833-active:#fff0ee;--pink-macaron-925-125:#352724;--pink-macaron-925-125-hover:#614a45;--pink-macaron-925-125-active:#795d57;--pink-macaron-main-689:#e18b76;--pink-macaron-850-200:#52312a;--pink-tuile-975-75:#281b19;--pink-tuile-975-75-hover:#513a37;--pink-tuile-975-75-active:#694c48;--pink-tuile-950-100:#2f211f;--pink-tuile-950-100-hover:#5a423e;--pink-tuile-950-100-active:#725550;--pink-tuile-sun-425-moon-750:#ff9575;--pink-tuile-sun-425-moon-750-hover:#ffc4b7;--pink-tuile-sun-425-moon-750-active:#ffd8d0;--pink-tuile-925-125:#372624;--pink-tuile-925-125-hover:#644845;--pink-tuile-925-125-active:#7d5b57;--pink-tuile-main-556:#ce614a;--pink-tuile-850-200:#55302a;--yellow-tournesol-975-75:#221d11;--yellow-tournesol-975-75-hover:#473e29;--yellow-tournesol-975-75-active:#5c5136;--yellow-tournesol-950-100:#292416;--yellow-tournesol-950-100-hover:#4f472f;--yellow-tournesol-950-100-active:#655b3d;--yellow-tournesol-sun-407-moon-922:#ffe552;--yellow-tournesol-sun-407-moon-922-hover:#e1c700;--yellow-tournesol-sun-407-moon-922-active:#cab300;--yellow-tournesol-925-125:#302a1a;--yellow-tournesol-925-125-hover:#584e34;--yellow-tournesol-925-125-active:#6f6342;--yellow-tournesol-main-731:#c8aa39;--yellow-tournesol-850-200:#43391a;--yellow-moutarde-975-75:#231d14;--yellow-moutarde-975-75-hover:#483e2e;--yellow-moutarde-975-75-active:#5e513d;--yellow-moutarde-950-100:#2a2319;--yellow-moutarde-950-100-hover:#514534;--yellow-moutarde-950-100-active:#685944;--yellow-moutarde-sun-348-moon-860:#ffca00;--yellow-moutarde-sun-348-moon-860-hover:#cda200;--yellow-moutarde-sun-348-moon-860-active:#b28c00;--yellow-moutarde-925-125:#30291d;--yellow-moutarde-925-125-hover:#584d39;--yellow-moutarde-925-125-active:#6f6149;--yellow-moutarde-main-679:#c3992a;--yellow-moutarde-850-200:#453820;--orange-terre-battue-975-75:#281a16;--orange-terre-battue-975-75-hover:#513932;--orange-terre-battue-975-75-active:#6a4b42;--orange-terre-battue-950-100:#31201c;--orange-terre-battue-950-100-hover:#5d403a;--orange-terre-battue-950-100-active:#77534a;--orange-terre-battue-sun-370-moon-672:#ff732c;--orange-terre-battue-sun-370-moon-672-hover:#ffa48b;--orange-terre-battue-sun-370-moon-672-active:#ffbbab;--orange-terre-battue-925-125:#382621;--orange-terre-battue-925-125-hover:#664840;--orange-terre-battue-925-125-active:#7f5b51;--orange-terre-battue-main-645:#e4794a;--orange-terre-battue-850-200:#543125;--brown-cafe-creme-975-75:#211d16;--brown-cafe-creme-975-75-hover:#453e31;--brown-cafe-creme-975-75-active:#5a5141;--brown-cafe-creme-950-100:#28241c;--brown-cafe-creme-950-100-hover:#4e4739;--brown-cafe-creme-950-100-active:#635b4a;--brown-cafe-creme-sun-383-moon-885:#ecd7a2;--brown-cafe-creme-sun-383-moon-885-hover:#c5b386;--brown-cafe-creme-sun-383-moon-885-active:#af9f77;--brown-cafe-creme-925-125:#2e2a21;--brown-cafe-creme-925-125-hover:#554e3f;--brown-cafe-creme-925-125-active:#6b6351;--brown-cafe-creme-main-782:#d1b781;--brown-cafe-creme-850-200:#423925;--brown-caramel-975-75:#251c16;--brown-caramel-975-75-hover:#4c3c31;--brown-caramel-975-75-active:#624e41;--brown-caramel-950-100:#2c221c;--brown-caramel-950-100-hover:#554439;--brown-caramel-950-100-active:#6c574a;--brown-caramel-sun-425-moon-901:#fbd8ab;--brown-caramel-sun-425-moon-901-hover:#efb547;--brown-caramel-sun-425-moon-901-active:#d6a23e;--brown-caramel-925-125:#332821;--brown-caramel-925-125-hover:#5d4b40;--brown-caramel-925-125-active:#755f51;--brown-caramel-main-648:#c08c65;--brown-caramel-850-200:#4b3525;--brown-opera-975-75:#241c17;--brown-opera-975-75-hover:#4a3c33;--brown-opera-975-75-active:#604f44;--brown-opera-950-100:#2b221c;--brown-opera-950-100-hover:#53443a;--brown-opera-950-100-active:#6a574a;--brown-opera-sun-395-moon-820:#e6be92;--brown-opera-sun-395-moon-820-hover:#f2e2d3;--brown-opera-sun-395-moon-820-active:#f8f0e9;--brown-opera-925-125:#322821;--brown-opera-925-125-hover:#5c4b40;--brown-opera-925-125-active:#735f51;--brown-opera-main-680:#bd987a;--brown-opera-850-200:#493625;--beige-gris-galet-975-75:#211d19;--beige-gris-galet-975-75-hover:#453e37;--beige-gris-galet-975-75-active:#595148;--beige-gris-galet-950-100:#28231f;--beige-gris-galet-950-100-hover:#4e453f;--beige-gris-galet-950-100-active:#635950;--beige-gris-galet-sun-407-moon-821:#d0c3b7;--beige-gris-galet-sun-407-moon-821-hover:#eae5e1;--beige-gris-galet-sun-407-moon-821-active:#f4f2f0;--beige-gris-galet-925-125:#2e2924;--beige-gris-galet-925-125-hover:#554d45;--beige-gris-galet-925-125-active:#6b6157;--beige-gris-galet-main-702:#aea397;--beige-gris-galet-850-200:#433829}.fr-artwork-decorative{fill:var(--artwork-decorative-blue-france)}.fr-artwork-minor{fill:var(--artwork-minor-red-marianne)}.fr-artwork-major{fill:var(--artwork-major-blue-france)}h1,h2,h3{color:var(--text-title-grey)}.fr-logo{--text-spacing:0;--underline-img:none;color:var(--text-title-grey);display:inline-block;font-size:1.05rem;font-weight:700;letter-spacing:-.01em;line-height:1.0317460317em;text-indent:-.1em;text-transform:uppercase;vertical-align:middle}.fr-logo:before{background-image:url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 44 18'%3E%3Cpath fill='%23fff' d='M11.3 10.2c-.9.6-1.7 1.3-2.3 2.1v-.1c.4-.5.7-1 1-1.5.4-.2.7-.5 1-.8.5-.5 1-1 1.7-1.3.3-.1.5-.1.8 0-.1.1-.2.1-.4.2H13v-.1c-.3.3-.7.5-1 .9-.1.2-.2.6-.7.6 0 .1.1 0 0 0zm1.6 4.6c0-.1-.1 0-.2 0l-.1.1-.1.1-.2.2s.1.1.2 0l.1-.1c.1 0 .2-.1.2-.2.1 0 .1 0 .1-.1 0 .1 0 0 0 0zm-1.6-4.3c.1 0 .2 0 .2-.1s.1-.1.1-.1v-.1c-.2.1-.3.2-.3.3zm2.4 1.9s0-.1 0 0c.1-.1.2-.1.3-.1.7-.1 1.4-.3 2.1-.6-.8-.5-1.7-.9-2.6-1h.1c-.1-.1-.3-.1-.5-.2h.1c-.2-.1-.5-.1-.7-.2.1 0 .2-.2.2-.3h-.1c-.4.2-.6.5-.8.9.2.1.5 0 .7.1h-.3c-.1 0-.2.1-.2.2h.1c-.1 0-.1.1-.2.1.1.1.2 0 .4 0 0 .1.1.1.1.1-.1 0-.2.1-.3.3-.1.2-.2.2-.3.3v.1c-.3.2-.6.5-.9.8v.1c-.1.1-.2.1-.2.2v.1c.4-.1.6-.4 1-.5l.6-.3c.2 0 .3-.1.5-.1v.1h.2c0 .1-.2 0-.1.1s.3.1.4 0c.2-.2.3-.2.4-.2zM12.4 14c-.4.2-.9.2-1.2.4 0 0 0 .1-.1.1 0 0-.1 0-.1.1-.1 0-.1.1-.2.2l-.1.1s0 .1.1 0l.1-.1s-.1.1-.1.2V15.3l-.1.1s0 .1-.1.1l-.1.1.2-.2.1-.1h.2s0-.1.1-.1c.1-.1.2-.2.3-.2h.1c.1-.1.3-.1.4-.2.1-.1.2-.2.3-.2.2-.2.5-.3.8-.5-.1 0-.2-.1-.3-.1 0 .1-.2 0-.3 0zM30 9.7c-.1.2-.4.2-.6.3-.2.2 0 .4.1.5.1.3-.2.5-.4.5.1.1.2.1.2.1 0 .2.2.2.1.4s-.5.3-.3.5c.1.2.1.5 0 .7-.1.2-.3.4-.5.5-.2.1-.4.1-.6 0-.1 0-.1-.1-.2-.1-.5-.1-1-.2-1.5-.2-.1 0-.3.1-.4.1-.1.1-.3.2-.4.3l-.1.1c-.1.1-.2.2-.2.3-.1.2-.2.4-.2.6-.2.5-.2 1 0 1.4 0 0 1 .3 1.7.6.2.1.5.2.7.4l1.7 1H13.2l1.6-1c.6-.4 1.3-.7 2-1 .5-.2 1.1-.5 1.5-.9.2-.2.3-.4.5-.5.3-.4.6-.7 1-1l.3-.3s0-.1.1-.1c-.2.1-.2.2-.4.2 0 0-.1 0 0-.1s.2-.2.3-.2v-.1c-.4 0-.7.2-1 .5h-.2c-.5.2-.8.5-1.2.7v-.1c-.2.1-.4.2-.5.2-.2 0-.5.1-.8 0-.4 0-.7.1-1.1.2-.2.1-.4.1-.6.2v.1l-.2.2c-.2.1-.3.2-.5.4l-.5.5h-.1l.1-.1.1-.1c0-.1.1-.1.1-.2.2-.1.3-.3.5-.4 0 0-.1 0 0 0 0 0 0-.1.1-.1l-.1.1c-.1.1-.1.2-.2.2v-.1-.1l.2-.2c.1-.1.2-.1.3-.2h.1c-.2.1-.3.1-.5.2H14h-.1c0-.1.1-.1.2-.2h.1c1-.8 2.3-.6 3.4-1 .1-.1.2-.1.3-.2.1-.1.3-.2.5-.3.2-.2.4-.4.5-.7v-.1c-.4.4-.8.7-1.3 1-.6.2-1.3.4-2 .4 0-.1.1-.1.1-.1 0-.1.1-.1.1-.2h.1s0-.1.1-.1h.1c-.1-.1-.3.1-.4 0 .1-.1 0-.2.1-.2h.1s0-.1.1-.1c.5-.3.9-.5 1.3-.7-.1 0-.1.1-.2 0 .1 0 0-.1.1-.1.3-.1.6-.3.9-.4-.1 0-.2.1-.3 0 .1 0 .1-.1.2-.1v-.1h0c0-.1.1 0 .2-.1h-.1c.1-.1.2-.2.4-.2 0-.1-.1 0-.1-.1h.1-.5c-.1 0 0-.1 0-.1.1-.2.2-.5.3-.7h-.1c-.3.3-.8.5-1.2.6h-.2c-.2.1-.4.1-.5 0-.1-.1-.2-.2-.3-.2-.2-.1-.5-.3-.8-.4-.7-.2-1.5-.4-2.3-.3.3-.1.7-.2 1.1-.3.5-.2 1-.3 1.5-.3h-.3c-.4 0-.9.1-1.3.2-.3.1-.6.2-.9.2-.2.1-.3.2-.5.2v-.1c.3-.4.7-.7 1.1-.8.5-.1 1.1 0 1.6.1.4 0 .8.1 1.1.2.1 0 .2.2.3.3.2.1.4 0 .5.1v-.2c.1-.1.3 0 .4 0 .2-.2-.2-.4-.3-.6v-.1c.2.2.5.4.7.6.1.1.5.2.5 0-.2-.3-.4-.6-.7-.9v-.2c-.1 0-.1 0-.1-.1-.1-.1-.1-.2-.1-.3-.1-.2 0-.4-.1-.5-.1-.2-.1-.3-.1-.5-.1-.5-.2-1-.3-1.4-.1-.6.3-1 .6-1.5.2-.4.5-.7.8-1 .1-.4.3-.7.6-1 .3-.3.6-.5.9-.6.3-.1.5-.2.8-.3l2.5-.4H25l1.8.3c.1 0 .2 0 .2.1.1.1.3.2.4.2.2.1.4.3.6.5.1.1.2.3.1.4-.1.1-.1.4-.2.4-.2.1-.4.1-.6.1-.1 0-.2 0-.4-.1.5.2.9.4 1.2.8 0 .1.2.1.3.1v.1c-.1.1-.1.1-.1.2h.1c.1-.1.1-.4.3-.3.2.1.2.3.1.4-.1.1-.2.2-.4.3v.2c.1.1.1.2.2.4s.1.5.2.7c.1.5.2.9.2 1.4 0 .2-.1.5 0 .7l.3.6c.1.2.2.3.3.5.2.3.6.6.4 1zm-15.6 5.2c-.1 0-.1.1-.1.1s.1 0 .1-.1zm5.8-1.8c-.1.1 0 0 0 0zm-6.7-.2c0 .1.1 0 .1 0 .2-.1.5 0 .6-.2-.1-.1-.2 0-.2-.1-.1 0-.2 0-.2.1-.1.1-.3.1-.3.2z'/%3E%3Cpath fill='gray' d='M27.9 6.8c.1 0 .3 0 .3.1-.1.2-.4.3-.6.5h-.1c-.1.1-.1.2-.1.2h-.3c.1.1.3.2.5.2l.1.1h.2V8c-.1.1-.2.1-.4.1.2.1.5.1.7 0 .2-.1 0-.4.1-.5-.1 0 0-.1-.1-.1.1-.1.1-.2.2-.2s.1 0 .2-.1c0-.1-.1-.1-.1-.2.2-.1.3-.3.3-.5 0-.1-.3-.1-.4-.2h-.5c-.2 0-.3.1-.5.1l-.6.3c.2-.1.4-.1.7-.2 0 .3.2.3.4.3'/%3E%3C/svg%3E"),linear-gradient(90deg,#000091,#000091 50%,#e1000f 0,#e1000f),linear-gradient(90deg,#161616,#161616);background-position:0 -.0625rem,0 0,0 0;background-repeat:no-repeat,no-repeat,no-repeat;background-size:2.75rem 1.125rem,2.75rem 1rem,0;content:"";display:block;height:1rem;margin-bottom:.3333333333rem;width:2.75rem}.fr-logo:after{background-image:url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 252 180'%3E%3Cdefs%3E%3Csymbol id='a' viewBox='0 0 11 15.5'%3E%3Cpath d='M10.4 5.3C11.9 1.5 10.1 0 7.9 0 4.2 0 0 6.5 0 11.7c0 2.5 1.2 3.8 3 3.8 2.1 0 4.3-2 6.2-5.5h-1c-1.2 1.5-2.6 2.6-3.9 2.6-1.3 0-2-.8-2-2.6a10.7 10.7 0 01.3-2.2zm-4-3.1c1.1 0 2 .8 1.5 2.6L3.1 6.1c.8-2.2 2.2-4 3.4-4z'/%3E%3C/symbol%3E%3Csymbol id='b' viewBox='0 0 12.4 21.8'%3E%3Cuse width='11' height='15.5' y='6.4' href='%23a'/%3E%3Cpath d='M7.9 4.7L12.4.6V0h-3L6.7 4.7H8z'/%3E%3C/symbol%3E%3Csymbol id='c' viewBox='0 0 11.5 19'%3E%3Cpath d='M1.7 5.7h2.6L.1 17.1a1.3 1.3 0 001.2 2c3 0 6.4-2.6 7.8-6.2h-.7a9.4 9.4 0 01-5.1 3.5L7 5.7H11l.5-1.6H7.7L9 0H7.6L4.9 4.1l-3.2.4v1.2z'/%3E%3C/symbol%3E%3Csymbol id='d' viewBox='0 0 9.8 21.9'%3E%3Cpath d='M7.6 8c.3-1-.4-1.6-1-1.6-2.2 0-5 2.1-6 5h.7A5.6 5.6 0 014.4 9L.1 20.3a1.1 1.1 0 001 1.6c2.2 0 4.7-2 5.8-5H6A5.6 5.6 0 013 19.5zM8 3.7a1.8 1.8 0 001.8-1.8A1.8 1.8 0 008 0a1.8 1.8 0 00-1.8 1.8A1.8 1.8 0 008 3.6'/%3E%3C/symbol%3E%3Csymbol id='e' viewBox='0 0 14.8 15.5'%3E%3Cpath d='M3.3 3.1c.7 0 1 1 0 3.4l-3 6.8c-.7 1.3 0 2.2 1.2 2.2a1.3 1.3 0 001.5-1l3-8C7.4 4.8 10 3 11 3s.8.6.3 1.6l-4.6 9a1.3 1.3 0 001.1 1.9c2.3 0 5-2 6-5h-.6A5.6 5.6 0 0110 13l4-8a6.1 6.1 0 00.8-2.8A2 2 0 0012.6 0c-2 0-3.6 2.2-6 5V2.8C6.6 1.4 6.1 0 4.8 0 3.2 0 1.8 2.5.7 4.9h.7c.7-1.1 1.3-1.8 2-1.8'/%3E%3C/symbol%3E%3Csymbol id='f' viewBox='0 0 12 15.5'%3E%3Cpath d='M11.8 3.5c.5-1.9.2-3.5-1.2-3.5-1.8 0-2.3 1.2-4 5V2.8C6.5 1.3 6 0 4.6 0 3.1 0 1.7 2.5.5 5h.8C2 3.7 2.8 3 3.3 3c.7 0 1 1 0 3.4l-3 6.8c-.7 1.3 0 2.1 1.2 2.1a1.3 1.3 0 001.5-1l3-8a50.3 50.3 0 012.6-3h3.2z'/%3E%3C/symbol%3E%3Csymbol id='g' viewBox='0 0 14.7 16.2'%3E%3Cpath d='M10.5 13.1c-.6 0-1-1 0-3.4L14.6.1 13.4 0l-1.3 1.3h-.3C6.1 1.3 0 8.6 0 14.2a2 2 0 002.1 2.1c1.7 0 3.3-2.4 5.2-5l-.1 1c-.3 2.6.6 4 2 4 1.5 0 3-2.4 4-4.9h-.7c-.7 1.1-1.5 1.8-2 1.8zM7.9 9.8c-1.3 1.6-3.4 3.5-4.3 3.5-.5 0-.9-.5-.9-1.6 0-3.5 4-8.2 6-8.2a4.2 4.2 0 011.4.2z'/%3E%3C/symbol%3E%3Csymbol id='h' viewBox='0 0 21.9 19.8'%3E%3Cpath d='M11.2 19.8l.3-.9c-3.8-.7-4.3-.7-2.7-4.8l1.4-3.9h3c1.9 0 1.9.9 1.6 3h1l2.6-6.9h-1c-1 1.6-1.8 2.9-3.8 2.9h-3l2-5.6c.8-2 1.1-2.4 3.7-2.4h.7c2.6 0 3 .7 3 3.5h1l.9-4.7H7.3L7 .9c3 .6 3.3.9 2 4.8L5.7 14c-1.5 3.9-2 4.2-5.5 4.8l-.3.9z'/%3E%3C/symbol%3E%3Csymbol id='i' viewBox='0 0 10.1 21.9'%3E%3Cpath d='M2.9 19.4L10.1.3 9.8 0l-5 .6v.6l1 .7c.9.7.6 1.3-.2 3.4L.2 19.9a1.3 1.3 0 001.1 2c2.3 0 4.7-2.1 5.8-5h-.7a6.5 6.5 0 01-3.5 2.5'/%3E%3C/symbol%3E%3Csymbol id='j' viewBox='0 0 18 22'%3E%3Cpath d='M18 .6h-4.3a3.8 3.8 0 00-2.1-.6A6.6 6.6 0 005 6.5a3.3 3.3 0 003 3.6c-1.9.8-3 1.8-3 2.9a1.7 1.7 0 00.9 1.5c-4.3 1.3-6 2.8-6 4.7 0 2 2.6 2.8 5.6 2.8 5.3 0 9.6-2.7 9.6-5.1 0-1.8-1.6-2.5-4.3-3.3-2.2-.7-3.2-.8-3.2-1.6A2.4 2.4 0 019 10.2a6.6 6.6 0 006.1-6.5 4.5 4.5 0 00-.2-1.5h2.5zM9.8 16.2c2.1.7 3 1 3 1.6 0 1.4-2 2.5-5.6 2.5-2.7 0-4-.6-4-2 0-1.5 1.4-2.5 3.5-3.3a21.5 21.5 0 003 1.2zM9 9c-1 0-1.3-.8-1.3-1.7 0-2.8 1.4-6.2 3.5-6.2 1 0 1.3.8 1.3 1.6 0 2.9-1.4 6.3-3.5 6.3z'/%3E%3C/symbol%3E%3Csymbol id='k' viewBox='0 0 23 25.1'%3E%3Cpath d='M14.3 15.6c1.9 0 2 .8 1.6 2.8H17l2.5-6.8h-1c-1 1.6-1.7 2.9-3.8 2.9h-4.1l2-5.6c.7-2 1-2.4 3.7-2.4H18c2.6 0 3 .7 3 3.5h1l.9-4.7H7.3l-.3.9c3 .6 3.3.9 2 4.8l-3.2 8.4c-1.5 3.9-2 4.2-5.6 4.8l-.2 1h17.4l3.2-5h-1.2c-2 2-4 3.8-8 3.8-4.7 0-4.3-.3-2.7-4.6l1.4-3.8h4.2zm2.3-11.8L21 .6V0h-3l-2.6 3.9h1.2v-.1z'/%3E%3C/symbol%3E%3Csymbol id='l' viewBox='0 0 13.6 21.8'%3E%3Cpath d='M11.4 6.4c-2 0-4 2.2-5.8 4.8L9.6.3 9.4 0l-5 .6V1l1 .8c.9.7.6 1.3-.2 3.4L.8 16.8A13.9 13.9 0 000 19c0 1.4 1.8 2.7 3.5 2.7 3.8 0 10-6.9 10-12.2 0-2.3-.5-3.2-2.1-3.2zM4.8 19.5c-.8 0-1.9-.7-1.9-1.3a15.5 15.5 0 01.8-2.2L5 12.7C6.3 11 8.4 9.3 9.6 9.3c.7 0 1.2.4 1.2 1.5 0 3.1-2.9 8.7-6 8.7z'/%3E%3C/symbol%3E%3Csymbol id='m' viewBox='0 0 19.2 19.9'%3E%3Cpath d='M17.6 0H7.3L7 .9c3 .6 3.3.9 2 4.8l-3.2 8.5c-1.5 3.9-2 4.2-5.5 4.8L0 20h15.7l3.5-6H18c-2 2-4.2 4.8-7.7 4.8-2.7 0-3-.5-1.6-4.5l3.1-8.5c1.4-3.9 2-4.2 5.5-4.8z'/%3E%3C/symbol%3E%3Csymbol id='n' viewBox='0 0 126 90'%3E%3Cuse width='12.4' height='21.8' x='112.7' y='66.1' href='%23b'/%3E%3Cuse width='11.5' height='19' x='102.2' y='69' href='%23c'/%3E%3Cuse width='9.8' height='21.9' x='93.6' y='66.1' href='%23d'/%3E%3Cuse width='14.8' height='15.5' x='77.2' y='72.5' href='%23e'/%3E%3Cuse width='12' height='15.5' x='65.7' y='72.5' href='%23f'/%3E%3Cuse width='11' height='15.5' x='54.3' y='72.5' href='%23a'/%3E%3Cuse width='11.5' height='19' x='43.7' y='69' href='%23c'/%3E%3Cuse width='14.7' height='16.2' x='28.9' y='71.8' href='%23g'/%3E%3Cuse width='12' height='15.5' x='19.6' y='72.5' href='%23f'/%3E%3Cuse width='21.9' height='19.8' y='67.6' href='%23h'/%3E%3Cuse width='12.4' height='21.8' x='77.3' y='33.1' href='%23b'/%3E%3Cuse width='11.5' height='19' x='66.8' y='36' href='%23c'/%3E%3Cuse width='9.8' height='21.9' x='58.2' y='33' href='%23d'/%3E%3Cuse width='10.1' height='21.9' x='49.4' y='33.1' href='%23i'/%3E%3Cuse width='14.7' height='16.2' x='34.9' y='38.8' href='%23g'/%3E%3Cuse width='18' height='22' x='18.6' y='39.4' href='%23j'/%3E%3Cuse width='23' height='25.1' y='29.3' href='%23k'/%3E%3Cuse width='12.4' height='21.8' x='76.8' y='.1' href='%23b'/%3E%3Cuse width='11.5' height='19' x='66.2' y='2.9' href='%23c'/%3E%3Cuse width='12' height='15.5' x='54.8' y='6.5' href='%23f'/%3E%3Cuse width='11' height='15.5' x='43.4' y='6.4' href='%23a'/%3E%3Cuse width='13.6' height='21.8' x='29.4' y='.1' href='%23l'/%3E%3Cuse width='9.8' height='21.9' x='20.6' href='%23d'/%3E%3Cuse width='19.2' height='19.9' y='1.4' href='%23m'/%3E%3C/symbol%3E%3C/defs%3E%3Cuse fill='%23161616' width='126' height='90' x='0' y='0' href='%23n'/%3E%3Cuse fill='%23fff' width='126' height='90' x='126' y='90' href='%23n'/%3E%3C/svg%3E");background-position:0 calc(100% + 1.875rem);background-repeat:no-repeat;background-size:5.25rem 3.75rem;content:"";display:block;min-width:2.625rem;padding-top:2.2083333333rem}[data-fr-theme=dark] .fr-logo:after{background-position:-2.625rem 100%}.fr-btn{--text-spacing:0;--title-spacing:0;--underline-img:none;--hover-tint:var(--hover);--idle:transparent;--hover:var(--background-action-high-blue-france-hover);--active:var(--background-action-high-blue-france-active);align-items:center;background-color:var(--background-action-high-blue-france);color:var(--text-inverted-blue-france);display:inline-flex;flex-direction:row;font-size:1rem;font-weight:500;line-height:1.5rem;min-height:2.5rem;padding:.5rem 1rem;width:-moz-fit-content;width:fit-content;z-index:1}.fr-btn:after,.fr-btn:before{display:block}.fr-btn[target=_blank]{max-height:none;max-width:100%;overflow:initial}.fr-btn[target=_blank]:after{--icon-size:1rem;content:"";margin-left:.5rem;margin-right:-.125rem}.fr-btn[target=_blank]:before{content:none}.fr-btn[class*=" fr-fi-"]:not([class*=fr-btn--icon-]),.fr-btn[class^=fr-fi-]:not([class*=fr-btn--icon-]){max-height:2.5rem;max-width:2.5rem;overflow:hidden;padding-left:.5rem;padding-right:.5rem;white-space:nowrap}.fr-btn[class*=" fr-fi-"]:not([class*=fr-btn--icon-]):before,.fr-btn[class^=fr-fi-]:not([class*=fr-btn--icon-]):before{--icon-size:1.5rem;margin-left:0;margin-right:.5rem}.fr-btn--close{display:flex;font-size:.875rem;line-height:1.5rem;margin-left:auto;margin-right:-1rem;max-height:none;max-width:100%;min-height:2rem;overflow:initial;padding:.25rem .75rem}.fr-btn--close:after{--icon-size:1rem;background-color:currentColor;content:"";display:inline-block;flex:0 0 auto;height:var(--icon-size);margin-left:.5rem;margin-right:-.125rem;-webkit-mask-image:url(icons/system/close-line.svg);mask-image:url(icons/system/close-line.svg);-webkit-mask-size:100% 100%;mask-size:100% 100%;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}.fr-btn--close:before{content:none}.fr-btn:disabled,a.fr-btn:not([href]){--idle:transparent;--hover:var(--background-disabled-grey-hover);--active:var(--background-disabled-grey-active);background-color:var(--background-disabled-grey);color:var(--text-disabled-grey)}.fr-btn--close{--hover:inherit;--active:inherit;background-color:transparent;color:var(--text-action-high-blue-france)}.fr-btn--close:disabled,a.fr-btn--close:not([href]){--hover:inherit;--active:inherit;background-color:transparent;color:var(--text-disabled-grey)}.fr-label{color:var(--text-label-grey);display:block;font-size:1rem;line-height:1.5rem}.fr-label+.fr-input{margin-top:.5rem}.fr-hint-text{--text-spacing:0 0 1rem;display:block;font-size:.75rem;line-height:1.25rem}.fr-hint-text+.fr-hint-text{margin-top:.25rem}.fr-fieldset{align-items:flex-end;border:0;display:flex;flex-direction:row;flex-wrap:wrap;margin:0 -.75rem 1rem;padding:0 .25rem;position:relative}.fr-fieldset__legend{color:var(--text-title-grey);font-size:1rem;font-weight:700;line-height:1.5rem;margin-bottom:1rem;margin-left:-.25rem;margin-right:-.25rem;padding-left:.75rem;padding-right:.75rem;width:100%}.fr-fieldset__legend .fr-hint-text{font-weight:400;margin-top:.5rem}.fr-fieldset__legend>.fr-fieldset:last-child:after,.fr-fieldset__legend>h1:last-child:after,.fr-fieldset__legend>h2:last-child:after,.fr-fieldset__legend>h3:last-child:after,.fr-fieldset__legend>p:last-child:after{content:"";display:block;margin-bottom:-1rem}.fr-hint-text{color:var(--text-mention-grey)}.fr-fieldset:disabled .fr-fieldset__legend,.fr-fieldset:disabled .fr-label{color:var(--text-disabled-grey)}.fr-fieldset__content{margin-left:.5rem;position:relative;width:100%}.fr-fieldset__content .fr-radio-group:first-child{margin-top:-1rem}.fr-fieldset__content .fr-radio-group label{padding:.75rem 0}.fr-fieldset__content .fr-radio-group label:before{margin-top:.75rem}.fr-link--icon-left[class*=" fr-fi-"],.fr-link--icon-left[class^=fr-fi-]{max-height:none;max-width:100%;overflow:initial}.fr-link--icon-left[class*=" fr-fi-"]:before,.fr-link--icon-left[class^=fr-fi-]:before{--icon-size:1rem;margin-left:-.125rem;margin-right:.5rem}.fr-sidemenu{--ul-type:none;--ol-type:none;--ul-start:0;--ol-start:0;--xl-block:0;--li-bottom:0;--ol-content:none;--underline-img:none;--text-spacing:0;--title-spacing:0;box-shadow:inset 0 -1px 0 0 var(--border-default-grey),inset 0 1px 0 0 var(--border-default-grey);margin-left:-1rem;margin-right:-1rem;position:relative}.fr-sidemenu a:not([href]){cursor:default}.fr-sidemenu .fr-collapse{margin:-.25rem -.25rem 0;padding:.25rem .25rem 0}.fr-sidemenu__title{box-shadow:inset 0 -1px 0 0 var(--border-default-grey);color:var(--text-title-grey);font-size:1.125rem;font-weight:700;line-height:1.75rem;padding:1rem 0}.fr-sidemenu__list{font-weight:700}.fr-sidemenu__list .fr-sidemenu__list{font-weight:400;margin:0 .5rem 1.5rem}.fr-sidemenu__list .fr-sidemenu__list .fr-sidemenu__btn{font-size:1rem;font-weight:400;line-height:1.5rem}.fr-sidemenu__list .fr-sidemenu__list .fr-sidemenu__list .fr-sidemenu__btn{font-size:.875rem;line-height:1.5rem}.fr-sidemenu__inner>.fr-collapse{margin:-.25rem .75rem 0;padding:.25rem .25rem 0}.fr-sidemenu__btn{--hover-tint:var(--hover);--active-tint:var(--active);align-items:center;color:var(--text-action-high-grey);display:flex;flex-direction:row;font-size:1rem;font-weight:700;line-height:1.5rem;padding:.75rem .5rem;position:relative;text-align:left;width:100%}.fr-sidemenu__btn[aria-current]:before{--idle:transparent;--hover:var(--border-active-blue-france-hover);--active:var(--border-active-blue-france-active);background-color:var(--border-active-blue-france);bottom:.75rem;content:"";left:0;position:absolute;top:.75rem;width:2px}.fr-sidemenu__btn[aria-expanded]{align-items:center;display:flex;flex-direction:row}.fr-sidemenu__btn[aria-expanded]:after{--icon-size:1rem;background-color:currentColor;content:"";display:inline-block;flex:0 0 auto;height:var(--icon-size);margin-left:auto;margin-right:0;-webkit-mask-image:url(icons/system/arrow-down-s-line.svg);mask-image:url(icons/system/arrow-down-s-line.svg);-webkit-mask-size:100% 100%;mask-size:100% 100%;transition:transform .3s;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}.fr-sidemenu__btn[aria-expanded=true]:after{transform:rotate(-180deg)}.fr-sidemenu__inner>.fr-sidemenu__btn{font-weight:400;width:100%}.fr-sidemenu__inner>.fr-sidemenu__btn:after{margin-right:1rem}.fr-sidemenu__inner>.fr-sidemenu__btn:before{--icon-size:1rem;background-color:currentColor;content:"";display:inline-block;flex:0 0 auto;height:var(--icon-size);margin-left:.5rem;margin-right:.5rem;-webkit-mask-image:url(icons/system/menu-2-fill.svg);mask-image:url(icons/system/menu-2-fill.svg);-webkit-mask-size:100% 100%;mask-size:100% 100%;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}.fr-sidemenu__btn[aria-current]{color:var(--text-active-blue-france)}.fr-pagination__link{--text-spacing:0;--title-spacing:0;--hover-tint:var(--hover);--underline-img:none;align-items:center;display:inline-flex;flex-direction:row;font-size:1rem;line-height:1.5rem;margin-bottom:1rem;margin-left:.125rem;margin-right:.125rem;min-height:2rem;min-width:2rem;padding:.25rem .75rem;position:relative;width:-moz-fit-content;width:fit-content;z-index:1}.fr-pagination__link:after,.fr-pagination__link:before{display:block}.fr-pagination{--underline-img:none;--ul-type:none;--ol-type:none;--ul-start:0;--ol-start:0;--xl-block:0;--li-bottom:0;--ol-content:none;color:var(--text-action-high-grey)}.fr-pagination__list{align-items:center;display:flex;flex-direction:row;flex-wrap:wrap;justify-content:flex-start}.fr-pagination__list>:first-child,.fr-pagination__list>:first-child *{margin-left:0}.fr-pagination__list>:last-child,.fr-pagination__list>:last-child *{margin-right:0}.fr-pagination__link[aria-current]:not([href]){cursor:default;pointer-events:none}.fr-pagination__link--prev{font-size:1rem;line-height:1.5rem;max-height:2rem;max-width:2rem;min-height:2rem;overflow:hidden;padding:.25rem;white-space:nowrap}.fr-pagination__link--prev:before{--icon-size:1.5rem;background-color:currentColor;content:"";display:inline-block;flex:0 0 auto;height:var(--icon-size);margin-left:0;margin-right:.25rem;-webkit-mask-image:url(icons/system/arrow-left-s-line.svg);mask-image:url(icons/system/arrow-left-s-line.svg);-webkit-mask-size:100% 100%;mask-size:100% 100%;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}.fr-pagination__link--next{font-size:1rem;line-height:1.5rem;max-height:2rem;max-width:2rem;min-height:2rem;overflow:hidden;padding:.25rem;white-space:nowrap}.fr-pagination__link--next:before{--icon-size:1.5rem;background-color:currentColor;content:"";display:inline-block;flex:0 0 auto;height:var(--icon-size);margin-left:0;margin-right:.25rem;-webkit-mask-image:url(icons/system/arrow-right-s-line.svg);mask-image:url(icons/system/arrow-right-s-line.svg);-webkit-mask-size:100% 100%;mask-size:100% 100%;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}.fr-pagination__link--prev{margin-left:-.625rem;margin-right:.875rem}.fr-pagination__link--next{margin-left:.875rem;margin-right:-.625rem}.fr-pagination__link[aria-current]{--idle:transparent;--hover:var(--background-active-blue-france-hover);--active:var(--background-active-blue-france-active);background-color:var(--background-active-blue-france);color:var(--text-inverted-blue-france)}.fr-pagination__link:not([aria-current]):disabled,a.fr-pagination__link:not([aria-current]):not([href]){color:var(--text-disabled-grey)}.fr-radio-group{position:relative}.fr-radio-group input[type=radio]{height:1.5rem;margin:0;opacity:0;position:absolute;width:1.5rem}.fr-radio-group input[type=radio]+label{-webkit-tap-highlight-color:transparent;align-items:center;display:flex;flex-direction:row;flex-wrap:wrap;justify-content:flex-start;margin-left:2rem;position:relative}.fr-radio-group input[type=radio]+label .fr-hint-text{margin:0;width:100%}.fr-radio-group input[type=radio]+label:before{border-radius:50%;box-shadow:inset 0 0 0 1px var(--border-action-high-grey),inset 0 0 0 12px var(--background-default-grey),inset 0 0 0 12px var(--background-action-high-blue-france);content:"";display:inline-block;height:1.5rem;left:-2rem;margin-right:.5rem;position:absolute;top:0;width:1.5rem}.fr-radio-rich{position:relative}.fr-radio-rich input[type=radio]{height:1rem;left:1.75rem;top:calc(50% - .5rem);width:1rem}.fr-radio-rich input[type=radio]+label{--idle:transparent;--hover:var(--background-default-grey-hover);--active:var(--background-default-grey-active);align-items:flex-start;background-color:var(--background-default-grey);box-shadow:inset 0 0 0 1px var(--border-default-grey);display:flex;flex-direction:column;justify-content:center;margin-left:0;min-height:5.5rem;padding:.5rem 6.5rem .5rem 3.5rem;width:100%}.fr-radio-rich input[type=radio]+label:before{box-shadow:inset 0 0 0 1px var(--border-action-high-grey),inset 0 0 0 8px var(--background-default-grey),inset 0 0 0 8px var(--background-action-high-blue-france);height:1rem;left:1.75rem;margin-top:-.5rem;position:absolute;top:50%;width:1rem}.fr-radio-rich input[type=radio]+label .fr-hint-text{margin-left:0}.fr-radio-rich input[type=radio]:disabled~.fr-radio-rich__img{filter:grayscale(1)}.fr-radio-rich input[type=radio]:not(:disabled)~label{--hover-tint:var(--hover);--active-tint:var(--active)}.fr-radio-rich input[type=radio]:not(:disabled)~label:hover{background-color:var(--hover-tint)}.fr-radio-rich input[type=radio]:not(:disabled)~label:active{background-color:var(--active-tint)}.fr-radio-rich input[type=radio]:not(:disabled)~label:hover~.fr-radio-rich__img{--brightness:calc(100% + var(--brighten)*10%)}.fr-radio-rich input[type=radio]:not(:disabled)~label:active~.fr-radio-rich__img{--brightness:calc(100% + var(--brighten)*20%)}.fr-radio-rich__img{box-shadow:inset 1px 0 0 0 var(--border-default-grey);display:flex;filter:brightness(var(--brightness));flex-direction:row;height:5rem;padding-left:.25rem;pointer-events:none;position:absolute;right:.25rem;top:.25rem;width:5.25rem}.fr-radio-rich__img svg{max-width:5rem;object-fit:cover}.fr-radio-group input[type=radio]:disabled+label:before{box-shadow:inset 0 0 0 1px var(--border-disabled-grey),inset 0 0 0 12px var(--background-default-grey),inset 0 0 0 12px var(--text-disabled-grey)}.fr-radio-group input[type=radio]:checked+label:before{box-shadow:inset 0 0 0 1px var(--border-action-high-grey),inset 0 0 0 6px var(--background-default-grey),inset 0 0 0 12px var(--background-action-high-blue-france)}.fr-radio-group input[type=radio]:checked:disabled+label:before{box-shadow:inset 0 0 0 1px var(--border-disabled-grey),inset 0 0 0 6px var(--background-default-grey),inset 0 0 0 12px var(--text-disabled-grey)}.fr-radio-rich input[type=radio]:disabled+label:before{box-shadow:inset 0 0 0 1px var(--border-disabled-grey),inset 0 0 0 8px var(--background-default-grey),inset 0 0 0 8px var(--text-disabled-grey)}.fr-radio-rich input[type=radio]:checked+label{box-shadow:inset 0 0 0 1px var(--border-action-high-blue-france)}.fr-radio-rich input[type=radio]:checked+label:before{box-shadow:inset 0 0 0 1px var(--border-action-high-grey),inset 0 0 0 4px var(--background-default-grey),inset 0 0 0 8px var(--background-action-high-blue-france)}.fr-radio-rich input[type=radio]:checked:disabled+label{box-shadow:inset 0 0 0 1px var(--text-disabled-grey)}.fr-radio-rich input[type=radio]:checked:disabled+label:before{box-shadow:inset 0 0 0 1px var(--border-disabled-grey),inset 0 0 0 4px var(--background-default-grey),inset 0 0 0 8px var(--text-disabled-grey)}.fr-fieldset .fr-fieldset__content .fr-radio-rich:first-child input[type=radio]+label{margin-top:.75rem}.fr-fieldset .fr-fieldset__content .fr-radio-rich input[type=radio]+label{margin-bottom:1rem;margin-top:.5rem}.fr-fieldset .fr-fieldset__content .fr-radio-rich:last-child input[type=radio]+label{margin-bottom:.75rem}.fr-modal{--ground:2000;align-items:stretch;background-color:hsla(0,0%,9%,.64);border:none;bottom:0;color:inherit;display:flex;flex-direction:column;height:100%;justify-content:space-between;left:0;margin:0;opacity:0;padding:0;position:fixed;right:0;top:0;transition:opacity .3s,visibility .3s;visibility:hidden;width:100%;z-index:1750}.fr-modal>.fr-container{pointer-events:none}.fr-modal:focus{outline:none}.fr-modal:before{content:""}.fr-modal:after,.fr-modal:before{display:block;flex:1 0 2rem;height:2rem;width:0}.fr-modal--top:before,.fr-modal:after{content:none}.fr-modal--top:after{content:""}.fr-modal--opened{height:100%;opacity:1;transition:opacity .3s,visibility .3s;visibility:inherit;width:100%}.fr-modal__body{--modal-max-height:calc(100vh - 2rem);--idle:transparent;--hover:var(--background-lifted-grey-hover);--active:var(--background-lifted-grey-active);background-color:var(--background-lifted-grey);filter:drop-shadow(var(--lifted-shadow));flex:1 1 auto;max-height:var(--modal-max-height);overflow-y:auto;pointer-events:all;z-index:calc(var(--ground) + 2000)}.fr-modal__header{align-items:center;display:flex;flex:auto 0 0;padding:1rem 1rem .5rem}.fr-modal__content{margin-bottom:3.5rem;padding-left:1rem;padding-right:1rem}.fr-modal__footer{--idle:transparent;--hover:var(--background-lifted-grey-hover);--active:var(--background-lifted-grey-active);background-color:var(--background-lifted-grey);bottom:0;display:flex;flex:auto 0 0;margin-top:-2.5rem;padding:1rem;position:sticky;transition:box-shadow .3s}.fr-modal__title{--title-spacing:0 0 1rem 0;color:var(--text-title-grey);font-size:1.375rem;font-weight:700;line-height:1.75rem}.fr-modal__title[class*=" fr-fi-"],.fr-modal__title[class^=fr-fi-]{margin-right:.5rem}.fr-nav{--underline-img:none;--ul-type:none;--ol-type:none;--ul-start:0;--ol-start:0;--xl-block:0;--li-bottom:0;--ol-content:none;--text-spacing:0;--title-spacing:0}.fr-nav__list{display:flex;flex-direction:column;margin:0;padding:0}.fr-nav__list>*>.fr-nav__btn,.fr-nav__list>*>.fr-nav__link,.fr-nav__list>.fr-nav__btn,.fr-nav__list>.fr-nav__link{font-weight:700}.fr-nav__item{align-items:stretch;display:flex;flex:0 1 auto;flex-direction:column;position:relative}.fr-nav__item:before{bottom:0;box-shadow:0 -1px 0 0 var(--border-default-grey),inset 0 -1px 0 0 var(--border-default-grey);content:"";display:block;height:100%;left:0;pointer-events:none;position:absolute;right:0;top:0;width:100%}.fr-nav__item .fr-btn{min-height:3rem}.fr-nav__btn,.fr-nav__link{--hover-tint:var(--hover);--active-tint:var(--active);color:var(--text-action-high-grey);font-size:1rem;line-height:1.5rem;padding:.75rem 0;text-align:left;width:100%}.fr-nav__btn[aria-current],.fr-nav__link[aria-current]{color:var(--text-active-blue-france);position:relative}.fr-nav__btn[aria-current]:before,.fr-nav__link[aria-current]:before{--idle:transparent;--hover:var(--background-active-blue-france-hover);--active:var(--background-active-blue-france-active);background-color:var(--background-active-blue-france);content:"";display:block;height:1.5rem;left:-1rem;margin-top:-.75rem;position:absolute;top:50%;width:2px}.fr-nav__link{display:block}.fr-nav__link[aria-current]:not([href]){cursor:default;pointer-events:none}.fr-nav__btn{align-items:center;display:flex;flex-direction:row;justify-content:space-between}.fr-nav__btn:after{--icon-size:1rem;background-color:currentColor;content:"";display:inline-block;flex:0 0 auto;height:var(--icon-size);margin-left:.5rem;margin-right:0;-webkit-mask-image:url(icons/system/arrow-down-s-line.svg);mask-image:url(icons/system/arrow-down-s-line.svg);-webkit-mask-size:100% 100%;mask-size:100% 100%;transition:transform .3s;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}.fr-nav__btn[aria-expanded=true]:after{transform:rotate(-180deg)}.fr-menu{margin:-4px -1rem;padding:4px 1rem;width:auto}.fr-menu__list{margin:0;padding:.5rem 0 1.5rem}.fr-menu .fr-nav__link{padding-left:1rem;padding-right:1rem}.fr-menu .fr-nav__link:before{left:0}.fr-nav__item:first-child:before{box-shadow:inset 0 -1px 0 0 var(--border-default-grey)}.fr-nav__item:last-child:before{box-shadow:0 -1px 0 0 var(--border-default-grey)}.fr-footer{--ul-type:none;--ol-type:none;--ul-start:0;--ol-start:0;--xl-block:0;--li-bottom:0;--ol-content:none;box-shadow:inset 0 2px 0 0 var(--border-plain-blue-france),inset 0 -1px 0 0 var(--border-default-grey);padding-top:2.5rem;width:100%}.fr-footer__body{align-items:center;display:flex;flex-direction:row;flex-wrap:wrap;margin-bottom:1rem}.fr-footer__body+.fr-footer__bottom{margin-top:1rem}.fr-footer__brand{align-items:center;display:flex;flex-basis:100%;flex-direction:row}.fr-footer__brand .fr-logo{font-size:1.05rem;margin:-1rem;padding:1rem}.fr-footer__brand .fr-logo:before{background-position:0 -.0625rem,0 0,0 0;background-size:2.75rem 1.125rem,2.75rem 1rem,0;height:1rem;margin-bottom:.3333333333rem;width:2.75rem}.fr-footer__brand .fr-logo:after{background-position:0 calc(100% + 1.875rem);background-size:5.25rem 3.75rem;min-width:2.625rem;padding-top:2.2083333333rem}[data-fr-theme=dark] .fr-footer__brand .fr-logo:after{background-position:-2.625rem 100%}.fr-footer__content{display:flex;flex-basis:100%;flex-wrap:wrap;margin-top:1.5rem}.fr-footer__content-desc{--underline-img:linear-gradient(0deg,currentColor,currentColor);--text-spacing:0 0 0.5rem 0;font-size:.875rem;line-height:1.5rem;width:100%}.fr-footer__content-list{align-self:center;display:flex;flex-direction:row;flex-wrap:wrap}.fr-footer__content-list>li{margin-bottom:.5rem;margin-right:1rem;margin-top:.5rem}.fr-footer__content-list>li:before{content:none}.fr-footer__content-list>li:last-child{margin-right:0}.fr-footer__content-link{font-size:.875rem;font-weight:700;line-height:1.5rem}.fr-footer__content-link:not(:hover):not(:active){--underline-idle-width:0}.fr-footer__bottom{align-items:center;box-shadow:inset 0 1px 0 0 var(--border-default-grey);display:flex;flex-direction:row;flex-wrap:wrap;margin-top:2.5rem}.fr-footer__bottom .fr-btn{color:var(--text-mention-grey);font-size:.75rem;line-height:1.25rem;max-height:none;max-width:100%;min-height:1.25rem;overflow:initial;padding:0 .5rem}.fr-footer__bottom .fr-btn:before{--icon-size:1rem;margin-left:-.125rem;margin-right:.5rem}.fr-footer__bottom-list{align-items:center;flex-wrap:wrap;margin:0;padding:.5rem 0 1rem;width:100%}.fr-footer__bottom-item{display:inline;margin:.5rem 0 0 .25rem;position:relative}.fr-footer__bottom-item:before{box-shadow:inset 0 0 0 1px var(--border-default-grey);content:"";display:inline-block;height:1rem;margin-bottom:.5rem;margin-right:.25rem;margin-top:.5rem;position:relative;vertical-align:middle;width:1px}.fr-footer__bottom-item:first-child{margin:.5rem 0 0}.fr-footer__bottom-item:first-child:before{content:none}.fr-footer__bottom-link{color:var(--text-mention-grey);font-size:.75rem;line-height:1.25rem}.fr-footer__bottom-link:not(:hover):not(:active){--underline-idle-width:0}.fr-footer__bottom-copy{--text-spacing:0 0 1rem 0;color:var(--text-mention-grey);margin-top:.5rem}.fr-footer__bottom-copy *{font-size:.75rem;line-height:1.25rem}.fr-footer__content-link{color:var(--text-title-grey)}.fr-input{--idle:transparent;--hover:var(--background-contrast-grey-hover);--active:var(--background-contrast-grey-active);background-color:var(--background-contrast-grey);border-radius:.25rem .25rem 0 0;box-shadow:inset 0 -2px 0 0 var(--border-plain-grey);color:var(--text-label-grey);display:block;font-size:1rem;line-height:1.5rem;padding:.5rem 1rem;width:100%}.fr-input::placeholder{color:var(--text-mention-grey);font-style:italic;opacity:1}.fr-input::-webkit-contacts-auto-fill-button{--idle:transparent;--hover:var(--text-label-grey-hover);--active:var(--text-label-grey-active);background-color:var(--text-label-grey);cursor:pointer}.fr-input:not(textarea){max-height:2.5rem}.fr-input:disabled{box-shadow:inset 0 -2px 0 0 var(--border-disabled-grey);color:var(--text-disabled-grey)}.fr-input:-webkit-autofill,.fr-input:-webkit-autofill:focus,.fr-input:-webkit-autofill:hover,.fr-input:autofill,.fr-input:autofill:focus,.fr-input:autofill:hover{-webkit-text-fill-color:var(--text-label-grey);box-shadow:inset 0 -2px 0 0 var(--border-plain-grey),inset 0 0 0 1000px var(--background-contrast-info)}.fr-search-bar{display:flex;flex-direction:row}.fr-search-bar .fr-label{clip:rect(0,0,0,0);border:0;height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;white-space:nowrap;width:1px}.fr-search-bar .fr-input{border-radius:.25rem 0 0;box-shadow:inset 0 -2px 0 0 var(--border-action-high-blue-france);margin:0;max-height:none}.fr-search-bar .fr-input::placeholder{font-style:italic}.fr-search-bar .fr-btn{border-radius:0 .25rem 0 0;flex:1 0 auto;font-size:1rem;line-height:1.5rem;max-height:2.5rem;max-width:2.5rem;min-height:2.5rem;overflow:hidden;padding:.5rem;white-space:nowrap}.fr-search-bar .fr-btn:before{--icon-size:1.5rem;background-color:currentColor;content:"";display:inline-block;flex:0 0 auto;height:var(--icon-size);margin-left:0;margin-right:.5rem;-webkit-mask-image:url(icons/system/search-line.svg);mask-image:url(icons/system/search-line.svg);-webkit-mask-size:100% 100%;mask-size:100% 100%;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}.fr-header{--underline-img:none;--ul-type:none;--ol-type:none;--ul-start:0;--ol-start:0;--xl-block:0;--li-bottom:0;--ol-content:none;--text-spacing:0;--title-spacing:0;position:relative;width:100%}.fr-header__body-row{align-items:center;display:flex;flex-direction:row;justify-content:flex-start;margin:0 -1rem}.fr-header__brand{--idle:transparent;--hover:var(--background-raised-grey-hover);--active:var(--background-raised-grey-active);background-color:var(--background-raised-grey);filter:drop-shadow(var(--raised-shadow));flex-wrap:wrap;padding-left:.25rem;padding-right:.25rem;z-index:calc(var(--ground) + 500)}.fr-header__brand,.fr-header__brand-top{align-items:center;display:flex;flex-direction:row;justify-content:flex-start;width:100%}.fr-header__logo{flex:0 0 auto;order:1;padding:.75rem}.fr-header__logo .fr-logo{font-size:.7875rem;margin:-.75rem;padding:.75rem}.fr-header__logo .fr-logo:before{background-position:0 -.046875rem,0 0,0 0;background-size:2.0625rem .84375rem,2.0625rem .75rem,0;height:.75rem;margin-bottom:.25rem;width:2.0625rem}.fr-header__logo .fr-logo:after{background-position:0 calc(100% + 1.40625rem);background-size:3.9375rem 2.8125rem;min-width:1.96875rem;padding-top:1.65625rem}[data-fr-theme=dark] .fr-header__logo .fr-logo:after{background-position:-1.96875rem 100%}.fr-header__service{box-shadow:inset 0 1px 0 0 var(--border-default-grey);margin-left:.75rem;margin-right:.75rem;padding-bottom:.75rem;padding-top:.75rem;width:100%}.fr-header__service-title{font-size:1.125rem;font-weight:700;line-height:1.5rem}.fr-header .fr-modal{--idle:transparent;--hover:var(--background-lifted-grey-hover);--active:var(--background-lifted-grey-active);background-color:var(--background-lifted-grey);justify-content:normal;overflow:auto}.fr-header .fr-modal:not([role=dialog]){transition:none}.fr-header .fr-modal:after,.fr-header .fr-modal:before{content:none}.fr-header .fr-modal>*>.fr-btn--close{margin-bottom:1.5rem}.fr-header .fr-modal>.fr-container{height:100%;padding-bottom:4.5rem;padding-top:1rem;pointer-events:all}.fr-header__navbar{align-items:flex-end;align-self:flex-start;display:flex;flex:0 0 auto;flex-direction:row;margin-left:auto;order:3;padding:.25rem;z-index:calc(var(--ground) + 1000)}.fr-header__navbar .fr-btn{--hover:inherit;--active:inherit;background-color:transparent;color:var(--text-action-high-blue-france);flex:0 0 auto;font-size:1rem;line-height:1.5rem;max-height:2.5rem;max-width:2.5rem;min-height:2.5rem;overflow:hidden;padding:.5rem;white-space:nowrap}.fr-header__navbar .fr-btn:before{--icon-size:1.5rem;margin-left:0;margin-right:.5rem}.fr-header__navbar .fr-btn--menu:after,.fr-header__navbar .fr-btn--menu:before{--icon-size:1.5rem;background-color:currentColor;display:inline-block;flex:0 0 auto;height:var(--icon-size);-webkit-mask-image:url(icons/system/menu-fill.svg);mask-image:url(icons/system/menu-fill.svg);-webkit-mask-size:100% 100%;mask-size:100% 100%;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}.fr-header__navbar .fr-btn--menu:before{content:""}.fr-header__navbar .fr-btn--search:after,.fr-header__navbar .fr-btn--search:before{--icon-size:1.5rem;background-color:currentColor;display:inline-block;flex:0 0 auto;height:var(--icon-size);-webkit-mask-image:url(icons/system/search-line.svg);mask-image:url(icons/system/search-line.svg);-webkit-mask-size:100% 100%;mask-size:100% 100%;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}.fr-header__navbar .fr-btn--search:before{content:""}.fr-header .fr-header__menu-links:after{content:"";display:block;height:1px;margin:.75rem -1rem;width:calc(100% + 2rem)}.fr-header__menu-links:after{box-shadow:inset 0 1px 0 0 var(--border-default-grey)}.fr-header__menu-links .fr-btn{--hover:inherit;--active:inherit;background-color:transparent;box-shadow:none;color:var(--text-action-high-blue-france)}.fr-header__menu-links .fr-btn:disabled,.fr-header__menu-links a.fr-btn:not([href]){--hover:inherit;--active:inherit;background-color:transparent;color:var(--text-disabled-grey)}.fr-header__navbar .fr-btn:disabled,.fr-header__navbar a.fr-btn:not([href]){--hover:inherit;--active:inherit;background-color:transparent;color:var(--text-disabled-grey)}.fr-header__navbar .fr-btn--menu{color:var(--text-default-grey)}@media (min-width:36em){
+ */a{--hover-tint:var(--idle);--active-tint:var(--active);color:inherit;text-decoration:none}:root{--underline-max-width:100%;--underline-hover-width:0;--underline-idle-width:var(--underline-max-width);--underline-x:calc(var(--underline-max-width)*0);--underline-thickness:max(1px,0.0625em);--underline-img:linear-gradient(0deg,currentColor,currentColor);--external-link-content:"";--ul-type:disc;--ol-type:decimal;--ul-start:1rem;--ol-start:1.5rem;--xl-block:0.5rem;--li-bottom:0.25rem;--xl-base:1em;--ol-content:counters(li-counter,".") ".  ";--text-spacing:0 0 1.5rem;--title-spacing:0 0 1.5rem;--display-spacing:0 0 2rem;--background-default-grey:var(--grey-1000-50);--background-default-grey-hover:var(--grey-1000-50-hover);--background-default-grey-active:var(--grey-1000-50-active);--background-alt-grey:var(--grey-975-75);--background-alt-grey-hover:var(--grey-975-75-hover);--background-alt-grey-active:var(--grey-975-75-active);--background-alt-blue-france:var(--blue-france-975-75);--background-alt-blue-france-hover:var(--blue-france-975-75-hover);--background-alt-blue-france-active:var(--blue-france-975-75-active);--background-alt-red-marianne:var(--red-marianne-975-75);--background-alt-red-marianne-hover:var(--red-marianne-975-75-hover);--background-alt-red-marianne-active:var(--red-marianne-975-75-active);--background-alt-green-tilleul-verveine:var(--green-tilleul-verveine-975-75);--background-alt-green-tilleul-verveine-hover:var(--green-tilleul-verveine-975-75-hover);--background-alt-green-tilleul-verveine-active:var(--green-tilleul-verveine-975-75-active);--background-alt-green-bourgeon:var(--green-bourgeon-975-75);--background-alt-green-bourgeon-hover:var(--green-bourgeon-975-75-hover);--background-alt-green-bourgeon-active:var(--green-bourgeon-975-75-active);--background-alt-green-emeraude:var(--green-emeraude-975-75);--background-alt-green-emeraude-hover:var(--green-emeraude-975-75-hover);--background-alt-green-emeraude-active:var(--green-emeraude-975-75-active);--background-alt-green-menthe:var(--green-menthe-975-75);--background-alt-green-menthe-hover:var(--green-menthe-975-75-hover);--background-alt-green-menthe-active:var(--green-menthe-975-75-active);--background-alt-green-archipel:var(--green-archipel-975-75);--background-alt-green-archipel-hover:var(--green-archipel-975-75-hover);--background-alt-green-archipel-active:var(--green-archipel-975-75-active);--background-alt-blue-ecume:var(--blue-ecume-975-75);--background-alt-blue-ecume-hover:var(--blue-ecume-975-75-hover);--background-alt-blue-ecume-active:var(--blue-ecume-975-75-active);--background-alt-blue-cumulus:var(--blue-cumulus-975-75);--background-alt-blue-cumulus-hover:var(--blue-cumulus-975-75-hover);--background-alt-blue-cumulus-active:var(--blue-cumulus-975-75-active);--background-alt-purple-glycine:var(--purple-glycine-975-75);--background-alt-purple-glycine-hover:var(--purple-glycine-975-75-hover);--background-alt-purple-glycine-active:var(--purple-glycine-975-75-active);--background-alt-pink-macaron:var(--pink-macaron-975-75);--background-alt-pink-macaron-hover:var(--pink-macaron-975-75-hover);--background-alt-pink-macaron-active:var(--pink-macaron-975-75-active);--background-alt-pink-tuile:var(--pink-tuile-975-75);--background-alt-pink-tuile-hover:var(--pink-tuile-975-75-hover);--background-alt-pink-tuile-active:var(--pink-tuile-975-75-active);--background-alt-yellow-tournesol:var(--yellow-tournesol-975-75);--background-alt-yellow-tournesol-hover:var(--yellow-tournesol-975-75-hover);--background-alt-yellow-tournesol-active:var(--yellow-tournesol-975-75-active);--background-alt-yellow-moutarde:var(--yellow-moutarde-975-75);--background-alt-yellow-moutarde-hover:var(--yellow-moutarde-975-75-hover);--background-alt-yellow-moutarde-active:var(--yellow-moutarde-975-75-active);--background-alt-orange-terre-battue:var(--orange-terre-battue-975-75);--background-alt-orange-terre-battue-hover:var(--orange-terre-battue-975-75-hover);--background-alt-orange-terre-battue-active:var(--orange-terre-battue-975-75-active);--background-alt-brown-cafe-creme:var(--brown-cafe-creme-975-75);--background-alt-brown-cafe-creme-hover:var(--brown-cafe-creme-975-75-hover);--background-alt-brown-cafe-creme-active:var(--brown-cafe-creme-975-75-active);--background-alt-brown-caramel:var(--brown-caramel-975-75);--background-alt-brown-caramel-hover:var(--brown-caramel-975-75-hover);--background-alt-brown-caramel-active:var(--brown-caramel-975-75-active);--background-alt-brown-opera:var(--brown-opera-975-75);--background-alt-brown-opera-hover:var(--brown-opera-975-75-hover);--background-alt-brown-opera-active:var(--brown-opera-975-75-active);--background-alt-beige-gris-galet:var(--beige-gris-galet-975-75);--background-alt-beige-gris-galet-hover:var(--beige-gris-galet-975-75-hover);--background-alt-beige-gris-galet-active:var(--beige-gris-galet-975-75-active);--background-contrast-grey:var(--grey-950-100);--background-contrast-grey-hover:var(--grey-950-100-hover);--background-contrast-grey-active:var(--grey-950-100-active);--background-contrast-blue-france:var(--blue-france-950-100);--background-contrast-blue-france-hover:var(--blue-france-950-100-hover);--background-contrast-blue-france-active:var(--blue-france-950-100-active);--background-contrast-red-marianne:var(--red-marianne-950-100);--background-contrast-red-marianne-hover:var(--red-marianne-950-100-hover);--background-contrast-red-marianne-active:var(--red-marianne-950-100-active);--background-contrast-green-tilleul-verveine:var(--green-tilleul-verveine-950-100);--background-contrast-green-tilleul-verveine-hover:var(--green-tilleul-verveine-950-100-hover);--background-contrast-green-tilleul-verveine-active:var(--green-tilleul-verveine-950-100-active);--background-contrast-green-bourgeon:var(--green-bourgeon-950-100);--background-contrast-green-bourgeon-hover:var(--green-bourgeon-950-100-hover);--background-contrast-green-bourgeon-active:var(--green-bourgeon-950-100-active);--background-contrast-green-emeraude:var(--green-emeraude-950-100);--background-contrast-green-emeraude-hover:var(--green-emeraude-950-100-hover);--background-contrast-green-emeraude-active:var(--green-emeraude-950-100-active);--background-contrast-green-menthe:var(--green-menthe-950-100);--background-contrast-green-menthe-hover:var(--green-menthe-950-100-hover);--background-contrast-green-menthe-active:var(--green-menthe-950-100-active);--background-contrast-green-archipel:var(--green-archipel-950-100);--background-contrast-green-archipel-hover:var(--green-archipel-950-100-hover);--background-contrast-green-archipel-active:var(--green-archipel-950-100-active);--background-contrast-blue-ecume:var(--blue-ecume-950-100);--background-contrast-blue-ecume-hover:var(--blue-ecume-950-100-hover);--background-contrast-blue-ecume-active:var(--blue-ecume-950-100-active);--background-contrast-blue-cumulus:var(--blue-cumulus-950-100);--background-contrast-blue-cumulus-hover:var(--blue-cumulus-950-100-hover);--background-contrast-blue-cumulus-active:var(--blue-cumulus-950-100-active);--background-contrast-purple-glycine:var(--purple-glycine-950-100);--background-contrast-purple-glycine-hover:var(--purple-glycine-950-100-hover);--background-contrast-purple-glycine-active:var(--purple-glycine-950-100-active);--background-contrast-pink-macaron:var(--pink-macaron-950-100);--background-contrast-pink-macaron-hover:var(--pink-macaron-950-100-hover);--background-contrast-pink-macaron-active:var(--pink-macaron-950-100-active);--background-contrast-pink-tuile:var(--pink-tuile-950-100);--background-contrast-pink-tuile-hover:var(--pink-tuile-950-100-hover);--background-contrast-pink-tuile-active:var(--pink-tuile-950-100-active);--background-contrast-yellow-tournesol:var(--yellow-tournesol-950-100);--background-contrast-yellow-tournesol-hover:var(--yellow-tournesol-950-100-hover);--background-contrast-yellow-tournesol-active:var(--yellow-tournesol-950-100-active);--background-contrast-yellow-moutarde:var(--yellow-moutarde-950-100);--background-contrast-yellow-moutarde-hover:var(--yellow-moutarde-950-100-hover);--background-contrast-yellow-moutarde-active:var(--yellow-moutarde-950-100-active);--background-contrast-orange-terre-battue:var(--orange-terre-battue-950-100);--background-contrast-orange-terre-battue-hover:var(--orange-terre-battue-950-100-hover);--background-contrast-orange-terre-battue-active:var(--orange-terre-battue-950-100-active);--background-contrast-brown-cafe-creme:var(--brown-cafe-creme-950-100);--background-contrast-brown-cafe-creme-hover:var(--brown-cafe-creme-950-100-hover);--background-contrast-brown-cafe-creme-active:var(--brown-cafe-creme-950-100-active);--background-contrast-brown-caramel:var(--brown-caramel-950-100);--background-contrast-brown-caramel-hover:var(--brown-caramel-950-100-hover);--background-contrast-brown-caramel-active:var(--brown-caramel-950-100-active);--background-contrast-brown-opera:var(--brown-opera-950-100);--background-contrast-brown-opera-hover:var(--brown-opera-950-100-hover);--background-contrast-brown-opera-active:var(--brown-opera-950-100-active);--background-contrast-beige-gris-galet:var(--beige-gris-galet-950-100);--background-contrast-beige-gris-galet-hover:var(--beige-gris-galet-950-100-hover);--background-contrast-beige-gris-galet-active:var(--beige-gris-galet-950-100-active);--background-contrast-info:var(--info-950-100);--background-contrast-info-hover:var(--info-950-100-hover);--background-contrast-info-active:var(--info-950-100-active);--background-contrast-success:var(--success-950-100);--background-contrast-success-hover:var(--success-950-100-hover);--background-contrast-success-active:var(--success-950-100-active);--background-contrast-warning:var(--warning-950-100);--background-contrast-warning-hover:var(--warning-950-100-hover);--background-contrast-warning-active:var(--warning-950-100-active);--background-contrast-error:var(--error-950-100);--background-contrast-error-hover:var(--error-950-100-hover);--background-contrast-error-active:var(--error-950-100-active);--background-flat-grey:var(--grey-200-850);--background-flat-info:var(--info-425-625);--background-flat-success:var(--success-425-625);--background-flat-warning:var(--warning-425-625);--background-flat-error:var(--error-425-625);--background-action-high-blue-france:var(--blue-france-sun-113-625);--background-action-high-blue-france-hover:var(--blue-france-sun-113-625-hover);--background-action-high-blue-france-active:var(--blue-france-sun-113-625-active);--background-action-high-red-marianne:var(--red-marianne-425-625);--background-action-high-red-marianne-hover:var(--red-marianne-425-625-hover);--background-action-high-red-marianne-active:var(--red-marianne-425-625-active);--background-action-high-green-tilleul-verveine:var(--green-tilleul-verveine-sun-418-moon-817);--background-action-high-green-tilleul-verveine-hover:var(--green-tilleul-verveine-sun-418-moon-817-hover);--background-action-high-green-tilleul-verveine-active:var(--green-tilleul-verveine-sun-418-moon-817-active);--background-action-high-green-bourgeon:var(--green-bourgeon-sun-425-moon-759);--background-action-high-green-bourgeon-hover:var(--green-bourgeon-sun-425-moon-759-hover);--background-action-high-green-bourgeon-active:var(--green-bourgeon-sun-425-moon-759-active);--background-action-high-green-emeraude:var(--green-emeraude-sun-425-moon-753);--background-action-high-green-emeraude-hover:var(--green-emeraude-sun-425-moon-753-hover);--background-action-high-green-emeraude-active:var(--green-emeraude-sun-425-moon-753-active);--background-action-high-green-menthe:var(--green-menthe-sun-373-moon-652);--background-action-high-green-menthe-hover:var(--green-menthe-sun-373-moon-652-hover);--background-action-high-green-menthe-active:var(--green-menthe-sun-373-moon-652-active);--background-action-high-green-archipel:var(--green-archipel-sun-391-moon-716);--background-action-high-green-archipel-hover:var(--green-archipel-sun-391-moon-716-hover);--background-action-high-green-archipel-active:var(--green-archipel-sun-391-moon-716-active);--background-action-high-blue-ecume:var(--blue-ecume-sun-247-moon-675);--background-action-high-blue-ecume-hover:var(--blue-ecume-sun-247-moon-675-hover);--background-action-high-blue-ecume-active:var(--blue-ecume-sun-247-moon-675-active);--background-action-high-blue-cumulus:var(--blue-cumulus-sun-368-moon-732);--background-action-high-blue-cumulus-hover:var(--blue-cumulus-sun-368-moon-732-hover);--background-action-high-blue-cumulus-active:var(--blue-cumulus-sun-368-moon-732-active);--background-action-high-purple-glycine:var(--purple-glycine-sun-319-moon-630);--background-action-high-purple-glycine-hover:var(--purple-glycine-sun-319-moon-630-hover);--background-action-high-purple-glycine-active:var(--purple-glycine-sun-319-moon-630-active);--background-action-high-pink-macaron:var(--pink-macaron-sun-406-moon-833);--background-action-high-pink-macaron-hover:var(--pink-macaron-sun-406-moon-833-hover);--background-action-high-pink-macaron-active:var(--pink-macaron-sun-406-moon-833-active);--background-action-high-pink-tuile:var(--pink-tuile-sun-425-moon-750);--background-action-high-pink-tuile-hover:var(--pink-tuile-sun-425-moon-750-hover);--background-action-high-pink-tuile-active:var(--pink-tuile-sun-425-moon-750-active);--background-action-high-yellow-tournesol:var(--yellow-tournesol-sun-407-moon-922);--background-action-high-yellow-tournesol-hover:var(--yellow-tournesol-sun-407-moon-922-hover);--background-action-high-yellow-tournesol-active:var(--yellow-tournesol-sun-407-moon-922-active);--background-action-high-yellow-moutarde:var(--yellow-moutarde-sun-348-moon-860);--background-action-high-yellow-moutarde-hover:var(--yellow-moutarde-sun-348-moon-860-hover);--background-action-high-yellow-moutarde-active:var(--yellow-moutarde-sun-348-moon-860-active);--background-action-high-orange-terre-battue:var(--orange-terre-battue-sun-370-moon-672);--background-action-high-orange-terre-battue-hover:var(--orange-terre-battue-sun-370-moon-672-hover);--background-action-high-orange-terre-battue-active:var(--orange-terre-battue-sun-370-moon-672-active);--background-action-high-brown-cafe-creme:var(--brown-cafe-creme-sun-383-moon-885);--background-action-high-brown-cafe-creme-hover:var(--brown-cafe-creme-sun-383-moon-885-hover);--background-action-high-brown-cafe-creme-active:var(--brown-cafe-creme-sun-383-moon-885-active);--background-action-high-brown-caramel:var(--brown-caramel-sun-425-moon-901);--background-action-high-brown-caramel-hover:var(--brown-caramel-sun-425-moon-901-hover);--background-action-high-brown-caramel-active:var(--brown-caramel-sun-425-moon-901-active);--background-action-high-brown-opera:var(--brown-opera-sun-395-moon-820);--background-action-high-brown-opera-hover:var(--brown-opera-sun-395-moon-820-hover);--background-action-high-brown-opera-active:var(--brown-opera-sun-395-moon-820-active);--background-action-high-beige-gris-galet:var(--beige-gris-galet-sun-407-moon-821);--background-action-high-beige-gris-galet-hover:var(--beige-gris-galet-sun-407-moon-821-hover);--background-action-high-beige-gris-galet-active:var(--beige-gris-galet-sun-407-moon-821-active);--background-action-high-info:var(--info-425-625);--background-action-high-info-hover:var(--info-425-625-hover);--background-action-high-info-active:var(--info-425-625-active);--background-action-high-success:var(--success-425-625);--background-action-high-success-hover:var(--success-425-625-hover);--background-action-high-success-active:var(--success-425-625-active);--background-action-high-warning:var(--warning-425-625);--background-action-high-warning-hover:var(--warning-425-625-hover);--background-action-high-warning-active:var(--warning-425-625-active);--background-action-high-error:var(--error-425-625);--background-action-high-error-hover:var(--error-425-625-hover);--background-action-high-error-active:var(--error-425-625-active);--background-action-low-blue-france:var(--blue-france-925-125);--background-action-low-blue-france-hover:var(--blue-france-925-125-hover);--background-action-low-blue-france-active:var(--blue-france-925-125-active);--background-action-low-red-marianne:var(--red-marianne-925-125);--background-action-low-red-marianne-hover:var(--red-marianne-925-125-hover);--background-action-low-red-marianne-active:var(--red-marianne-925-125-active);--background-action-low-green-tilleul-verveine:var(--green-tilleul-verveine-925-125);--background-action-low-green-tilleul-verveine-hover:var(--green-tilleul-verveine-925-125-hover);--background-action-low-green-tilleul-verveine-active:var(--green-tilleul-verveine-925-125-active);--background-action-low-green-bourgeon:var(--green-bourgeon-925-125);--background-action-low-green-bourgeon-hover:var(--green-bourgeon-925-125-hover);--background-action-low-green-bourgeon-active:var(--green-bourgeon-925-125-active);--background-action-low-green-emeraude:var(--green-emeraude-925-125);--background-action-low-green-emeraude-hover:var(--green-emeraude-925-125-hover);--background-action-low-green-emeraude-active:var(--green-emeraude-925-125-active);--background-action-low-green-menthe:var(--green-menthe-925-125);--background-action-low-green-menthe-hover:var(--green-menthe-925-125-hover);--background-action-low-green-menthe-active:var(--green-menthe-925-125-active);--background-action-low-green-archipel:var(--green-archipel-925-125);--background-action-low-green-archipel-hover:var(--green-archipel-925-125-hover);--background-action-low-green-archipel-active:var(--green-archipel-925-125-active);--background-action-low-blue-ecume:var(--blue-ecume-925-125);--background-action-low-blue-ecume-hover:var(--blue-ecume-925-125-hover);--background-action-low-blue-ecume-active:var(--blue-ecume-925-125-active);--background-action-low-blue-cumulus:var(--blue-cumulus-925-125);--background-action-low-blue-cumulus-hover:var(--blue-cumulus-925-125-hover);--background-action-low-blue-cumulus-active:var(--blue-cumulus-925-125-active);--background-action-low-purple-glycine:var(--purple-glycine-925-125);--background-action-low-purple-glycine-hover:var(--purple-glycine-925-125-hover);--background-action-low-purple-glycine-active:var(--purple-glycine-925-125-active);--background-action-low-pink-macaron:var(--pink-macaron-925-125);--background-action-low-pink-macaron-hover:var(--pink-macaron-925-125-hover);--background-action-low-pink-macaron-active:var(--pink-macaron-925-125-active);--background-action-low-pink-tuile:var(--pink-tuile-925-125);--background-action-low-pink-tuile-hover:var(--pink-tuile-925-125-hover);--background-action-low-pink-tuile-active:var(--pink-tuile-925-125-active);--background-action-low-yellow-tournesol:var(--yellow-tournesol-925-125);--background-action-low-yellow-tournesol-hover:var(--yellow-tournesol-925-125-hover);--background-action-low-yellow-tournesol-active:var(--yellow-tournesol-925-125-active);--background-action-low-yellow-moutarde:var(--yellow-moutarde-925-125);--background-action-low-yellow-moutarde-hover:var(--yellow-moutarde-925-125-hover);--background-action-low-yellow-moutarde-active:var(--yellow-moutarde-925-125-active);--background-action-low-orange-terre-battue:var(--orange-terre-battue-925-125);--background-action-low-orange-terre-battue-hover:var(--orange-terre-battue-925-125-hover);--background-action-low-orange-terre-battue-active:var(--orange-terre-battue-925-125-active);--background-action-low-brown-cafe-creme:var(--brown-cafe-creme-925-125);--background-action-low-brown-cafe-creme-hover:var(--brown-cafe-creme-925-125-hover);--background-action-low-brown-cafe-creme-active:var(--brown-cafe-creme-925-125-active);--background-action-low-brown-caramel:var(--brown-caramel-925-125);--background-action-low-brown-caramel-hover:var(--brown-caramel-925-125-hover);--background-action-low-brown-caramel-active:var(--brown-caramel-925-125-active);--background-action-low-brown-opera:var(--brown-opera-925-125);--background-action-low-brown-opera-hover:var(--brown-opera-925-125-hover);--background-action-low-brown-opera-active:var(--brown-opera-925-125-active);--background-action-low-beige-gris-galet:var(--beige-gris-galet-925-125);--background-action-low-beige-gris-galet-hover:var(--beige-gris-galet-925-125-hover);--background-action-low-beige-gris-galet-active:var(--beige-gris-galet-925-125-active);--background-active-blue-france:var(--blue-france-sun-113-625);--background-active-blue-france-hover:var(--blue-france-sun-113-625-hover);--background-active-blue-france-active:var(--blue-france-sun-113-625-active);--background-active-red-marianne:var(--red-marianne-425-625);--background-active-red-marianne-hover:var(--red-marianne-425-625-hover);--background-active-red-marianne-active:var(--red-marianne-425-625-active);--background-open-blue-france:var(--blue-france-925-125);--background-open-blue-france-hover:var(--blue-france-925-125-hover);--background-open-blue-france-active:var(--blue-france-925-125-active);--background-open-red-marianne:var(--red-marianne-925-125);--background-open-red-marianne-hover:var(--red-marianne-925-125-hover);--background-open-red-marianne-active:var(--red-marianne-925-125-active);--background-disabled-grey:var(--grey-925-125);--background-raised-grey:var(--grey-1000-75);--background-raised-grey-hover:var(--grey-1000-75-hover);--background-raised-grey-active:var(--grey-1000-75-active);--background-overlap-grey:var(--grey-1000-100);--background-overlap-grey-hover:var(--grey-1000-100-hover);--background-overlap-grey-active:var(--grey-1000-100-active);--background-lifted-grey:var(--grey-1000-75);--background-lifted-grey-hover:var(--grey-1000-75-hover);--background-lifted-grey-active:var(--grey-1000-75-active);--background-alt-raised-grey:var(--grey-975-100);--background-alt-raised-grey-hover:var(--grey-975-100-hover);--background-alt-raised-grey-active:var(--grey-975-100-active);--background-alt-overlap-grey:var(--grey-975-125);--background-alt-overlap-grey-hover:var(--grey-975-125-hover);--background-alt-overlap-grey-active:var(--grey-975-125-active);--background-contrast-raised-grey:var(--grey-950-125);--background-contrast-raised-grey-hover:var(--grey-950-125-hover);--background-contrast-raised-grey-active:var(--grey-950-125-active);--background-contrast-overlap-grey:var(--grey-950-150);--background-contrast-overlap-grey-hover:var(--grey-950-150-hover);--background-contrast-overlap-grey-active:var(--grey-950-150-active);--text-default-grey:var(--grey-200-850);--text-default-info:var(--info-425-625);--text-default-success:var(--success-425-625);--text-default-warning:var(--warning-425-625);--text-default-error:var(--error-425-625);--text-action-high-grey:var(--grey-50-1000);--text-action-high-blue-france:var(--blue-france-sun-113-625);--text-action-high-red-marianne:var(--red-marianne-425-625);--text-action-high-green-tilleul-verveine:var(--green-tilleul-verveine-sun-418-moon-817);--text-action-high-green-bourgeon:var(--green-bourgeon-sun-425-moon-759);--text-action-high-green-emeraude:var(--green-emeraude-sun-425-moon-753);--text-action-high-green-menthe:var(--green-menthe-sun-373-moon-652);--text-action-high-green-archipel:var(--green-archipel-sun-391-moon-716);--text-action-high-blue-ecume:var(--blue-ecume-sun-247-moon-675);--text-action-high-blue-cumulus:var(--blue-cumulus-sun-368-moon-732);--text-action-high-purple-glycine:var(--purple-glycine-sun-319-moon-630);--text-action-high-pink-macaron:var(--pink-macaron-sun-406-moon-833);--text-action-high-pink-tuile:var(--pink-tuile-sun-425-moon-750);--text-action-high-yellow-tournesol:var(--yellow-tournesol-sun-407-moon-922);--text-action-high-yellow-moutarde:var(--yellow-moutarde-sun-348-moon-860);--text-action-high-orange-terre-battue:var(--orange-terre-battue-sun-370-moon-672);--text-action-high-brown-cafe-creme:var(--brown-cafe-creme-sun-383-moon-885);--text-action-high-brown-caramel:var(--brown-caramel-sun-425-moon-901);--text-action-high-brown-opera:var(--brown-opera-sun-395-moon-820);--text-action-high-beige-gris-galet:var(--beige-gris-galet-sun-407-moon-821);--text-title-grey:var(--grey-50-1000);--text-title-blue-france:var(--blue-france-sun-113-625);--text-title-red-marianne:var(--red-marianne-425-625);--text-label-grey:var(--grey-50-1000);--text-label-blue-france:var(--blue-france-sun-113-625);--text-label-red-marianne:var(--red-marianne-425-625);--text-label-green-tilleul-verveine:var(--green-tilleul-verveine-sun-418-moon-817);--text-label-green-bourgeon:var(--green-bourgeon-sun-425-moon-759);--text-label-green-emeraude:var(--green-emeraude-sun-425-moon-753);--text-label-green-menthe:var(--green-menthe-sun-373-moon-652);--text-label-green-archipel:var(--green-archipel-sun-391-moon-716);--text-label-blue-ecume:var(--blue-ecume-sun-247-moon-675);--text-label-blue-cumulus:var(--blue-cumulus-sun-368-moon-732);--text-label-purple-glycine:var(--purple-glycine-sun-319-moon-630);--text-label-pink-macaron:var(--pink-macaron-sun-406-moon-833);--text-label-pink-tuile:var(--pink-tuile-sun-425-moon-750);--text-label-yellow-tournesol:var(--yellow-tournesol-sun-407-moon-922);--text-label-yellow-moutarde:var(--yellow-moutarde-sun-348-moon-860);--text-label-orange-terre-battue:var(--orange-terre-battue-sun-370-moon-672);--text-label-brown-cafe-creme:var(--brown-cafe-creme-sun-383-moon-885);--text-label-brown-caramel:var(--brown-caramel-sun-425-moon-901);--text-label-brown-opera:var(--brown-opera-sun-395-moon-820);--text-label-beige-gris-galet:var(--beige-gris-galet-sun-407-moon-821);--text-active-grey:var(--grey-50-1000);--text-active-blue-france:var(--blue-france-sun-113-625);--text-active-red-marianne:var(--red-marianne-425-625);--text-mention-grey:var(--grey-425-625);--text-inverted-grey:var(--grey-1000-50);--text-inverted-blue-france:var(--blue-france-975-sun-113);--text-inverted-red-marianne:var(--red-marianne-975-75);--text-inverted-info:var(--info-975-75);--text-inverted-success:var(--success-975-75);--text-inverted-warning:var(--warning-975-75);--text-inverted-error:var(--error-975-75);--text-inverted-green-tilleul-verveine:var(--green-tilleul-verveine-975-75);--text-inverted-green-bourgeon:var(--green-bourgeon-975-75);--text-inverted-green-emeraude:var(--green-emeraude-975-75);--text-inverted-green-menthe:var(--green-menthe-975-75);--text-inverted-green-archipel:var(--green-archipel-975-75);--text-inverted-blue-ecume:var(--blue-ecume-975-75);--text-inverted-blue-cumulus:var(--blue-cumulus-975-75);--text-inverted-purple-glycine:var(--purple-glycine-975-75);--text-inverted-pink-macaron:var(--pink-macaron-975-75);--text-inverted-pink-tuile:var(--pink-tuile-975-75);--text-inverted-yellow-tournesol:var(--yellow-tournesol-975-75);--text-inverted-yellow-moutarde:var(--yellow-moutarde-975-75);--text-inverted-orange-terre-battue:var(--orange-terre-battue-975-75);--text-inverted-brown-cafe-creme:var(--brown-cafe-creme-975-75);--text-inverted-brown-caramel:var(--brown-caramel-975-75);--text-inverted-brown-opera:var(--brown-opera-975-75);--text-inverted-beige-gris-galet:var(--beige-gris-galet-975-75);--text-disabled-grey:var(--grey-625-425);--border-default-grey:var(--grey-900-175);--border-default-blue-france:var(--blue-france-main-525);--border-default-red-marianne:var(--red-marianne-main-472);--border-default-green-tilleul-verveine:var(--green-tilleul-verveine-main-707);--border-default-green-bourgeon:var(--green-bourgeon-main-640);--border-default-green-emeraude:var(--green-emeraude-main-632);--border-default-green-menthe:var(--green-menthe-main-548);--border-default-green-archipel:var(--green-archipel-main-557);--border-default-blue-ecume:var(--blue-ecume-main-400);--border-default-blue-cumulus:var(--blue-cumulus-main-526);--border-default-purple-glycine:var(--purple-glycine-main-494);--border-default-pink-macaron:var(--pink-macaron-main-689);--border-default-pink-tuile:var(--pink-tuile-main-556);--border-default-yellow-tournesol:var(--yellow-tournesol-main-731);--border-default-yellow-moutarde:var(--yellow-moutarde-main-679);--border-default-orange-terre-battue:var(--orange-terre-battue-main-645);--border-default-brown-cafe-creme:var(--brown-cafe-creme-main-782);--border-default-brown-caramel:var(--brown-caramel-main-648);--border-default-brown-opera:var(--brown-opera-main-680);--border-default-beige-gris-galet:var(--beige-gris-galet-main-702);--border-active-blue-france:var(--blue-france-sun-113-625);--border-active-red-marianne:var(--red-marianne-425-625);--border-action-high-grey:var(--grey-50-1000);--border-action-high-blue-france:var(--blue-france-sun-113-625);--border-action-high-red-marianne:var(--red-marianne-425-625);--border-action-high-info:var(--info-425-625);--border-action-high-success:var(--success-425-625);--border-action-high-warning:var(--warning-425-625);--border-action-high-error:var(--error-425-625);--border-action-low-blue-france:var(--blue-france-850-200);--border-action-low-red-marianne:var(--red-marianne-850-200);--border-action-low-green-tilleul-verveine:var(--green-tilleul-verveine-850-200);--border-action-low-green-bourgeon:var(--green-bourgeon-850-200);--border-action-low-green-emeraude:var(--green-emeraude-850-200);--border-action-low-green-menthe:var(--green-menthe-850-200);--border-action-low-green-archipel:var(--green-archipel-850-200);--border-action-low-blue-ecume:var(--blue-ecume-850-200);--border-action-low-blue-cumulus:var(--blue-cumulus-850-200);--border-action-low-purple-glycine:var(--purple-glycine-850-200);--border-action-low-pink-macaron:var(--pink-macaron-850-200);--border-action-low-pink-tuile:var(--pink-tuile-850-200);--border-action-low-yellow-tournesol:var(--yellow-tournesol-850-200);--border-action-low-yellow-moutarde:var(--yellow-moutarde-850-200);--border-action-low-orange-terre-battue:var(--orange-terre-battue-850-200);--border-action-low-brown-cafe-creme:var(--brown-cafe-creme-850-200);--border-action-low-brown-caramel:var(--brown-caramel-850-200);--border-action-low-brown-opera:var(--brown-opera-850-200);--border-action-low-beige-gris-galet:var(--beige-gris-galet-850-200);--border-open-blue-france:var(--blue-france-925-125);--border-open-red-marianne:var(--red-marianne-925-125);--border-plain-grey:var(--grey-200-850);--border-plain-blue-france:var(--blue-france-sun-113-625);--border-plain-red-marianne:var(--red-marianne-425-625);--border-plain-info:var(--info-425-625);--border-plain-success:var(--success-425-625);--border-plain-warning:var(--warning-425-625);--border-plain-error:var(--error-425-625);--border-plain-green-tilleul-verveine:var(--green-tilleul-verveine-sun-418-moon-817);--border-plain-green-bourgeon:var(--green-bourgeon-sun-425-moon-759);--border-plain-green-emeraude:var(--green-emeraude-sun-425-moon-753);--border-plain-green-menthe:var(--green-menthe-sun-373-moon-652);--border-plain-green-archipel:var(--green-archipel-sun-391-moon-716);--border-plain-blue-ecume:var(--blue-ecume-sun-247-moon-675);--border-plain-blue-cumulus:var(--blue-cumulus-sun-368-moon-732);--border-plain-purple-glycine:var(--purple-glycine-sun-319-moon-630);--border-plain-pink-macaron:var(--pink-macaron-sun-406-moon-833);--border-plain-pink-tuile:var(--pink-tuile-sun-425-moon-750);--border-plain-yellow-tournesol:var(--yellow-tournesol-sun-407-moon-922);--border-plain-yellow-moutarde:var(--yellow-moutarde-sun-348-moon-860);--border-plain-orange-terre-battue:var(--orange-terre-battue-sun-370-moon-672);--border-plain-brown-cafe-creme:var(--brown-cafe-creme-sun-383-moon-885);--border-plain-brown-caramel:var(--brown-caramel-sun-425-moon-901);--border-plain-brown-opera:var(--brown-opera-sun-395-moon-820);--border-plain-beige-gris-galet:var(--beige-gris-galet-sun-407-moon-821);--border-disabled-grey:var(--grey-925-125);--artwork-major-blue-france:var(--blue-france-sun-113-625);--artwork-major-blue-france-hover:var(--blue-france-sun-113-625-hover);--artwork-major-blue-france-active:var(--blue-france-sun-113-625-active);--artwork-major-red-marianne:var(--red-marianne-425-625);--artwork-major-red-marianne-hover:var(--red-marianne-425-625-hover);--artwork-major-red-marianne-active:var(--red-marianne-425-625-active);--artwork-major-green-tilleul-verveine:var(--green-tilleul-verveine-sun-418-moon-817);--artwork-major-green-tilleul-verveine-hover:var(--green-tilleul-verveine-sun-418-moon-817-hover);--artwork-major-green-tilleul-verveine-active:var(--green-tilleul-verveine-sun-418-moon-817-active);--artwork-major-green-bourgeon:var(--green-bourgeon-sun-425-moon-759);--artwork-major-green-bourgeon-hover:var(--green-bourgeon-sun-425-moon-759-hover);--artwork-major-green-bourgeon-active:var(--green-bourgeon-sun-425-moon-759-active);--artwork-major-green-emeraude:var(--green-emeraude-sun-425-moon-753);--artwork-major-green-emeraude-hover:var(--green-emeraude-sun-425-moon-753-hover);--artwork-major-green-emeraude-active:var(--green-emeraude-sun-425-moon-753-active);--artwork-major-green-menthe:var(--green-menthe-sun-373-moon-652);--artwork-major-green-menthe-hover:var(--green-menthe-sun-373-moon-652-hover);--artwork-major-green-menthe-active:var(--green-menthe-sun-373-moon-652-active);--artwork-major-green-archipel:var(--green-archipel-sun-391-moon-716);--artwork-major-green-archipel-hover:var(--green-archipel-sun-391-moon-716-hover);--artwork-major-green-archipel-active:var(--green-archipel-sun-391-moon-716-active);--artwork-major-blue-ecume:var(--blue-ecume-sun-247-moon-675);--artwork-major-blue-ecume-hover:var(--blue-ecume-sun-247-moon-675-hover);--artwork-major-blue-ecume-active:var(--blue-ecume-sun-247-moon-675-active);--artwork-major-blue-cumulus:var(--blue-cumulus-sun-368-moon-732);--artwork-major-blue-cumulus-hover:var(--blue-cumulus-sun-368-moon-732-hover);--artwork-major-blue-cumulus-active:var(--blue-cumulus-sun-368-moon-732-active);--artwork-major-purple-glycine:var(--purple-glycine-sun-319-moon-630);--artwork-major-purple-glycine-hover:var(--purple-glycine-sun-319-moon-630-hover);--artwork-major-purple-glycine-active:var(--purple-glycine-sun-319-moon-630-active);--artwork-major-pink-macaron:var(--pink-macaron-sun-406-moon-833);--artwork-major-pink-macaron-hover:var(--pink-macaron-sun-406-moon-833-hover);--artwork-major-pink-macaron-active:var(--pink-macaron-sun-406-moon-833-active);--artwork-major-pink-tuile:var(--pink-tuile-sun-425-moon-750);--artwork-major-pink-tuile-hover:var(--pink-tuile-sun-425-moon-750-hover);--artwork-major-pink-tuile-active:var(--pink-tuile-sun-425-moon-750-active);--artwork-major-yellow-tournesol:var(--yellow-tournesol-sun-407-moon-922);--artwork-major-yellow-tournesol-hover:var(--yellow-tournesol-sun-407-moon-922-hover);--artwork-major-yellow-tournesol-active:var(--yellow-tournesol-sun-407-moon-922-active);--artwork-major-yellow-moutarde:var(--yellow-moutarde-sun-348-moon-860);--artwork-major-yellow-moutarde-hover:var(--yellow-moutarde-sun-348-moon-860-hover);--artwork-major-yellow-moutarde-active:var(--yellow-moutarde-sun-348-moon-860-active);--artwork-major-orange-terre-battue:var(--orange-terre-battue-sun-370-moon-672);--artwork-major-orange-terre-battue-hover:var(--orange-terre-battue-sun-370-moon-672-hover);--artwork-major-orange-terre-battue-active:var(--orange-terre-battue-sun-370-moon-672-active);--artwork-major-brown-cafe-creme:var(--brown-cafe-creme-sun-383-moon-885);--artwork-major-brown-cafe-creme-hover:var(--brown-cafe-creme-sun-383-moon-885-hover);--artwork-major-brown-cafe-creme-active:var(--brown-cafe-creme-sun-383-moon-885-active);--artwork-major-brown-caramel:var(--brown-caramel-sun-425-moon-901);--artwork-major-brown-caramel-hover:var(--brown-caramel-sun-425-moon-901-hover);--artwork-major-brown-caramel-active:var(--brown-caramel-sun-425-moon-901-active);--artwork-major-brown-opera:var(--brown-opera-sun-395-moon-820);--artwork-major-brown-opera-hover:var(--brown-opera-sun-395-moon-820-hover);--artwork-major-brown-opera-active:var(--brown-opera-sun-395-moon-820-active);--artwork-major-beige-gris-galet:var(--beige-gris-galet-sun-407-moon-821);--artwork-major-beige-gris-galet-hover:var(--beige-gris-galet-sun-407-moon-821-hover);--artwork-major-beige-gris-galet-active:var(--beige-gris-galet-sun-407-moon-821-active);--artwork-minor-blue-france:var(--blue-france-main-525);--artwork-minor-red-marianne:var(--red-marianne-main-472);--artwork-minor-green-tilleul-verveine:var(--green-tilleul-verveine-main-707);--artwork-minor-green-bourgeon:var(--green-bourgeon-main-640);--artwork-minor-green-emeraude:var(--green-emeraude-main-632);--artwork-minor-green-menthe:var(--green-menthe-main-548);--artwork-minor-green-archipel:var(--green-archipel-main-557);--artwork-minor-blue-ecume:var(--blue-ecume-main-400);--artwork-minor-blue-cumulus:var(--blue-cumulus-main-526);--artwork-minor-purple-glycine:var(--purple-glycine-main-494);--artwork-minor-pink-macaron:var(--pink-macaron-main-689);--artwork-minor-pink-tuile:var(--pink-tuile-main-556);--artwork-minor-yellow-tournesol:var(--yellow-tournesol-main-731);--artwork-minor-yellow-moutarde:var(--yellow-moutarde-main-679);--artwork-minor-orange-terre-battue:var(--orange-terre-battue-main-645);--artwork-minor-brown-cafe-creme:var(--brown-cafe-creme-main-782);--artwork-minor-brown-caramel:var(--brown-caramel-main-648);--artwork-minor-brown-opera:var(--brown-opera-main-680);--artwork-minor-beige-gris-galet:var(--beige-gris-galet-main-702);--artwork-decorative-grey:var(--grey-950-100);--artwork-decorative-blue-france:var(--blue-france-950-100);--artwork-decorative-red-marianne:var(--red-marianne-950-100);--artwork-decorative-green-tilleul-verveine:var(--green-tilleul-verveine-950-100);--artwork-decorative-green-bourgeon:var(--green-bourgeon-950-100);--artwork-decorative-green-emeraude:var(--green-emeraude-950-100);--artwork-decorative-green-menthe:var(--green-menthe-950-100);--artwork-decorative-green-archipel:var(--green-archipel-950-100);--artwork-decorative-blue-ecume:var(--blue-ecume-950-100);--artwork-decorative-blue-cumulus:var(--blue-cumulus-950-100);--artwork-decorative-purple-glycine:var(--purple-glycine-950-100);--artwork-decorative-pink-macaron:var(--pink-macaron-950-100);--artwork-decorative-pink-tuile:var(--pink-tuile-950-100);--artwork-decorative-yellow-tournesol:var(--yellow-tournesol-950-100);--artwork-decorative-yellow-moutarde:var(--yellow-moutarde-950-100);--artwork-decorative-orange-terre-battue:var(--orange-terre-battue-950-100);--artwork-decorative-brown-cafe-creme:var(--brown-cafe-creme-950-100);--artwork-decorative-brown-caramel:var(--brown-caramel-950-100);--artwork-decorative-brown-opera:var(--brown-opera-950-100);--artwork-decorative-beige-gris-galet:var(--beige-gris-galet-950-100);--artwork-background-grey:var(--grey-975-75);--artwork-background-blue-france:var(--blue-france-975-75);--artwork-background-red-marianne:var(--red-marianne-975-75);--artwork-background-green-tilleul-verveine:var(--green-tilleul-verveine-975-75);--artwork-background-green-bourgeon:var(--green-bourgeon-975-75);--artwork-background-green-emeraude:var(--green-emeraude-975-75);--artwork-background-green-menthe:var(--green-menthe-975-75);--artwork-background-green-archipel:var(--green-archipel-975-75);--artwork-background-blue-ecume:var(--blue-ecume-975-75);--artwork-background-blue-cumulus:var(--blue-cumulus-975-75);--artwork-background-purple-glycine:var(--purple-glycine-975-75);--artwork-background-pink-macaron:var(--pink-macaron-975-75);--artwork-background-pink-tuile:var(--pink-tuile-975-75);--artwork-background-yellow-tournesol:var(--yellow-tournesol-975-75);--artwork-background-yellow-moutarde:var(--yellow-moutarde-975-75);--artwork-background-orange-terre-battue:var(--orange-terre-battue-975-75);--artwork-background-brown-cafe-creme:var(--brown-cafe-creme-975-75);--artwork-background-brown-caramel:var(--brown-caramel-975-75);--artwork-background-brown-opera:var(--brown-opera-975-75);--artwork-background-beige-gris-galet:var(--beige-gris-galet-975-75);--artwork-motif-grey:var(--grey-925-125);--artwork-motif-blue-france:var(--blue-france-925-125);--artwork-motif-red-marianne:var(--red-marianne-925-125);--artwork-motif-green-tilleul-verveine:var(--green-tilleul-verveine-925-125);--artwork-motif-green-bourgeon:var(--green-bourgeon-925-125);--artwork-motif-green-emeraude:var(--green-emeraude-925-125);--artwork-motif-green-menthe:var(--green-menthe-925-125);--artwork-motif-green-archipel:var(--green-archipel-925-125);--artwork-motif-blue-ecume:var(--blue-ecume-925-125);--artwork-motif-blue-cumulus:var(--blue-cumulus-925-125);--artwork-motif-purple-glycine:var(--purple-glycine-925-125);--artwork-motif-pink-macaron:var(--pink-macaron-925-125);--artwork-motif-pink-tuile:var(--pink-tuile-925-125);--artwork-motif-yellow-tournesol:var(--yellow-tournesol-925-125);--artwork-motif-yellow-moutarde:var(--yellow-moutarde-925-125);--artwork-motif-orange-terre-battue:var(--orange-terre-battue-925-125);--artwork-motif-brown-cafe-creme:var(--brown-cafe-creme-925-125);--artwork-motif-brown-caramel:var(--brown-caramel-925-125);--artwork-motif-brown-opera:var(--brown-opera-925-125);--artwork-motif-beige-gris-galet:var(--beige-gris-galet-925-125);--grey-1000-50:#fff;--grey-1000-50-hover:#f6f6f6;--grey-1000-50-active:#ededed;--grey-975-75:#f6f6f6;--grey-975-75-hover:#dfdfdf;--grey-975-75-active:#cfcfcf;--grey-950-100:#eee;--grey-950-100-hover:#d2d2d2;--grey-950-100-active:#c1c1c1;--grey-200-850:#3a3a3a;--grey-925-125:#e5e5e5;--grey-1000-75:#fff;--grey-1000-75-hover:#f6f6f6;--grey-1000-75-active:#ededed;--grey-1000-100:#fff;--grey-1000-100-hover:#f6f6f6;--grey-1000-100-active:#ededed;--grey-975-100:#f6f6f6;--grey-975-100-hover:#dfdfdf;--grey-975-100-active:#cfcfcf;--grey-975-125:#f6f6f6;--grey-975-125-hover:#dfdfdf;--grey-975-125-active:#cfcfcf;--grey-950-125:#eee;--grey-950-125-hover:#d2d2d2;--grey-950-125-active:#c1c1c1;--grey-950-150:#eee;--grey-950-150-hover:#d2d2d2;--grey-950-150-active:#c1c1c1;--grey-50-1000:#161616;--grey-425-625:#666;--grey-625-425:#929292;--grey-900-175:#ddd;--blue-france-975-75:#f5f5fe;--blue-france-975-75-hover:#dcdcfc;--blue-france-975-75-active:#cbcbfa;--blue-france-950-100:#ececfe;--blue-france-950-100-hover:#cecefc;--blue-france-950-100-active:#bbbbfc;--blue-france-sun-113-625:#000091;--blue-france-sun-113-625-hover:#1212ff;--blue-france-sun-113-625-active:#2323ff;--blue-france-925-125:#e3e3fd;--blue-france-925-125-hover:#c1c1fb;--blue-france-925-125-active:#adadf9;--blue-france-975-sun-113:#f5f5fe;--blue-france-main-525:#6a6af4;--blue-france-850-200:#cacafb;--red-marianne-975-75:#fef4f4;--red-marianne-975-75-hover:#fcd7d7;--red-marianne-975-75-active:#fac4c4;--red-marianne-950-100:#fee9e9;--red-marianne-950-100-hover:#fdc5c5;--red-marianne-950-100-active:#fcafaf;--red-marianne-425-625:#c9191e;--red-marianne-425-625-hover:#f93f42;--red-marianne-425-625-active:#f95a5c;--red-marianne-925-125:#fddede;--red-marianne-925-125-hover:#fbb6b6;--red-marianne-925-125-active:#fa9e9e;--red-marianne-main-472:#e1000f;--red-marianne-850-200:#fcbfbf;--info-950-100:#e8edff;--info-950-100-hover:#c2d1ff;--info-950-100-active:#a9bfff;--info-425-625:#0063cb;--info-425-625-hover:#3b87ff;--info-425-625-active:#6798ff;--info-975-75:#f4f6ff;--success-950-100:#b8fec9;--success-950-100-hover:#46fd89;--success-950-100-active:#34eb7b;--success-425-625:#18753c;--success-425-625-hover:#27a959;--success-425-625-active:#2fc368;--success-975-75:#dffee6;--warning-950-100:#ffe9e6;--warning-950-100-hover:#ffc6bd;--warning-950-100-active:#ffb0a2;--warning-425-625:#b34000;--warning-425-625-hover:#ff6218;--warning-425-625-active:#ff7a55;--warning-975-75:#fff4f3;--error-950-100:#ffe9e9;--error-950-100-hover:#ffc5c5;--error-950-100-active:#ffafaf;--error-425-625:#ce0500;--error-425-625-hover:#ff2725;--error-425-625-active:#ff4140;--error-975-75:#fff4f4;--green-tilleul-verveine-975-75:#fef7da;--green-tilleul-verveine-975-75-hover:#fce552;--green-tilleul-verveine-975-75-active:#ebd54c;--green-tilleul-verveine-950-100:#fceeac;--green-tilleul-verveine-950-100-hover:#e8d45c;--green-tilleul-verveine-950-100-active:#d4c254;--green-tilleul-verveine-sun-418-moon-817:#66673d;--green-tilleul-verveine-sun-418-moon-817-hover:#929359;--green-tilleul-verveine-sun-418-moon-817-active:#a7a967;--green-tilleul-verveine-925-125:#fbe769;--green-tilleul-verveine-925-125-hover:#d7c655;--green-tilleul-verveine-925-125-active:#c2b24c;--green-tilleul-verveine-main-707:#b7a73f;--green-tilleul-verveine-850-200:#e2cf58;--green-bourgeon-975-75:#e6feda;--green-bourgeon-975-75-hover:#a7fc62;--green-bourgeon-975-75-active:#98ed4d;--green-bourgeon-950-100:#c9fcac;--green-bourgeon-950-100-hover:#9ae95d;--green-bourgeon-950-100-active:#8dd555;--green-bourgeon-sun-425-moon-759:#447049;--green-bourgeon-sun-425-moon-759-hover:#639f6a;--green-bourgeon-sun-425-moon-759-active:#72b77a;--green-bourgeon-925-125:#a9fb68;--green-bourgeon-925-125-hover:#8ed654;--green-bourgeon-925-125-active:#7fc04b;--green-bourgeon-main-640:#68a532;--green-bourgeon-850-200:#95e257;--green-emeraude-975-75:#e3fdeb;--green-emeraude-975-75-hover:#94f9b9;--green-emeraude-975-75-active:#6df1a3;--green-emeraude-950-100:#c3fad5;--green-emeraude-950-100-hover:#77eda5;--green-emeraude-950-100-active:#6dd897;--green-emeraude-sun-425-moon-753:#297254;--green-emeraude-sun-425-moon-753-hover:#3ea47a;--green-emeraude-sun-425-moon-753-active:#49bc8d;--green-emeraude-925-125:#9ef9be;--green-emeraude-925-125-hover:#69df97;--green-emeraude-925-125-active:#5ec988;--green-emeraude-main-632:#00a95f;--green-emeraude-850-200:#6fe49d;--green-menthe-975-75:#dffdf7;--green-menthe-975-75-hover:#84f9e7;--green-menthe-975-75-active:#70ebd8;--green-menthe-950-100:#bafaee;--green-menthe-950-100-hover:#79e7d5;--green-menthe-950-100-active:#6fd3c3;--green-menthe-sun-373-moon-652:#37635f;--green-menthe-sun-373-moon-652-hover:#53918c;--green-menthe-sun-373-moon-652-active:#62a9a2;--green-menthe-925-125:#8bf8e7;--green-menthe-925-125-hover:#6ed5c5;--green-menthe-925-125-active:#62bfb1;--green-menthe-main-548:#009081;--green-menthe-850-200:#73e0cf;--green-archipel-975-75:#e5fbfd;--green-archipel-975-75-hover:#99f2f8;--green-archipel-975-75-active:#73e9f0;--green-archipel-950-100:#c7f6fc;--green-archipel-950-100-hover:#64ecf8;--green-archipel-950-100-active:#5bd8e3;--green-archipel-sun-391-moon-716:#006a6f;--green-archipel-sun-391-moon-716-hover:#009fa7;--green-archipel-sun-391-moon-716-active:#00bbc3;--green-archipel-925-125:#a6f2fa;--green-archipel-925-125-hover:#62dbe5;--green-archipel-925-125-active:#58c5cf;--green-archipel-main-557:#009099;--green-archipel-850-200:#60e0eb;--blue-ecume-975-75:#f4f6fe;--blue-ecume-975-75-hover:#d7dffb;--blue-ecume-975-75-active:#c3cffa;--blue-ecume-950-100:#e9edfe;--blue-ecume-950-100-hover:#c5d0fc;--blue-ecume-950-100-active:#adbffc;--blue-ecume-sun-247-moon-675:#2f4077;--blue-ecume-sun-247-moon-675-hover:#4e68bb;--blue-ecume-sun-247-moon-675-active:#667dcf;--blue-ecume-925-125:#dee5fd;--blue-ecume-925-125-hover:#b4c5fb;--blue-ecume-925-125-active:#99b3f9;--blue-ecume-main-400:#465f9d;--blue-ecume-850-200:#bfccfb;--blue-cumulus-975-75:#f3f6fe;--blue-cumulus-975-75-hover:#d3dffc;--blue-cumulus-975-75-active:#bed0fa;--blue-cumulus-950-100:#e6eefe;--blue-cumulus-950-100-hover:#bcd3fc;--blue-cumulus-950-100-active:#9fc3fc;--blue-cumulus-sun-368-moon-732:#3558a2;--blue-cumulus-sun-368-moon-732-hover:#5982e0;--blue-cumulus-sun-368-moon-732-active:#7996e6;--blue-cumulus-925-125:#dae6fd;--blue-cumulus-925-125-hover:#a9c8fb;--blue-cumulus-925-125-active:#8ab8f9;--blue-cumulus-main-526:#417dc4;--blue-cumulus-850-200:#b6cffb;--purple-glycine-975-75:#fef3fd;--purple-glycine-975-75-hover:#fcd4f8;--purple-glycine-975-75-active:#fabff5;--purple-glycine-950-100:#fee7fc;--purple-glycine-950-100-hover:#fdc0f8;--purple-glycine-950-100-active:#fca8f6;--purple-glycine-sun-319-moon-630:#6e445a;--purple-glycine-sun-319-moon-630-hover:#a66989;--purple-glycine-sun-319-moon-630-active:#bb7f9e;--purple-glycine-925-125:#fddbfa;--purple-glycine-925-125-hover:#fbaff5;--purple-glycine-925-125-active:#fa96f2;--purple-glycine-main-494:#a558a0;--purple-glycine-850-200:#fbb8f6;--pink-macaron-975-75:#fef4f2;--pink-macaron-975-75-hover:#fcd8d0;--pink-macaron-975-75-active:#fac5b8;--pink-macaron-950-100:#fee9e6;--pink-macaron-950-100-hover:#fdc6bd;--pink-macaron-950-100-active:#fcb0a2;--pink-macaron-sun-406-moon-833:#8d533e;--pink-macaron-sun-406-moon-833-hover:#ca795c;--pink-macaron-sun-406-moon-833-active:#e08e73;--pink-macaron-925-125:#fddfda;--pink-macaron-925-125-hover:#fbb8ab;--pink-macaron-925-125-active:#faa18d;--pink-macaron-main-689:#e18b76;--pink-macaron-850-200:#fcc0b4;--pink-tuile-975-75:#fef4f3;--pink-tuile-975-75-hover:#fcd7d3;--pink-tuile-975-75-active:#fac4be;--pink-tuile-950-100:#fee9e7;--pink-tuile-950-100-hover:#fdc6c0;--pink-tuile-950-100-active:#fcb0a7;--pink-tuile-sun-425-moon-750:#a94645;--pink-tuile-sun-425-moon-750-hover:#d5706f;--pink-tuile-sun-425-moon-750-active:#da8a89;--pink-tuile-925-125:#fddfdb;--pink-tuile-925-125-hover:#fbb8ad;--pink-tuile-925-125-active:#faa191;--pink-tuile-main-556:#ce614a;--pink-tuile-850-200:#fcbfb7;--yellow-tournesol-975-75:#fef6e3;--yellow-tournesol-975-75-hover:#fce086;--yellow-tournesol-975-75-active:#f5d24b;--yellow-tournesol-950-100:#feecc2;--yellow-tournesol-950-100-hover:#fbd335;--yellow-tournesol-950-100-active:#e6c130;--yellow-tournesol-sun-407-moon-922:#716043;--yellow-tournesol-sun-407-moon-922-hover:#a28a62;--yellow-tournesol-sun-407-moon-922-active:#ba9f72;--yellow-tournesol-925-125:#fde39c;--yellow-tournesol-925-125-hover:#e9c53b;--yellow-tournesol-925-125-active:#d3b235;--yellow-tournesol-main-731:#c8aa39;--yellow-tournesol-850-200:#efcb3a;--yellow-moutarde-975-75:#fef5e8;--yellow-moutarde-975-75-hover:#fcdca3;--yellow-moutarde-975-75-active:#fbcd64;--yellow-moutarde-950-100:#feebd0;--yellow-moutarde-950-100-hover:#fdcd6d;--yellow-moutarde-950-100-active:#f4be30;--yellow-moutarde-sun-348-moon-860:#695240;--yellow-moutarde-sun-348-moon-860-hover:#9b7b61;--yellow-moutarde-sun-348-moon-860-active:#b58f72;--yellow-moutarde-925-125:#fde2b5;--yellow-moutarde-925-125-hover:#f6c43c;--yellow-moutarde-925-125-active:#dfb135;--yellow-moutarde-main-679:#c3992a;--yellow-moutarde-850-200:#fcc63a;--orange-terre-battue-975-75:#fef4f2;--orange-terre-battue-975-75-hover:#fcd8d0;--orange-terre-battue-975-75-active:#fac5b8;--orange-terre-battue-950-100:#fee9e5;--orange-terre-battue-950-100-hover:#fdc6ba;--orange-terre-battue-950-100-active:#fcb09e;--orange-terre-battue-sun-370-moon-672:#755348;--orange-terre-battue-sun-370-moon-672-hover:#ab7b6b;--orange-terre-battue-sun-370-moon-672-active:#c68f7d;--orange-terre-battue-925-125:#fddfd8;--orange-terre-battue-925-125-hover:#fbb8a5;--orange-terre-battue-925-125-active:#faa184;--orange-terre-battue-main-645:#e4794a;--orange-terre-battue-850-200:#fcc0b0;--brown-cafe-creme-975-75:#fbf6ed;--brown-cafe-creme-975-75-hover:#f2deb6;--brown-cafe-creme-975-75-active:#eacf91;--brown-cafe-creme-950-100:#f7ecdb;--brown-cafe-creme-950-100-hover:#edce94;--brown-cafe-creme-950-100-active:#dabd84;--brown-cafe-creme-sun-383-moon-885:#685c48;--brown-cafe-creme-sun-383-moon-885-hover:#97866a;--brown-cafe-creme-sun-383-moon-885-active:#ae9b7b;--brown-cafe-creme-925-125:#f4e3c7;--brown-cafe-creme-925-125-hover:#e1c386;--brown-cafe-creme-925-125-active:#ccb078;--brown-cafe-creme-main-782:#d1b781;--brown-cafe-creme-850-200:#e7ca8e;--brown-caramel-975-75:#fbf5f2;--brown-caramel-975-75-hover:#f1dbcf;--brown-caramel-975-75-active:#ecc9b5;--brown-caramel-950-100:#f7ebe5;--brown-caramel-950-100-hover:#eccbb9;--brown-caramel-950-100-active:#e6b79a;--brown-caramel-sun-425-moon-901:#845d48;--brown-caramel-sun-425-moon-901-hover:#bb8568;--brown-caramel-sun-425-moon-901-active:#d69978;--brown-caramel-925-125:#f3e2d9;--brown-caramel-925-125-hover:#e7bea6;--brown-caramel-925-125-active:#e1a982;--brown-caramel-main-648:#c08c65;--brown-caramel-850-200:#eac7b2;--brown-opera-975-75:#fbf5f2;--brown-opera-975-75-hover:#f1dbcf;--brown-opera-975-75-active:#ecc9b5;--brown-opera-950-100:#f7ece4;--brown-opera-950-100-hover:#eccdb3;--brown-opera-950-100-active:#e6ba90;--brown-opera-sun-395-moon-820:#745b47;--brown-opera-sun-395-moon-820-hover:#a78468;--brown-opera-sun-395-moon-820-active:#c09979;--brown-opera-925-125:#f3e2d7;--brown-opera-925-125-hover:#e7bfa0;--brown-opera-925-125-active:#deaa7e;--brown-opera-main-680:#bd987a;--brown-opera-850-200:#eac7ad;--beige-gris-galet-975-75:#f9f6f2;--beige-gris-galet-975-75-hover:#eadecd;--beige-gris-galet-975-75-active:#e1ceb1;--beige-gris-galet-950-100:#f3ede5;--beige-gris-galet-950-100-hover:#e1d0b5;--beige-gris-galet-950-100-active:#d1bea2;--beige-gris-galet-sun-407-moon-821:#6a6156;--beige-gris-galet-sun-407-moon-821-hover:#988b7c;--beige-gris-galet-sun-407-moon-821-active:#afa08f;--beige-gris-galet-925-125:#eee4d9;--beige-gris-galet-925-125-hover:#dbc3a4;--beige-gris-galet-925-125-active:#c6b094;--beige-gris-galet-main-702:#aea397;--beige-gris-galet-850-200:#e0cab0;--ground:0;--shadow-color:rgba(0,0,18,.16);--raised-shadow:0 1px 3px var(--shadow-color);--overlap-shadow:0 2px 6px var(--shadow-color);--lifted-shadow:0 3px 9px var(--shadow-color);box-sizing:border-box}[href]{background-image:var(--underline-img),var(--underline-img);background-position:var(--underline-x) 100%,var(--underline-x) calc(100% - var(--underline-thickness));background-repeat:no-repeat,no-repeat;background-size:var(--underline-hover-width) calc(var(--underline-thickness)*2),var(--underline-idle-width) var(--underline-thickness);transition:background-size 0s}[target=_blank]:after,[target=_blank][class*=" fr-fi-"]:after,[target=_blank][class^=fr-fi-]:after{--icon-size:1rem;background-color:currentColor;content:var(--external-link-content);display:inline-block;flex:0 0 auto;height:var(--icon-size);margin-left:.25rem;-webkit-mask-image:url(icons/system/external-link-line.svg);mask-image:url(icons/system/external-link-line.svg);-webkit-mask-size:100% 100%;mask-size:100% 100%;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}button{border:none;color:inherit;font-family:inherit}button,input,select{-webkit-appearance:none;-moz-appearance:none;appearance:none;background-color:transparent;margin:0}input,select{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;-webkit-text-size-adjust:100%;border:0;border-radius:0;font-family:Marianne,arial,sans-serif;text-rendering:optimizeLegibility}input[type=radio]{-webkit-appearance:auto;-moz-appearance:auto;appearance:auto}a,button,input,input[type=button],input[type=image],input[type=radio]+label:before,select{outline-color:#0a76f6;outline-offset:2px;outline-width:2px}a:focus,button:focus,input:focus,input[type=button]:focus,input[type=image]:focus,input[type=radio]:focus+label:before,select:focus{outline-style:solid}a:focus:not(:focus-visible),button:focus:not(:focus-visible),input:focus:not(:focus-visible),input[type=button]:focus:not(:focus-visible),input[type=image]:focus:not(:focus-visible),input[type=radio]:focus:not(:focus-visible)+label:before,select:focus:not(:focus-visible){outline-style:none}a:focus-visible,button:focus-visible,input:focus-visible,input[type=button]:focus-visible,input[type=image]:focus-visible,input[type=radio]:focus-visible+label:before,select:focus-visible{outline-style:solid}button,input[type=button],input[type=image]{--hover-tint:var(--hover);--active-tint:var(--active)}a,button,input[type=button],input[type=file],input[type=image],input[type=radio],input[type=radio]+label,select{cursor:pointer}a:not([href]),button:disabled,input:disabled,input[type=button]:disabled,input[type=file]:disabled,input[type=image]:disabled,input[type=radio]:disabled,input[type=radio]:disabled+label,select:disabled{cursor:not-allowed}a:not([href]),button:disabled,input:disabled,input[type=radio]:disabled,input[type=radio]:disabled+label{color:var(--text-disabled-grey);opacity:1}.fr-enlarge-link{position:relative}.fr-enlarge-link a{background-image:none;outline-width:0}.fr-enlarge-link a:before{bottom:0;content:"";display:block;height:100%;left:0;outline-color:inherit;outline-offset:2px;outline-style:inherit;outline-width:2px;position:absolute;right:0;top:0;width:100%;z-index:1}@font-face{font-display:swap;font-family:Marianne;font-style:normal;font-weight:300;src:url(fonts/Marianne-Light.woff2) format("woff2"),url(fonts/Marianne-Light.woff) format("woff")}@font-face{font-display:swap;font-family:Marianne;font-style:italic;font-weight:300;src:url(fonts/Marianne-Light_Italic.woff2) format("woff2"),url(fonts/Marianne-Light_Italic.woff) format("woff")}@font-face{font-display:swap;font-family:Marianne;font-style:normal;font-weight:400;src:url(fonts/Marianne-Regular.woff2) format("woff2"),url(fonts/Marianne-Regular.woff) format("woff")}@font-face{font-display:swap;font-family:Marianne;font-style:italic;font-weight:400;src:url(fonts/Marianne-Regular_Italic.woff2) format("woff2"),url(fonts/Marianne-Regular_Italic.woff) format("woff")}@font-face{font-display:swap;font-family:Marianne;font-style:normal;font-weight:500;src:url(fonts/Marianne-Medium.woff2) format("woff2"),url(fonts/Marianne-Medium.woff) format("woff")}@font-face{font-display:swap;font-family:Marianne;font-style:italic;font-weight:500;src:url(fonts/Marianne-Medium_Italic.woff2) format("woff2"),url(fonts/Marianne-Medium_Italic.woff) format("woff")}@font-face{font-display:swap;font-family:Marianne;font-style:normal;font-weight:700;src:url(fonts/Marianne-Bold.woff2) format("woff2"),url(fonts/Marianne-Bold.woff) format("woff")}@font-face{font-display:swap;font-family:Marianne;font-style:italic;font-weight:700;src:url(fonts/Marianne-Bold_Italic.woff2) format("woff2"),url(fonts/Marianne-Bold_Italic.woff) format("woff")}@font-face{font-display:swap;font-family:Spectral;font-style:normal;font-weight:400;src:url(fonts/Spectral-Regular.woff2) format("woff2"),url(fonts/Spectral-Regular.woff) format("woff")}@font-face{font-display:swap;font-family:Spectral;font-style:normal;font-weight:900;src:url(fonts/Spectral-ExtraBold.woff2) format("woff2"),url(fonts/Spectral-ExtraBold.woff) format("woff")}h3{font-size:1.5rem;line-height:2rem}h2,h3{font-weight:700;margin:var(--title-spacing)}h2{font-size:1.75rem;line-height:2.25rem}h1{font-size:2rem;font-weight:700;line-height:2.5rem;margin:var(--title-spacing)}p{font-size:1rem;line-height:1.5rem;margin:var(--text-spacing)}ul{--xl-size:var(--xl-base);margin:0;margin-block-end:var(--xl-block);margin-block-start:var(--xl-block);padding:0}ul{list-style-type:var(--ul-type);padding-inline-start:var(--ul-start)}ul>li::marker{font-size:calc(var(--xl-size)*.9)}li{--xl-base:calc(var(--xl-size)*0.9);padding-bottom:var(--li-bottom)}.fr-text--regular{font-weight:400!important}*,:after,:before{box-sizing:inherit}body{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;-webkit-text-size-adjust:100%;--idle:transparent;--hover:var(--background-default-grey-hover);--active:var(--background-default-grey-active);background-color:var(--background-default-grey);color:var(--text-default-grey);font-family:Marianne,arial,sans-serif;font-size:1rem;line-height:1.5rem;margin:0;padding:0;text-rendering:optimizeLegibility}[class*=" fr-fi-"]:after,[class*=" fr-fi-"]:before,[class^=fr-fi-]:after,[class^=fr-fi-]:before{--icon-size:1.5rem;background-color:currentColor;display:inline-block;flex:0 0 auto;height:var(--icon-size);-webkit-mask-size:100% 100%;mask-size:100% 100%;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}[class*=" fr-fi-"]:before,[class^=fr-fi-]:before{content:""}hr{background-image:linear-gradient(0deg,var(--border-default-grey),var(--border-default-grey));background-position:0 0;background-repeat:no-repeat;background-size:100% 1px;border:0;display:block;margin:0;padding:var(--text-spacing)}.fr-grid-row{display:flex;flex-wrap:wrap;margin:0;padding:0}.fr-grid-row--center{justify-content:center}.fr-container{margin-left:auto;margin-right:auto;padding-left:1rem;padding-right:1rem;width:100%}.fr-container--fluid{max-width:none;overflow:hidden;padding-left:0;padding-right:0}.fr-col-12{flex:0 0 100%;max-width:100%;width:100%}.fr-collapse{--collapse-max-height:0;--collapse:-99999px;--collapser:"";max-height:0;max-height:var(--collapse-max-height);overflow:hidden;transition:visibility .3s}.fr-collapse:before{content:"";content:var(--collapser);display:block;margin-top:0;transition:margin-top .3s}.fr-collapse:not(.fr-collapse--expanded){visibility:hidden}.fr-collapse:not(.fr-collapse--expanded):before{margin-top:-99999px;margin-top:var(--collapse)}.fr-mb-0-5v{margin-bottom:.125rem!important}.fr-mx-auto{margin-left:auto}.fr-mx-auto{margin-right:auto}.fr-py-12v{padding-top:3rem!important}.fr-py-12v{padding-bottom:3rem!important}:root[data-fr-theme=dark]{--shadow-color:rgba(0,0,18,.32);--grey-1000-50:#161616;--grey-1000-50-hover:#343434;--grey-1000-50-active:#474747;--grey-975-75:#1e1e1e;--grey-975-75-hover:#3f3f3f;--grey-975-75-active:#525252;--grey-950-100:#242424;--grey-950-100-hover:#474747;--grey-950-100-active:#5b5b5b;--grey-200-850:#cecece;--grey-925-125:#2a2a2a;--grey-1000-75:#1e1e1e;--grey-1000-75-hover:#3f3f3f;--grey-1000-75-active:#525252;--grey-1000-100:#242424;--grey-1000-100-hover:#474747;--grey-1000-100-active:#5b5b5b;--grey-975-100:#242424;--grey-975-100-hover:#474747;--grey-975-100-active:#5b5b5b;--grey-975-125:#2a2a2a;--grey-975-125-hover:#4e4e4e;--grey-975-125-active:#636363;--grey-950-125:#2a2a2a;--grey-950-125-hover:#4e4e4e;--grey-950-125-active:#636363;--grey-950-150:#2f2f2f;--grey-950-150-hover:#545454;--grey-950-150-active:#696969;--grey-50-1000:#fff;--grey-425-625:#929292;--grey-625-425:#666;--grey-900-175:#353535;--blue-france-975-75:#1b1b35;--blue-france-975-75-hover:#3a3a68;--blue-france-975-75-active:#4d4d83;--blue-france-950-100:#21213f;--blue-france-950-100-hover:#424275;--blue-france-950-100-active:#56568c;--blue-france-sun-113-625:#8585f6;--blue-france-sun-113-625-hover:#b1b1f9;--blue-france-sun-113-625-active:#c6c6fb;--blue-france-925-125:#272747;--blue-france-925-125-hover:#4a4a7d;--blue-france-925-125-active:#5e5e90;--blue-france-975-sun-113:#000091;--blue-france-main-525:#6a6af4;--blue-france-850-200:#313178;--red-marianne-975-75:#2b1919;--red-marianne-975-75-hover:#573737;--red-marianne-975-75-active:#704848;--red-marianne-950-100:#331f1f;--red-marianne-950-100-hover:#613f3f;--red-marianne-950-100-active:#7b5151;--red-marianne-425-625:#f95c5e;--red-marianne-425-625-hover:#fa9293;--red-marianne-425-625-active:#fbabac;--red-marianne-925-125:#3b2424;--red-marianne-925-125-hover:#6b4545;--red-marianne-925-125-active:#865757;--red-marianne-main-472:#e1000f;--red-marianne-850-200:#5e2a2b;--info-950-100:#1d2437;--info-950-100-hover:#3b4767;--info-950-100-active:#4c5b83;--info-425-625:#518fff;--info-425-625-hover:#98b4ff;--info-425-625-active:#b4c7ff;--info-975-75:#171d2e;--success-950-100:#19271d;--success-950-100-hover:#344c3b;--success-950-100-active:#44624d;--success-425-625:#27a658;--success-425-625-hover:#36d975;--success-425-625-active:#3df183;--success-975-75:#142117;--warning-950-100:#361e19;--warning-950-100-hover:#663d35;--warning-950-100-active:#824f44;--warning-425-625:#fc5d00;--warning-425-625-hover:#ff8c73;--warning-425-625-active:#ffa595;--warning-975-75:#2d1814;--error-950-100:#391c1c;--error-950-100-hover:#6c3a3a;--error-950-100-active:#894b4b;--error-425-625:#ff5655;--error-425-625-hover:#ff8c8c;--error-425-625-active:#ffa6a6;--error-975-75:#301717;--green-tilleul-verveine-975-75:#201e14;--green-tilleul-verveine-975-75-hover:#433f2e;--green-tilleul-verveine-975-75-active:#57533d;--green-tilleul-verveine-950-100:#272419;--green-tilleul-verveine-950-100-hover:#4c4734;--green-tilleul-verveine-950-100-active:#615b44;--green-tilleul-verveine-sun-418-moon-817:#d8c634;--green-tilleul-verveine-sun-418-moon-817-hover:#fee943;--green-tilleul-verveine-sun-418-moon-817-active:#fef1ab;--green-tilleul-verveine-925-125:#2d2a1d;--green-tilleul-verveine-925-125-hover:#534f39;--green-tilleul-verveine-925-125-active:#696349;--green-tilleul-verveine-main-707:#b7a73f;--green-tilleul-verveine-850-200:#3f3a20;--green-bourgeon-975-75:#182014;--green-bourgeon-975-75-hover:#35432e;--green-bourgeon-975-75-active:#46573d;--green-bourgeon-950-100:#1e2719;--green-bourgeon-950-100-hover:#3d4c34;--green-bourgeon-950-100-active:#4e6144;--green-bourgeon-sun-425-moon-759:#99c221;--green-bourgeon-sun-425-moon-759-hover:#baec2a;--green-bourgeon-sun-425-moon-759-active:#c9fd2e;--green-bourgeon-925-125:#232d1d;--green-bourgeon-925-125-hover:#435339;--green-bourgeon-925-125-active:#556949;--green-bourgeon-main-640:#68a532;--green-bourgeon-850-200:#2a401a;--green-emeraude-975-75:#142018;--green-emeraude-975-75-hover:#2e4335;--green-emeraude-975-75-active:#3d5846;--green-emeraude-950-100:#19271e;--green-emeraude-950-100-hover:#344c3d;--green-emeraude-950-100-active:#44624f;--green-emeraude-sun-425-moon-753:#34cb6a;--green-emeraude-sun-425-moon-753-hover:#42fb84;--green-emeraude-sun-425-moon-753-active:#80fda3;--green-emeraude-925-125:#1e2e23;--green-emeraude-925-125-hover:#3b5543;--green-emeraude-925-125-active:#4b6b55;--green-emeraude-main-632:#00a95f;--green-emeraude-850-200:#21402c;--green-menthe-975-75:#15201e;--green-menthe-975-75-hover:#30433f;--green-menthe-975-75-active:#3f5753;--green-menthe-950-100:#1a2624;--green-menthe-950-100-hover:#364b47;--green-menthe-950-100-active:#46605b;--green-menthe-sun-373-moon-652:#21ab8e;--green-menthe-sun-373-moon-652-hover:#2eddb8;--green-menthe-sun-373-moon-652-active:#34f4cc;--green-menthe-925-125:#1f2d2a;--green-menthe-925-125-hover:#3c534e;--green-menthe-925-125-active:#4d6963;--green-menthe-main-548:#009081;--green-menthe-850-200:#223f3a;--green-archipel-975-75:#152021;--green-archipel-975-75-hover:#2f4345;--green-archipel-975-75-active:#3f5759;--green-archipel-950-100:#1a2628;--green-archipel-950-100-hover:#364a4e;--green-archipel-950-100-active:#465f63;--green-archipel-sun-391-moon-716:#34bab5;--green-archipel-sun-391-moon-716-hover:#43e9e2;--green-archipel-sun-391-moon-716-active:#4cfdf6;--green-archipel-925-125:#1f2c2e;--green-archipel-925-125-hover:#3c5255;--green-archipel-925-125-active:#4d676b;--green-archipel-main-557:#009099;--green-archipel-850-200:#233e41;--blue-ecume-975-75:#171d2f;--blue-ecume-975-75-hover:#333e5e;--blue-ecume-975-75-active:#445179;--blue-ecume-950-100:#1d2437;--blue-ecume-950-100-hover:#3b4767;--blue-ecume-950-100-active:#4c5b83;--blue-ecume-sun-247-moon-675:#869ece;--blue-ecume-sun-247-moon-675-hover:#b8c5e2;--blue-ecume-sun-247-moon-675-active:#ced6ea;--blue-ecume-925-125:#222940;--blue-ecume-925-125-hover:#424d73;--blue-ecume-925-125-active:#536190;--blue-ecume-main-400:#465f9d;--blue-ecume-850-200:#273962;--blue-cumulus-975-75:#171e2b;--blue-cumulus-975-75-hover:#333f56;--blue-cumulus-975-75-active:#43536f;--blue-cumulus-950-100:#1c2433;--blue-cumulus-950-100-hover:#3a4761;--blue-cumulus-950-100-active:#4a5b7b;--blue-cumulus-sun-368-moon-732:#7ab1e8;--blue-cumulus-sun-368-moon-732-hover:#bad2f2;--blue-cumulus-sun-368-moon-732-active:#d2e2f6;--blue-cumulus-925-125:#212a3a;--blue-cumulus-925-125-hover:#404f69;--blue-cumulus-925-125-active:#516384;--blue-cumulus-main-526:#417dc4;--blue-cumulus-850-200:#263b58;--purple-glycine-975-75:#251a24;--purple-glycine-975-75-hover:#4c394a;--purple-glycine-975-75-active:#634a60;--purple-glycine-950-100:#2c202b;--purple-glycine-950-100-hover:#554053;--purple-glycine-950-100-active:#6c536a;--purple-glycine-sun-319-moon-630:#ce70cc;--purple-glycine-sun-319-moon-630-hover:#dfa4dd;--purple-glycine-sun-319-moon-630-active:#e7bbe6;--purple-glycine-925-125:#332632;--purple-glycine-925-125-hover:#5d485c;--purple-glycine-925-125-active:#755b73;--purple-glycine-main-494:#a558a0;--purple-glycine-850-200:#502e4d;--pink-macaron-975-75:#261b19;--pink-macaron-975-75-hover:#4e3a37;--pink-macaron-975-75-active:#654c48;--pink-macaron-950-100:#2e211f;--pink-macaron-950-100-hover:#58423f;--pink-macaron-950-100-active:#705551;--pink-macaron-sun-406-moon-833:#ffb7ae;--pink-macaron-sun-406-moon-833-hover:#ffe0dc;--pink-macaron-sun-406-moon-833-active:#fff0ee;--pink-macaron-925-125:#352724;--pink-macaron-925-125-hover:#614a45;--pink-macaron-925-125-active:#795d57;--pink-macaron-main-689:#e18b76;--pink-macaron-850-200:#52312a;--pink-tuile-975-75:#281b19;--pink-tuile-975-75-hover:#513a37;--pink-tuile-975-75-active:#694c48;--pink-tuile-950-100:#2f211f;--pink-tuile-950-100-hover:#5a423e;--pink-tuile-950-100-active:#725550;--pink-tuile-sun-425-moon-750:#ff9575;--pink-tuile-sun-425-moon-750-hover:#ffc4b7;--pink-tuile-sun-425-moon-750-active:#ffd8d0;--pink-tuile-925-125:#372624;--pink-tuile-925-125-hover:#644845;--pink-tuile-925-125-active:#7d5b57;--pink-tuile-main-556:#ce614a;--pink-tuile-850-200:#55302a;--yellow-tournesol-975-75:#221d11;--yellow-tournesol-975-75-hover:#473e29;--yellow-tournesol-975-75-active:#5c5136;--yellow-tournesol-950-100:#292416;--yellow-tournesol-950-100-hover:#4f472f;--yellow-tournesol-950-100-active:#655b3d;--yellow-tournesol-sun-407-moon-922:#ffe552;--yellow-tournesol-sun-407-moon-922-hover:#e1c700;--yellow-tournesol-sun-407-moon-922-active:#cab300;--yellow-tournesol-925-125:#302a1a;--yellow-tournesol-925-125-hover:#584e34;--yellow-tournesol-925-125-active:#6f6342;--yellow-tournesol-main-731:#c8aa39;--yellow-tournesol-850-200:#43391a;--yellow-moutarde-975-75:#231d14;--yellow-moutarde-975-75-hover:#483e2e;--yellow-moutarde-975-75-active:#5e513d;--yellow-moutarde-950-100:#2a2319;--yellow-moutarde-950-100-hover:#514534;--yellow-moutarde-950-100-active:#685944;--yellow-moutarde-sun-348-moon-860:#ffca00;--yellow-moutarde-sun-348-moon-860-hover:#cda200;--yellow-moutarde-sun-348-moon-860-active:#b28c00;--yellow-moutarde-925-125:#30291d;--yellow-moutarde-925-125-hover:#584d39;--yellow-moutarde-925-125-active:#6f6149;--yellow-moutarde-main-679:#c3992a;--yellow-moutarde-850-200:#453820;--orange-terre-battue-975-75:#281a16;--orange-terre-battue-975-75-hover:#513932;--orange-terre-battue-975-75-active:#6a4b42;--orange-terre-battue-950-100:#31201c;--orange-terre-battue-950-100-hover:#5d403a;--orange-terre-battue-950-100-active:#77534a;--orange-terre-battue-sun-370-moon-672:#ff732c;--orange-terre-battue-sun-370-moon-672-hover:#ffa48b;--orange-terre-battue-sun-370-moon-672-active:#ffbbab;--orange-terre-battue-925-125:#382621;--orange-terre-battue-925-125-hover:#664840;--orange-terre-battue-925-125-active:#7f5b51;--orange-terre-battue-main-645:#e4794a;--orange-terre-battue-850-200:#543125;--brown-cafe-creme-975-75:#211d16;--brown-cafe-creme-975-75-hover:#453e31;--brown-cafe-creme-975-75-active:#5a5141;--brown-cafe-creme-950-100:#28241c;--brown-cafe-creme-950-100-hover:#4e4739;--brown-cafe-creme-950-100-active:#635b4a;--brown-cafe-creme-sun-383-moon-885:#ecd7a2;--brown-cafe-creme-sun-383-moon-885-hover:#c5b386;--brown-cafe-creme-sun-383-moon-885-active:#af9f77;--brown-cafe-creme-925-125:#2e2a21;--brown-cafe-creme-925-125-hover:#554e3f;--brown-cafe-creme-925-125-active:#6b6351;--brown-cafe-creme-main-782:#d1b781;--brown-cafe-creme-850-200:#423925;--brown-caramel-975-75:#251c16;--brown-caramel-975-75-hover:#4c3c31;--brown-caramel-975-75-active:#624e41;--brown-caramel-950-100:#2c221c;--brown-caramel-950-100-hover:#554439;--brown-caramel-950-100-active:#6c574a;--brown-caramel-sun-425-moon-901:#fbd8ab;--brown-caramel-sun-425-moon-901-hover:#efb547;--brown-caramel-sun-425-moon-901-active:#d6a23e;--brown-caramel-925-125:#332821;--brown-caramel-925-125-hover:#5d4b40;--brown-caramel-925-125-active:#755f51;--brown-caramel-main-648:#c08c65;--brown-caramel-850-200:#4b3525;--brown-opera-975-75:#241c17;--brown-opera-975-75-hover:#4a3c33;--brown-opera-975-75-active:#604f44;--brown-opera-950-100:#2b221c;--brown-opera-950-100-hover:#53443a;--brown-opera-950-100-active:#6a574a;--brown-opera-sun-395-moon-820:#e6be92;--brown-opera-sun-395-moon-820-hover:#f2e2d3;--brown-opera-sun-395-moon-820-active:#f8f0e9;--brown-opera-925-125:#322821;--brown-opera-925-125-hover:#5c4b40;--brown-opera-925-125-active:#735f51;--brown-opera-main-680:#bd987a;--brown-opera-850-200:#493625;--beige-gris-galet-975-75:#211d19;--beige-gris-galet-975-75-hover:#453e37;--beige-gris-galet-975-75-active:#595148;--beige-gris-galet-950-100:#28231f;--beige-gris-galet-950-100-hover:#4e453f;--beige-gris-galet-950-100-active:#635950;--beige-gris-galet-sun-407-moon-821:#d0c3b7;--beige-gris-galet-sun-407-moon-821-hover:#eae5e1;--beige-gris-galet-sun-407-moon-821-active:#f4f2f0;--beige-gris-galet-925-125:#2e2924;--beige-gris-galet-925-125-hover:#554d45;--beige-gris-galet-925-125-active:#6b6157;--beige-gris-galet-main-702:#aea397;--beige-gris-galet-850-200:#433829}.fr-artwork-decorative{fill:var(--artwork-decorative-blue-france)}.fr-artwork-minor{fill:var(--artwork-minor-red-marianne)}.fr-artwork-major{fill:var(--artwork-major-blue-france)}h1,h2,h3{color:var(--text-title-grey)}.fr-logo{--text-spacing:0;--underline-img:none;color:var(--text-title-grey);display:inline-block;font-size:1.05rem;font-weight:700;letter-spacing:-.01em;line-height:1.0317460317em;text-indent:-.1em;text-transform:uppercase;vertical-align:middle}.fr-logo:before{background-image:url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 44 18'%3E%3Cpath fill='%23fff' d='M11.3 10.2c-.9.6-1.7 1.3-2.3 2.1v-.1c.4-.5.7-1 1-1.5.4-.2.7-.5 1-.8.5-.5 1-1 1.7-1.3.3-.1.5-.1.8 0-.1.1-.2.1-.4.2H13v-.1c-.3.3-.7.5-1 .9-.1.2-.2.6-.7.6 0 .1.1 0 0 0zm1.6 4.6c0-.1-.1 0-.2 0l-.1.1-.1.1-.2.2s.1.1.2 0l.1-.1c.1 0 .2-.1.2-.2.1 0 .1 0 .1-.1 0 .1 0 0 0 0zm-1.6-4.3c.1 0 .2 0 .2-.1s.1-.1.1-.1v-.1c-.2.1-.3.2-.3.3zm2.4 1.9s0-.1 0 0c.1-.1.2-.1.3-.1.7-.1 1.4-.3 2.1-.6-.8-.5-1.7-.9-2.6-1h.1c-.1-.1-.3-.1-.5-.2h.1c-.2-.1-.5-.1-.7-.2.1 0 .2-.2.2-.3h-.1c-.4.2-.6.5-.8.9.2.1.5 0 .7.1h-.3c-.1 0-.2.1-.2.2h.1c-.1 0-.1.1-.2.1.1.1.2 0 .4 0 0 .1.1.1.1.1-.1 0-.2.1-.3.3-.1.2-.2.2-.3.3v.1c-.3.2-.6.5-.9.8v.1c-.1.1-.2.1-.2.2v.1c.4-.1.6-.4 1-.5l.6-.3c.2 0 .3-.1.5-.1v.1h.2c0 .1-.2 0-.1.1s.3.1.4 0c.2-.2.3-.2.4-.2zM12.4 14c-.4.2-.9.2-1.2.4 0 0 0 .1-.1.1 0 0-.1 0-.1.1-.1 0-.1.1-.2.2l-.1.1s0 .1.1 0l.1-.1s-.1.1-.1.2V15.3l-.1.1s0 .1-.1.1l-.1.1.2-.2.1-.1h.2s0-.1.1-.1c.1-.1.2-.2.3-.2h.1c.1-.1.3-.1.4-.2.1-.1.2-.2.3-.2.2-.2.5-.3.8-.5-.1 0-.2-.1-.3-.1 0 .1-.2 0-.3 0zM30 9.7c-.1.2-.4.2-.6.3-.2.2 0 .4.1.5.1.3-.2.5-.4.5.1.1.2.1.2.1 0 .2.2.2.1.4s-.5.3-.3.5c.1.2.1.5 0 .7-.1.2-.3.4-.5.5-.2.1-.4.1-.6 0-.1 0-.1-.1-.2-.1-.5-.1-1-.2-1.5-.2-.1 0-.3.1-.4.1-.1.1-.3.2-.4.3l-.1.1c-.1.1-.2.2-.2.3-.1.2-.2.4-.2.6-.2.5-.2 1 0 1.4 0 0 1 .3 1.7.6.2.1.5.2.7.4l1.7 1H13.2l1.6-1c.6-.4 1.3-.7 2-1 .5-.2 1.1-.5 1.5-.9.2-.2.3-.4.5-.5.3-.4.6-.7 1-1l.3-.3s0-.1.1-.1c-.2.1-.2.2-.4.2 0 0-.1 0 0-.1s.2-.2.3-.2v-.1c-.4 0-.7.2-1 .5h-.2c-.5.2-.8.5-1.2.7v-.1c-.2.1-.4.2-.5.2-.2 0-.5.1-.8 0-.4 0-.7.1-1.1.2-.2.1-.4.1-.6.2v.1l-.2.2c-.2.1-.3.2-.5.4l-.5.5h-.1l.1-.1.1-.1c0-.1.1-.1.1-.2.2-.1.3-.3.5-.4 0 0-.1 0 0 0 0 0 0-.1.1-.1l-.1.1c-.1.1-.1.2-.2.2v-.1-.1l.2-.2c.1-.1.2-.1.3-.2h.1c-.2.1-.3.1-.5.2H14h-.1c0-.1.1-.1.2-.2h.1c1-.8 2.3-.6 3.4-1 .1-.1.2-.1.3-.2.1-.1.3-.2.5-.3.2-.2.4-.4.5-.7v-.1c-.4.4-.8.7-1.3 1-.6.2-1.3.4-2 .4 0-.1.1-.1.1-.1 0-.1.1-.1.1-.2h.1s0-.1.1-.1h.1c-.1-.1-.3.1-.4 0 .1-.1 0-.2.1-.2h.1s0-.1.1-.1c.5-.3.9-.5 1.3-.7-.1 0-.1.1-.2 0 .1 0 0-.1.1-.1.3-.1.6-.3.9-.4-.1 0-.2.1-.3 0 .1 0 .1-.1.2-.1v-.1h0c0-.1.1 0 .2-.1h-.1c.1-.1.2-.2.4-.2 0-.1-.1 0-.1-.1h.1-.5c-.1 0 0-.1 0-.1.1-.2.2-.5.3-.7h-.1c-.3.3-.8.5-1.2.6h-.2c-.2.1-.4.1-.5 0-.1-.1-.2-.2-.3-.2-.2-.1-.5-.3-.8-.4-.7-.2-1.5-.4-2.3-.3.3-.1.7-.2 1.1-.3.5-.2 1-.3 1.5-.3h-.3c-.4 0-.9.1-1.3.2-.3.1-.6.2-.9.2-.2.1-.3.2-.5.2v-.1c.3-.4.7-.7 1.1-.8.5-.1 1.1 0 1.6.1.4 0 .8.1 1.1.2.1 0 .2.2.3.3.2.1.4 0 .5.1v-.2c.1-.1.3 0 .4 0 .2-.2-.2-.4-.3-.6v-.1c.2.2.5.4.7.6.1.1.5.2.5 0-.2-.3-.4-.6-.7-.9v-.2c-.1 0-.1 0-.1-.1-.1-.1-.1-.2-.1-.3-.1-.2 0-.4-.1-.5-.1-.2-.1-.3-.1-.5-.1-.5-.2-1-.3-1.4-.1-.6.3-1 .6-1.5.2-.4.5-.7.8-1 .1-.4.3-.7.6-1 .3-.3.6-.5.9-.6.3-.1.5-.2.8-.3l2.5-.4H25l1.8.3c.1 0 .2 0 .2.1.1.1.3.2.4.2.2.1.4.3.6.5.1.1.2.3.1.4-.1.1-.1.4-.2.4-.2.1-.4.1-.6.1-.1 0-.2 0-.4-.1.5.2.9.4 1.2.8 0 .1.2.1.3.1v.1c-.1.1-.1.1-.1.2h.1c.1-.1.1-.4.3-.3.2.1.2.3.1.4-.1.1-.2.2-.4.3v.2c.1.1.1.2.2.4s.1.5.2.7c.1.5.2.9.2 1.4 0 .2-.1.5 0 .7l.3.6c.1.2.2.3.3.5.2.3.6.6.4 1zm-15.6 5.2c-.1 0-.1.1-.1.1s.1 0 .1-.1zm5.8-1.8c-.1.1 0 0 0 0zm-6.7-.2c0 .1.1 0 .1 0 .2-.1.5 0 .6-.2-.1-.1-.2 0-.2-.1-.1 0-.2 0-.2.1-.1.1-.3.1-.3.2z'/%3E%3Cpath fill='gray' d='M27.9 6.8c.1 0 .3 0 .3.1-.1.2-.4.3-.6.5h-.1c-.1.1-.1.2-.1.2h-.3c.1.1.3.2.5.2l.1.1h.2V8c-.1.1-.2.1-.4.1.2.1.5.1.7 0 .2-.1 0-.4.1-.5-.1 0 0-.1-.1-.1.1-.1.1-.2.2-.2s.1 0 .2-.1c0-.1-.1-.1-.1-.2.2-.1.3-.3.3-.5 0-.1-.3-.1-.4-.2h-.5c-.2 0-.3.1-.5.1l-.6.3c.2-.1.4-.1.7-.2 0 .3.2.3.4.3'/%3E%3C/svg%3E"),linear-gradient(90deg,#000091,#000091 50%,#e1000f 0,#e1000f),linear-gradient(90deg,#161616,#161616);background-position:0 -.0625rem,0 0,0 0;background-repeat:no-repeat,no-repeat,no-repeat;background-size:2.75rem 1.125rem,2.75rem 1rem,0;content:"";display:block;height:1rem;margin-bottom:.3333333333rem;width:2.75rem}.fr-logo:after{background-image:url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 252 180'%3E%3Cdefs%3E%3Csymbol id='a' viewBox='0 0 11 15.5'%3E%3Cpath d='M10.4 5.3C11.9 1.5 10.1 0 7.9 0 4.2 0 0 6.5 0 11.7c0 2.5 1.2 3.8 3 3.8 2.1 0 4.3-2 6.2-5.5h-1c-1.2 1.5-2.6 2.6-3.9 2.6-1.3 0-2-.8-2-2.6a10.7 10.7 0 01.3-2.2zm-4-3.1c1.1 0 2 .8 1.5 2.6L3.1 6.1c.8-2.2 2.2-4 3.4-4z'/%3E%3C/symbol%3E%3Csymbol id='b' viewBox='0 0 12.4 21.8'%3E%3Cuse width='11' height='15.5' y='6.4' href='%23a'/%3E%3Cpath d='M7.9 4.7L12.4.6V0h-3L6.7 4.7H8z'/%3E%3C/symbol%3E%3Csymbol id='c' viewBox='0 0 11.5 19'%3E%3Cpath d='M1.7 5.7h2.6L.1 17.1a1.3 1.3 0 001.2 2c3 0 6.4-2.6 7.8-6.2h-.7a9.4 9.4 0 01-5.1 3.5L7 5.7H11l.5-1.6H7.7L9 0H7.6L4.9 4.1l-3.2.4v1.2z'/%3E%3C/symbol%3E%3Csymbol id='d' viewBox='0 0 9.8 21.9'%3E%3Cpath d='M7.6 8c.3-1-.4-1.6-1-1.6-2.2 0-5 2.1-6 5h.7A5.6 5.6 0 014.4 9L.1 20.3a1.1 1.1 0 001 1.6c2.2 0 4.7-2 5.8-5H6A5.6 5.6 0 013 19.5zM8 3.7a1.8 1.8 0 001.8-1.8A1.8 1.8 0 008 0a1.8 1.8 0 00-1.8 1.8A1.8 1.8 0 008 3.6'/%3E%3C/symbol%3E%3Csymbol id='e' viewBox='0 0 14.8 15.5'%3E%3Cpath d='M3.3 3.1c.7 0 1 1 0 3.4l-3 6.8c-.7 1.3 0 2.2 1.2 2.2a1.3 1.3 0 001.5-1l3-8C7.4 4.8 10 3 11 3s.8.6.3 1.6l-4.6 9a1.3 1.3 0 001.1 1.9c2.3 0 5-2 6-5h-.6A5.6 5.6 0 0110 13l4-8a6.1 6.1 0 00.8-2.8A2 2 0 0012.6 0c-2 0-3.6 2.2-6 5V2.8C6.6 1.4 6.1 0 4.8 0 3.2 0 1.8 2.5.7 4.9h.7c.7-1.1 1.3-1.8 2-1.8'/%3E%3C/symbol%3E%3Csymbol id='f' viewBox='0 0 12 15.5'%3E%3Cpath d='M11.8 3.5c.5-1.9.2-3.5-1.2-3.5-1.8 0-2.3 1.2-4 5V2.8C6.5 1.3 6 0 4.6 0 3.1 0 1.7 2.5.5 5h.8C2 3.7 2.8 3 3.3 3c.7 0 1 1 0 3.4l-3 6.8c-.7 1.3 0 2.1 1.2 2.1a1.3 1.3 0 001.5-1l3-8a50.3 50.3 0 012.6-3h3.2z'/%3E%3C/symbol%3E%3Csymbol id='g' viewBox='0 0 14.7 16.2'%3E%3Cpath d='M10.5 13.1c-.6 0-1-1 0-3.4L14.6.1 13.4 0l-1.3 1.3h-.3C6.1 1.3 0 8.6 0 14.2a2 2 0 002.1 2.1c1.7 0 3.3-2.4 5.2-5l-.1 1c-.3 2.6.6 4 2 4 1.5 0 3-2.4 4-4.9h-.7c-.7 1.1-1.5 1.8-2 1.8zM7.9 9.8c-1.3 1.6-3.4 3.5-4.3 3.5-.5 0-.9-.5-.9-1.6 0-3.5 4-8.2 6-8.2a4.2 4.2 0 011.4.2z'/%3E%3C/symbol%3E%3Csymbol id='h' viewBox='0 0 21.9 19.8'%3E%3Cpath d='M11.2 19.8l.3-.9c-3.8-.7-4.3-.7-2.7-4.8l1.4-3.9h3c1.9 0 1.9.9 1.6 3h1l2.6-6.9h-1c-1 1.6-1.8 2.9-3.8 2.9h-3l2-5.6c.8-2 1.1-2.4 3.7-2.4h.7c2.6 0 3 .7 3 3.5h1l.9-4.7H7.3L7 .9c3 .6 3.3.9 2 4.8L5.7 14c-1.5 3.9-2 4.2-5.5 4.8l-.3.9z'/%3E%3C/symbol%3E%3Csymbol id='i' viewBox='0 0 10.1 21.9'%3E%3Cpath d='M2.9 19.4L10.1.3 9.8 0l-5 .6v.6l1 .7c.9.7.6 1.3-.2 3.4L.2 19.9a1.3 1.3 0 001.1 2c2.3 0 4.7-2.1 5.8-5h-.7a6.5 6.5 0 01-3.5 2.5'/%3E%3C/symbol%3E%3Csymbol id='j' viewBox='0 0 18 22'%3E%3Cpath d='M18 .6h-4.3a3.8 3.8 0 00-2.1-.6A6.6 6.6 0 005 6.5a3.3 3.3 0 003 3.6c-1.9.8-3 1.8-3 2.9a1.7 1.7 0 00.9 1.5c-4.3 1.3-6 2.8-6 4.7 0 2 2.6 2.8 5.6 2.8 5.3 0 9.6-2.7 9.6-5.1 0-1.8-1.6-2.5-4.3-3.3-2.2-.7-3.2-.8-3.2-1.6A2.4 2.4 0 019 10.2a6.6 6.6 0 006.1-6.5 4.5 4.5 0 00-.2-1.5h2.5zM9.8 16.2c2.1.7 3 1 3 1.6 0 1.4-2 2.5-5.6 2.5-2.7 0-4-.6-4-2 0-1.5 1.4-2.5 3.5-3.3a21.5 21.5 0 003 1.2zM9 9c-1 0-1.3-.8-1.3-1.7 0-2.8 1.4-6.2 3.5-6.2 1 0 1.3.8 1.3 1.6 0 2.9-1.4 6.3-3.5 6.3z'/%3E%3C/symbol%3E%3Csymbol id='k' viewBox='0 0 23 25.1'%3E%3Cpath d='M14.3 15.6c1.9 0 2 .8 1.6 2.8H17l2.5-6.8h-1c-1 1.6-1.7 2.9-3.8 2.9h-4.1l2-5.6c.7-2 1-2.4 3.7-2.4H18c2.6 0 3 .7 3 3.5h1l.9-4.7H7.3l-.3.9c3 .6 3.3.9 2 4.8l-3.2 8.4c-1.5 3.9-2 4.2-5.6 4.8l-.2 1h17.4l3.2-5h-1.2c-2 2-4 3.8-8 3.8-4.7 0-4.3-.3-2.7-4.6l1.4-3.8h4.2zm2.3-11.8L21 .6V0h-3l-2.6 3.9h1.2v-.1z'/%3E%3C/symbol%3E%3Csymbol id='l' viewBox='0 0 13.6 21.8'%3E%3Cpath d='M11.4 6.4c-2 0-4 2.2-5.8 4.8L9.6.3 9.4 0l-5 .6V1l1 .8c.9.7.6 1.3-.2 3.4L.8 16.8A13.9 13.9 0 000 19c0 1.4 1.8 2.7 3.5 2.7 3.8 0 10-6.9 10-12.2 0-2.3-.5-3.2-2.1-3.2zM4.8 19.5c-.8 0-1.9-.7-1.9-1.3a15.5 15.5 0 01.8-2.2L5 12.7C6.3 11 8.4 9.3 9.6 9.3c.7 0 1.2.4 1.2 1.5 0 3.1-2.9 8.7-6 8.7z'/%3E%3C/symbol%3E%3Csymbol id='m' viewBox='0 0 19.2 19.9'%3E%3Cpath d='M17.6 0H7.3L7 .9c3 .6 3.3.9 2 4.8l-3.2 8.5c-1.5 3.9-2 4.2-5.5 4.8L0 20h15.7l3.5-6H18c-2 2-4.2 4.8-7.7 4.8-2.7 0-3-.5-1.6-4.5l3.1-8.5c1.4-3.9 2-4.2 5.5-4.8z'/%3E%3C/symbol%3E%3Csymbol id='n' viewBox='0 0 126 90'%3E%3Cuse width='12.4' height='21.8' x='112.7' y='66.1' href='%23b'/%3E%3Cuse width='11.5' height='19' x='102.2' y='69' href='%23c'/%3E%3Cuse width='9.8' height='21.9' x='93.6' y='66.1' href='%23d'/%3E%3Cuse width='14.8' height='15.5' x='77.2' y='72.5' href='%23e'/%3E%3Cuse width='12' height='15.5' x='65.7' y='72.5' href='%23f'/%3E%3Cuse width='11' height='15.5' x='54.3' y='72.5' href='%23a'/%3E%3Cuse width='11.5' height='19' x='43.7' y='69' href='%23c'/%3E%3Cuse width='14.7' height='16.2' x='28.9' y='71.8' href='%23g'/%3E%3Cuse width='12' height='15.5' x='19.6' y='72.5' href='%23f'/%3E%3Cuse width='21.9' height='19.8' y='67.6' href='%23h'/%3E%3Cuse width='12.4' height='21.8' x='77.3' y='33.1' href='%23b'/%3E%3Cuse width='11.5' height='19' x='66.8' y='36' href='%23c'/%3E%3Cuse width='9.8' height='21.9' x='58.2' y='33' href='%23d'/%3E%3Cuse width='10.1' height='21.9' x='49.4' y='33.1' href='%23i'/%3E%3Cuse width='14.7' height='16.2' x='34.9' y='38.8' href='%23g'/%3E%3Cuse width='18' height='22' x='18.6' y='39.4' href='%23j'/%3E%3Cuse width='23' height='25.1' y='29.3' href='%23k'/%3E%3Cuse width='12.4' height='21.8' x='76.8' y='.1' href='%23b'/%3E%3Cuse width='11.5' height='19' x='66.2' y='2.9' href='%23c'/%3E%3Cuse width='12' height='15.5' x='54.8' y='6.5' href='%23f'/%3E%3Cuse width='11' height='15.5' x='43.4' y='6.4' href='%23a'/%3E%3Cuse width='13.6' height='21.8' x='29.4' y='.1' href='%23l'/%3E%3Cuse width='9.8' height='21.9' x='20.6' href='%23d'/%3E%3Cuse width='19.2' height='19.9' y='1.4' href='%23m'/%3E%3C/symbol%3E%3C/defs%3E%3Cuse fill='%23161616' width='126' height='90' x='0' y='0' href='%23n'/%3E%3Cuse fill='%23fff' width='126' height='90' x='126' y='90' href='%23n'/%3E%3C/svg%3E");background-position:0 calc(100% + 1.875rem);background-repeat:no-repeat;background-size:5.25rem 3.75rem;content:"";display:block;min-width:2.625rem;padding-top:2.2083333333rem}[data-fr-theme=dark] .fr-logo:after{background-position:-2.625rem 100%}.fr-btn{--text-spacing:0;--title-spacing:0;--underline-img:none;--hover-tint:var(--hover);--idle:transparent;--hover:var(--background-action-high-blue-france-hover);--active:var(--background-action-high-blue-france-active);align-items:center;background-color:var(--background-action-high-blue-france);color:var(--text-inverted-blue-france);display:inline-flex;flex-direction:row;font-size:1rem;font-weight:500;line-height:1.5rem;min-height:2.5rem;padding:.5rem 1rem;width:-moz-fit-content;width:fit-content;z-index:1}.fr-btn:after,.fr-btn:before{display:block}.fr-btn[target=_blank]{max-height:none;max-width:100%;overflow:initial}.fr-btn[target=_blank]:after{--icon-size:1rem;content:"";margin-left:.5rem;margin-right:-.125rem}.fr-btn[target=_blank]:before{content:none}.fr-btn[class*=" fr-fi-"]:not([class*=fr-btn--icon-]),.fr-btn[class^=fr-fi-]:not([class*=fr-btn--icon-]){max-height:2.5rem;max-width:2.5rem;overflow:hidden;padding-left:.5rem;padding-right:.5rem;white-space:nowrap}.fr-btn[class*=" fr-fi-"]:not([class*=fr-btn--icon-]):before,.fr-btn[class^=fr-fi-]:not([class*=fr-btn--icon-]):before{--icon-size:1.5rem;margin-left:0;margin-right:.5rem}.fr-btn--close{display:flex;font-size:.875rem;line-height:1.5rem;margin-left:auto;margin-right:-1rem;max-height:none;max-width:100%;min-height:2rem;overflow:initial;padding:.25rem .75rem}.fr-btn--close:after{--icon-size:1rem;background-color:currentColor;content:"";display:inline-block;flex:0 0 auto;height:var(--icon-size);margin-left:.5rem;margin-right:-.125rem;-webkit-mask-image:url(icons/system/close-line.svg);mask-image:url(icons/system/close-line.svg);-webkit-mask-size:100% 100%;mask-size:100% 100%;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}.fr-btn--close:before{content:none}.fr-btn:disabled,a.fr-btn:not([href]){--idle:transparent;--hover:var(--background-disabled-grey-hover);--active:var(--background-disabled-grey-active);background-color:var(--background-disabled-grey);color:var(--text-disabled-grey)}.fr-btn--close{--hover:inherit;--active:inherit;background-color:transparent;color:var(--text-action-high-blue-france)}.fr-btn--close:disabled,a.fr-btn--close:not([href]){--hover:inherit;--active:inherit;background-color:transparent;color:var(--text-disabled-grey)}.fr-label{color:var(--text-label-grey);display:block;font-size:1rem;line-height:1.5rem}.fr-label+.fr-input{margin-top:.5rem}.fr-hint-text{--text-spacing:0 0 1rem;display:block;font-size:.75rem;line-height:1.25rem}.fr-hint-text+.fr-hint-text{margin-top:.25rem}.fr-fieldset{align-items:flex-end;border:0;display:flex;flex-direction:row;flex-wrap:wrap;margin:0 -.75rem 1rem;padding:0 .25rem;position:relative}.fr-fieldset__legend{color:var(--text-title-grey);font-size:1rem;font-weight:700;line-height:1.5rem;margin-bottom:1rem;margin-left:-.25rem;margin-right:-.25rem;padding-left:.75rem;padding-right:.75rem;width:100%}.fr-fieldset__legend .fr-hint-text{font-weight:400;margin-top:.5rem}.fr-fieldset__legend>.fr-fieldset:last-child:after,.fr-fieldset__legend>h1:last-child:after,.fr-fieldset__legend>h2:last-child:after,.fr-fieldset__legend>h3:last-child:after,.fr-fieldset__legend>p:last-child:after{content:"";display:block;margin-bottom:-1rem}.fr-hint-text{color:var(--text-mention-grey)}.fr-fieldset:disabled .fr-fieldset__legend,.fr-fieldset:disabled .fr-label{color:var(--text-disabled-grey)}.fr-fieldset__content{margin-left:.5rem;position:relative;width:100%}.fr-fieldset__content .fr-radio-group:first-child{margin-top:-1rem}.fr-fieldset__content .fr-radio-group label{padding:.75rem 0}.fr-fieldset__content .fr-radio-group label:before{margin-top:.75rem}.fr-link--icon-left[class*=" fr-fi-"],.fr-link--icon-left[class^=fr-fi-]{max-height:none;max-width:100%;overflow:initial}.fr-link--icon-left[class*=" fr-fi-"]:before,.fr-link--icon-left[class^=fr-fi-]:before{--icon-size:1rem;margin-left:-.125rem;margin-right:.5rem}.fr-sidemenu{--ul-type:none;--ol-type:none;--ul-start:0;--ol-start:0;--xl-block:0;--li-bottom:0;--ol-content:none;--underline-img:none;--text-spacing:0;--title-spacing:0;box-shadow:inset 0 -1px 0 0 var(--border-default-grey),inset 0 1px 0 0 var(--border-default-grey);margin-left:-1rem;margin-right:-1rem;position:relative}.fr-sidemenu a:not([href]){cursor:default}.fr-sidemenu .fr-collapse{margin:-.25rem -.25rem 0;padding:.25rem .25rem 0}.fr-sidemenu__title{box-shadow:inset 0 -1px 0 0 var(--border-default-grey);color:var(--text-title-grey);font-size:1.125rem;font-weight:700;line-height:1.75rem;padding:1rem 0}.fr-sidemenu__list{font-weight:700}.fr-sidemenu__list .fr-sidemenu__list{font-weight:400;margin:0 .5rem 1.5rem}.fr-sidemenu__list .fr-sidemenu__list .fr-sidemenu__btn{font-size:1rem;font-weight:400;line-height:1.5rem}.fr-sidemenu__list .fr-sidemenu__list .fr-sidemenu__list .fr-sidemenu__btn{font-size:.875rem;line-height:1.5rem}.fr-sidemenu__inner>.fr-collapse{margin:-.25rem .75rem 0;padding:.25rem .25rem 0}.fr-sidemenu__btn{--hover-tint:var(--hover);--active-tint:var(--active);align-items:center;color:var(--text-action-high-grey);display:flex;flex-direction:row;font-size:1rem;font-weight:700;line-height:1.5rem;padding:.75rem .5rem;position:relative;text-align:left;width:100%}.fr-sidemenu__btn[aria-current]:before{--idle:transparent;--hover:var(--border-active-blue-france-hover);--active:var(--border-active-blue-france-active);background-color:var(--border-active-blue-france);bottom:.75rem;content:"";left:0;position:absolute;top:.75rem;width:2px}.fr-sidemenu__btn[aria-expanded]{align-items:center;display:flex;flex-direction:row}.fr-sidemenu__btn[aria-expanded]:after{--icon-size:1rem;background-color:currentColor;content:"";display:inline-block;flex:0 0 auto;height:var(--icon-size);margin-left:auto;margin-right:0;-webkit-mask-image:url(icons/system/arrow-down-s-line.svg);mask-image:url(icons/system/arrow-down-s-line.svg);-webkit-mask-size:100% 100%;mask-size:100% 100%;transition:transform .3s;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}.fr-sidemenu__btn[aria-expanded=true]:after{transform:rotate(-180deg)}.fr-sidemenu__inner>.fr-sidemenu__btn{font-weight:400;width:100%}.fr-sidemenu__inner>.fr-sidemenu__btn:after{margin-right:1rem}.fr-sidemenu__inner>.fr-sidemenu__btn:before{--icon-size:1rem;background-color:currentColor;content:"";display:inline-block;flex:0 0 auto;height:var(--icon-size);margin-left:.5rem;margin-right:.5rem;-webkit-mask-image:url(icons/system/menu-2-fill.svg);mask-image:url(icons/system/menu-2-fill.svg);-webkit-mask-size:100% 100%;mask-size:100% 100%;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}.fr-sidemenu__btn[aria-current]{color:var(--text-active-blue-france)}.fr-pagination__link{--text-spacing:0;--title-spacing:0;--hover-tint:var(--hover);--underline-img:none;align-items:center;display:inline-flex;flex-direction:row;font-size:1rem;line-height:1.5rem;margin-bottom:1rem;margin-left:.125rem;margin-right:.125rem;min-height:2rem;min-width:2rem;padding:.25rem .75rem;position:relative;width:-moz-fit-content;width:fit-content;z-index:1}.fr-pagination__link:after,.fr-pagination__link:before{display:block}.fr-pagination{--underline-img:none;--ul-type:none;--ol-type:none;--ul-start:0;--ol-start:0;--xl-block:0;--li-bottom:0;--ol-content:none;color:var(--text-action-high-grey)}.fr-pagination__list{align-items:center;display:flex;flex-direction:row;flex-wrap:wrap;justify-content:flex-start}.fr-pagination__list>:first-child,.fr-pagination__list>:first-child *{margin-left:0}.fr-pagination__list>:last-child,.fr-pagination__list>:last-child *{margin-right:0}.fr-pagination__link[aria-current]:not([href]){cursor:default;pointer-events:none}.fr-pagination__link--prev{font-size:1rem;line-height:1.5rem;max-height:2rem;max-width:2rem;min-height:2rem;overflow:hidden;padding:.25rem;white-space:nowrap}.fr-pagination__link--prev:before{--icon-size:1.5rem;background-color:currentColor;content:"";display:inline-block;flex:0 0 auto;height:var(--icon-size);margin-left:0;margin-right:.25rem;-webkit-mask-image:url(icons/system/arrow-left-s-line.svg);mask-image:url(icons/system/arrow-left-s-line.svg);-webkit-mask-size:100% 100%;mask-size:100% 100%;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}.fr-pagination__link--next{font-size:1rem;line-height:1.5rem;max-height:2rem;max-width:2rem;min-height:2rem;overflow:hidden;padding:.25rem;white-space:nowrap}.fr-pagination__link--next:before{--icon-size:1.5rem;background-color:currentColor;content:"";display:inline-block;flex:0 0 auto;height:var(--icon-size);margin-left:0;margin-right:.25rem;-webkit-mask-image:url(icons/system/arrow-right-s-line.svg);mask-image:url(icons/system/arrow-right-s-line.svg);-webkit-mask-size:100% 100%;mask-size:100% 100%;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}.fr-pagination__link--prev{margin-left:-.625rem;margin-right:.875rem}.fr-pagination__link--next{margin-left:.875rem;margin-right:-.625rem}.fr-pagination__link[aria-current]{--idle:transparent;--hover:var(--background-active-blue-france-hover);--active:var(--background-active-blue-france-active);background-color:var(--background-active-blue-france);color:var(--text-inverted-blue-france)}.fr-pagination__link:not([aria-current]):disabled,a.fr-pagination__link:not([aria-current]):not([href]){color:var(--text-disabled-grey)}.fr-radio-group{position:relative}.fr-radio-group input[type=radio]{height:1.5rem;margin:0;opacity:0;position:absolute;width:1.5rem}.fr-radio-group input[type=radio]+label{-webkit-tap-highlight-color:transparent;align-items:center;display:flex;flex-direction:row;flex-wrap:wrap;justify-content:flex-start;margin-left:2rem;position:relative}.fr-radio-group input[type=radio]+label .fr-hint-text{margin:0;width:100%}.fr-radio-group input[type=radio]+label:before{border-radius:50%;box-shadow:inset 0 0 0 1px var(--border-action-high-grey),inset 0 0 0 12px var(--background-default-grey),inset 0 0 0 12px var(--background-action-high-blue-france);content:"";display:inline-block;height:1.5rem;left:-2rem;margin-right:.5rem;position:absolute;top:0;width:1.5rem}.fr-radio-rich{position:relative}.fr-radio-rich input[type=radio]{height:1rem;left:1.75rem;top:calc(50% - .5rem);width:1rem}.fr-radio-rich input[type=radio]+label{--idle:transparent;--hover:var(--background-default-grey-hover);--active:var(--background-default-grey-active);align-items:flex-start;background-color:var(--background-default-grey);box-shadow:inset 0 0 0 1px var(--border-default-grey);display:flex;flex-direction:column;justify-content:center;margin-left:0;min-height:5.5rem;padding:.5rem 6.5rem .5rem 3.5rem;width:100%}.fr-radio-rich input[type=radio]+label:before{box-shadow:inset 0 0 0 1px var(--border-action-high-grey),inset 0 0 0 8px var(--background-default-grey),inset 0 0 0 8px var(--background-action-high-blue-france);height:1rem;left:1.75rem;margin-top:-.5rem;position:absolute;top:50%;width:1rem}.fr-radio-rich input[type=radio]+label .fr-hint-text{margin-left:0}.fr-radio-rich input[type=radio]:disabled~.fr-radio-rich__img{filter:grayscale(1)}.fr-radio-rich input[type=radio]:not(:disabled)~label{--hover-tint:var(--hover);--active-tint:var(--active)}.fr-radio-rich input[type=radio]:not(:disabled)~label:hover{background-color:var(--hover-tint)}.fr-radio-rich input[type=radio]:not(:disabled)~label:active{background-color:var(--active-tint)}.fr-radio-rich input[type=radio]:not(:disabled)~label:hover~.fr-radio-rich__img{--brightness:calc(100% + var(--brighten)*10%)}.fr-radio-rich input[type=radio]:not(:disabled)~label:active~.fr-radio-rich__img{--brightness:calc(100% + var(--brighten)*20%)}.fr-radio-rich__img{box-shadow:inset 1px 0 0 0 var(--border-default-grey);display:flex;filter:brightness(var(--brightness));flex-direction:row;height:5rem;padding-left:.25rem;pointer-events:none;position:absolute;right:.25rem;top:.25rem;width:5.25rem}.fr-radio-rich__img svg{max-width:5rem;object-fit:cover}.fr-radio-group input[type=radio]:disabled+label:before{box-shadow:inset 0 0 0 1px var(--border-disabled-grey),inset 0 0 0 12px var(--background-default-grey),inset 0 0 0 12px var(--text-disabled-grey)}.fr-radio-group input[type=radio]:checked+label:before{box-shadow:inset 0 0 0 1px var(--border-action-high-grey),inset 0 0 0 6px var(--background-default-grey),inset 0 0 0 12px var(--background-action-high-blue-france)}.fr-radio-group input[type=radio]:checked:disabled+label:before{box-shadow:inset 0 0 0 1px var(--border-disabled-grey),inset 0 0 0 6px var(--background-default-grey),inset 0 0 0 12px var(--text-disabled-grey)}.fr-radio-rich input[type=radio]:disabled+label:before{box-shadow:inset 0 0 0 1px var(--border-disabled-grey),inset 0 0 0 8px var(--background-default-grey),inset 0 0 0 8px var(--text-disabled-grey)}.fr-radio-rich input[type=radio]:checked+label{box-shadow:inset 0 0 0 1px var(--border-action-high-blue-france)}.fr-radio-rich input[type=radio]:checked+label:before{box-shadow:inset 0 0 0 1px var(--border-action-high-grey),inset 0 0 0 4px var(--background-default-grey),inset 0 0 0 8px var(--background-action-high-blue-france)}.fr-radio-rich input[type=radio]:checked:disabled+label{box-shadow:inset 0 0 0 1px var(--text-disabled-grey)}.fr-radio-rich input[type=radio]:checked:disabled+label:before{box-shadow:inset 0 0 0 1px var(--border-disabled-grey),inset 0 0 0 4px var(--background-default-grey),inset 0 0 0 8px var(--text-disabled-grey)}.fr-fieldset .fr-fieldset__content .fr-radio-rich:first-child input[type=radio]+label{margin-top:.75rem}.fr-fieldset .fr-fieldset__content .fr-radio-rich input[type=radio]+label{margin-bottom:1rem;margin-top:.5rem}.fr-fieldset .fr-fieldset__content .fr-radio-rich:last-child input[type=radio]+label{margin-bottom:.75rem}.fr-modal{--ground:2000;align-items:stretch;background-color:hsla(0,0%,9%,.64);border:none;bottom:0;color:inherit;display:flex;flex-direction:column;height:100%;justify-content:space-between;left:0;margin:0;opacity:0;padding:0;position:fixed;right:0;top:0;transition:opacity .3s,visibility .3s;visibility:hidden;width:100%;z-index:1750}.fr-modal>.fr-container{pointer-events:none}.fr-modal:focus{outline:none}.fr-modal:before{content:""}.fr-modal:after,.fr-modal:before{display:block;flex:1 0 2rem;height:2rem;width:0}.fr-modal--top:before,.fr-modal:after{content:none}.fr-modal--top:after{content:""}.fr-modal--opened{height:100%;opacity:1;transition:opacity .3s,visibility .3s;visibility:inherit;width:100%}.fr-modal__body{--modal-max-height:calc(100vh - 2rem);--idle:transparent;--hover:var(--background-lifted-grey-hover);--active:var(--background-lifted-grey-active);background-color:var(--background-lifted-grey);filter:drop-shadow(var(--lifted-shadow));flex:1 1 auto;max-height:var(--modal-max-height);overflow-y:auto;pointer-events:all;z-index:calc(var(--ground) + 2000)}.fr-modal__header{align-items:center;display:flex;flex:auto 0 0;padding:1rem 1rem .5rem}.fr-modal__content{margin-bottom:3.5rem;padding-left:1rem;padding-right:1rem}.fr-modal__footer{--idle:transparent;--hover:var(--background-lifted-grey-hover);--active:var(--background-lifted-grey-active);background-color:var(--background-lifted-grey);bottom:0;display:flex;flex:auto 0 0;margin-top:-2.5rem;padding:1rem;position:sticky;transition:box-shadow .3s}.fr-modal__title{--title-spacing:0 0 1rem 0;color:var(--text-title-grey);font-size:1.375rem;font-weight:700;line-height:1.75rem}.fr-modal__title[class*=" fr-fi-"],.fr-modal__title[class^=fr-fi-]{margin-right:.5rem}.fr-nav{--underline-img:none;--ul-type:none;--ol-type:none;--ul-start:0;--ol-start:0;--xl-block:0;--li-bottom:0;--ol-content:none;--text-spacing:0;--title-spacing:0}.fr-nav__list{display:flex;flex-direction:column;margin:0;padding:0}.fr-nav__list>*>.fr-nav__btn,.fr-nav__list>*>.fr-nav__link,.fr-nav__list>.fr-nav__btn,.fr-nav__list>.fr-nav__link{font-weight:700}.fr-nav__item{align-items:stretch;display:flex;flex:0 1 auto;flex-direction:column;position:relative}.fr-nav__item:before{bottom:0;box-shadow:0 -1px 0 0 var(--border-default-grey),inset 0 -1px 0 0 var(--border-default-grey);content:"";display:block;height:100%;left:0;pointer-events:none;position:absolute;right:0;top:0;width:100%}.fr-nav__item .fr-btn{min-height:3rem}.fr-nav__btn,.fr-nav__link{--hover-tint:var(--hover);--active-tint:var(--active);color:var(--text-action-high-grey);font-size:1rem;line-height:1.5rem;padding:.75rem 0;text-align:left;width:100%}.fr-nav__btn[aria-current],.fr-nav__link[aria-current]{color:var(--text-active-blue-france);position:relative}.fr-nav__btn[aria-current]:before,.fr-nav__link[aria-current]:before{--idle:transparent;--hover:var(--background-active-blue-france-hover);--active:var(--background-active-blue-france-active);background-color:var(--background-active-blue-france);content:"";display:block;height:1.5rem;left:-1rem;margin-top:-.75rem;position:absolute;top:50%;width:2px}.fr-nav__link{display:block}.fr-nav__link[aria-current]:not([href]){cursor:default;pointer-events:none}.fr-nav__btn{align-items:center;display:flex;flex-direction:row;justify-content:space-between}.fr-nav__btn:after{--icon-size:1rem;background-color:currentColor;content:"";display:inline-block;flex:0 0 auto;height:var(--icon-size);margin-left:.5rem;margin-right:0;-webkit-mask-image:url(icons/system/arrow-down-s-line.svg);mask-image:url(icons/system/arrow-down-s-line.svg);-webkit-mask-size:100% 100%;mask-size:100% 100%;transition:transform .3s;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}.fr-nav__btn[aria-expanded=true]:after{transform:rotate(-180deg)}.fr-menu{margin:-4px -1rem;padding:4px 1rem;width:auto}.fr-menu__list{margin:0;padding:.5rem 0 1.5rem}.fr-menu .fr-nav__link{padding-left:1rem;padding-right:1rem}.fr-menu .fr-nav__link:before{left:0}.fr-nav__item:first-child:before{box-shadow:inset 0 -1px 0 0 var(--border-default-grey)}.fr-nav__item:last-child:before{box-shadow:0 -1px 0 0 var(--border-default-grey)}.fr-footer{--ul-type:none;--ol-type:none;--ul-start:0;--ol-start:0;--xl-block:0;--li-bottom:0;--ol-content:none;box-shadow:inset 0 2px 0 0 var(--border-plain-blue-france),inset 0 -1px 0 0 var(--border-default-grey);padding-top:2.5rem;width:100%}.fr-footer__body{align-items:center;display:flex;flex-direction:row;flex-wrap:wrap;margin-bottom:1rem}.fr-footer__body+.fr-footer__bottom{margin-top:1rem}.fr-footer__brand{align-items:center;display:flex;flex-basis:100%;flex-direction:row}.fr-footer__brand .fr-logo{font-size:1.05rem;margin:-1rem;padding:1rem}.fr-footer__brand .fr-logo:before{background-position:0 -.0625rem,0 0,0 0;background-size:2.75rem 1.125rem,2.75rem 1rem,0;height:1rem;margin-bottom:.3333333333rem;width:2.75rem}.fr-footer__brand .fr-logo:after{background-position:0 calc(100% + 1.875rem);background-size:5.25rem 3.75rem;min-width:2.625rem;padding-top:2.2083333333rem}[data-fr-theme=dark] .fr-footer__brand .fr-logo:after{background-position:-2.625rem 100%}.fr-footer__content{display:flex;flex-basis:100%;flex-wrap:wrap;margin-top:1.5rem}.fr-footer__content-desc{--underline-img:linear-gradient(0deg,currentColor,currentColor);--text-spacing:0 0 0.5rem 0;font-size:.875rem;line-height:1.5rem;width:100%}.fr-footer__content-list{align-self:center;display:flex;flex-direction:row;flex-wrap:wrap}.fr-footer__content-list>li{margin-bottom:.5rem;margin-right:1rem;margin-top:.5rem}.fr-footer__content-list>li:before{content:none}.fr-footer__content-list>li:last-child{margin-right:0}.fr-footer__content-link{font-size:.875rem;font-weight:700;line-height:1.5rem}.fr-footer__content-link:not(:hover):not(:active){--underline-idle-width:0}.fr-footer__bottom{align-items:center;box-shadow:inset 0 1px 0 0 var(--border-default-grey);display:flex;flex-direction:row;flex-wrap:wrap;margin-top:2.5rem}.fr-footer__bottom .fr-btn{color:var(--text-mention-grey);font-size:.75rem;line-height:1.25rem;max-height:none;max-width:100%;min-height:1.25rem;overflow:initial;padding:0 .5rem}.fr-footer__bottom .fr-btn:before{--icon-size:1rem;margin-left:-.125rem;margin-right:.5rem}.fr-footer__bottom-list{align-items:center;flex-wrap:wrap;margin:0;padding:.5rem 0 1rem;width:100%}.fr-footer__bottom-item{display:inline;margin:.5rem 0 0 .25rem;position:relative}.fr-footer__bottom-item:before{box-shadow:inset 0 0 0 1px var(--border-default-grey);content:"";display:inline-block;height:1rem;margin-bottom:.5rem;margin-right:.25rem;margin-top:.5rem;position:relative;vertical-align:middle;width:1px}.fr-footer__bottom-item:first-child{margin:.5rem 0 0}.fr-footer__bottom-item:first-child:before{content:none}.fr-footer__bottom-link{color:var(--text-mention-grey);font-size:.75rem;line-height:1.25rem}.fr-footer__bottom-link:not(:hover):not(:active){--underline-idle-width:0}.fr-footer__bottom-copy{--text-spacing:0 0 1rem 0;color:var(--text-mention-grey);margin-top:.5rem}.fr-footer__bottom-copy *{font-size:.75rem;line-height:1.25rem}.fr-footer__content-link{color:var(--text-title-grey)}.fr-input{--idle:transparent;--hover:var(--background-contrast-grey-hover);--active:var(--background-contrast-grey-active);background-color:var(--background-contrast-grey);border-radius:.25rem .25rem 0 0;box-shadow:inset 0 -2px 0 0 var(--border-plain-grey);color:var(--text-label-grey);display:block;font-size:1rem;line-height:1.5rem;padding:.5rem 1rem;width:100%}.fr-input::placeholder{color:var(--text-mention-grey);font-style:italic;opacity:1}.fr-input::-webkit-contacts-auto-fill-button{--idle:transparent;--hover:var(--text-label-grey-hover);--active:var(--text-label-grey-active);background-color:var(--text-label-grey);cursor:pointer}.fr-input:not(textarea){max-height:2.5rem}.fr-input:disabled{box-shadow:inset 0 -2px 0 0 var(--border-disabled-grey);color:var(--text-disabled-grey)}.fr-input:-webkit-autofill,.fr-input:-webkit-autofill:focus,.fr-input:-webkit-autofill:hover,.fr-input:autofill,.fr-input:autofill:focus,.fr-input:autofill:hover{-webkit-text-fill-color:var(--text-label-grey);box-shadow:inset 0 -2px 0 0 var(--border-plain-grey),inset 0 0 0 1000px var(--background-contrast-info)}.fr-search-bar{display:flex;flex-direction:row}.fr-search-bar .fr-label{clip:rect(0,0,0,0);border:0;height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;white-space:nowrap;width:1px}.fr-search-bar .fr-input{border-radius:.25rem 0 0;box-shadow:inset 0 -2px 0 0 var(--border-action-high-blue-france);margin:0;max-height:none}.fr-search-bar .fr-input::placeholder{font-style:italic}.fr-search-bar .fr-btn{border-radius:0 .25rem 0 0;flex:1 0 auto;font-size:1rem;line-height:1.5rem;max-height:2.5rem;max-width:2.5rem;min-height:2.5rem;overflow:hidden;padding:.5rem;white-space:nowrap}.fr-search-bar .fr-btn:before{--icon-size:1.5rem;background-color:currentColor;content:"";display:inline-block;flex:0 0 auto;height:var(--icon-size);margin-left:0;margin-right:.5rem;-webkit-mask-image:url(icons/system/search-line.svg);mask-image:url(icons/system/search-line.svg);-webkit-mask-size:100% 100%;mask-size:100% 100%;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}.fr-header{--underline-img:none;--ul-type:none;--ol-type:none;--ul-start:0;--ol-start:0;--xl-block:0;--li-bottom:0;--ol-content:none;--text-spacing:0;--title-spacing:0;position:relative;width:100%}.fr-header__body-row{align-items:center;display:flex;flex-direction:row;justify-content:flex-start;margin:0 -1rem}.fr-header__brand{--idle:transparent;--hover:var(--background-raised-grey-hover);--active:var(--background-raised-grey-active);background-color:var(--background-raised-grey);filter:drop-shadow(var(--raised-shadow));flex-wrap:wrap;padding-left:.25rem;padding-right:.25rem;z-index:calc(var(--ground) + 500)}.fr-header__brand,.fr-header__brand-top{align-items:center;display:flex;flex-direction:row;justify-content:flex-start;width:100%}.fr-header__logo{flex:0 0 auto;order:1;padding:.75rem}.fr-header__logo .fr-logo{font-size:.7875rem;margin:-.75rem;padding:.75rem}.fr-header__logo .fr-logo:before{background-position:0 -.046875rem,0 0,0 0;background-size:2.0625rem .84375rem,2.0625rem .75rem,0;height:.75rem;margin-bottom:.25rem;width:2.0625rem}.fr-header__logo .fr-logo:after{background-position:0 calc(100% + 1.40625rem);background-size:3.9375rem 2.8125rem;min-width:1.96875rem;padding-top:1.65625rem}[data-fr-theme=dark] .fr-header__logo .fr-logo:after{background-position:-1.96875rem 100%}.fr-header__service{box-shadow:inset 0 1px 0 0 var(--border-default-grey);margin-left:.75rem;margin-right:.75rem;padding-bottom:.75rem;padding-top:.75rem;width:100%}.fr-header__service-title{font-size:1.125rem;font-weight:700;line-height:1.5rem}.fr-header .fr-modal{--idle:transparent;--hover:var(--background-lifted-grey-hover);--active:var(--background-lifted-grey-active);background-color:var(--background-lifted-grey);justify-content:normal;overflow:auto}.fr-header .fr-modal:not([role=dialog]){transition:none}.fr-header .fr-modal:after,.fr-header .fr-modal:before{content:none}.fr-header .fr-modal>*>.fr-btn--close{margin-bottom:1.5rem}.fr-header .fr-modal>.fr-container{height:100%;padding-bottom:4.5rem;padding-top:1rem;pointer-events:all}.fr-header__navbar{align-items:flex-end;align-self:flex-start;display:flex;flex:0 0 auto;flex-direction:row;margin-left:auto;order:3;padding:.25rem;z-index:calc(var(--ground) + 1000)}.fr-header__navbar .fr-btn{--hover:inherit;--active:inherit;background-color:transparent;color:var(--text-action-high-blue-france);flex:0 0 auto;font-size:1rem;line-height:1.5rem;max-height:2.5rem;max-width:2.5rem;min-height:2.5rem;overflow:hidden;padding:.5rem;white-space:nowrap}.fr-header__navbar .fr-btn:before{--icon-size:1.5rem;margin-left:0;margin-right:.5rem}.fr-header__navbar .fr-btn--menu:after,.fr-header__navbar .fr-btn--menu:before{--icon-size:1.5rem;background-color:currentColor;display:inline-block;flex:0 0 auto;height:var(--icon-size);-webkit-mask-image:url(icons/system/menu-fill.svg);mask-image:url(icons/system/menu-fill.svg);-webkit-mask-size:100% 100%;mask-size:100% 100%;vertical-align:calc((.75em - var(--icon-size))*.5);width:var(--icon-size)}.fr-header__navbar .fr-btn--menu:before{content:""}.fr-header .fr-header__menu-links:after{content:"";display:block;height:1px;margin:.75rem -1rem;width:calc(100% + 2rem)}.fr-header__menu-links:after{box-shadow:inset 0 1px 0 0 var(--border-default-grey)}.fr-header__menu-links .fr-btn{--hover:inherit;--active:inherit;background-color:transparent;box-shadow:none;color:var(--text-action-high-blue-france)}.fr-header__menu-links .fr-btn:disabled,.fr-header__menu-links a.fr-btn:not([href]){--hover:inherit;--active:inherit;background-color:transparent;color:var(--text-disabled-grey)}.fr-header__navbar .fr-btn:disabled,.fr-header__navbar a.fr-btn:not([href]){--hover:inherit;--active:inherit;background-color:transparent;color:var(--text-disabled-grey)}.fr-header__navbar .fr-btn--menu{color:var(--text-default-grey)}@media (min-width:36em){
   /*! media sm */
   /*! media sm */
   /*! media sm */
   /*! media sm */
   /*! media sm */
   /*! media sm */
   /*! media sm */
```

### Comparing `mkdocs_dsfr-0.3.1/dsfr/dsfr.module.min.js` & `mkdocs_dsfr-0.4.0/dsfr/dsfr.module.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/dsfr.nomodule.min.js` & `mkdocs_dsfr-0.4.0/dsfr/dsfr.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/favicon/android-chrome-192x192.png` & `mkdocs_dsfr-0.4.0/dsfr/favicon/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/favicon/android-chrome-512x512.png` & `mkdocs_dsfr-0.4.0/dsfr/favicon/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/favicon/apple-touch-icon.png` & `mkdocs_dsfr-0.4.0/dsfr/favicon/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/favicon/favicon.ico` & `mkdocs_dsfr-0.4.0/dsfr/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/favicon/favicon.svg` & `mkdocs_dsfr-0.4.0/dsfr/favicon/favicon.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Bold.woff` & `mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Bold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Bold.woff2` & `mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Bold.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Bold_Italic.woff` & `mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Bold_Italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Bold_Italic.woff2` & `mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Bold_Italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Light.woff` & `mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Light.woff`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Light.woff2` & `mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Light.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Light_Italic.woff` & `mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Light_Italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Light_Italic.woff2` & `mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Light_Italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Medium.woff` & `mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Medium.woff`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Medium.woff2` & `mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Medium.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Medium_Italic.woff` & `mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Medium_Italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Medium_Italic.woff2` & `mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Medium_Italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Regular.woff` & `mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Regular.woff`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Regular.woff2` & `mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Regular.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Regular_Italic.woff` & `mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Regular_Italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/fonts/Marianne-Regular_Italic.woff2` & `mkdocs_dsfr-0.4.0/dsfr/fonts/Marianne-Regular_Italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/fonts/Spectral-ExtraBold.woff` & `mkdocs_dsfr-0.4.0/dsfr/fonts/Spectral-ExtraBold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/fonts/Spectral-ExtraBold.woff2` & `mkdocs_dsfr-0.4.0/dsfr/fonts/Spectral-ExtraBold.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/fonts/Spectral-Regular.woff` & `mkdocs_dsfr-0.4.0/dsfr/fonts/Spectral-Regular.woff`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/fonts/Spectral-Regular.woff2` & `mkdocs_dsfr-0.4.0/dsfr/fonts/Spectral-Regular.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/footer.html` & `mkdocs_dsfr-0.4.0/dsfr/footer.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,25 @@
 <footer class="fr-footer" role="contentinfo" id="footer">
     <div class="fr-container">
         <div class="fr-footer__body">
             <div class="fr-footer__brand fr-enlarge-link">
                 <a href="/" title="Retour à l'accueil du site - Nom de l'entité (ministère, secrétariat d'état, gouvernement)">
                     <p class="fr-logo">
-                        Intitulé
-                        <br>officiel
+                        {{ config.theme.intitule }}
                     </p>
                 </a>
             </div>
             <div class="fr-footer__content">
-                <p class="fr-footer__content-desc">Lorem [...] elit ut.</p>
+                <p class="fr-footer__content-desc">{{ config.theme.footer.description }}</p>
                 <ul class="fr-footer__content-list">
+                    {% for link in config.theme.footer.links %}
                     <li class="fr-footer__content-item">
-                        <a class="fr-footer__content-link" target="_blank" href="https://legifrance.gouv.fr">legifrance.gouv.fr</a>
-                    </li>
-                    <li class="fr-footer__content-item">
-                        <a class="fr-footer__content-link" target="_blank" href="https://gouvernement.fr">gouvernement.fr</a>
-                    </li>
-                    <li class="fr-footer__content-item">
-                        <a class="fr-footer__content-link" target="_blank" href="https://service-public.fr">service-public.fr</a>
-                    </li>
-                    <li class="fr-footer__content-item">
-                        <a class="fr-footer__content-link" target="_blank" href="https://data.gouv.fr">data.gouv.fr</a>
+                        <a class="fr-footer__content-link" target="_blank" href="{{ link.url }}">{{ link.name }}</a>
                     </li>
+                    {% endfor %}
                 </ul>
             </div>
         </div>
         <div class="fr-footer__bottom">
             <ul class="fr-footer__bottom-list">
                 <li class="fr-footer__bottom-item">
                     <a class="fr-footer__bottom-link" href="#">Plan du site</a>
```

#### html2text {}

```diff
@@ -1,14 +1,12 @@
-IntitulÃ©
-officiel
-Lorem [...] elit ut.
-    * legifrance.gouv.fr
-    * gouvernement.fr
-    * service-public.fr
-    * data.gouv.fr
+{{_config.theme.intitule_}}
+{{ config.theme.footer.description }}
+    * {% for link in config.theme.footer.links %}
+    * {{_link.name_}}
+    * {% endfor %}
     * Plan_du_site
     * AccessibilitÃ©_:_non/partiellement/totalement_conforme
     * Mentions_lÃ©gales
     * DonnÃ©es_personnelles
     * Gestion_des_cookies
     * ParamÃ¨tres d'affichage
 Sauf mention contraire, tous les contenus de ce site sont sous licence_etalab-
```

### Comparing `mkdocs_dsfr-0.3.1/dsfr/header.html` & `mkdocs_dsfr-0.4.0/dsfr/header.html`

 * *Files 4% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 						<div class="fr-header__logo">
 							<p class="fr-logo">
 								{{ config.theme.intitule }}
 							</p>
 						</div>
 
 						<div class="fr-header__navbar">
-							{% if not config.theme.no_search %}
+							{% if not config.theme.header.no_search %}
 								<button class="fr-btn--search fr-btn" data-fr-opened="false" aria-controls="modal-541" id="button-542" title="Rechercher">
 									Rechercher
 								</button>
 							{% endif %}
 							<button class="fr-btn--menu fr-btn" data-fr-opened="false" aria-controls="modal-543" aria-haspopup="menu" id="button-544" title="Menu">
 								Menu
 							</button>
 						</div>
 					</div>
 					<div class="fr-header__service">
 						<a href="/" title="{{ config.theme.titre }}">
 							<p class="fr-header__service-title">
-								{{ config.theme.titre }}
+								{{ config.theme.header.titre }}
 							</p>
 						</a>
-						<p class="fr-header__service-tagline">{{ config.theme.soustitre }}</p>
+						<p class="fr-header__service-tagline">{{ config.theme.header.sous_titre }}</p>
 					</div>
 				</div>
 				<div class="fr-header__tools">
 					<div class="fr-header__search fr-modal" id="modal-541">
 						<div class="fr-container fr-container-lg--fluid">
 							<button class="fr-btn--close fr-btn" aria-controls="modal-541" title="Fermer">
 								Fermer
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {{ config.theme.intitule }}
-{% if not config.theme.no_search %}  Rechercher  {% endif %}  Menu
-{{_config.theme.titre_}}
-{{ config.theme.soustitre }}
+{% if not config.theme.header.no_search %}  Rechercher  {% endif %}  Menu
+{{_config.theme.header.titre_}}
+{{ config.theme.header.sous_titre }}
  Fermer  {% if not config.theme.no_search %}
  Rechercher  [Unknown INPUT type]  Rechercher
 {% endif %}
  Fermer
 {% include "nav.html" %}
```

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/buildings/ancient-gate-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/buildings/ancient-gate-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/buildings/store-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/buildings/store-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/business/global-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/business/global-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/business/global-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/business/global-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/design/brush-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/design/brush-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/design/palette-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/design/palette-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/development/bug-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/development/bug-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/device/dashboard-3-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/device/dashboard-3-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/device/dashboard-3-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/device/dashboard-3-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/device/phone-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/device/phone-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/device/wifi-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/device/wifi-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/device/wifi-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/device/wifi-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/editor/h-3.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/editor/h-3.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/editor/h-6.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/editor/h-6.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/health/dislike-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/health/dislike-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/health/heart-pulse-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/health/heart-pulse-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/health/lungs-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/health/lungs-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/health/microscope-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/health/microscope-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/health/microscope-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/health/microscope-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/health/surgical-mask-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/health/surgical-mask-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/health/thermometer-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/health/thermometer-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/health/virus-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/health/virus-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/health/virus-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/health/virus-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/chrome-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/chrome-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/chrome-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/chrome-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/edge-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/edge-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/firefox-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/firefox-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/firefox-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/firefox-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/fr--dailymotion-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/fr--dailymotion-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/fr--dailymotion-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/fr--dailymotion-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/fr--tiktok-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/fr--tiktok-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/github-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/github-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/github-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/github-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/google-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/google-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/ie-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/ie-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/ie-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/ie-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/instagram-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/instagram-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/instagram-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/instagram-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/linkedin-box-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/linkedin-box-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/mastodon-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/mastodon-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/mastodon-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/mastodon-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/safari-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/safari-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/safari-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/safari-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/slack-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/slack-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/slack-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/slack-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/snapchat-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/snapchat-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/snapchat-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/snapchat-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/twitter-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/twitter-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/twitter-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/twitter-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/vimeo-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/vimeo-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/vimeo-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/vimeo-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/logo/youtube-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/logo/youtube-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/map/earth-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/map/earth-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/map/earth-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/map/earth-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/map/france-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/map/france-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/map/france-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/map/france-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/map/ship-2-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/map/ship-2-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/map/ship-2-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/map/ship-2-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/media/volume-up-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/media/volume-up-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/media/volume-up-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/media/volume-up-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/others/recycle-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/others/recycle-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/others/recycle-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/others/recycle-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/others/scales-3-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/others/scales-3-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/system/eye-off-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/system/eye-off-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/system/settings-5-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/system/settings-5-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/system/settings-5-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/system/settings-5-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/user/account-pin-circle-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/user/account-pin-circle-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/user/team-line.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/user/team-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/icons/user/user-setting-fill.svg` & `mkdocs_dsfr-0.4.0/dsfr/icons/user/user-setting-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/js/base.js` & `mkdocs_dsfr-0.4.0/dsfr/js/base.js`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/js/bootstrap.min.js` & `mkdocs_dsfr-0.4.0/dsfr/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/js/jquery-1.10.2.min.js` & `mkdocs_dsfr-0.4.0/dsfr/js/jquery-1.10.2.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/lateral.html` & `mkdocs_dsfr-0.4.0/dsfr/lateral.html`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/nav.html` & `mkdocs_dsfr-0.4.0/dsfr/nav.html`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/prev-next-nav.html` & `mkdocs_dsfr-0.4.0/dsfr/prev-next-nav.html`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/search.html` & `mkdocs_dsfr-0.4.0/dsfr/search.html`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/README.md` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/README.md` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.main.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.main.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.main.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.main.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-buildings/icons-buildings.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-buildings/icons-buildings.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/README.md` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.legacy.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.legacy.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.legacy.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.legacy.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.main.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.main.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.main.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.main.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-business/icons-business.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-business/icons-business.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/README.md` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.legacy.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.legacy.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.legacy.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.legacy.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.main.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.main.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.main.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.main.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-communication/icons-communication.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-communication/icons-communication.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/README.md` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.legacy.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.legacy.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.legacy.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.legacy.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.main.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.main.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.main.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.main.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-design/icons-design.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-design/icons-design.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/README.md` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.legacy.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.legacy.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.legacy.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.legacy.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.main.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.main.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.main.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.main.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-development/icons-development.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-development/icons-development.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/README.md` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.legacy.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.legacy.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.legacy.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.legacy.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.main.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.main.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.main.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.main.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-device/icons-device.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-device/icons-device.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/README.md` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.legacy.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.legacy.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.legacy.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.legacy.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.main.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.main.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.main.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.main.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-document/icons-document.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-document/icons-document.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/README.md` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.legacy.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.legacy.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.legacy.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.legacy.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.main.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.main.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.main.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.main.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-editor/icons-editor.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-editor/icons-editor.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/README.md` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.legacy.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.legacy.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.legacy.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.legacy.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.main.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.main.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.main.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.main.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-finance/icons-finance.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-finance/icons-finance.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/README.md` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.legacy.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.legacy.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.legacy.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.legacy.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.main.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.main.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.main.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.main.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-health/icons-health.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-health/icons-health.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/README.md` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.legacy.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.legacy.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.legacy.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.legacy.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.main.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.main.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.main.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.main.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-logo/icons-logo.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-logo/icons-logo.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/README.md` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.legacy.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.legacy.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.legacy.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.legacy.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.main.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.main.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.main.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.main.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-map/icons-map.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-map/icons-map.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/README.md` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.legacy.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.legacy.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.legacy.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.legacy.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.main.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.main.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.main.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.main.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-media/icons-media.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-media/icons-media.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/README.md` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.legacy.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.legacy.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.legacy.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.legacy.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.main.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.main.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.main.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.main.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-others/icons-others.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-others/icons-others.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/README.md` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.legacy.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.legacy.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.legacy.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.legacy.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.main.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.main.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.main.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.main.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-system/icons-system.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-system/icons-system.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/README.md` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.legacy.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.legacy.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.legacy.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.legacy.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.main.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.main.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.main.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.main.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-user/icons-user.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-user/icons-user.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/README.md` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.legacy.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.legacy.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.legacy.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.legacy.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.main.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.main.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.main.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.main.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons-weather/icons-weather.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons-weather/icons-weather.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.legacy.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.legacy.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.legacy.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.legacy.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.main.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.main.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.main.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.main.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.min.css` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/dsfr/utility/icons/icons.min.css.map` & `mkdocs_dsfr-0.4.0/dsfr/utility/icons/icons.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_dsfr-0.3.1/pyproject.toml` & `mkdocs_dsfr-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mkdocs-dsfr"
-version = "0.3.1"
+version = "0.4.0"
 description = "DSFR theme for Mkdocs"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
     "mkdocs>=1.4",
 ]
```

