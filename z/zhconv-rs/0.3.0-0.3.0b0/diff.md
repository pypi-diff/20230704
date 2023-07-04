# Comparing `tmp/zhconv_rs-0.3.0.tar.gz` & `tmp/zhconv_rs-0.3.0b0.tar.gz`

## Comparing `zhconv_rs-0.3.0.tar` & `zhconv_rs-0.3.0b0.tar`

### file list

```diff
@@ -1,477 +1,477 @@
--rw-r--r--   0        0        0     1874 1970-01-01 00:00:00.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/Cargo.toml
--rw-r--r--   0     1001      123      426 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/.gitattributes
--rw-r--r--   0     1001      123     1775 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/.github/workflows/main.yml
--rw-r--r--   0     1001      123     2445 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/.github/workflows/npm.yml
--rw-r--r--   0     1001      123     1973 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/.github/workflows/pyo3.yml
--rw-r--r--   0     1001      123     2703 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/.github/workflows/release.yml
--rw-r--r--   0     1001      123       20 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/.gitignore
--rw-r--r--   0     1001      123    35149 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/LICENSE
--rw-r--r--   0     1001      123    10306 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/README.md
--rw-r--r--   0     1001      123   284864 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/benches/25328-0.txt
--rw-r--r--   0     1001      123      198 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/benches/LICENSE.md
--rw-r--r--   0     1001      123  3261912 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/benches/data3185k.txt
--rw-r--r--   0     1001      123    55192 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/benches/data54k.txt
--rw-r--r--   0     1001      123   705845 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/benches/data689k.txt
--rw-r--r--   0     1001      123    79133 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/benches/wikitext.txt
--rw-r--r--   0     1001      123     6243 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/benches/zhconv_benchmark.rs
--rw-r--r--   0     1001      123    21088 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/build.rs
--rw-r--r--   0     1001      123      532 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/HKVariants.txt
--rw-r--r--   0     1001      123     2709 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/HKVariantsRevPhrases.txt
--rw-r--r--   0     1001      123      870 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/README.md
--rw-r--r--   0     1001      123    34353 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/STCharacters.txt
--rw-r--r--   0     1001      123  1004153 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/STPhrases.txt
--rw-r--r--   0     1001      123    34627 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/TSCharacters.txt
--rw-r--r--   0     1001      123     5161 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/TSPhrases.txt
--rw-r--r--   0     1001      123     7611 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/TWPhrasesIT.txt
--rw-r--r--   0     1001      123     2121 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/TWPhrasesName.txt
--rw-r--r--   0     1001      123      571 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/TWPhrasesOther.txt
--rw-r--r--   0     1001      123      312 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/TWVariants.txt
--rw-r--r--   0     1001      123     1075 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/TWVariantsRevPhrases.txt
--rw-r--r--   0     1001      123   447718 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/ZhConversion.php
--rw-r--r--   0     1001      123     7470 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/1D.json
--rw-r--r--   0     1001      123     4660 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/2016年太平洋颱風季.json
--rw-r--r--   0     1001      123     4462 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/2017年太平洋颱風季.json
--rw-r--r--   0     1001      123     4953 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/2018年太平洋颱風季.json
--rw-r--r--   0     1001      123     4967 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/2019年太平洋颱風季.json
--rw-r--r--   0     1001      123     4150 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/2020年太平洋颱風季.json
--rw-r--r--   0     1001      123     3977 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/2021年太平洋颱風季.json
--rw-r--r--   0     1001      123     4396 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/2022年太平洋颱風季.json
--rw-r--r--   0     1001      123      311 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/2023年太平洋颱風季.json
--rw-r--r--   0     1001      123    18639 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/24.json
--rw-r--r--   0     1001      123     1347 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/A Pink.json
--rw-r--r--   0     1001      123     1436 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/A Song of Ice and Fire.json
--rw-r--r--   0     1001      123     4784 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/ACmilan.json
--rw-r--r--   0     1001      123     4078 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/ALeague.json
--rw-r--r--   0     1001      123    12349 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/AT Places.json
--rw-r--r--   0     1001      123    12270 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/AU Places.json
--rw-r--r--   0     1001      123     2618 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Adventure Time.json
--rw-r--r--   0     1001      123    24747 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Aero.json
--rw-r--r--   0     1001      123     4785 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Aikatsu.json
--rw-r--r--   0     1001      123    44770 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Anime.json
--rw-r--r--   0     1001      123    11339 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Apple.json
--rw-r--r--   0     1001      123     6426 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Aquatics.json
--rw-r--r--   0     1001      123     3127 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Ariana Grande.json
--rw-r--r--   0     1001      123      682 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Artist.json
--rw-r--r--   0     1001      123    11447 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Astronomy.json
--rw-r--r--   0     1001      123     4837 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Avatar.json
--rw-r--r--   0     1001      123     3325 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Avril Lavigne.json
--rw-r--r--   0     1001      123    46163 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/BE Places.json
--rw-r--r--   0     1001      123    11395 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/BUDDYCOMPLEX.json
--rw-r--r--   0     1001      123    10696 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Badminton.json
--rw-r--r--   0     1001      123     2277 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Bakuman.json
--rw-r--r--   0     1001      123     1911 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Battle Spirits.json
--rw-r--r--   0     1001      123   108138 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Bird.json
--rw-r--r--   0     1001      123   891099 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/BirdG.json
--rw-r--r--   0     1001      123   528555 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/BirdP.json
--rw-r--r--   0     1001      123     3893 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Black Mirror.json
--rw-r--r--   0     1001      123     3895 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Bridge.json
--rw-r--r--   0     1001      123     7962 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Britney Spears.json
--rw-r--r--   0     1001      123     7729 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Bundesliga.json
--rw-r--r--   0     1001      123    66546 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Butterfly.json
--rw-r--r--   0     1001      123     3715 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/C&C.json
--rw-r--r--   0     1001      123    17645 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/CA Places.json
--rw-r--r--   0     1001      123     2454 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/CANAAN.json
--rw-r--r--   0     1001      123    33866 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/CH Places.json
--rw-r--r--   0     1001      123    13534 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/COD.json
--rw-r--r--   0     1001      123     9143 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/CWBTyphoonOld.json
--rw-r--r--   0     1001      123     6467 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Canada.json
--rw-r--r--   0     1001      123     4462 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Carnivorous Plant.json
--rw-r--r--   0     1001      123    10024 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Cartoon.json
--rw-r--r--   0     1001      123      883 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Chanel.json
--rw-r--r--   0     1001      123    18060 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Chemistry.json
--rw-r--r--   0     1001      123     5155 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Code Black.json
--rw-r--r--   0     1001      123     7909 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Code Geass.json
--rw-r--r--   0     1001      123     2053 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/CodeLyoko.json
--rw-r--r--   0     1001      123     3078 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Coldplay.json
--rw-r--r--   0     1001      123    11955 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Communication.json
--rw-r--r--   0     1001      123     5620 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Composer.json
--rw-r--r--   0     1001      123     4654 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Copyright.json
--rw-r--r--   0     1001      123    92366 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Counter-Strike.json
--rw-r--r--   0     1001      123      294 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/County.json
--rw-r--r--   0     1001      123    17698 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Crazyracing Kartrider.json
--rw-r--r--   0     1001      123     3200 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Cyber Formula.json
--rw-r--r--   0     1001      123     6089 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Cyclone.json
--rw-r--r--   0     1001      123     1381 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/DCComics.json
--rw-r--r--   0     1001      123   103362 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/DE Places.json
--rw-r--r--   0     1001      123    10853 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Danball Senki.json
--rw-r--r--   0     1001      123     1129 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Dance.json
--rw-r--r--   0     1001      123     1629 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Death Note.json
--rw-r--r--   0     1001      123     6663 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Diablo.json
--rw-r--r--   0     1001      123      783 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Die Weiße Rose.json
--rw-r--r--   0     1001      123    17587 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Digimon.json
--rw-r--r--   0     1001      123    33790 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Disney.json
--rw-r--r--   0     1001      123     3249 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Doctor Who.json
--rw-r--r--   0     1001      123     7180 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Doraemon.json
--rw-r--r--   0     1001      123    15722 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/DragonBall.json
--rw-r--r--   0     1001      123    28035 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/DreamWorks.json
--rw-r--r--   0     1001      123     5595 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/ED.json
--rw-r--r--   0     1001      123    23292 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/EPL.json
--rw-r--r--   0     1001      123     6196 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/EU.json
--rw-r--r--   0     1001      123    10152 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Earthquake.json
--rw-r--r--   0     1001      123    34462 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Ecology.json
--rw-r--r--   0     1001      123    25054 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Economics.json
--rw-r--r--   0     1001      123    16745 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Electronics.json
--rw-r--r--   0     1001      123     1949 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Esports.json
--rw-r--r--   0     1001      123     5832 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Eyeshield21.json
--rw-r--r--   0     1001      123    16682 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/F1.json
--rw-r--r--   0     1001      123    12291 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/FAcup.json
--rw-r--r--   0     1001      123   112357 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/FR Places.json
--rw-r--r--   0     1001      123     5415 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Family Guy.json
--rw-r--r--   0     1001      123    38198 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Firearms.json
--rw-r--r--   0     1001      123    26299 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Food.json
--rw-r--r--   0     1001      123    23933 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Football.json
--rw-r--r--   0     1001      123     1431 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Friends.json
--rw-r--r--   0     1001      123     2301 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Fringe.json
--rw-r--r--   0     1001      123     5440 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Frozen.json
--rw-r--r--   0     1001      123    16568 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/FullmetalAlchemist.json
--rw-r--r--   0     1001      123     3114 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Futurama.json
--rw-r--r--   0     1001      123    30810 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GBF.json
--rw-r--r--   0     1001      123     6024 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GGundam.json
--rw-r--r--   0     1001      123     5068 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GOSICK.json
--rw-r--r--   0     1001      123     5201 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GZFC.json
--rw-r--r--   0     1001      123     6847 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Games-zh.json
--rw-r--r--   0     1001      123    75060 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Games.json
--rw-r--r--   0     1001      123     2196 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GaoGaiGar.json
--rw-r--r--   0     1001      123     1586 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Geography.json
--rw-r--r--   0     1001      123     2860 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Getter Robo.json
--rw-r--r--   0     1001      123     6273 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Ghibli.json
--rw-r--r--   0     1001      123     7545 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Glee.json
--rw-r--r--   0     1001      123     5456 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GossipGirl.json
--rw-r--r--   0     1001      123     5846 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Guardians of Ga'Hoole.json
--rw-r--r--   0     1001      123    28072 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Gundam00.json
--rw-r--r--   0     1001      123    21085 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GundamAGE.json
--rw-r--r--   0     1001      123    32810 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GundamIBO.json
--rw-r--r--   0     1001      123    37988 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GundamSeed.json
--rw-r--r--   0     1001      123    12889 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GundamTWFM.json
--rw-r--r--   0     1001      123    72213 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GundamUC.json
--rw-r--r--   0     1001      123     7502 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GundamW.json
--rw-r--r--   0     1001      123     7651 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/HTGAWM.json
--rw-r--r--   0     1001      123    14605 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/HUNTER.json
--rw-r--r--   0     1001      123     6381 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Half-Life.json
--rw-r--r--   0     1001      123     1213 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Hannibal Lecter.json
--rw-r--r--   0     1001      123    69432 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/HarryPotter.json
--rw-r--r--   0     1001      123      771 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Hawaii Five-0.json
--rw-r--r--   0     1001      123     4149 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Hayate the Combat Butler.json
--rw-r--r--   0     1001      123    10198 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Heroes of the Storm.json
--rw-r--r--   0     1001      123    12525 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/House.json
--rw-r--r--   0     1001      123     1670 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/IMF.json
--rw-r--r--   0     1001      123   186279 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/IT.json
--rw-r--r--   0     1001      123     2734 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/JLeague.json
--rw-r--r--   0     1001      123   214806 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/JP Show.json
--rw-r--r--   0     1001      123    12353 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/James Bond.json
--rw-r--r--   0     1001      123    14545 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Jewelpet.json
--rw-r--r--   0     1001      123     1814 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Justin Bieber.json
--rw-r--r--   0     1001      123     6140 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/KLeague.json
--rw-r--r--   0     1001      123    71612 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/KO Movie.json
--rw-r--r--   0     1001      123    31224 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/KO Show.json
--rw-r--r--   0     1001      123   124806 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/KO TV Show.json
--rw-r--r--   0     1001      123    30116 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/KamenRider.json
--rw-r--r--   0     1001      123     3400 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Kao.json
--rw-r--r--   0     1001      123     1214 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Katy Perry.json
--rw-r--r--   0     1001      123     1403 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Korea Comparison.json
--rw-r--r--   0     1001      123    27780 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Korea.json
--rw-r--r--   0     1001      123      563 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Korean.json
--rw-r--r--   0     1001      123     1494 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/LEGO.json
--rw-r--r--   0     1001      123    20622 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/LOL.json
--rw-r--r--   0     1001      123     5749 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/LR.json
--rw-r--r--   0     1001      123     7789 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/La casa de papel.json
--rw-r--r--   0     1001      123     2998 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Lady Gaga.json
--rw-r--r--   0     1001      123     5497 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Lana Del Rey.json
--rw-r--r--   0     1001      123     2009 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Laos.json
--rw-r--r--   0     1001      123     1545 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Legend of the Guardians.json
--rw-r--r--   0     1001      123     2412 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Les Misérables.json
--rw-r--r--   0     1001      123    64760 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Lifesciences.json
--rw-r--r--   0     1001      123      200 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Linguistics.json
--rw-r--r--   0     1001      123     3038 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Linkin.json
--rw-r--r--   0     1001      123     2381 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Lorde.json
--rw-r--r--   0     1001      123    96457 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/LuaIT.json
--rw-r--r--   0     1001      123   242697 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/LuaMovie.json
--rw-r--r--   0     1001      123   113609 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/LuaShow.json
--rw-r--r--   0     1001      123    14349 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MA.json
--rw-r--r--   0     1001      123     5674 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MCD.json
--rw-r--r--   0     1001      123     7228 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MCFC.json
--rw-r--r--   0     1001      123     3350 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MLS.json
--rw-r--r--   0     1001      123    14999 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MUFC.json
--rw-r--r--   0     1001      123    14862 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MY.json
--rw-r--r--   0     1001      123    17706 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Mabinogi.json
--rw-r--r--   0     1001      123    14833 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MapleStory.json
--rw-r--r--   0     1001      123      946 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Mariah Carey.json
--rw-r--r--   0     1001      123      215 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MarvelNetflix.json
--rw-r--r--   0     1001      123    34592 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Math.json
--rw-r--r--   0     1001      123    11580 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Mazinger.json
--rw-r--r--   0     1001      123     5877 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/McDonald's.json
--rw-r--r--   0     1001      123    16322 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MediaWiki special.json
--rw-r--r--   0     1001      123    11410 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MediaWiki.json
--rw-r--r--   0     1001      123    19988 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Medicine.json
--rw-r--r--   0     1001      123     1285 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Michael Jackson.json
--rw-r--r--   0     1001      123      183 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MigTest.json
--rw-r--r--   0     1001      123     3043 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Might&Magic.json
--rw-r--r--   0     1001      123    44509 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Military.json
--rw-r--r--   0     1001      123     7029 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Minecraft.json
--rw-r--r--   0     1001      123   442700 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Movie.json
--rw-r--r--   0     1001      123    28123 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Music.json
--rw-r--r--   0     1001      123    44930 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/My Little Pony.json
--rw-r--r--   0     1001      123     8118 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MyHeroAcademia.json
--rw-r--r--   0     1001      123    14670 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/NARUTO.json
--rw-r--r--   0     1001      123    77638 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/NBA.json
--rw-r--r--   0     1001      123     5860 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/NFL.json
--rw-r--r--   0     1001      123     1095 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/NHL.json
--rw-r--r--   0     1001      123    12730 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Nintendo.json
--rw-r--r--   0     1001      123     7719 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Nobel Prize.json
--rw-r--r--   0     1001      123    37371 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/OnePiece.json
--rw-r--r--   0     1001      123    10030 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Organization.json
--rw-r--r--   0     1001      123     4166 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Overwatch.json
--rw-r--r--   0     1001      123     3308 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/P&G.json
--rw-r--r--   0     1001      123     2081 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/PHL Places.json
--rw-r--r--   0     1001      123    94006 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/People.json
--rw-r--r--   0     1001      123     3404 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/PeppaPig.json
--rw-r--r--   0     1001      123     2479 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Percy Jackson.json
--rw-r--r--   0     1001      123     3168 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/PerryClass.json
--rw-r--r--   0     1001      123     6642 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Pesticide.json
--rw-r--r--   0     1001      123     2918 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Photography.json
--rw-r--r--   0     1001      123    28389 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Physics.json
--rw-r--r--   0     1001      123     4149 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Pichi Pichi Pitch.json
--rw-r--r--   0     1001      123      966 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Pinnacle Islands.json
--rw-r--r--   0     1001      123    34697 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Pixar.json
--rw-r--r--   0     1001      123    20027 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Pokemon-old.json
--rw-r--r--   0     1001      123    20296 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Pokemon.json
--rw-r--r--   0     1001      123    67585 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/PoliticiansUK.json
--rw-r--r--   0     1001      123     8551 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Popes.json
--rw-r--r--   0     1001      123     3495 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Power Rangers.json
--rw-r--r--   0     1001      123    31357 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/PresidentsUS.json
--rw-r--r--   0     1001      123    11576 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Pretty Rhythm.json
--rw-r--r--   0     1001      123     5719 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/PrisonBreak.json
--rw-r--r--   0     1001      123    17999 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Psychology.json
--rw-r--r--   0     1001      123    49490 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Racing.json
--rw-r--r--   0     1001      123    37973 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Railway.json
--rw-r--r--   0     1001      123     2496 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/RainbowSixSiege.json
--rw-r--r--   0     1001      123    11105 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Reborn.json
--rw-r--r--   0     1001      123     6151 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/ResidentEvil.json
--rw-r--r--   0     1001      123     3555 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Rihanna.json
--rw-r--r--   0     1001      123    35731 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/SAO.json
--rw-r--r--   0     1001      123     1842 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/SARS-CoV-2 variant.json
--rw-r--r--   0     1001      123     5934 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/SEGA.json
--rw-r--r--   0     1001      123     4084 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/SNSD.json
--rw-r--r--   0     1001      123     2282 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/SPL.json
--rw-r--r--   0     1001      123     1598 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/SPY×FAMILY.json
--rw-r--r--   0     1001      123     3803 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Sailor Moon.json
--rw-r--r--   0     1001      123     9438 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/SaintSeiyaOmega.json
--rw-r--r--   0     1001      123    74396 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Sandbox.json
--rw-r--r--   0     1001      123     1837 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Selena Gomez.json
--rw-r--r--   0     1001      123    24202 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Shinkalion.json
--rw-r--r--   0     1001      123     8677 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Shipname.json
--rw-r--r--   0     1001      123   270643 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Show.json
--rw-r--r--   0     1001      123     3132 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Shugo Chara!.json
--rw-r--r--   0     1001      123     2253 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Sia.json
--rw-r--r--   0     1001      123     2266 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Signals and Systems.json
--rw-r--r--   0     1001      123      372 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Signpost.json
--rw-r--r--   0     1001      123    11351 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Sim.json
--rw-r--r--   0     1001      123    20778 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Simpsons.json
--rw-r--r--   0     1001      123    10767 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Snooker.json
--rw-r--r--   0     1001      123     2588 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/SouthPark.json
--rw-r--r--   0     1001      123     9718 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/SpongeBob SquarePants.json
--rw-r--r--   0     1001      123    10794 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Sports.json
--rw-r--r--   0     1001      123    17092 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Square Enix.json
--rw-r--r--   0     1001      123     7526 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/StarCraft.json
--rw-r--r--   0     1001      123    11391 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/StarCraft2.json
--rw-r--r--   0     1001      123    27435 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/StarTrek.json
--rw-r--r--   0     1001      123    12653 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/StarWars.json
--rw-r--r--   0     1001      123     6942 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/StephenKing.json
--rw-r--r--   0     1001      123      549 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Summon Night.json
--rw-r--r--   0     1001      123     1674 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/TCM.json
--rw-r--r--   0     1001      123      275 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/TLeague.json
--rw-r--r--   0     1001      123   105974 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/TV.json
--rw-r--r--   0     1001      123     5543 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Table Tennis.json
--rw-r--r--   0     1001      123     3650 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Tales.json
--rw-r--r--   0     1001      123     5286 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Tamagotchi.json
--rw-r--r--   0     1001      123    11981 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Taylor Swift.json
--rw-r--r--   0     1001      123     2419 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Telcom.json
--rw-r--r--   0     1001      123    71368 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Tennis.json
--rw-r--r--   0     1001      123      115 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/TfL.json
--rw-r--r--   0     1001      123      521 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/The Chainsmokers.json
--rw-r--r--   0     1001      123    12593 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/The Witcher.json
--rw-r--r--   0     1001      123     4828 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/The World God Only Knows.json
--rw-r--r--   0     1001      123     3120 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/TheBeatles.json
--rw-r--r--   0     1001      123     2346 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/ThePeanuts.json
--rw-r--r--   0     1001      123     3570 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Toaru.json
--rw-r--r--   0     1001      123    24126 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Transformers.json
--rw-r--r--   0     1001      123     4352 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Transport for London.json
--rw-r--r--   0     1001      123    44492 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Transport.json
--rw-r--r--   0     1001      123    35103 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/TropicalCycloneName.json
--rw-r--r--   0     1001      123     3253 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Twilight.json
--rw-r--r--   0     1001      123     6974 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/TyphoonNew.json
--rw-r--r--   0     1001      123    25610 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/TyphoonOld.json
--rw-r--r--   0     1001      123     4728 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/UA toponyms.json
--rw-r--r--   0     1001      123    42557 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/UK Places.json
--rw-r--r--   0     1001      123     3707 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/US CA Cities.json
--rw-r--r--   0     1001      123     5434 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/US Government.json
--rw-r--r--   0     1001      123      584 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/US Senators.json
--rw-r--r--   0     1001      123    27748 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/USState.json
--rw-r--r--   0     1001      123    22229 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Ultraman.json
--rw-r--r--   0     1001      123     1791 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Unilever.json
--rw-r--r--   0     1001      123     7171 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Unit.json
--rw-r--r--   0     1001      123     6267 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Urban.json
--rw-r--r--   0     1001      123      802 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/VLeague.json
--rw-r--r--   0     1001      123     2372 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Valkyria.json
--rw-r--r--   0     1001      123     1272 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/WORKING!!.json
--rw-r--r--   0     1001      123    18912 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Warcraft.json
--rw-r--r--   0     1001      123     1024 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Warhammer.json
--rw-r--r--   0     1001      123    11262 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Warriors.json
--rw-r--r--   0     1001      123     1547 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Watch.json
--rw-r--r--   0     1001      123     5103 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Weather.json
--rw-r--r--   0     1001      123    14791 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Windows.json
--rw-r--r--   0     1001      123    26033 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Wow.json
--rw-r--r--   0     1001      123     8357 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Yes! 光之美少女5.json
--rw-r--r--   0     1001      123    63286 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/ZH Show.json
--rw-r--r--   0     1001      123     9963 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/arsenal.json
--rwxr-xr-x   0     1001      123     1629 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/check1.py
--rw-r--r--   0     1001      123    14239 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/chelsea.json
--rw-r--r--   0     1001      123     8008 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/fcbarcelona.json
--rw-r--r--   0     1001      123    34236 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/fcbayern.json
--rw-r--r--   0     1001      123     4414 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/free license.json
--rw-r--r--   0     1001      123     1071 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/inter.json
--rw-r--r--   0     1001      123    25910 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/laliga.json
--rw-r--r--   0     1001      123     4300 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/leek.json
--rw-r--r--   0     1001      123     4246 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/ligue.json
--rw-r--r--   0     1001      123    24883 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/liverpoolfc.json
--rw-r--r--   0     1001      123     8135 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/loghorizon.json
--rw-r--r--   0     1001      123    17062 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/magi.json
--rwxr-xr-x   0     1001      123     1497 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/merge_for_web.py
--rw-r--r--   0     1001      123    27273 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/neo-noir.json
--rw-r--r--   0     1001      123     4240 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/regalia.json
--rw-r--r--   0     1001      123     3967 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/specialpages.json
--rw-r--r--   0     1001      123    39998 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/uefa.json
--rw-r--r--   0     1001      123     8235 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/vital.json
--rw-r--r--   0     1001      123    13742 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/一拳超人.json
--rw-r--r--   0     1001      123     1103 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/伊拉克足球.json
--rw-r--r--   0     1001      123     2735 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/伊斯蘭.json
--rw-r--r--   0     1001      123     2399 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/伊朗足球.json
--rw-r--r--   0     1001      123     1615 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/佛教.json
--rw-r--r--   0     1001      123     3677 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/俄超.json
--rw-r--r--   0     1001      123    13456 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/俱乐部足球联赛.json
--rw-r--r--   0     1001      123    26449 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/列斯聯.json
--rw-r--r--   0     1001      123     2010 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/加超聯.json
--rw-r--r--   0     1001      123    11913 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/南美球會.json
--rw-r--r--   0     1001      123     1870 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/博弈论.json
--rw-r--r--   0     1001      123     2466 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/卡塔尔星级足球联赛.json
--rw-r--r--   0     1001      123     2990 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/叙利亚职业足球联赛.json
--rw-r--r--   0     1001      123     4356 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/名偵探柯南.json
--rw-r--r--   0     1001      123     7683 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/咕嚕咕嚕魔法陣.json
--rw-r--r--   0     1001      123     3368 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/咲-Saki-.json
--rw-r--r--   0     1001      123      413 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/單雙書名號轉換.json
--rw-r--r--   0     1001      123     8161 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/四驅兄弟.json
--rw-r--r--   0     1001      123     1765 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/圍棋.json
--rw-r--r--   0     1001      123    91171 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/地名.json
--rw-r--r--   0     1001      123    11946 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/声临其境.json
--rw-r--r--   0     1001      123    16032 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/妖怪手錶.json
--rw-r--r--   0     1001      123     4612 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/姓氏.json
--rw-r--r--   0     1001      123     1706 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/娛樂.json
--rw-r--r--   0     1001      123     6143 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/小魔女DoReMi.json
--rw-r--r--   0     1001      123     1049 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/巴勒斯坦职业足球联赛.json
--rw-r--r--   0     1001      123     3401 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/巴林职业足球联赛.json
--rw-r--r--   0     1001      123     7552 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/幸福爆發！光之美少女.json
--rw-r--r--   0     1001      123    18532 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/意甲.json
--rw-r--r--   0     1001      123     5596 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/愛天使傳說.json
--rw-r--r--   0     1001      123     8810 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/戰鬥陀螺 鋼鐵奇兵.json
--rw-r--r--   0     1001      123     5374 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/打工吧！魔王大人.json
--rw-r--r--   0     1001      123    12531 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/政治人物.json
--rw-r--r--   0     1001      123    24277 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/文學.json
--rw-r--r--   0     1001      123    21774 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/星光樂園.json
--rw-r--r--   0     1001      123     2086 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/暗影诗章 (动画).json
--rw-r--r--   0     1001      123     1937 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/村上春樹.json
--rw-r--r--   0     1001      123     2512 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/核能.json
--rw-r--r--   0     1001      123     7040 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/機獸系列.json
--rw-r--r--   0     1001      123      672 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/民族.json
--rw-r--r--   0     1001      123     7491 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/沙特职业足球联赛.json
--rw-r--r--   0     1001      123     2691 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/泰國人名.json
--rw-r--r--   0     1001      123     1917 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/涼宮春日的憂鬱.json
--rw-r--r--   0     1001      123     4807 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/潘朵拉之心.json
--rw-r--r--   0     1001      123     3560 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/烏茲別克足球會.json
--rw-r--r--   0     1001      123     7746 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/爆丸.json
--rw-r--r--   0     1001      123     1968 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/畜牧.json
--rw-r--r--   0     1001      123      476 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/當個創世神.json
--rw-r--r--   0     1001      123     4081 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/百變小櫻.json
--rw-r--r--   0     1001      123     1690 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/科威特职业足球联赛.json
--rw-r--r--   0     1001      123     4326 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/童話槍手小紅帽.json
--rw-r--r--   0     1001      123     1287 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/约旦职业足球联赛.json
--rw-r--r--   0     1001      123    50765 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/美国漫画.json
--rw-r--r--   0     1001      123      358 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/艾维里奥斯.json
--rw-r--r--   0     1001      123     4284 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/荷蘭足球聯賽.json
--rw-r--r--   0     1001      123     5889 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/菁英殺機.json
--rw-r--r--   0     1001      123     2402 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/葡超.json
--rw-r--r--   0     1001      123     4186 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/蠟筆小新.json
--rw-r--r--   0     1001      123      332 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/语言与语音.json
--rw-r--r--   0     1001      123     4180 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/通靈王.json
--rw-r--r--   0     1001      123    12331 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/進擊的巨人.json
--rw-r--r--   0     1001      123      964 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/釣魚臺列嶼.json
--rw-r--r--   0     1001      123    29385 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/閃電十一人.json
--rw-r--r--   0     1001      123     2453 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/闇.json
--rw-r--r--   0     1001      123      919 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/阿曼职业足球联赛.json
--rw-r--r--   0     1001      123     4315 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/阿联酋职业足球联赛.json
--rw-r--r--   0     1001      123     2845 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/降世神通.json
--rw-r--r--   0     1001      123     1889 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/音樂劇.json
--rw-r--r--   0     1001      123     5499 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/驅魔少年.json
--rw-r--r--   0     1001      123    14375 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/马来人名地名.json
--rw-r--r--   0     1001      123    16434 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/鬥陣特攻.json
--rw-r--r--   0     1001      123     5689 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/魔法咪路咪路.json
--rw-r--r--   0     1001      123     1103 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/黎巴嫩职业足球联赛.json
--rw-r--r--   0     1001      123    10818 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/黑執事.json
--rw-r--r--   0     1001      123     2840 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/黑塔系列.json
--rw-r--r--   0     1001      123     5472 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/poetry.lock
--rw-r--r--   0     1001      123      308 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/pyproject.toml
--rwxr-xr-x   0     1001      123     3645 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/update_basic.py
--rwxr-xr-x   0     1001      123    12250 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/data/update_cgroups.py
--rwxr-xr-x   0     1001      123      857 2023-07-04 16:29:49.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/run-maturin-action.sh
--rw-r--r--   0     1001      123    31484 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/src/converter.rs
--rw-r--r--   0     1001      123     4185 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/src/converters.rs
--rw-r--r--   0     1001      123    12566 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/src/lib.rs
--rw-r--r--   0     1001      123     2060 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/src/pagerules.rs
--rw-r--r--   0     1001      123    12791 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/src/rule.rs
--rw-r--r--   0     1001      123    10556 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/src/tables.rs
--rw-r--r--   0     1001      123     1246 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/src/utils.rs
--rw-r--r--   0     1001      123     8918 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/src/variant.rs
--rw-r--r--   0     1001      123     2880 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/src/wasm.rs
--rw-r--r--   0     1001      123      342 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/.gitignore
--rw-r--r--   0     1001      123     2113 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/README.md
--rw-r--r--   0     1001      123     5266 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/bench.tmp
--rw-r--r--   0     1001      123     1407 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/config-overrides.js
--rw-r--r--   0     1001      123     1350 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/package.json
--rw-r--r--   0     1001      123  3976144 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/public/cgroups.json
--rw-r--r--   0     1001      123     2159 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/public/index.html
--rw-r--r--   0     1001      123     3870 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/public/logo.ico
--rw-r--r--   0     1001      123     5347 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/public/logo192.png
--rw-r--r--   0     1001      123     9664 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/public/logo512.png
--rw-r--r--   0     1001      123      475 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/public/manifest.json
--rw-r--r--   0     1001      123       67 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/public/robots.txt
--rwxr-xr-x   0     1001      123    23159 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/rustup.sh
--rw-r--r--   0     1001      123      564 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/App.css
--rw-r--r--   0     1001      123      273 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/App.test.tsx
--rw-r--r--   0     1001      123     3332 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/App.tsx
--rw-r--r--   0     1001      123     4309 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/AboutDialog.tsx
--rw-r--r--   0     1001      123      882 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/CGroupCheckbox.tsx
--rw-r--r--   0     1001      123     6667 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/CGroupSelect.tsx
--rw-r--r--   0     1001      123     4808 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/ConvertButton.tsx
--rw-r--r--   0     1001      123     4230 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/Footer.tsx
--rw-r--r--   0     1001      123     3547 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/Header.tsx
--rw-r--r--   0     1001      123     2720 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/InputEditor.tsx
--rw-r--r--   0     1001      123     3874 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/OptionsControl.tsx
--rw-r--r--   0     1001      123      820 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/OutputEditor.tsx
--rw-r--r--   0     1001      123      552 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/OutputStatusLine.tsx
--rw-r--r--   0     1001      123      217 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/editorCommon.tsx
--rw-r--r--   0     1001      123      366 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/index.css
--rw-r--r--   0     1001      123      500 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/index.tsx
--rw-r--r--   0     1001      123     2632 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/logo.svg
--rw-r--r--   0     1001      123       40 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/react-app-env.d.ts
--rw-r--r--   0     1001      123      425 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/reportWebVitals.ts
--rw-r--r--   0     1001      123      241 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/setupTests.ts
--rw-r--r--   0     1001      123      150 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/utils.ts
--rw-r--r--   0     1001      123      535 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/tsconfig.json
--rw-r--r--   0     1001      123   539286 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/local_dependencies/zhconv/web/yarn.lock
--rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 zhconv_rs-0.3.0/Cargo.toml
--rw-r--r--   0     1001      123      685 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/.gitignore
--rw-r--r--   0     1001      123    10306 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/README.md
--rw-r--r--   0     1001      123      643 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/pyproject.toml
--rw-r--r--   0     1001      123     9265 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/src/lib.rs
--rw-r--r--   0     1001      123      995 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/zhconv_rs.pyi
--rw-r--r--   0     1001      123    26156 2023-07-04 16:29:12.000000 zhconv_rs-0.3.0/Cargo.lock
--rw-r--r--   0        0        0    11075 1970-01-01 00:00:00.000000 zhconv_rs-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1863 1970-01-01 00:00:00.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/Cargo.toml
+-rw-r--r--   0     1001      123      426 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/.gitattributes
+-rw-r--r--   0     1001      123     1775 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/.github/workflows/main.yml
+-rw-r--r--   0     1001      123     2445 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/.github/workflows/npm.yml
+-rw-r--r--   0     1001      123     1973 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/.github/workflows/pyo3.yml
+-rw-r--r--   0     1001      123     2703 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/.github/workflows/release.yml
+-rw-r--r--   0     1001      123       20 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/.gitignore
+-rw-r--r--   0     1001      123    35149 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/LICENSE
+-rw-r--r--   0     1001      123    10364 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/README.md
+-rw-r--r--   0     1001      123   284864 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/25328-0.txt
+-rw-r--r--   0     1001      123      198 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/LICENSE.md
+-rw-r--r--   0     1001      123  3261912 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/data3185k.txt
+-rw-r--r--   0     1001      123    55192 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/data54k.txt
+-rw-r--r--   0     1001      123   705845 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/data689k.txt
+-rw-r--r--   0     1001      123    79133 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/wikitext.txt
+-rw-r--r--   0     1001      123     5755 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/zhconv_benchmark.rs
+-rw-r--r--   0     1001      123    19923 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/build.rs
+-rw-r--r--   0     1001      123      532 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/HKVariants.txt
+-rw-r--r--   0     1001      123     2709 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/HKVariantsRevPhrases.txt
+-rw-r--r--   0     1001      123      870 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/README.md
+-rw-r--r--   0     1001      123    34353 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/STCharacters.txt
+-rw-r--r--   0     1001      123  1004153 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/STPhrases.txt
+-rw-r--r--   0     1001      123    34627 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TSCharacters.txt
+-rw-r--r--   0     1001      123     5161 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TSPhrases.txt
+-rw-r--r--   0     1001      123     7611 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TWPhrasesIT.txt
+-rw-r--r--   0     1001      123     2121 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TWPhrasesName.txt
+-rw-r--r--   0     1001      123      571 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TWPhrasesOther.txt
+-rw-r--r--   0     1001      123      312 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TWVariants.txt
+-rw-r--r--   0     1001      123     1075 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TWVariantsRevPhrases.txt
+-rw-r--r--   0     1001      123   447718 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/ZhConversion.php
+-rw-r--r--   0     1001      123     7470 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/1D.json
+-rw-r--r--   0     1001      123     4660 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2016年太平洋颱風季.json
+-rw-r--r--   0     1001      123     4462 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2017年太平洋颱風季.json
+-rw-r--r--   0     1001      123     4953 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2018年太平洋颱風季.json
+-rw-r--r--   0     1001      123     4967 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2019年太平洋颱風季.json
+-rw-r--r--   0     1001      123     4150 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2020年太平洋颱風季.json
+-rw-r--r--   0     1001      123     3977 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2021年太平洋颱風季.json
+-rw-r--r--   0     1001      123     4396 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2022年太平洋颱風季.json
+-rw-r--r--   0     1001      123      311 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2023年太平洋颱風季.json
+-rw-r--r--   0     1001      123    18639 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/24.json
+-rw-r--r--   0     1001      123     1347 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/A Pink.json
+-rw-r--r--   0     1001      123     1436 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/A Song of Ice and Fire.json
+-rw-r--r--   0     1001      123     4784 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ACmilan.json
+-rw-r--r--   0     1001      123     4078 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ALeague.json
+-rw-r--r--   0     1001      123    12349 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/AT Places.json
+-rw-r--r--   0     1001      123    12270 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/AU Places.json
+-rw-r--r--   0     1001      123     2618 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Adventure Time.json
+-rw-r--r--   0     1001      123    24747 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Aero.json
+-rw-r--r--   0     1001      123     4785 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Aikatsu.json
+-rw-r--r--   0     1001      123    44770 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Anime.json
+-rw-r--r--   0     1001      123    11339 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Apple.json
+-rw-r--r--   0     1001      123     6426 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Aquatics.json
+-rw-r--r--   0     1001      123     3127 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Ariana Grande.json
+-rw-r--r--   0     1001      123      682 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Artist.json
+-rw-r--r--   0     1001      123    11447 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Astronomy.json
+-rw-r--r--   0     1001      123     4837 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Avatar.json
+-rw-r--r--   0     1001      123     3325 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Avril Lavigne.json
+-rw-r--r--   0     1001      123    46163 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/BE Places.json
+-rw-r--r--   0     1001      123    11395 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/BUDDYCOMPLEX.json
+-rw-r--r--   0     1001      123    10696 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Badminton.json
+-rw-r--r--   0     1001      123     2277 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Bakuman.json
+-rw-r--r--   0     1001      123     1911 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Battle Spirits.json
+-rw-r--r--   0     1001      123   108138 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Bird.json
+-rw-r--r--   0     1001      123   891099 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/BirdG.json
+-rw-r--r--   0     1001      123   528555 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/BirdP.json
+-rw-r--r--   0     1001      123     3893 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Black Mirror.json
+-rw-r--r--   0     1001      123     3895 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Bridge.json
+-rw-r--r--   0     1001      123     7962 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Britney Spears.json
+-rw-r--r--   0     1001      123     7729 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Bundesliga.json
+-rw-r--r--   0     1001      123    66546 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Butterfly.json
+-rw-r--r--   0     1001      123     3715 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/C&C.json
+-rw-r--r--   0     1001      123    17645 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/CA Places.json
+-rw-r--r--   0     1001      123     2454 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/CANAAN.json
+-rw-r--r--   0     1001      123    33866 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/CH Places.json
+-rw-r--r--   0     1001      123    13534 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/COD.json
+-rw-r--r--   0     1001      123     9143 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/CWBTyphoonOld.json
+-rw-r--r--   0     1001      123     6467 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Canada.json
+-rw-r--r--   0     1001      123     4462 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Carnivorous Plant.json
+-rw-r--r--   0     1001      123    10024 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Cartoon.json
+-rw-r--r--   0     1001      123      883 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Chanel.json
+-rw-r--r--   0     1001      123    18060 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Chemistry.json
+-rw-r--r--   0     1001      123     5155 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Code Black.json
+-rw-r--r--   0     1001      123     7909 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Code Geass.json
+-rw-r--r--   0     1001      123     2053 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/CodeLyoko.json
+-rw-r--r--   0     1001      123     3078 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Coldplay.json
+-rw-r--r--   0     1001      123    11955 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Communication.json
+-rw-r--r--   0     1001      123     5620 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Composer.json
+-rw-r--r--   0     1001      123     4654 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Copyright.json
+-rw-r--r--   0     1001      123    92366 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Counter-Strike.json
+-rw-r--r--   0     1001      123      294 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/County.json
+-rw-r--r--   0     1001      123    17698 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Crazyracing Kartrider.json
+-rw-r--r--   0     1001      123     3200 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Cyber Formula.json
+-rw-r--r--   0     1001      123     6089 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Cyclone.json
+-rw-r--r--   0     1001      123     1381 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/DCComics.json
+-rw-r--r--   0     1001      123   103362 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/DE Places.json
+-rw-r--r--   0     1001      123    10853 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Danball Senki.json
+-rw-r--r--   0     1001      123     1129 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Dance.json
+-rw-r--r--   0     1001      123     1629 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Death Note.json
+-rw-r--r--   0     1001      123     6663 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Diablo.json
+-rw-r--r--   0     1001      123      783 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Die Weiße Rose.json
+-rw-r--r--   0     1001      123    17587 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Digimon.json
+-rw-r--r--   0     1001      123    33790 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Disney.json
+-rw-r--r--   0     1001      123     3249 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Doctor Who.json
+-rw-r--r--   0     1001      123     7180 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Doraemon.json
+-rw-r--r--   0     1001      123    15722 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/DragonBall.json
+-rw-r--r--   0     1001      123    28035 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/DreamWorks.json
+-rw-r--r--   0     1001      123     5595 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ED.json
+-rw-r--r--   0     1001      123    23292 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/EPL.json
+-rw-r--r--   0     1001      123     6196 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/EU.json
+-rw-r--r--   0     1001      123    10152 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Earthquake.json
+-rw-r--r--   0     1001      123    34462 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Ecology.json
+-rw-r--r--   0     1001      123    25054 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Economics.json
+-rw-r--r--   0     1001      123    16745 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Electronics.json
+-rw-r--r--   0     1001      123     1949 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Esports.json
+-rw-r--r--   0     1001      123     5832 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Eyeshield21.json
+-rw-r--r--   0     1001      123    16682 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/F1.json
+-rw-r--r--   0     1001      123    12291 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/FAcup.json
+-rw-r--r--   0     1001      123   112357 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/FR Places.json
+-rw-r--r--   0     1001      123     5415 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Family Guy.json
+-rw-r--r--   0     1001      123    38198 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Firearms.json
+-rw-r--r--   0     1001      123    26299 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Food.json
+-rw-r--r--   0     1001      123    23933 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Football.json
+-rw-r--r--   0     1001      123     1431 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Friends.json
+-rw-r--r--   0     1001      123     2301 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Fringe.json
+-rw-r--r--   0     1001      123     5440 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Frozen.json
+-rw-r--r--   0     1001      123    16568 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/FullmetalAlchemist.json
+-rw-r--r--   0     1001      123     3114 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Futurama.json
+-rw-r--r--   0     1001      123    30810 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GBF.json
+-rw-r--r--   0     1001      123     6024 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GGundam.json
+-rw-r--r--   0     1001      123     5068 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GOSICK.json
+-rw-r--r--   0     1001      123     5201 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GZFC.json
+-rw-r--r--   0     1001      123     6847 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Games-zh.json
+-rw-r--r--   0     1001      123    75060 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Games.json
+-rw-r--r--   0     1001      123     2196 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GaoGaiGar.json
+-rw-r--r--   0     1001      123     1586 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Geography.json
+-rw-r--r--   0     1001      123     2860 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Getter Robo.json
+-rw-r--r--   0     1001      123     6273 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Ghibli.json
+-rw-r--r--   0     1001      123     7545 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Glee.json
+-rw-r--r--   0     1001      123     5456 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GossipGirl.json
+-rw-r--r--   0     1001      123     5846 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Guardians of Ga'Hoole.json
+-rw-r--r--   0     1001      123    28072 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Gundam00.json
+-rw-r--r--   0     1001      123    21085 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamAGE.json
+-rw-r--r--   0     1001      123    32810 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamIBO.json
+-rw-r--r--   0     1001      123    37988 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamSeed.json
+-rw-r--r--   0     1001      123    12889 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamTWFM.json
+-rw-r--r--   0     1001      123    72213 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamUC.json
+-rw-r--r--   0     1001      123     7502 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamW.json
+-rw-r--r--   0     1001      123     7651 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/HTGAWM.json
+-rw-r--r--   0     1001      123    14605 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/HUNTER.json
+-rw-r--r--   0     1001      123     6381 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Half-Life.json
+-rw-r--r--   0     1001      123     1213 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Hannibal Lecter.json
+-rw-r--r--   0     1001      123    69432 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/HarryPotter.json
+-rw-r--r--   0     1001      123      771 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Hawaii Five-0.json
+-rw-r--r--   0     1001      123     4149 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Hayate the Combat Butler.json
+-rw-r--r--   0     1001      123    10198 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Heroes of the Storm.json
+-rw-r--r--   0     1001      123    12525 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/House.json
+-rw-r--r--   0     1001      123     1670 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/IMF.json
+-rw-r--r--   0     1001      123   186279 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/IT.json
+-rw-r--r--   0     1001      123     2734 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/JLeague.json
+-rw-r--r--   0     1001      123   214806 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/JP Show.json
+-rw-r--r--   0     1001      123    12353 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/James Bond.json
+-rw-r--r--   0     1001      123    14545 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Jewelpet.json
+-rw-r--r--   0     1001      123     1814 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Justin Bieber.json
+-rw-r--r--   0     1001      123     6140 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/KLeague.json
+-rw-r--r--   0     1001      123    71612 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/KO Movie.json
+-rw-r--r--   0     1001      123    31224 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/KO Show.json
+-rw-r--r--   0     1001      123   124806 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/KO TV Show.json
+-rw-r--r--   0     1001      123    30116 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/KamenRider.json
+-rw-r--r--   0     1001      123     3400 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Kao.json
+-rw-r--r--   0     1001      123     1214 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Katy Perry.json
+-rw-r--r--   0     1001      123     1403 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Korea Comparison.json
+-rw-r--r--   0     1001      123    27780 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Korea.json
+-rw-r--r--   0     1001      123      563 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Korean.json
+-rw-r--r--   0     1001      123     1494 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LEGO.json
+-rw-r--r--   0     1001      123    20622 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LOL.json
+-rw-r--r--   0     1001      123     5749 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LR.json
+-rw-r--r--   0     1001      123     7789 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/La casa de papel.json
+-rw-r--r--   0     1001      123     2998 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Lady Gaga.json
+-rw-r--r--   0     1001      123     5497 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Lana Del Rey.json
+-rw-r--r--   0     1001      123     2009 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Laos.json
+-rw-r--r--   0     1001      123     1545 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Legend of the Guardians.json
+-rw-r--r--   0     1001      123     2412 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Les Misérables.json
+-rw-r--r--   0     1001      123    64760 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Lifesciences.json
+-rw-r--r--   0     1001      123      200 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Linguistics.json
+-rw-r--r--   0     1001      123     3038 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Linkin.json
+-rw-r--r--   0     1001      123     2381 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Lorde.json
+-rw-r--r--   0     1001      123    96457 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LuaIT.json
+-rw-r--r--   0     1001      123   242697 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LuaMovie.json
+-rw-r--r--   0     1001      123   113609 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LuaShow.json
+-rw-r--r--   0     1001      123    14349 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MA.json
+-rw-r--r--   0     1001      123     5674 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MCD.json
+-rw-r--r--   0     1001      123     7228 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MCFC.json
+-rw-r--r--   0     1001      123     3350 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MLS.json
+-rw-r--r--   0     1001      123    14999 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MUFC.json
+-rw-r--r--   0     1001      123    14862 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MY.json
+-rw-r--r--   0     1001      123    17706 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Mabinogi.json
+-rw-r--r--   0     1001      123    14833 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MapleStory.json
+-rw-r--r--   0     1001      123      946 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Mariah Carey.json
+-rw-r--r--   0     1001      123      215 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MarvelNetflix.json
+-rw-r--r--   0     1001      123    34592 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Math.json
+-rw-r--r--   0     1001      123    11580 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Mazinger.json
+-rw-r--r--   0     1001      123     5877 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/McDonald's.json
+-rw-r--r--   0     1001      123    16322 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MediaWiki special.json
+-rw-r--r--   0     1001      123    11410 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MediaWiki.json
+-rw-r--r--   0     1001      123    19988 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Medicine.json
+-rw-r--r--   0     1001      123     1285 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Michael Jackson.json
+-rw-r--r--   0     1001      123      183 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MigTest.json
+-rw-r--r--   0     1001      123     3043 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Might&Magic.json
+-rw-r--r--   0     1001      123    44509 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Military.json
+-rw-r--r--   0     1001      123     7029 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Minecraft.json
+-rw-r--r--   0     1001      123   442700 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Movie.json
+-rw-r--r--   0     1001      123    28123 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Music.json
+-rw-r--r--   0     1001      123    44930 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/My Little Pony.json
+-rw-r--r--   0     1001      123     8118 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MyHeroAcademia.json
+-rw-r--r--   0     1001      123    14670 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/NARUTO.json
+-rw-r--r--   0     1001      123    77638 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/NBA.json
+-rw-r--r--   0     1001      123     5860 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/NFL.json
+-rw-r--r--   0     1001      123     1095 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/NHL.json
+-rw-r--r--   0     1001      123    12730 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Nintendo.json
+-rw-r--r--   0     1001      123     7719 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Nobel Prize.json
+-rw-r--r--   0     1001      123    37371 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/OnePiece.json
+-rw-r--r--   0     1001      123    10030 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Organization.json
+-rw-r--r--   0     1001      123     4166 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Overwatch.json
+-rw-r--r--   0     1001      123     3308 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/P&G.json
+-rw-r--r--   0     1001      123     2081 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PHL Places.json
+-rw-r--r--   0     1001      123    94006 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/People.json
+-rw-r--r--   0     1001      123     3404 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PeppaPig.json
+-rw-r--r--   0     1001      123     2479 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Percy Jackson.json
+-rw-r--r--   0     1001      123     3168 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PerryClass.json
+-rw-r--r--   0     1001      123     6642 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pesticide.json
+-rw-r--r--   0     1001      123     2918 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Photography.json
+-rw-r--r--   0     1001      123    28389 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Physics.json
+-rw-r--r--   0     1001      123     4149 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pichi Pichi Pitch.json
+-rw-r--r--   0     1001      123      966 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pinnacle Islands.json
+-rw-r--r--   0     1001      123    34697 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pixar.json
+-rw-r--r--   0     1001      123    20027 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pokemon-old.json
+-rw-r--r--   0     1001      123    20296 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pokemon.json
+-rw-r--r--   0     1001      123    67585 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PoliticiansUK.json
+-rw-r--r--   0     1001      123     8551 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Popes.json
+-rw-r--r--   0     1001      123     3495 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Power Rangers.json
+-rw-r--r--   0     1001      123    31357 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PresidentsUS.json
+-rw-r--r--   0     1001      123    11576 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pretty Rhythm.json
+-rw-r--r--   0     1001      123     5719 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PrisonBreak.json
+-rw-r--r--   0     1001      123    17999 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Psychology.json
+-rw-r--r--   0     1001      123    49490 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Racing.json
+-rw-r--r--   0     1001      123    37973 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Railway.json
+-rw-r--r--   0     1001      123     2496 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/RainbowSixSiege.json
+-rw-r--r--   0     1001      123    11105 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Reborn.json
+-rw-r--r--   0     1001      123     6151 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ResidentEvil.json
+-rw-r--r--   0     1001      123     3555 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Rihanna.json
+-rw-r--r--   0     1001      123    35731 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SAO.json
+-rw-r--r--   0     1001      123     1842 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SARS-CoV-2 variant.json
+-rw-r--r--   0     1001      123     5934 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SEGA.json
+-rw-r--r--   0     1001      123     4084 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SNSD.json
+-rw-r--r--   0     1001      123     2282 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SPL.json
+-rw-r--r--   0     1001      123     1598 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SPY×FAMILY.json
+-rw-r--r--   0     1001      123     3803 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Sailor Moon.json
+-rw-r--r--   0     1001      123     9438 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SaintSeiyaOmega.json
+-rw-r--r--   0     1001      123    74396 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Sandbox.json
+-rw-r--r--   0     1001      123     1837 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Selena Gomez.json
+-rw-r--r--   0     1001      123    24202 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Shinkalion.json
+-rw-r--r--   0     1001      123     8677 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Shipname.json
+-rw-r--r--   0     1001      123   270643 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Show.json
+-rw-r--r--   0     1001      123     3132 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Shugo Chara!.json
+-rw-r--r--   0     1001      123     2253 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Sia.json
+-rw-r--r--   0     1001      123     2266 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Signals and Systems.json
+-rw-r--r--   0     1001      123      372 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Signpost.json
+-rw-r--r--   0     1001      123    11351 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Sim.json
+-rw-r--r--   0     1001      123    20778 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Simpsons.json
+-rw-r--r--   0     1001      123    10767 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Snooker.json
+-rw-r--r--   0     1001      123     2588 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SouthPark.json
+-rw-r--r--   0     1001      123     9718 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SpongeBob SquarePants.json
+-rw-r--r--   0     1001      123    10794 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Sports.json
+-rw-r--r--   0     1001      123    17092 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Square Enix.json
+-rw-r--r--   0     1001      123     7526 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/StarCraft.json
+-rw-r--r--   0     1001      123    11391 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/StarCraft2.json
+-rw-r--r--   0     1001      123    27435 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/StarTrek.json
+-rw-r--r--   0     1001      123    12653 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/StarWars.json
+-rw-r--r--   0     1001      123     6942 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/StephenKing.json
+-rw-r--r--   0     1001      123      549 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Summon Night.json
+-rw-r--r--   0     1001      123     1674 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TCM.json
+-rw-r--r--   0     1001      123      275 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TLeague.json
+-rw-r--r--   0     1001      123   105974 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TV.json
+-rw-r--r--   0     1001      123     5543 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Table Tennis.json
+-rw-r--r--   0     1001      123     3650 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Tales.json
+-rw-r--r--   0     1001      123     5286 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Tamagotchi.json
+-rw-r--r--   0     1001      123    11981 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Taylor Swift.json
+-rw-r--r--   0     1001      123     2419 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Telcom.json
+-rw-r--r--   0     1001      123    71368 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Tennis.json
+-rw-r--r--   0     1001      123      115 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TfL.json
+-rw-r--r--   0     1001      123      521 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/The Chainsmokers.json
+-rw-r--r--   0     1001      123    12593 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/The Witcher.json
+-rw-r--r--   0     1001      123     4828 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/The World God Only Knows.json
+-rw-r--r--   0     1001      123     3120 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TheBeatles.json
+-rw-r--r--   0     1001      123     2346 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ThePeanuts.json
+-rw-r--r--   0     1001      123     3570 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Toaru.json
+-rw-r--r--   0     1001      123    24126 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Transformers.json
+-rw-r--r--   0     1001      123     4352 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Transport for London.json
+-rw-r--r--   0     1001      123    44492 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Transport.json
+-rw-r--r--   0     1001      123    35103 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TropicalCycloneName.json
+-rw-r--r--   0     1001      123     3253 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Twilight.json
+-rw-r--r--   0     1001      123     6974 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TyphoonNew.json
+-rw-r--r--   0     1001      123    25610 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TyphoonOld.json
+-rw-r--r--   0     1001      123     4728 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/UA toponyms.json
+-rw-r--r--   0     1001      123    42557 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/UK Places.json
+-rw-r--r--   0     1001      123     3707 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/US CA Cities.json
+-rw-r--r--   0     1001      123     5434 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/US Government.json
+-rw-r--r--   0     1001      123      584 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/US Senators.json
+-rw-r--r--   0     1001      123    27748 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/USState.json
+-rw-r--r--   0     1001      123    22229 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Ultraman.json
+-rw-r--r--   0     1001      123     1791 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Unilever.json
+-rw-r--r--   0     1001      123     7171 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Unit.json
+-rw-r--r--   0     1001      123     6267 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Urban.json
+-rw-r--r--   0     1001      123      802 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/VLeague.json
+-rw-r--r--   0     1001      123     2372 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Valkyria.json
+-rw-r--r--   0     1001      123     1272 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/WORKING!!.json
+-rw-r--r--   0     1001      123    18912 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Warcraft.json
+-rw-r--r--   0     1001      123     1024 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Warhammer.json
+-rw-r--r--   0     1001      123    11262 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Warriors.json
+-rw-r--r--   0     1001      123     1547 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Watch.json
+-rw-r--r--   0     1001      123     5103 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Weather.json
+-rw-r--r--   0     1001      123    14791 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Windows.json
+-rw-r--r--   0     1001      123    26033 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Wow.json
+-rw-r--r--   0     1001      123     8357 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Yes! 光之美少女5.json
+-rw-r--r--   0     1001      123    63286 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ZH Show.json
+-rw-r--r--   0     1001      123     9963 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/arsenal.json
+-rwxr-xr-x   0     1001      123     1629 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/check1.py
+-rw-r--r--   0     1001      123    14239 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/chelsea.json
+-rw-r--r--   0     1001      123     8008 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/fcbarcelona.json
+-rw-r--r--   0     1001      123    34236 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/fcbayern.json
+-rw-r--r--   0     1001      123     4414 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/free license.json
+-rw-r--r--   0     1001      123     1071 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/inter.json
+-rw-r--r--   0     1001      123    25910 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/laliga.json
+-rw-r--r--   0     1001      123     4300 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/leek.json
+-rw-r--r--   0     1001      123     4246 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ligue.json
+-rw-r--r--   0     1001      123    24883 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/liverpoolfc.json
+-rw-r--r--   0     1001      123     8135 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/loghorizon.json
+-rw-r--r--   0     1001      123    17062 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/magi.json
+-rwxr-xr-x   0     1001      123     1497 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/merge_for_web.py
+-rw-r--r--   0     1001      123    27273 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/neo-noir.json
+-rw-r--r--   0     1001      123     4240 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/regalia.json
+-rw-r--r--   0     1001      123     3967 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/specialpages.json
+-rw-r--r--   0     1001      123    39998 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/uefa.json
+-rw-r--r--   0     1001      123     8235 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/vital.json
+-rw-r--r--   0     1001      123    13742 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/一拳超人.json
+-rw-r--r--   0     1001      123     1103 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/伊拉克足球.json
+-rw-r--r--   0     1001      123     2735 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/伊斯蘭.json
+-rw-r--r--   0     1001      123     2399 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/伊朗足球.json
+-rw-r--r--   0     1001      123     1615 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/佛教.json
+-rw-r--r--   0     1001      123     3677 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/俄超.json
+-rw-r--r--   0     1001      123    13456 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/俱乐部足球联赛.json
+-rw-r--r--   0     1001      123    26449 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/列斯聯.json
+-rw-r--r--   0     1001      123     2010 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/加超聯.json
+-rw-r--r--   0     1001      123    11913 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/南美球會.json
+-rw-r--r--   0     1001      123     1870 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/博弈论.json
+-rw-r--r--   0     1001      123     2466 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/卡塔尔星级足球联赛.json
+-rw-r--r--   0     1001      123     2990 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/叙利亚职业足球联赛.json
+-rw-r--r--   0     1001      123     4356 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/名偵探柯南.json
+-rw-r--r--   0     1001      123     7683 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/咕嚕咕嚕魔法陣.json
+-rw-r--r--   0     1001      123     3368 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/咲-Saki-.json
+-rw-r--r--   0     1001      123      413 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/單雙書名號轉換.json
+-rw-r--r--   0     1001      123     8161 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/四驅兄弟.json
+-rw-r--r--   0     1001      123     1765 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/圍棋.json
+-rw-r--r--   0     1001      123    91171 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/地名.json
+-rw-r--r--   0     1001      123    11946 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/声临其境.json
+-rw-r--r--   0     1001      123    16032 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/妖怪手錶.json
+-rw-r--r--   0     1001      123     4612 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/姓氏.json
+-rw-r--r--   0     1001      123     1706 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/娛樂.json
+-rw-r--r--   0     1001      123     6143 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/小魔女DoReMi.json
+-rw-r--r--   0     1001      123     1049 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/巴勒斯坦职业足球联赛.json
+-rw-r--r--   0     1001      123     3401 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/巴林职业足球联赛.json
+-rw-r--r--   0     1001      123     7552 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/幸福爆發！光之美少女.json
+-rw-r--r--   0     1001      123    18532 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/意甲.json
+-rw-r--r--   0     1001      123     5596 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/愛天使傳說.json
+-rw-r--r--   0     1001      123     8810 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/戰鬥陀螺 鋼鐵奇兵.json
+-rw-r--r--   0     1001      123     5374 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/打工吧！魔王大人.json
+-rw-r--r--   0     1001      123    12531 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/政治人物.json
+-rw-r--r--   0     1001      123    24277 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/文學.json
+-rw-r--r--   0     1001      123    21774 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/星光樂園.json
+-rw-r--r--   0     1001      123     2086 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/暗影诗章 (动画).json
+-rw-r--r--   0     1001      123     1937 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/村上春樹.json
+-rw-r--r--   0     1001      123     2512 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/核能.json
+-rw-r--r--   0     1001      123     7040 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/機獸系列.json
+-rw-r--r--   0     1001      123      672 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/民族.json
+-rw-r--r--   0     1001      123     7491 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/沙特职业足球联赛.json
+-rw-r--r--   0     1001      123     2691 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/泰國人名.json
+-rw-r--r--   0     1001      123     1917 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/涼宮春日的憂鬱.json
+-rw-r--r--   0     1001      123     4807 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/潘朵拉之心.json
+-rw-r--r--   0     1001      123     3560 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/烏茲別克足球會.json
+-rw-r--r--   0     1001      123     7746 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/爆丸.json
+-rw-r--r--   0     1001      123     1968 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/畜牧.json
+-rw-r--r--   0     1001      123      476 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/當個創世神.json
+-rw-r--r--   0     1001      123     4081 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/百變小櫻.json
+-rw-r--r--   0     1001      123     1690 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/科威特职业足球联赛.json
+-rw-r--r--   0     1001      123     4326 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/童話槍手小紅帽.json
+-rw-r--r--   0     1001      123     1287 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/约旦职业足球联赛.json
+-rw-r--r--   0     1001      123    50765 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/美国漫画.json
+-rw-r--r--   0     1001      123      358 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/艾维里奥斯.json
+-rw-r--r--   0     1001      123     4284 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/荷蘭足球聯賽.json
+-rw-r--r--   0     1001      123     5889 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/菁英殺機.json
+-rw-r--r--   0     1001      123     2402 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/葡超.json
+-rw-r--r--   0     1001      123     4186 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/蠟筆小新.json
+-rw-r--r--   0     1001      123      332 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/语言与语音.json
+-rw-r--r--   0     1001      123     4180 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/通靈王.json
+-rw-r--r--   0     1001      123    12331 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/進擊的巨人.json
+-rw-r--r--   0     1001      123      964 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/釣魚臺列嶼.json
+-rw-r--r--   0     1001      123    29385 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/閃電十一人.json
+-rw-r--r--   0     1001      123     2453 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/闇.json
+-rw-r--r--   0     1001      123      919 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/阿曼职业足球联赛.json
+-rw-r--r--   0     1001      123     4315 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/阿联酋职业足球联赛.json
+-rw-r--r--   0     1001      123     2845 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/降世神通.json
+-rw-r--r--   0     1001      123     1889 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/音樂劇.json
+-rw-r--r--   0     1001      123     5499 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/驅魔少年.json
+-rw-r--r--   0     1001      123    14375 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/马来人名地名.json
+-rw-r--r--   0     1001      123    16434 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/鬥陣特攻.json
+-rw-r--r--   0     1001      123     5689 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/魔法咪路咪路.json
+-rw-r--r--   0     1001      123     1103 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/黎巴嫩职业足球联赛.json
+-rw-r--r--   0     1001      123    10818 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/黑執事.json
+-rw-r--r--   0     1001      123     2840 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/黑塔系列.json
+-rw-r--r--   0     1001      123     5472 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/poetry.lock
+-rw-r--r--   0     1001      123      308 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/pyproject.toml
+-rwxr-xr-x   0     1001      123     3645 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/update_basic.py
+-rwxr-xr-x   0     1001      123    12250 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/update_cgroups.py
+-rwxr-xr-x   0     1001      123      857 2023-06-27 06:57:43.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/run-maturin-action.sh
+-rw-r--r--   0     1001      123    30931 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/converter.rs
+-rw-r--r--   0     1001      123     4198 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/converters.rs
+-rw-r--r--   0     1001      123     9591 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/lib.rs
+-rw-r--r--   0     1001      123     2060 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/pagerules.rs
+-rw-r--r--   0     1001      123    12790 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/rule.rs
+-rw-r--r--   0     1001      123    10529 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/tables.rs
+-rw-r--r--   0     1001      123     1217 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/utils.rs
+-rw-r--r--   0     1001      123     8918 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/variant.rs
+-rw-r--r--   0     1001      123     2880 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/wasm.rs
+-rw-r--r--   0     1001      123      342 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/.gitignore
+-rw-r--r--   0     1001      123     2113 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/README.md
+-rw-r--r--   0     1001      123     5266 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/bench.tmp
+-rw-r--r--   0     1001      123     1407 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/config-overrides.js
+-rw-r--r--   0     1001      123     1350 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/package.json
+-rw-r--r--   0     1001      123  3976144 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/cgroups.json
+-rw-r--r--   0     1001      123     2159 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/index.html
+-rw-r--r--   0     1001      123     3870 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/logo.ico
+-rw-r--r--   0     1001      123     5347 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/logo192.png
+-rw-r--r--   0     1001      123     9664 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/logo512.png
+-rw-r--r--   0     1001      123      475 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/manifest.json
+-rw-r--r--   0     1001      123       67 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/robots.txt
+-rwxr-xr-x   0     1001      123    23159 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/rustup.sh
+-rw-r--r--   0     1001      123      564 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/App.css
+-rw-r--r--   0     1001      123      273 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/App.test.tsx
+-rw-r--r--   0     1001      123     3332 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/App.tsx
+-rw-r--r--   0     1001      123     4309 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/AboutDialog.tsx
+-rw-r--r--   0     1001      123      882 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/CGroupCheckbox.tsx
+-rw-r--r--   0     1001      123     6667 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/CGroupSelect.tsx
+-rw-r--r--   0     1001      123     4808 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/ConvertButton.tsx
+-rw-r--r--   0     1001      123     4230 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/Footer.tsx
+-rw-r--r--   0     1001      123     3547 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/Header.tsx
+-rw-r--r--   0     1001      123     2720 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/InputEditor.tsx
+-rw-r--r--   0     1001      123     3874 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/OptionsControl.tsx
+-rw-r--r--   0     1001      123      820 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/OutputEditor.tsx
+-rw-r--r--   0     1001      123      552 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/OutputStatusLine.tsx
+-rw-r--r--   0     1001      123      217 2023-06-27 06:57:10.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/editorCommon.tsx
+-rw-r--r--   0     1001      123      366 2023-06-27 06:57:10.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/index.css
+-rw-r--r--   0     1001      123      500 2023-06-27 06:57:10.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/index.tsx
+-rw-r--r--   0     1001      123     2632 2023-06-27 06:57:10.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/logo.svg
+-rw-r--r--   0     1001      123       40 2023-06-27 06:57:10.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/react-app-env.d.ts
+-rw-r--r--   0     1001      123      425 2023-06-27 06:57:10.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/reportWebVitals.ts
+-rw-r--r--   0     1001      123      241 2023-06-27 06:57:10.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/setupTests.ts
+-rw-r--r--   0     1001      123      150 2023-06-27 06:57:10.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/utils.ts
+-rw-r--r--   0     1001      123      535 2023-06-27 06:57:10.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/tsconfig.json
+-rw-r--r--   0     1001      123   539286 2023-06-27 06:57:10.000000 zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/yarn.lock
+-rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 zhconv_rs-0.3.0b0/Cargo.toml
+-rw-r--r--   0     1001      123      685 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/.gitignore
+-rw-r--r--   0     1001      123    10364 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/README.md
+-rw-r--r--   0     1001      123      643 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/pyproject.toml
+-rw-r--r--   0     1001      123     5065 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/src/lib.rs
+-rw-r--r--   0     1001      123      758 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/zhconv_rs.pyi
+-rw-r--r--   0     1001      123    23998 2023-06-27 06:57:09.000000 zhconv_rs-0.3.0b0/Cargo.lock
+-rw-r--r--   0        0        0    11135 1970-01-01 00:00:00.000000 zhconv_rs-0.3.0b0/PKG-INFO
```

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/Cargo.toml` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,53 +2,55 @@
 authors = ["Hung-I Wang <whygowe@gmail.com>"]
 categories = ["text-processing", "localization", "value-formatting", "wasm"]
 description = "Traditional/Simplified and regional Chinese variants converter based on MediaWiki & OpenCC rulesets and powered by AC automata  轉換简体、繁體及兩岸、新馬中文地區詞，基於MediaWiki和OpenCC之字詞轉換表"
 edition = "2021"
 license = "GPL-2.0-or-later"
 name = "zhconv"
 repository = "https://github.com/Gowee/zhconv-rs"
-version = "0.3.0"
+version = "0.3.0-beta"
 
 [lib]
 crate-type = ["cdylib", "rlib"]
 
 [features]
 # OpenCC rulesets are activated by default.
 # Disabling the feature would boost performance further at the cost of less accuracy.
+compress = []
 default = ["opencc", "compress"]
-opencc = ["lazy_static"]
-compress = ["zstd", "ruzstd"]
+opencc = ["aho-corasick", "lazy_static"]
 
 [dependencies]
 daachorse = "1.0"
 itertools = "0.10"
-lazy_static = "1.4" # TODO: switch to once_cell
+lazy_static = "1.4"
 once_cell = "1.8"
 regex = "1.5"
-ruzstd = { version = "0.4", optional = true }
-strum = { version = "0.24", features = ["derive"] }
+ruzstd = {version = "0.4"}
+strum = {version = "0.24", features = ["derive"]}
 
 [target.'cfg(target_arch = "wasm32")'.dependencies]
 wasm-bindgen = "0.2"
 
 # The `console_error_panic_hook` crate provides better debugging of panics by
 # logging them with `console.error`. This is great for development, but requires
 # all the `std::fmt` and `std::panicking` infrastructure, so isn't great for
 # code size when deploying.
 console_error_panic_hook = {version = "0.1"}#, default-features = true, optional = true}
 
 [build-dependencies]
+aho-corasick = {version = "1.0", optional = true}
 daachorse = "1.0"
 hex-literal = "0.4"
 itertools = "0.10"
-lazy_static = { version = "1.4", optional = true }
+lazy_static = {version = "1.4", optional = true}
+lz4_flex = "0.10"
 once_cell = "1.8"
 regex = "1.5"
 sha2 = "0.10"
-vergen = { version = "8.2", features = ["build", "git", "gitcl"] }
-zstd = { version = "0.12", optional = true }
+vergen = {version = "8.2", features = ["build", "git", "gitcl"]}
+zstd = "0.12"
 
 [[bench]]
 harness = false
 name = "zhconv_benchmark"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/.github/workflows/main.yml` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/.github/workflows/npm.yml` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/.github/workflows/npm.yml`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/.github/workflows/pyo3.yml` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/.github/workflows/pyo3.yml`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/.github/workflows/release.yml` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/LICENSE` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/LICENSE`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/README.md` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 [![docs.rs](https://docs.rs/zhconv/badge.svg)](https://docs.rs/zhconv)
 [![Crates.io](https://img.shields.io/crates/v/zhconv.svg)](https://crates.io/crates/zhconv)
 [![PyPI version](https://img.shields.io/pypi/v/zhconv-rs)](https://pypi.org/project/zhconv-rs/)
 [![NPM version](https://badge.fury.io/js/zhconv.svg)](https://www.npmjs.com/package/zhconv)
 # zhconv-rs 中文简繁及地區詞轉換
 zhconv-rs converts Chinese text among traditional/simplified scripts or regional variants (e.g. `zh-TW <-> zh-CN <-> zh-HK <-> zh-Hans <-> zh-Hant`), built on the top of rulesets from MediaWiki/Wikipedia and OpenCC.
 
-The implementation is powered by an [Aho-Corasick](https://github.com/daac-tools/daachorse) automaton, ensuring linear time complexity with respect to the length of input text and conversion rules (`O(n+m)`), processing dozens of MiBs text per second.
+The implementation is powered by the [Aho-Corasick](https://github.com/BurntSushi/aho-corasick) automaton, ensuring linear time complexity with respect to the length of input text and conversion rules (`O(n+m)`), processing dozens of MiBs text per second.
 
 🔗 **Web App: https://zhconv.pages.dev** (powered by WASM)
 
 ⚙️ **Cli**: `cargo install zhconv-cli` or check [releases](https://github.com/Gowee/zhconv-rs/releases).
 
-🦀 **Rust Crate**: `cargo add zhconv` (check [docs](https://docs.rs/zhconv/latest/zhconv/) for examples)
+🦀 **Rust Crate**: `cargo add zhconv` (see doc comments and [cli/](https://github.com/Gowee/zhconv-rs/tree/main/cli) for examples)
 
 🐍 **Python Package via PyO3**: `pip install zhconv-rs` (WASM with wheels)
 
 <details open>
  <summary>Python snippet</summary>
 
 ```python
@@ -116,19 +116,17 @@
 The benchmark was performed on a previous version that had only Mediawiki rulesets. In the newer version, with OpenCC rulesets activated by default, the performance may degrade ~2x.
 
 ## Differences with other converters
 * `ZhConver{sion,ter}.php` of MediaWiki: zhconv-rs just takes conversion tables listed in [`ZhConversion.php`](https://github.com/wikimedia/mediawiki/blob/master/includes/languages/data/ZhConversion.php#L14). MediaWiki relies on the inefficient PHP built-in function [`strtr`](https://github.com/php/php-src/blob/217fd932fa57d746ea4786b01d49321199a2f3d5/ext/standard/string.c#L2974). Under the basic mode, zhconv-rs guarantees linear time complexity (`T = O(n+m)` instead of `O(nm)`) and single-pass scanning of input text. Optionally, zhconv-rs supports the same conversion rule syntax with MediaWiki.
 * OpenCC: The [conversion rulesets](https://github.com/BYVoid/OpenCC/tree/master/data/dictionary) of OpenCC is independent of MediaWiki. The core [conversion implementation](https://github.dev/BYVoid/OpenCC/blob/21995f5ea058441423aaff3ee89b0a5d4747674c/src/Conversion.cpp#L27) of OpenCC is kinda similar to the aforementioned `strtr`. However, OpenCC supports pre-segmentation and maintains multiple rulesets which are applied successively. By contrast, the Aho-Corasick-powered zhconv-rs merges rulesets from MediaWiki and OpenCC in compile time and converts text in single-pass linear time, resulting in much more efficiency. Though, conversion results may differ in some cases.
 
 ## Limitations
-The converter takes leftmost-longest matching strategy. It gives priority to the leftmost-matched words or phrases. For instance, if a ruleset includes both `干 -> 幹` and `天干物燥 -> 天乾物燥`, the converter would prioritize `天乾物燥` because `天干物燥` gets matched earlier compared to `干` at a later position. The strategy yields good results in general, but may occasionally lead to wrong conversions.
+The converter utilizes an aho-corasick automaton with the leftmost-longest matching strategy. This strategy gives priority to the leftmost-matched words or phrases. For instance, if a ruleset includes both `干 -> 幹` and `天干物燥 -> 天乾物燥`, the converter would prioritize `天乾物燥` because `天干物燥` gets matched earlier compared to `干` at a later position. The strategy is generally effective but may occasionally lead to unexpected results.
 
-The implementation support most of the MediaWiki conversion rules. But it is not fully compliant with the original implementation.
-
-Besides, for wikitext, if input text contains global conversion rules (in MediaWiki syntax like -{H|zh-hans:鹿|zh-hant:马}-), the time complexity of the implementation may degrade to `O(n*m)` where `n` and `m` are the length of the text and the maximum lengths of sources words in conversion rulesets in the worst case (equivalent to brute-force).
+Futuremore, since an automaton is infeasible to update after being built, the converter must (re)build it from scratch for every ruleset. The automata for built-in rulesets (i.e. conversion tables) are built on demand and cached by default. However, if a short input text contains global conversion rules (in MediaWiki syntax like -{H|zh-hans:鹿|zh-hant:马}-), this process incurs a significant overhead, potentially being less efficient than a naive implementation.
 
 ## Credits
 All rulesets that power the converter come from the [MediaWiki](https://github.com/wikimedia/mediawiki) project and [OpenCC](https://github.com/BYVoid/OpenCC).
 
 The project takes the following projects/pages as references:
 - https://github.com/gumblex/zhconv : Python implementation of `zhConver{ter,sion}.php`.
 - https://github.com/BYVoid/OpenCC/ : Widely adopted Chinese converter.
```

#### html2text {}

```diff
@@ -4,25 +4,25 @@
 img.shields.io/crates/v/zhconv.svg)](https://crates.io/crates/zhconv) [![PyPI
 version](https://img.shields.io/pypi/v/zhconv-rs)](https://pypi.org/project/
 zhconv-rs/) [![NPM version](https://badge.fury.io/js/zhconv.svg)](https://
 www.npmjs.com/package/zhconv) # zhconv-rs ä¸­æç®ç¹åå°åè©è½æ
 zhconv-rs converts Chinese text among traditional/simplified scripts or
 regional variants (e.g. `zh-TW <-> zh-CN <-> zh-HK <-> zh-Hans <-> zh-Hant`),
 built on the top of rulesets from MediaWiki/Wikipedia and OpenCC. The
-implementation is powered by an [Aho-Corasick](https://github.com/daac-tools/
-daachorse) automaton, ensuring linear time complexity with respect to the
+implementation is powered by the [Aho-Corasick](https://github.com/BurntSushi/
+aho-corasick) automaton, ensuring linear time complexity with respect to the
 length of input text and conversion rules (`O(n+m)`), processing dozens of MiBs
 text per second. ð **Web App: https://zhconv.pages.dev** (powered by WASM)
 âï¸ **Cli**: `cargo install zhconv-cli` or check [releases](https://
 github.com/Gowee/zhconv-rs/releases). ð¦ **Rust Crate**: `cargo add zhconv`
-(check [docs](https://docs.rs/zhconv/latest/zhconv/) for examples) ð
-**Python Package via PyO3**: `pip install zhconv-rs` (WASM with wheels)  Python
-snippet ```python # > pip install zhconv_rs # Convert with builtin rulesets:
-from zhconv_rs import zhconv assert zhconv("å¤©å¹²ç©ç¥ å°å¿ç«ç", "zh-
-tw") == "å¤©ä¹¾ç©ç¥ å°å¿ç«ç­" assert zhconv
+(see doc comments and [cli/](https://github.com/Gowee/zhconv-rs/tree/main/cli)
+for examples) ð **Python Package via PyO3**: `pip install zhconv-rs` (WASM
+with wheels)  Python snippet ```python # > pip install zhconv_rs # Convert with
+builtin rulesets: from zhconv_rs import zhconv assert zhconv("å¤©å¹²ç©ç¥
+å°å¿ç«ç", "zh-tw") == "å¤©ä¹¾ç©ç¥ å°å¿ç«ç­" assert zhconv
 ("é§å¤±æ¨èºï¼æè¿·æ´¥æ¸¡", "zh-hans") == "é¾å¤±æ¥¼å°ï¼æè¿·æ´¥æ¸¡"
 assert zhconv("ã-{zh-hans:ä¸ä¸ªç«æªæ;zh-hant:ä¸åå®¢;zh-tw:ä¸åå®¢}-
 ãæ¯äºæ­·å±±å¤§Â·ä»²é¦¬çä½åã", "zh-cn", mediawiki=True) ==
 "ãä¸ä¸ªç«æªæãæ¯äºåå±±å¤§Â·ä»²é©¬çä½åã" assert zhconv("-
 {H|zh-cn:é¾é½å­¤å¿;zh-tw:å­¤éæ·;zh-hk:è¦æµ·å­¤é;zh-sg:é¾é½å­¤å¿;zh-
 mo:è¦æµ·å­¤é;}-ãé¾é½å­¤å¿ãæ¯æ¥å°æ¯Â·çæ´æ¯çä½åã", "zh-
 tw", True) == "ãå­¤éæ·ãæ¯æ¥ç¾æ¯Â·çæ´æ¯çä½åã" # Convert
@@ -80,31 +80,31 @@
 implementation](https://github.dev/BYVoid/OpenCC/blob/
 21995f5ea058441423aaff3ee89b0a5d4747674c/src/Conversion.cpp#L27) of OpenCC is
 kinda similar to the aforementioned `strtr`. However, OpenCC supports pre-
 segmentation and maintains multiple rulesets which are applied successively. By
 contrast, the Aho-Corasick-powered zhconv-rs merges rulesets from MediaWiki and
 OpenCC in compile time and converts text in single-pass linear time, resulting
 in much more efficiency. Though, conversion results may differ in some cases.
-## Limitations The converter takes leftmost-longest matching strategy. It gives
-priority to the leftmost-matched words or phrases. For instance, if a ruleset
-includes both `å¹² -> å¹¹` and `å¤©å¹²ç©ç¥ -> å¤©ä¹¾ç©ç¥`, the converter
-would prioritize `å¤©ä¹¾ç©ç¥` because `å¤©å¹²ç©ç¥` gets matched earlier
-compared to `å¹²` at a later position. The strategy yields good results in
-general, but may occasionally lead to wrong conversions. The implementation
-support most of the MediaWiki conversion rules. But it is not fully compliant
-with the original implementation. Besides, for wikitext, if input text contains
-global conversion rules (in MediaWiki syntax like -{H|zh-hans:é¹¿|zh-hant:é©¬}-
-), the time complexity of the implementation may degrade to `O(n*m)` where `n`
-and `m` are the length of the text and the maximum lengths of sources words in
-conversion rulesets in the worst case (equivalent to brute-force). ## Credits
-All rulesets that power the converter come from the [MediaWiki](https://
-github.com/wikimedia/mediawiki) project and [OpenCC](https://github.com/BYVoid/
-OpenCC). The project takes the following projects/pages as references: - https:
-//github.com/gumblex/zhconv : Python implementation of `zhConver
-{ter,sion}.php`. - https://github.com/BYVoid/OpenCC/ : Widely adopted Chinese
-converter. - https://zh.wikipedia.org/wiki/Wikipedia:å­è©è½æèç -
-https://zh.wikipedia.org/wiki/Help:é«çº§å­è¯è½¬æ¢è¯­æ³ - https://
-github.com/wikimedia/mediawiki/blob/master/includes/language/
-LanguageConverter.php  ## TODO - [x] Support [Module:CGroup](https://
-zh.wikipedia.org/wiki/Module:CGroup) - [ ] Propogate error properly with Anyhow
-and thiserror - [x] Python lib - [x] More exmaples in README - [x] Add rulesets
-from OpenCC
+## Limitations The converter utilizes an aho-corasick automaton with the
+leftmost-longest matching strategy. This strategy gives priority to the
+leftmost-matched words or phrases. For instance, if a ruleset includes both
+`å¹² -> å¹¹` and `å¤©å¹²ç©ç¥ -> å¤©ä¹¾ç©ç¥`, the converter would prioritize
+`å¤©ä¹¾ç©ç¥` because `å¤©å¹²ç©ç¥` gets matched earlier compared to `å¹²` at
+a later position. The strategy is generally effective but may occasionally lead
+to unexpected results. Futuremore, since an automaton is infeasible to update
+after being built, the converter must (re)build it from scratch for every
+ruleset. The automata for built-in rulesets (i.e. conversion tables) are built
+on demand and cached by default. However, if a short input text contains global
+conversion rules (in MediaWiki syntax like -{H|zh-hans:é¹¿|zh-hant:é©¬}-), this
+process incurs a significant overhead, potentially being less efficient than a
+naive implementation. ## Credits All rulesets that power the converter come
+from the [MediaWiki](https://github.com/wikimedia/mediawiki) project and
+[OpenCC](https://github.com/BYVoid/OpenCC). The project takes the following
+projects/pages as references: - https://github.com/gumblex/zhconv : Python
+implementation of `zhConver{ter,sion}.php`. - https://github.com/BYVoid/OpenCC/
+: Widely adopted Chinese converter. - https://zh.wikipedia.org/wiki/Wikipedia:
+å­è©è½æèç - https://zh.wikipedia.org/wiki/Help:
+é«çº§å­è¯è½¬æ¢è¯­æ³ - https://github.com/wikimedia/mediawiki/blob/master/
+includes/language/LanguageConverter.php  ## TODO - [x] Support [Module:CGroup]
+(https://zh.wikipedia.org/wiki/Module:CGroup) - [ ] Propogate error properly
+with Anyhow and thiserror - [x] Python lib - [x] More exmaples in README - [x]
+Add rulesets from OpenCC
```

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/benches/25328-0.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/25328-0.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/benches/data3185k.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/data3185k.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/benches/data54k.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/data54k.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/benches/data689k.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/data689k.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/benches/wikitext.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/wikitext.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/benches/zhconv_benchmark.rs` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/benches/zhconv_benchmark.rs`

 * *Files 4% similar despite different names*

```diff
@@ -138,26 +138,14 @@
                     + DATA3185K
                     + DATA3185K
                     + DATA3185K
                     + DATA3185K),
             )
         })
     });
-    c.bench_function("is_hans data55k", |b| {
-        b.iter_with_large_drop(|| zhconv::is_hans(DATA54K))
-    });
-    c.bench_function("infer_variant data55k", |b| {
-        b.iter_with_large_drop(|| zhconv::infer_variant(DATA54K))
-    });
-    c.bench_function("is_hans data3185k", |b| {
-        b.iter_with_large_drop(|| zhconv::is_hans(DATA3185K))
-    });
-    c.bench_function("infer_variant data3185k", |b| {
-        b.iter_with_large_drop(|| zhconv::infer_variant(DATA3185K))
-    });
 }
 
 criterion_group!(benches, criterion_benchmark);
 // criterion_group! {
 //     name = benches;
 //     config = Criterion::default().sample_size(500);
 //     targets = criterion_benchmark
```

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/build.rs` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/build.rs`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,14 @@
         hex!("bef60ceb4e57b6b062351406cb5d4644875574231d64787e03711317b7e773f3"),
     ),
 ];
 
 fn main() -> io::Result<()> {
     let zhconv = read_and_validate_file("data/ZhConversion.php", &MEDIAWIKI_SHA256);
     let mut zhconvs = parse_mediawiki(&zhconv);
-    #[allow(unused_variables, unused_mut)]
     for (name, mut pairs) in zhconvs.iter_mut() {
         // Load and append OpenCC rulesets to the Mediawiki ones
         // ref: https://github.com/BYVoid/OpenCC/blob/29d33fb8edb8c95e34691c8bd1ef76a50d0b5251/data/config/
 
         // Note: OpenCC conversion procededures take multi-pass for chaining rulesets.
         // For efficiency and re-using the existing implementation, we chain the rulesets
         // straightforward by chaining conversion pairs at different level in advance.
@@ -361,19 +360,15 @@
 fn sort_and_dedup(pairs: &mut Vec<(String, String)>) {
     pairs.sort_by(|a, b| b.0.len().cmp(&a.0.len()).then(a.0.cmp(&b.0)));
     pairs.dedup_by(|a, b| a.0 == b.0);
 }
 
 #[cfg(feature = "opencc")]
 mod opencc {
-
-    use daachorse::{
-        CharwiseDoubleArrayAhoCorasick, CharwiseDoubleArrayAhoCorasickBuilder, MatchKind,
-    };
-    // use aho_corasick::{AhoCorasick, AhoCorasickBuilder, MatchKind};
+    use aho_corasick::{AhoCorasick, AhoCorasickBuilder, MatchKind};
     use lazy_static::lazy_static;
     use std::collections::HashMap;
 
     use super::OPENCC_SHA256;
 
     lazy_static! {
         pub static ref OPENCC_SHA256_MAP: HashMap<String, [u8; 32]> = OPENCC_SHA256
@@ -429,93 +424,68 @@
             let mut prev_stage = None;
             $(load_opencc_to!(@load_stage $out, prev_stage, $stage);)*
             let (convs, _) = prev_stage.unwrap();
             $out.extend(convs.into_iter());
         };
     }
     pub(crate) use load_opencc_to;
+
     pub fn parse_opencc_to(
         out_conv: &mut HashMap<String, String>,
         out_revconv: &mut HashMap<String, String>,
         s: &str,
     ) {
         for line in s.lines().map(|l| l.trim()).filter(|l| !l.is_empty()) {
             let mut it = line.split_whitespace();
             if let (Some(f), Some(t)) = (it.next(), it.next()) {
                 out_conv.insert(f.to_owned(), t.to_owned());
-                // TODO: one-to-many mapping?
-                if !out_revconv.contains_key(t) {
-                    out_revconv.insert(t.to_owned(), f.to_owned());
-                }
+                out_revconv.insert(t.to_owned(), f.to_owned());
                 for tt in it {
-                    if !out_revconv.contains_key(t) {
-                        out_revconv.insert(tt.to_owned(), f.to_owned());
-                    }
+                    out_revconv.insert(tt.to_owned(), f.to_owned());
                 }
             }
         }
     }
 
     /// Simplified `ZhConverter` implementation for pre-processing rulesets from OpenCC
     pub struct SimpleConverter {
-        automaton: Option<CharwiseDoubleArrayAhoCorasick<usize>>,
-        target_words: Vec<String>,
+        automaton: AhoCorasick,
+        mapping: HashMap<String, String>,
     }
 
     impl From<HashMap<String, String>> for SimpleConverter {
         fn from(mapping: HashMap<String, String>) -> Self {
-            let mut target_words = Vec::with_capacity(mapping.len());
-            let automaton = if mapping.is_empty() {
-                None
-            } else {
-                Some(
-                    CharwiseDoubleArrayAhoCorasickBuilder::new()
-                        .match_kind(MatchKind::LeftmostLongest)
-                        .build(mapping.into_iter().map(|(f, t)| {
-                            target_words.push(t);
-                            f
-                        }))
-                        .expect("Conversion table is valid"),
-                )
-            };
-            Self {
-                automaton,
-                target_words,
-            }
+            let automaton = AhoCorasickBuilder::new()
+                .match_kind(MatchKind::LeftmostLongest)
+                .build(mapping.keys())
+                .unwrap();
+            Self { automaton, mapping }
         }
     }
 
     impl SimpleConverter {
         #[allow(dead_code)]
         pub fn build<'s>(pairs: impl Iterator<Item = (&'s str, &'s str)>) -> Self {
             let mapping = HashMap::from_iter(pairs.map(|(a, b)| (a.to_owned(), b.to_owned())));
             mapping.into()
         }
 
         pub fn convert(&self, text: &str) -> String {
-            match &self.automaton {
-                Some(automaton) => {
-                    let mut output = String::new();
-                    let mut last = 0;
-                    // leftmost-longest matching
-                    for (s, e, ti) in automaton
-                        .leftmost_find_iter(text)
-                        .map(|m| (m.start(), m.end(), m.value()))
-                    {
-                        if s > last {
-                            output.push_str(&text[last..s]);
-                        }
-                        output.push_str(&self.target_words[ti]);
-                        last = e;
-                    }
-                    output.push_str(&text[last..]);
-                    output
+            let mut output = String::new();
+            let mut last = 0;
+            // leftmost-longest matching
+            for (s, e) in self.automaton.find_iter(text).map(|m| (m.start(), m.end())) {
+                if s > last {
+                    output.push_str(&text[last..s]);
                 }
-                None => String::from(text),
+                output.push_str(self.mapping.get(&text[s..e]).unwrap());
+                last = e;
             }
+            output.push_str(&text[last..]);
+            output
         }
     }
 }
 
 fn read_and_validate_file(path: &str, sha256sum: &[u8; 32]) -> String {
     let data_dir = env::var_os("CARGO_MANIFEST_DIR").unwrap();
     let path = Path::new(&data_dir).join(path);
```

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/HKVariants.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/HKVariants.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/HKVariantsRevPhrases.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/HKVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/README.md` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/README.md`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/STCharacters.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/STCharacters.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/STPhrases.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/STPhrases.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/TSCharacters.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TSCharacters.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/TSPhrases.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TSPhrases.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/TWPhrasesIT.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TWPhrasesIT.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/TWPhrasesName.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TWPhrasesName.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/TWPhrasesOther.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TWPhrasesOther.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/TWVariantsRevPhrases.txt` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/TWVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/ZhConversion.php` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/ZhConversion.php`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/1D.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/1D.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/2016年太平洋颱風季.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2016年太平洋颱風季.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/2017年太平洋颱風季.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2017年太平洋颱風季.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/2018年太平洋颱風季.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2018年太平洋颱風季.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/2019年太平洋颱風季.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2019年太平洋颱風季.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/2020年太平洋颱風季.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2020年太平洋颱風季.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/2021年太平洋颱風季.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2021年太平洋颱風季.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/2022年太平洋颱風季.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/2022年太平洋颱風季.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/24.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/24.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/A Pink.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/A Pink.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/A Song of Ice and Fire.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/A Song of Ice and Fire.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/ACmilan.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ACmilan.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/ALeague.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ALeague.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/AT Places.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/AT Places.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/AU Places.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/AU Places.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Adventure Time.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Adventure Time.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Aero.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Aero.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Aikatsu.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Aikatsu.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Anime.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Anime.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Apple.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Apple.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Aquatics.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Aquatics.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Ariana Grande.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Ariana Grande.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Artist.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Artist.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Astronomy.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Astronomy.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Avatar.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Avatar.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Avril Lavigne.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Avril Lavigne.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/BE Places.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/BE Places.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/BUDDYCOMPLEX.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/BUDDYCOMPLEX.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Badminton.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Badminton.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Bakuman.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Bakuman.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Battle Spirits.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Battle Spirits.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Bird.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Bird.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/BirdG.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/BirdG.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/BirdP.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/BirdP.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Black Mirror.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Black Mirror.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Bridge.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Bridge.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Britney Spears.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Britney Spears.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Bundesliga.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Bundesliga.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Butterfly.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Butterfly.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/C&C.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/C&C.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/CA Places.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/CA Places.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/CANAAN.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/CANAAN.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/CH Places.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/CH Places.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/COD.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/COD.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/CWBTyphoonOld.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/CWBTyphoonOld.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Canada.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Canada.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Carnivorous Plant.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Carnivorous Plant.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Cartoon.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Cartoon.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Chanel.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Chanel.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Chemistry.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Chemistry.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Code Black.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Code Black.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Code Geass.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Code Geass.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/CodeLyoko.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/CodeLyoko.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Coldplay.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Coldplay.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Communication.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Communication.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Composer.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Composer.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Copyright.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Copyright.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Counter-Strike.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Counter-Strike.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Crazyracing Kartrider.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Crazyracing Kartrider.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Cyber Formula.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Cyber Formula.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Cyclone.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Cyclone.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/DCComics.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/DCComics.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/DE Places.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/DE Places.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Danball Senki.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Danball Senki.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Dance.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Dance.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Death Note.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Death Note.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Diablo.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Diablo.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Die Weiße Rose.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Die Weiße Rose.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Digimon.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Digimon.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Disney.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Disney.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Doctor Who.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Doctor Who.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Doraemon.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Doraemon.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/DragonBall.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/DragonBall.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/DreamWorks.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/DreamWorks.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/ED.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ED.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/EPL.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/EPL.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/EU.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/EU.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Earthquake.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Earthquake.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Ecology.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Ecology.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Economics.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Economics.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Electronics.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Electronics.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Esports.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Esports.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Eyeshield21.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Eyeshield21.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/F1.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/F1.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/FAcup.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/FAcup.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/FR Places.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/FR Places.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Family Guy.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Family Guy.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Firearms.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Firearms.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Food.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Food.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Football.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Football.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Friends.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Friends.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Fringe.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Fringe.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Frozen.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Frozen.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/FullmetalAlchemist.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/FullmetalAlchemist.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Futurama.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Futurama.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GBF.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GBF.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GGundam.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GGundam.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GOSICK.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GOSICK.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GZFC.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GZFC.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Games-zh.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Games-zh.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Games.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Games.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GaoGaiGar.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GaoGaiGar.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Geography.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Geography.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Getter Robo.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Getter Robo.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Ghibli.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Ghibli.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Glee.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Glee.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GossipGirl.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GossipGirl.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Guardians of Ga'Hoole.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Guardians of Ga'Hoole.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Gundam00.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Gundam00.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GundamAGE.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamAGE.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GundamIBO.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamIBO.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GundamSeed.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamSeed.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GundamTWFM.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamTWFM.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GundamUC.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamUC.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/GundamW.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/GundamW.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/HTGAWM.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/HTGAWM.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/HUNTER.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/HUNTER.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Half-Life.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Half-Life.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Hannibal Lecter.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Hannibal Lecter.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/HarryPotter.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/HarryPotter.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Hawaii Five-0.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Hawaii Five-0.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Hayate the Combat Butler.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Hayate the Combat Butler.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Heroes of the Storm.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Heroes of the Storm.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/House.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/House.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/IMF.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/IMF.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/IT.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/IT.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/JLeague.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/JLeague.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/JP Show.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/JP Show.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/James Bond.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/James Bond.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Jewelpet.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Jewelpet.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Justin Bieber.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Justin Bieber.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/KLeague.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/KLeague.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/KO Movie.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/KO Movie.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/KO Show.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/KO Show.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/KO TV Show.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/KO TV Show.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/KamenRider.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/KamenRider.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Kao.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Kao.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Katy Perry.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Katy Perry.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Korea Comparison.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Korea Comparison.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Korea.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Korea.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Korean.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Korean.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/LEGO.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LEGO.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/LOL.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LOL.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/LR.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LR.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/La casa de papel.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/La casa de papel.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Lady Gaga.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Lady Gaga.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Lana Del Rey.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Lana Del Rey.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Laos.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Laos.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Legend of the Guardians.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Legend of the Guardians.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Les Misérables.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Les Misérables.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Lifesciences.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Lifesciences.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Linkin.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Linkin.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Lorde.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Lorde.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/LuaIT.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LuaIT.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/LuaMovie.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LuaMovie.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/LuaShow.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/LuaShow.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MA.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MA.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MCD.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MCD.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MCFC.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MCFC.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MLS.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MLS.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MUFC.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MUFC.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MY.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MY.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Mabinogi.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Mabinogi.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MapleStory.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MapleStory.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Mariah Carey.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Mariah Carey.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Math.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Math.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Mazinger.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Mazinger.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/McDonald's.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/McDonald's.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MediaWiki special.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MediaWiki special.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MediaWiki.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MediaWiki.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Medicine.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Medicine.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Michael Jackson.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Michael Jackson.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Might&Magic.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Might&Magic.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Military.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Military.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Minecraft.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Minecraft.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Movie.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Movie.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Music.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Music.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/My Little Pony.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/My Little Pony.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/MyHeroAcademia.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/MyHeroAcademia.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/NARUTO.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/NARUTO.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/NBA.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/NBA.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/NFL.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/NFL.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/NHL.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/NHL.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Nintendo.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Nintendo.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Nobel Prize.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Nobel Prize.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/OnePiece.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/OnePiece.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Organization.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Organization.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Overwatch.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Overwatch.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/P&G.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/P&G.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/PHL Places.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PHL Places.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/People.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/People.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/PeppaPig.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PeppaPig.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Percy Jackson.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Percy Jackson.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/PerryClass.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PerryClass.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Pesticide.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pesticide.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Photography.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Photography.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Physics.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Physics.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Pichi Pichi Pitch.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pichi Pichi Pitch.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Pinnacle Islands.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pinnacle Islands.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Pixar.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pixar.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Pokemon-old.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pokemon-old.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Pokemon.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pokemon.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/PoliticiansUK.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PoliticiansUK.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Popes.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Popes.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Power Rangers.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Power Rangers.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/PresidentsUS.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PresidentsUS.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Pretty Rhythm.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Pretty Rhythm.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/PrisonBreak.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/PrisonBreak.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Psychology.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Psychology.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Racing.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Racing.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Railway.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Railway.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/RainbowSixSiege.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/RainbowSixSiege.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Reborn.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Reborn.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/ResidentEvil.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ResidentEvil.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Rihanna.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Rihanna.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/SAO.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SAO.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/SARS-CoV-2 variant.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SARS-CoV-2 variant.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/SEGA.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SEGA.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/SNSD.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SNSD.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/SPL.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SPL.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/SPY×FAMILY.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SPY×FAMILY.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Sailor Moon.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Sailor Moon.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/SaintSeiyaOmega.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SaintSeiyaOmega.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Sandbox.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Sandbox.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Selena Gomez.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Selena Gomez.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Shinkalion.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Shinkalion.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Shipname.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Shipname.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Show.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Show.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Shugo Chara!.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Shugo Chara!.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Sia.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Sia.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Signals and Systems.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Signals and Systems.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Sim.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Sim.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Simpsons.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Simpsons.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Snooker.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Snooker.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/SouthPark.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SouthPark.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/SpongeBob SquarePants.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/SpongeBob SquarePants.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Sports.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Sports.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Square Enix.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Square Enix.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/StarCraft.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/StarCraft.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/StarCraft2.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/StarCraft2.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/StarTrek.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/StarTrek.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/StarWars.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/StarWars.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/StephenKing.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/StephenKing.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Summon Night.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Summon Night.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/TCM.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TCM.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/TV.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TV.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Table Tennis.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Table Tennis.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Tales.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Tales.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Tamagotchi.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Tamagotchi.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Taylor Swift.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Taylor Swift.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Telcom.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Telcom.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Tennis.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Tennis.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/The Chainsmokers.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/The Chainsmokers.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/The Witcher.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/The Witcher.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/The World God Only Knows.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/The World God Only Knows.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/TheBeatles.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TheBeatles.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/ThePeanuts.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ThePeanuts.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Toaru.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Toaru.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Transformers.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Transformers.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Transport for London.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Transport for London.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Transport.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Transport.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/TropicalCycloneName.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TropicalCycloneName.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Twilight.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Twilight.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/TyphoonNew.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TyphoonNew.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/TyphoonOld.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/TyphoonOld.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/UA toponyms.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/UA toponyms.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/UK Places.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/UK Places.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/US CA Cities.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/US CA Cities.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/US Government.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/US Government.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/US Senators.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/US Senators.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/USState.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/USState.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Ultraman.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Ultraman.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Unilever.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Unilever.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Unit.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Unit.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Urban.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Urban.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/VLeague.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/VLeague.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Valkyria.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Valkyria.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/WORKING!!.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/WORKING!!.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Warcraft.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Warcraft.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Warhammer.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Warhammer.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Warriors.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Warriors.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Watch.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Watch.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Weather.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Weather.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Windows.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Windows.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Wow.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Wow.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/Yes! 光之美少女5.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/Yes! 光之美少女5.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/ZH Show.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ZH Show.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/arsenal.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/arsenal.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/check1.py` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/check1.py`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/chelsea.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/chelsea.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/fcbarcelona.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/fcbarcelona.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/fcbayern.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/fcbayern.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/free license.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/free license.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/inter.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/inter.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/laliga.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/laliga.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/leek.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/leek.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/ligue.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/ligue.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/liverpoolfc.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/liverpoolfc.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/loghorizon.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/loghorizon.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/magi.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/magi.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/merge_for_web.py` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/merge_for_web.py`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/neo-noir.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/neo-noir.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/regalia.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/regalia.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/specialpages.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/specialpages.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/uefa.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/uefa.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/vital.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/vital.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/一拳超人.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/一拳超人.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/伊拉克足球.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/伊拉克足球.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/伊斯蘭.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/伊斯蘭.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/伊朗足球.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/伊朗足球.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/佛教.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/佛教.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/俄超.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/俄超.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/俱乐部足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/俱乐部足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/列斯聯.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/列斯聯.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/加超聯.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/加超聯.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/南美球會.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/南美球會.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/博弈论.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/博弈论.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/卡塔尔星级足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/卡塔尔星级足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/叙利亚职业足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/叙利亚职业足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/名偵探柯南.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/名偵探柯南.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/咕嚕咕嚕魔法陣.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/咕嚕咕嚕魔法陣.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/咲-Saki-.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/咲-Saki-.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/四驅兄弟.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/四驅兄弟.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/圍棋.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/圍棋.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/地名.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/地名.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/声临其境.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/声临其境.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/妖怪手錶.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/妖怪手錶.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/姓氏.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/姓氏.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/娛樂.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/娛樂.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/小魔女DoReMi.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/小魔女DoReMi.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/巴勒斯坦职业足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/巴勒斯坦职业足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/巴林职业足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/巴林职业足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/幸福爆發！光之美少女.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/幸福爆發！光之美少女.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/意甲.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/意甲.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/愛天使傳說.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/愛天使傳說.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/戰鬥陀螺 鋼鐵奇兵.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/戰鬥陀螺 鋼鐵奇兵.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/打工吧！魔王大人.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/打工吧！魔王大人.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/政治人物.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/政治人物.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/文學.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/文學.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/星光樂園.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/星光樂園.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/暗影诗章 (动画).json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/暗影诗章 (动画).json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/村上春樹.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/村上春樹.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/核能.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/核能.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/機獸系列.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/機獸系列.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/民族.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/民族.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/沙特职业足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/沙特职业足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/泰國人名.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/泰國人名.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/涼宮春日的憂鬱.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/涼宮春日的憂鬱.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/潘朵拉之心.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/潘朵拉之心.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/烏茲別克足球會.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/烏茲別克足球會.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/爆丸.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/爆丸.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/畜牧.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/畜牧.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/百變小櫻.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/百變小櫻.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/科威特职业足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/科威特职业足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/童話槍手小紅帽.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/童話槍手小紅帽.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/约旦职业足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/约旦职业足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/美国漫画.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/美国漫画.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/荷蘭足球聯賽.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/荷蘭足球聯賽.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/菁英殺機.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/菁英殺機.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/葡超.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/葡超.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/蠟筆小新.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/蠟筆小新.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/通靈王.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/通靈王.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/進擊的巨人.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/進擊的巨人.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/釣魚臺列嶼.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/釣魚臺列嶼.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/閃電十一人.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/閃電十一人.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/闇.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/闇.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/阿曼职业足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/阿曼职业足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/阿联酋职业足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/阿联酋职业足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/降世神通.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/降世神通.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/音樂劇.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/音樂劇.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/驅魔少年.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/驅魔少年.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/马来人名地名.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/马来人名地名.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/鬥陣特攻.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/鬥陣特攻.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/魔法咪路咪路.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/魔法咪路咪路.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/黎巴嫩职业足球联赛.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/黎巴嫩职业足球联赛.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/黑執事.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/黑執事.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/cgroups/黑塔系列.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/cgroups/黑塔系列.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/poetry.lock` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/poetry.lock`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/update_basic.py` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/update_basic.py`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/data/update_cgroups.py` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/data/update_cgroups.py`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/run-maturin-action.sh` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/src/converter.rs` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/converter.rs`

 * *Files 1% similar despite different names*

```diff
@@ -312,16 +312,15 @@
 
     /// The general implementation of MediaWiki syntax-aware conversion.
     ///
     /// Equivalent to [`convert_as_wikitext_basic`](Self::convert_as_wikitext_basic) if
     /// `addtional_conv_lines` is set empty and both `skip_html_code_blocks` and
     /// `apply_global_rules` are set to `false`.
     ///
-    /// Equivalent to [`convert_as_wikitext_extended`](Self::convert_as_wikitext_extended),
-    /// otherwise.
+    /// Equivalent to [`convert_as_wikitext_extended`], otherwise.
     ///
     /// `addtional_conv_lines` looks like:
     /// ```text
     /// zh-cn:天堂执法者; zh-hk:夏威夷探案; zh-tw:檀島警騎2.0;
     /// zh-cn:史蒂芬·'史蒂夫'·麦格瑞特; zh-tw:史提夫·麥加雷; zh-hk:麥星帆;
     /// zh-cn:丹尼尔·'丹尼/丹诺'·威廉姆斯; zh-tw:丹尼·威廉斯; zh-hk:韋丹尼;
     /// ```
@@ -487,40 +486,21 @@
     //             let raw = unsafe { text.as_bytes_mut() };
     //             raw[wi..wi + tbp[0].len()].clone_from_slice(tbp[0].as_bytes());
     //             tbp.pop_front();
     //         }
     //     }
     // }
 
-    /// Search the text
-    #[doc(hidden)]
-    pub fn search<'s, 'i: 's>(
-        &'i self,
-        text: &'s str,
-    ) -> impl Iterator<Item = (usize, usize, &'i str)> + 's {
-        self.automaton
-            .as_ref()
-            .map(|automaton| {
-                automaton.leftmost_find_iter(text).map(|m| {
-                    (
-                        m.start(),
-                        m.end(),
-                        self.target_words[m.value() as usize].as_ref(),
-                    )
-                })
-            })
-            .into_iter()
-            .flatten()
-    }
-
-    /// Count the sum of lengths of source words to be replaced by the converter, in chars
-    #[doc(hidden)]
-    pub fn count_replaced(&self, text: &str) -> usize {
-        self.search(text)
-            .map(|(s, e, _to)| text[s..e].chars().count())
+    /// Count the sum of lengths of matched source words to be substituted in the given text, in bytes.
+    pub fn count_matched(&self, text: &str) -> usize {
+        let automaton = unwrap_or_return!(self.automaton.as_ref(), 0);
+
+        automaton
+            .leftmost_find_iter(text)
+            .map(|m| m.end() - m.start())
             .sum()
     }
 }
 
 /// A builder that helps build a [`ZhConverter`](ZhConverter).
 ///
 /// # Example
```

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/src/converters.rs` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/converters.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 //! Converters lazily built from built-in [`tables`](crate::tables).
 //!
-//! These converters are lazily loaded from serialized automata built at build-time, and cached for
-//! later use.
+//! These converters are lazily built on demand with [`dfa`](crate::ZhConverterBuilder::dfa)
+//! activated for better conversion performance, and cached for later use.
 
 use daachorse::CharwiseDoubleArrayAhoCorasick;
 use lazy_static::lazy_static; // TODO: once_cell
 
-#[cfg(feature = "compress")]
-use crate::utils::zstd_decompress;
-use crate::{tables::*, Variant, ZhConverter, ZhConverterBuilder};
+use crate::{tables::*, utils::zstd_decompress, Variant, ZhConverter, ZhConverterBuilder};
 
 // FIX: Doc
 
 // More specific rules should take precedence when merging (e.g. zh-TW > zh-Hant).
 // Since the converter build process relies on HashMap::extend, latter rules overwrite the early ones.
 lazy_static! {
     #[allow(non_upper_case_globals)]
```

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/src/lib.rs` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/lib.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 //! This crate provides a ZhConverter that converts Chinese variants among each other. The
-//! implementation is based on the [Aho-Corasick](https://docs.rs/daachorse) algorithm
+//! implementation is based on the [Aho-Corasick](https://docs.rs/aho-corasick/latest) automaton
 //! with the leftmost-longest matching strategy and linear time complexity with respect to the
 //! length of input text and conversion rules. It ships with a bunch of conversion tables,
 //! extracted from [zhConversion.php](https://phabricator.wikimedia.org/source/mediawiki/browse/master/includes/languages/data/ZhConversion.php)
 //! (maintained by MediaWiki and Chinese Wikipedia) and [OpenCC](https://github.com/BYVoid/OpenCC/tree/master/data/dictionary).
 //!
 //! While built-in rulesets work well for general case, the converter is never meant to be 100%
 //! accurate, especially for professional text. On Chinese Wikipedia, it is pretty common for
@@ -23,15 +23,15 @@
 //! ```
 //!
 //! # Example
 //!
 //! Basic conversion:
 //! ```
 //! use zhconv::{zhconv, Variant};
-//! assert_eq!(zhconv("天干物燥 小心火烛", "zh-Hant".parse().unwrap()), "天乾物燥 小心火燭");
+//! assert_eq!(zhconv("天干物燥 小心火烛", Variant::ZhHant), "天乾物燥 小心火燭");
 //! assert_eq!(zhconv("鼠曲草", Variant::ZhHant), "鼠麴草");
 //! assert_eq!(zhconv("阿拉伯联合酋长国", Variant::ZhHant), "阿拉伯聯合酋長國");
 //! assert_eq!(zhconv("阿拉伯联合酋长国", Variant::ZhTW), "阿拉伯聯合大公國");
 //! ```
 //!
 //! With MediaWiki conversion rules:
 //! ```
@@ -41,22 +41,14 @@
 //! assert_eq!(zhconv_mw("菊科草本植物包括-{zh-tw:鼠麴草;zh-cn:香茅;}-等。", Variant::ZhTW), "菊科草本植物包括鼠麴草等。");
 //! assert_eq!(zhconv_mw("-{H|zh:馬;zh-cn:鹿;}-馬克思主義", Variant::ZhCN), "鹿克思主义"); // global rule
 //! ```
 //!
 //! To load or add additional conversion rules such as CGroups or `(FROM, TO)` pairs,
 //! see [`ZhConverterBuilder`].
 //!
-//! Other useful function:
-//! ```
-//! use zhconv::{is_hans, is_hans_confidence, infer_variant, infer_variant_confidence};
-//! assert!(!is_hans("秋冬濁而春夏清，晞於朝而生於夕"));
-//! assert!(is_hans_confidence("滴瀝明花苑，葳蕤泫竹叢") < 0.5);
-//! println!("{}", infer_variant("錦字緘愁過薊水，寒衣將淚到遼城"));
-//! println!("{:?}", infer_variant_confidence("zhconv-rs 中文简繁及地區詞轉換"));
-//! ```
 
 mod converter;
 mod utils;
 
 pub mod converters;
 pub mod tables;
 
@@ -93,16 +85,16 @@
 /// The implementation scans the input text at first to extract possible global rules like
 /// `-{H|FOO BAR}-`.
 /// If there are no global rules, the overall time complexity is `O(n + n)`.
 /// Otherwise, the overall time complexity may degrade to `O(n + n * m)` in the worst case, where
 /// `n` is input text length and `m` is the maximum lengths of source words in conversion rulesets.
 ///
 /// In case global rules support are not expected, it is better to use
-/// `get_builtin_converter(target).convert_as_wikitext_basic(text)` instead, which incurs no extra
-/// overhead.
+/// `get_builtin_converter(target).convert_as_wikitext_basic(text)` instead, which runs in O(n)
+/// in general.
 ///   
 // /// Different from the implementation of MediaWiki, this crate use a automaton which makes it
 // /// infeasible to mutate global rules during converting. So the function always searches the text
 // /// for global rules such as `-{H|FOO BAR}-` in the first pass. If such rules exists, it build a
 // /// new converter from the scratch with built-in conversion tables, which **takes extra time**.
 // /// Otherwise, it just picks a built-in converter. Then it converts the text with the chosen
 // /// converter during when non-global rules are parsed and applied.
@@ -110,167 +102,105 @@
 /// For fine-grained control and custom conversion rules, check [`ZhConverter`].
 pub fn zhconv_mw(text: &str, target: Variant) -> String {
     get_builtin_converter(target).convert_as_wikitext_extended(text)
 }
 
 /// Determine whether the given text looks like Simplified Chinese over Traditional Chinese.
 ///
-/// Equivalent to `is_hans_confidence(text) > 0.5`.
+/// Equivalent to `is_hans_probability(text) > 0.5`.
 pub fn is_hans(text: &str) -> bool {
-    is_hans_confidence(text) > 0.5
+    is_hans_probability(text) > 0.5
 }
 
 /// Determine whether the given text looks like Simplified Chinese over Traditional Chinese.
 ///
 /// The return value is a real number in the range `[0, 1]` (inclusive) that indicates
 /// confidence level. A value close to 1 indicate high confidence. A value close to 0
 /// indicates low confidence. `0.5` indicates undeterminable (half-half).
 /// If there is no enough input, `NaN` is returned.
-pub fn is_hans_confidence(text: &str) -> f32 {
-    let non_hant_score = ZH_TO_HANT_CONVERTER.count_replaced(text) as f32;
-    let non_hans_score = ZH_TO_HANS_CONVERTER.count_replaced(text) as f32;
+pub fn is_hans_probability(text: &str) -> f32 {
+    let non_hant_score = ZH_TO_HANT_CONVERTER.count_matched(text) as f32;
+    let non_hans_score = ZH_TO_HANS_CONVERTER.count_matched(text) as f32;
     // let mut ratio = if non_hans_score == 0 {
     //     f32::MAX
     // } else {
     //     non_hant_score as f32 / non_hans_score as f32
     // } - 1.0;
     // if ratio < 0.0 {
     //     ratio = -(1.0 / (ratio + 1.0) - 1.0);
     // }
     // 1f32 / (1f32 + E.powf(-ratio))
     non_hant_score / (non_hans_score + non_hant_score)
 }
 
 /// Determine the Chinese variant of the input text.
 ///
-/// # Limitations
-/// Since the built-in conversion tables does not have actual rules specific to `zh-SG` / `zh-MO` /
-/// `zh-MY`, they would never be returned.
-///
-/// The accuracy has not been assessed. Avoid relying on this for serious purposes.
+/// # Returns
+/// Possible return values are only `ZhCN`, `ZhTW` and `ZhHK`.
 pub fn infer_variant(text: &str) -> Variant {
-    // let non_cn_score = ZH_TO_CN_CONVERTER.count_replaced(text);
-    // let non_tw_score = ZH_TO_TW_CONVERTER.count_replaced(text);
-    // let non_hk_score = ZH_TO_HK_CONVERTER.count_replaced(text);
-
-    // // authored by ChatGPT
-    // if non_cn_score <= non_tw_score && non_cn_score <= non_hk_score {
-    //     Variant::ZhCN
-    // } else if non_tw_score <= non_cn_score && non_tw_score <= non_hk_score {
-    //     Variant::ZhTW
-    // } else {
-    //     Variant::ZhHK
-    // }
-    infer_variant_confidence(text)[0].0
+    let non_cn_score = ZH_TO_CN_CONVERTER.count_matched(text);
+    let non_tw_score = ZH_TO_TW_CONVERTER.count_matched(text);
+    let non_hk_score = ZH_TO_HK_CONVERTER.count_matched(text);
+
+    // authored by ChatGPT
+    if non_cn_score <= non_tw_score && non_cn_score <= non_hk_score {
+        Variant::ZhCN
+    } else if non_tw_score <= non_cn_score && non_tw_score <= non_hk_score {
+        Variant::ZhTW
+    } else {
+        Variant::ZhHK
+    }
 }
 
 /// Determine the Chinese variant of the input text with confidence.
 ///
 /// # Returns
-/// An array of `(variant, confidence_level)`, in descendent order of `confidence_level`, where
-/// `confidence_level` is in the range `[0, 1]` (inclusive). `NaN` is returned if there is no
-/// enough input.
-///
-/// # Limitations
-/// The returned `confidence_level` of script variants (`ZhHant` and `ZhHans`) are always greater
-/// than region variants (`ZhTW`, `ZhCN` and `ZhHK`) with the current implementation.
-///
-/// The accuracy has not been assessed. Avoid relying on this for serious purposes.
+/// An array of `(variant, confidence_level)`, where `confidence_level` is in the range `[0, 1]`
+/// (inclusive). It can be `NaN` if there is no enough input, .
 // /// Note that, unlike [`is_hans_confidence`](is_hans_confidence), a `confidence_level` greater
 // /// than `0.5` might not imply high enough likelihood.
 pub fn infer_variant_confidence(text: &str) -> [(Variant, f32); 5] {
     // let total = text.len() as f32;
-    let non_cn_score = ZH_TO_CN_CONVERTER.count_replaced(text) as f32;
-    let non_tw_score = ZH_TO_TW_CONVERTER.count_replaced(text) as f32;
-    let non_hk_score = ZH_TO_HK_CONVERTER.count_replaced(text) as f32;
-    let non_hant_score = ZH_TO_HANT_CONVERTER.count_replaced(text) as f32;
-    let non_hans_score = ZH_TO_HANS_CONVERTER.count_replaced(text) as f32;
+    let non_cn_score = ZH_TO_CN_CONVERTER.count_matched(text) as f32;
+    let non_tw_score = ZH_TO_TW_CONVERTER.count_matched(text) as f32;
+    let non_hk_score = ZH_TO_HK_CONVERTER.count_matched(text) as f32;
+    let non_hant_score = ZH_TO_HANT_CONVERTER.count_matched(text) as f32;
+    let non_hans_score = ZH_TO_HANS_CONVERTER.count_matched(text) as f32;
 
     let total_score = non_cn_score + non_tw_score + non_hk_score - non_hant_score;
     // let region_total = non_cn_score + non_tw_score + non_hk_score - non_hant_score;
     // let script_total = non_hant_score + non_hans_score;
-    let hans = (
-        Variant::ZhHans,
-        1f32 - non_hans_score.min(total_score) / total_score,
-    );
-    let hant = (
-        Variant::ZhHant,
-        1f32 - non_hant_score.min(total_score) / total_score,
-    );
-    let tw = (
-        Variant::ZhTW,
-        1f32 - non_tw_score.min(total_score) / total_score,
-    );
-    let cn = (
-        Variant::ZhCN,
-        1f32 - non_cn_score.min(total_score) / total_score,
-    );
-    let hk = (
-        Variant::ZhHK,
-        1f32 - non_hk_score.min(total_score) / total_score,
-    );
-    // if hk and tw cannot be distinguished, we prefer hant
-    // we always prefer hans over cn, since we cannot really distinguish cn from hans with the
-    // current implementation
-    let mut confidence_map = if tw.1 == hk.1 {
-        [hans, hant, tw, cn, hk]
-    } else {
-        [tw, hk, hant, hans, cn]
-    };
+    let mut confidence_map = [
+        (
+            Variant::ZhCN,
+            1f32 - non_cn_score.min(total_score) / total_score,
+        ),
+        (
+            Variant::ZhTW,
+            1f32 - non_tw_score.min(total_score) / total_score,
+        ),
+        (
+            Variant::ZhHK,
+            1f32 - non_hk_score.min(total_score) / total_score,
+        ),
+        (
+            Variant::ZhHans,
+            1f32 - non_hans_score.min(total_score) / total_score,
+        ),
+        (
+            Variant::ZhHant,
+            1f32 - non_hant_score.min(total_score) / total_score,
+        ),
+    ];
     // let mut confidence_map = [(Variant::ZhCN, 1f32 - non_cn_score / region_total),(Variant::ZhTW, 1f32 - non_tw_score / region_total),(Variant::ZhHK, 1f32 - non_hk_score / region_total),(Variant::ZhHans,1f32 - non_hans_score / script_total),(Variant::ZhHant, 1f32 - non_hant_score / script_total)];
     // let mut confidence_map = [(Variant::ZhCN, non_cn_score),(Variant::ZhTW, non_tw_score),(Variant::ZhHK, non_hk_score),(Variant::ZhHans,non_hans_score),(Variant::ZhHant, non_hant_score), (Variant::Zh, total)];
 
     // let mut confidence_map = [
     //     (Variant::ZhCN, 1f32 - non_cn_score / total),
     //     (Variant::ZhTW, 1f32 - non_tw_score / total),
     //     (Variant::ZhHK, 1f32 - non_hk_score / total),
     //     (Variant::ZhHans, 1f32 - non_hans_score / total),
     //     (Variant::ZhHant, 1f32 - non_hant_score / total),
     // ];
     confidence_map.sort_by(|a, b| b.1.total_cmp(&a.1));
     confidence_map
 }
-
-/// A helper trait that truncates a str around a specified index in constant time (`O(1)`),
-/// intended to be used with `is_hans` and etc.
-pub trait TruncatedAround {
-    /// Truncate a str around the given index in constant time (`O(1)`).
-    ///
-    /// This method is intended to be used together with other functions like `is_hans` and
-    /// `infer_variant`, especially when dealing with large input texts that need to be processed
-    /// efficiently while tolerating less accuracy.
-    /// Note that this trait does not guarantee whether the truncation index is rounded up or down.
-    ///
-    /// # Examples
-    ///
-    /// ```
-    /// use zhconv::{TruncatedAround, is_hans};
-    /// use std::fs;
-    ///
-    /// let s = "鵲飛空繞樹月輪殊未圓";
-    /// assert_eq!(s.len(), 30);
-    /// assert_eq!(s.truncated_around(15), "鵲飛空繞樹");
-    /// assert_eq!(s.truncated_around(100), s);
-    ///
-    /// let ls = fs::read_to_string("benches/data3185k.txt").unwrap(); // long string
-    /// let tls = ls.truncated_around(100 * 1024 + 123); // truncated to ~ 100KiB
-    /// assert_eq!(is_hans(&ls), is_hans(&tls));
-    /// ```
-    fn truncated_around(&self, index: usize) -> &Self;
-}
-
-impl TruncatedAround for str {
-    fn truncated_around(&self, index: usize) -> &Self {
-        // Ref: std::str::ceil_char_boundary
-        if index > self.len() {
-            self
-        } else {
-            let upper_bound = Ord::min(index + 4, self.len());
-            for end in index..upper_bound {
-                if self.is_char_boundary(end) {
-                    return &self[..end];
-                }
-            }
-            unreachable!()
-        }
-    }
-}
```

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/src/pagerules.rs` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/pagerules.rs`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/src/rule.rs` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/rule.rs`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
             Map(m) => Some(m),
             _ => None,
         }
     }
 
     /// Get the inner bi-directional map, if any.
     ///
-    /// Typically intended to be used by [`PageRules`](crate::pagerules::PageRules) to extract the
+    /// Typically intended to be used by [`PageRules`](crate::pagerules:PageRules) to extract the
     /// map for a page title (e.g. `-{T|zh:黑;zh-cn:白}-`).
     pub fn get_bid(&self) -> Option<&VariantMap<String>> {
         self.as_map().map(|m| &m.bid)
     }
 
     /// Same as `from_str`, except that any unrecognized conv is treated as [`Conv::Asis`]
     pub fn from_str_infallible(s: &str) -> Conv {
```

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/src/tables.rs` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/tables.rs`

 * *Files 1% similar despite different names*

```diff
@@ -199,16 +199,16 @@
         .target(variant)
         .table(table)
         .build()
 }
 
 /// Get the builtin conversion tables for a target Chinese variant.
 ///
-/// Accessing raw tables are only useful when building a custom converter.
-/// Otherwise, there is [`get_builtin_converter`](crate::get_builtin_converter).
+/// Accessing raw tables are only necessary when building a custom converter.
+/// Otherwise, there is [`get_builtin_converter`].
 #[inline(always)]
 pub fn get_builtin_tables(target: Variant) -> &'static [Table<'static>] {
     use Variant::*;
 
     match target {
         Zh => &ZH_TABLES,
         ZhHant => &ZH_HANT_TABLES,
```

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/src/utils.rs` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/utils.rs`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     ($($item:item)*) => {$(
         #[cfg(target_arch = "wasm32")]
         $item
     )*}
 }
 pub(crate) use for_wasm;
 
-#[cfg(feature = "compress")]
 pub fn zstd_decompress(bytes: &[u8]) -> Vec<u8> {
     use std::io::Read;
 
     let mut buf = vec![];
     ruzstd::StreamingDecoder::new(bytes)
         .unwrap()
         .read_to_end(&mut buf)
```

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/src/variant.rs` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/variant.rs`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/src/wasm.rs` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/src/wasm.rs`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/README.md` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/README.md`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/bench.tmp` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/bench.tmp`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/config-overrides.js` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/config-overrides.js`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/package.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/package.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/public/cgroups.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/cgroups.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/public/index.html` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/index.html`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/public/logo.ico` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/logo.ico`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/public/logo192.png` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/logo192.png`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/public/logo512.png` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/public/logo512.png`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/rustup.sh` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/rustup.sh`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/App.css` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/App.css`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/App.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/App.tsx`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/AboutDialog.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/AboutDialog.tsx`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/CGroupCheckbox.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/CGroupCheckbox.tsx`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/CGroupSelect.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/CGroupSelect.tsx`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/ConvertButton.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/ConvertButton.tsx`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/Footer.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/Footer.tsx`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/Header.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/Header.tsx`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/InputEditor.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/InputEditor.tsx`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/OptionsControl.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/OptionsControl.tsx`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/OutputEditor.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/OutputEditor.tsx`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/components/OutputStatusLine.tsx` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/components/OutputStatusLine.tsx`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/src/logo.svg` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/src/logo.svg`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/tsconfig.json` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/tsconfig.json`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/local_dependencies/zhconv/web/yarn.lock` & `zhconv_rs-0.3.0b0/local_dependencies/zhconv/web/yarn.lock`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/Cargo.toml` & `zhconv_rs-0.3.0b0/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [package]
 name = "zhconv-pyo3"
-version = "0.3.0"
+version = "0.3.0-beta"
 edition = "2021"
 authors = ["Hung-I Wang <whygowe@gmail.com>"]
 license = "GPL-2.0-or-later"
 repository = "https://github.com/Gowee/zhconv-rs"
 description = "zhconv as in MediaWiki with extra rulesets from OpenCC, oxidized with more efficiency 🦀"
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "zhconv_rs"
 crate-type = ["cdylib"]
 
 [dependencies]
 zhconv = { path = "local_dependencies/zhconv" }
-pyo3 = { version = "0.19", features = ["extension-module"] }
-pyo3-file = "0.7.0"
+pyo3 = { version = "0.16", features = ["extension-module"] }
+pyo3-file = "0.5.0"
```

### Comparing `zhconv_rs-0.3.0/.gitignore` & `zhconv_rs-0.3.0b0/.gitignore`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/README.md` & `zhconv_rs-0.3.0b0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 [![docs.rs](https://docs.rs/zhconv/badge.svg)](https://docs.rs/zhconv)
 [![Crates.io](https://img.shields.io/crates/v/zhconv.svg)](https://crates.io/crates/zhconv)
 [![PyPI version](https://img.shields.io/pypi/v/zhconv-rs)](https://pypi.org/project/zhconv-rs/)
 [![NPM version](https://badge.fury.io/js/zhconv.svg)](https://www.npmjs.com/package/zhconv)
 # zhconv-rs 中文简繁及地區詞轉換
 zhconv-rs converts Chinese text among traditional/simplified scripts or regional variants (e.g. `zh-TW <-> zh-CN <-> zh-HK <-> zh-Hans <-> zh-Hant`), built on the top of rulesets from MediaWiki/Wikipedia and OpenCC.
 
-The implementation is powered by an [Aho-Corasick](https://github.com/daac-tools/daachorse) automaton, ensuring linear time complexity with respect to the length of input text and conversion rules (`O(n+m)`), processing dozens of MiBs text per second.
+The implementation is powered by the [Aho-Corasick](https://github.com/BurntSushi/aho-corasick) automaton, ensuring linear time complexity with respect to the length of input text and conversion rules (`O(n+m)`), processing dozens of MiBs text per second.
 
 🔗 **Web App: https://zhconv.pages.dev** (powered by WASM)
 
 ⚙️ **Cli**: `cargo install zhconv-cli` or check [releases](https://github.com/Gowee/zhconv-rs/releases).
 
-🦀 **Rust Crate**: `cargo add zhconv` (check [docs](https://docs.rs/zhconv/latest/zhconv/) for examples)
+🦀 **Rust Crate**: `cargo add zhconv` (see doc comments and [cli/](https://github.com/Gowee/zhconv-rs/tree/main/cli) for examples)
 
 🐍 **Python Package via PyO3**: `pip install zhconv-rs` (WASM with wheels)
 
 <details open>
  <summary>Python snippet</summary>
 
 ```python
@@ -116,19 +116,17 @@
 The benchmark was performed on a previous version that had only Mediawiki rulesets. In the newer version, with OpenCC rulesets activated by default, the performance may degrade ~2x.
 
 ## Differences with other converters
 * `ZhConver{sion,ter}.php` of MediaWiki: zhconv-rs just takes conversion tables listed in [`ZhConversion.php`](https://github.com/wikimedia/mediawiki/blob/master/includes/languages/data/ZhConversion.php#L14). MediaWiki relies on the inefficient PHP built-in function [`strtr`](https://github.com/php/php-src/blob/217fd932fa57d746ea4786b01d49321199a2f3d5/ext/standard/string.c#L2974). Under the basic mode, zhconv-rs guarantees linear time complexity (`T = O(n+m)` instead of `O(nm)`) and single-pass scanning of input text. Optionally, zhconv-rs supports the same conversion rule syntax with MediaWiki.
 * OpenCC: The [conversion rulesets](https://github.com/BYVoid/OpenCC/tree/master/data/dictionary) of OpenCC is independent of MediaWiki. The core [conversion implementation](https://github.dev/BYVoid/OpenCC/blob/21995f5ea058441423aaff3ee89b0a5d4747674c/src/Conversion.cpp#L27) of OpenCC is kinda similar to the aforementioned `strtr`. However, OpenCC supports pre-segmentation and maintains multiple rulesets which are applied successively. By contrast, the Aho-Corasick-powered zhconv-rs merges rulesets from MediaWiki and OpenCC in compile time and converts text in single-pass linear time, resulting in much more efficiency. Though, conversion results may differ in some cases.
 
 ## Limitations
-The converter takes leftmost-longest matching strategy. It gives priority to the leftmost-matched words or phrases. For instance, if a ruleset includes both `干 -> 幹` and `天干物燥 -> 天乾物燥`, the converter would prioritize `天乾物燥` because `天干物燥` gets matched earlier compared to `干` at a later position. The strategy yields good results in general, but may occasionally lead to wrong conversions.
+The converter utilizes an aho-corasick automaton with the leftmost-longest matching strategy. This strategy gives priority to the leftmost-matched words or phrases. For instance, if a ruleset includes both `干 -> 幹` and `天干物燥 -> 天乾物燥`, the converter would prioritize `天乾物燥` because `天干物燥` gets matched earlier compared to `干` at a later position. The strategy is generally effective but may occasionally lead to unexpected results.
 
-The implementation support most of the MediaWiki conversion rules. But it is not fully compliant with the original implementation.
-
-Besides, for wikitext, if input text contains global conversion rules (in MediaWiki syntax like -{H|zh-hans:鹿|zh-hant:马}-), the time complexity of the implementation may degrade to `O(n*m)` where `n` and `m` are the length of the text and the maximum lengths of sources words in conversion rulesets in the worst case (equivalent to brute-force).
+Futuremore, since an automaton is infeasible to update after being built, the converter must (re)build it from scratch for every ruleset. The automata for built-in rulesets (i.e. conversion tables) are built on demand and cached by default. However, if a short input text contains global conversion rules (in MediaWiki syntax like -{H|zh-hans:鹿|zh-hant:马}-), this process incurs a significant overhead, potentially being less efficient than a naive implementation.
 
 ## Credits
 All rulesets that power the converter come from the [MediaWiki](https://github.com/wikimedia/mediawiki) project and [OpenCC](https://github.com/BYVoid/OpenCC).
 
 The project takes the following projects/pages as references:
 - https://github.com/gumblex/zhconv : Python implementation of `zhConver{ter,sion}.php`.
 - https://github.com/BYVoid/OpenCC/ : Widely adopted Chinese converter.
```

#### html2text {}

```diff
@@ -4,25 +4,25 @@
 img.shields.io/crates/v/zhconv.svg)](https://crates.io/crates/zhconv) [![PyPI
 version](https://img.shields.io/pypi/v/zhconv-rs)](https://pypi.org/project/
 zhconv-rs/) [![NPM version](https://badge.fury.io/js/zhconv.svg)](https://
 www.npmjs.com/package/zhconv) # zhconv-rs ä¸­æç®ç¹åå°åè©è½æ
 zhconv-rs converts Chinese text among traditional/simplified scripts or
 regional variants (e.g. `zh-TW <-> zh-CN <-> zh-HK <-> zh-Hans <-> zh-Hant`),
 built on the top of rulesets from MediaWiki/Wikipedia and OpenCC. The
-implementation is powered by an [Aho-Corasick](https://github.com/daac-tools/
-daachorse) automaton, ensuring linear time complexity with respect to the
+implementation is powered by the [Aho-Corasick](https://github.com/BurntSushi/
+aho-corasick) automaton, ensuring linear time complexity with respect to the
 length of input text and conversion rules (`O(n+m)`), processing dozens of MiBs
 text per second. ð **Web App: https://zhconv.pages.dev** (powered by WASM)
 âï¸ **Cli**: `cargo install zhconv-cli` or check [releases](https://
 github.com/Gowee/zhconv-rs/releases). ð¦ **Rust Crate**: `cargo add zhconv`
-(check [docs](https://docs.rs/zhconv/latest/zhconv/) for examples) ð
-**Python Package via PyO3**: `pip install zhconv-rs` (WASM with wheels)  Python
-snippet ```python # > pip install zhconv_rs # Convert with builtin rulesets:
-from zhconv_rs import zhconv assert zhconv("å¤©å¹²ç©ç¥ å°å¿ç«ç", "zh-
-tw") == "å¤©ä¹¾ç©ç¥ å°å¿ç«ç­" assert zhconv
+(see doc comments and [cli/](https://github.com/Gowee/zhconv-rs/tree/main/cli)
+for examples) ð **Python Package via PyO3**: `pip install zhconv-rs` (WASM
+with wheels)  Python snippet ```python # > pip install zhconv_rs # Convert with
+builtin rulesets: from zhconv_rs import zhconv assert zhconv("å¤©å¹²ç©ç¥
+å°å¿ç«ç", "zh-tw") == "å¤©ä¹¾ç©ç¥ å°å¿ç«ç­" assert zhconv
 ("é§å¤±æ¨èºï¼æè¿·æ´¥æ¸¡", "zh-hans") == "é¾å¤±æ¥¼å°ï¼æè¿·æ´¥æ¸¡"
 assert zhconv("ã-{zh-hans:ä¸ä¸ªç«æªæ;zh-hant:ä¸åå®¢;zh-tw:ä¸åå®¢}-
 ãæ¯äºæ­·å±±å¤§Â·ä»²é¦¬çä½åã", "zh-cn", mediawiki=True) ==
 "ãä¸ä¸ªç«æªæãæ¯äºåå±±å¤§Â·ä»²é©¬çä½åã" assert zhconv("-
 {H|zh-cn:é¾é½å­¤å¿;zh-tw:å­¤éæ·;zh-hk:è¦æµ·å­¤é;zh-sg:é¾é½å­¤å¿;zh-
 mo:è¦æµ·å­¤é;}-ãé¾é½å­¤å¿ãæ¯æ¥å°æ¯Â·çæ´æ¯çä½åã", "zh-
 tw", True) == "ãå­¤éæ·ãæ¯æ¥ç¾æ¯Â·çæ´æ¯çä½åã" # Convert
@@ -80,31 +80,31 @@
 implementation](https://github.dev/BYVoid/OpenCC/blob/
 21995f5ea058441423aaff3ee89b0a5d4747674c/src/Conversion.cpp#L27) of OpenCC is
 kinda similar to the aforementioned `strtr`. However, OpenCC supports pre-
 segmentation and maintains multiple rulesets which are applied successively. By
 contrast, the Aho-Corasick-powered zhconv-rs merges rulesets from MediaWiki and
 OpenCC in compile time and converts text in single-pass linear time, resulting
 in much more efficiency. Though, conversion results may differ in some cases.
-## Limitations The converter takes leftmost-longest matching strategy. It gives
-priority to the leftmost-matched words or phrases. For instance, if a ruleset
-includes both `å¹² -> å¹¹` and `å¤©å¹²ç©ç¥ -> å¤©ä¹¾ç©ç¥`, the converter
-would prioritize `å¤©ä¹¾ç©ç¥` because `å¤©å¹²ç©ç¥` gets matched earlier
-compared to `å¹²` at a later position. The strategy yields good results in
-general, but may occasionally lead to wrong conversions. The implementation
-support most of the MediaWiki conversion rules. But it is not fully compliant
-with the original implementation. Besides, for wikitext, if input text contains
-global conversion rules (in MediaWiki syntax like -{H|zh-hans:é¹¿|zh-hant:é©¬}-
-), the time complexity of the implementation may degrade to `O(n*m)` where `n`
-and `m` are the length of the text and the maximum lengths of sources words in
-conversion rulesets in the worst case (equivalent to brute-force). ## Credits
-All rulesets that power the converter come from the [MediaWiki](https://
-github.com/wikimedia/mediawiki) project and [OpenCC](https://github.com/BYVoid/
-OpenCC). The project takes the following projects/pages as references: - https:
-//github.com/gumblex/zhconv : Python implementation of `zhConver
-{ter,sion}.php`. - https://github.com/BYVoid/OpenCC/ : Widely adopted Chinese
-converter. - https://zh.wikipedia.org/wiki/Wikipedia:å­è©è½æèç -
-https://zh.wikipedia.org/wiki/Help:é«çº§å­è¯è½¬æ¢è¯­æ³ - https://
-github.com/wikimedia/mediawiki/blob/master/includes/language/
-LanguageConverter.php  ## TODO - [x] Support [Module:CGroup](https://
-zh.wikipedia.org/wiki/Module:CGroup) - [ ] Propogate error properly with Anyhow
-and thiserror - [x] Python lib - [x] More exmaples in README - [x] Add rulesets
-from OpenCC
+## Limitations The converter utilizes an aho-corasick automaton with the
+leftmost-longest matching strategy. This strategy gives priority to the
+leftmost-matched words or phrases. For instance, if a ruleset includes both
+`å¹² -> å¹¹` and `å¤©å¹²ç©ç¥ -> å¤©ä¹¾ç©ç¥`, the converter would prioritize
+`å¤©ä¹¾ç©ç¥` because `å¤©å¹²ç©ç¥` gets matched earlier compared to `å¹²` at
+a later position. The strategy is generally effective but may occasionally lead
+to unexpected results. Futuremore, since an automaton is infeasible to update
+after being built, the converter must (re)build it from scratch for every
+ruleset. The automata for built-in rulesets (i.e. conversion tables) are built
+on demand and cached by default. However, if a short input text contains global
+conversion rules (in MediaWiki syntax like -{H|zh-hans:é¹¿|zh-hant:é©¬}-), this
+process incurs a significant overhead, potentially being less efficient than a
+naive implementation. ## Credits All rulesets that power the converter come
+from the [MediaWiki](https://github.com/wikimedia/mediawiki) project and
+[OpenCC](https://github.com/BYVoid/OpenCC). The project takes the following
+projects/pages as references: - https://github.com/gumblex/zhconv : Python
+implementation of `zhConver{ter,sion}.php`. - https://github.com/BYVoid/OpenCC/
+: Widely adopted Chinese converter. - https://zh.wikipedia.org/wiki/Wikipedia:
+å­è©è½æèç - https://zh.wikipedia.org/wiki/Help:
+é«çº§å­è¯è½¬æ¢è¯­æ³ - https://github.com/wikimedia/mediawiki/blob/master/
+includes/language/LanguageConverter.php  ## TODO - [x] Support [Module:CGroup]
+(https://zh.wikipedia.org/wiki/Module:CGroup) - [ ] Propogate error properly
+with Anyhow and thiserror - [x] Python lib - [x] More exmaples in README - [x]
+Add rulesets from OpenCC
```

### Comparing `zhconv_rs-0.3.0/pyproject.toml` & `zhconv_rs-0.3.0b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zhconv_rs-0.3.0/Cargo.lock` & `zhconv_rs-0.3.0b0/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "aho-corasick"
+version = "0.7.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1e37cfd5e7657ada45f742d6e99ca5788580b5c529dc78faf11ece6dc702656f"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
+name = "aho-corasick"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
@@ -27,26 +36,26 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "block-buffer"
-version = "0.10.4"
+version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
+checksum = "0bf7fe51849ea569fd452f37822f606a5cabb684dc918707a0193fd4664ff324"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.13.0"
+version = "3.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
+checksum = "37ccbd214614c6783386c1af30caf03192f17891059cecc394b4fb119e363de3"
 
 [[package]]
 name = "bytecount"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c676a478f63e9fa2dd5368a42f28bba0d6c560b775f38583c8bbaa7fcd67c9c"
 
@@ -54,17 +63,17 @@
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
 [[package]]
 name = "camino"
-version = "1.1.4"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c530edf18f37068ac2d977409ed5cd50d53d73bc653c7647b48eb78976ac9ae2"
+checksum = "35176a56fa5f5efe08df85cd5e68158471c2fa7057e85a5356ee4bd9787a6df9"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "cargo-platform"
 version = "0.1.2"
@@ -110,17 +119,17 @@
 dependencies = [
  "cfg-if",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.8"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
+checksum = "59a6001667ab124aebae2a495118e11d30984c3a653e99d86d58971708cf5e4b"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crypto-common"
 version = "0.1.6"
@@ -135,141 +144,103 @@
 name = "daachorse"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "63b7ef7a4be509357f4804d0a22e830daddb48f19fd604e4ad32ddce04a94c36"
 
 [[package]]
 name = "digest"
-version = "0.10.7"
+version = "0.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
+checksum = "f2fb860ca6fafa5552fb6d0e816a69c8e49f0908bf524e30a90d97c85892d506"
 dependencies = [
  "block-buffer",
  "crypto-common",
 ]
 
 [[package]]
 name = "either"
-version = "1.8.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
-
-[[package]]
-name = "errno"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
-dependencies = [
- "errno-dragonfly",
- "libc",
- "windows-sys",
-]
-
-[[package]]
-name = "errno-dragonfly"
-version = "0.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
-dependencies = [
- "cc",
- "libc",
-]
+checksum = "3f107b87b6afc2a64fd13cac55fe06d6c8859f12d4b14cbcdd2c67d0976781be"
 
 [[package]]
 name = "error-chain"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2d2f06b9cac1506ece98fe3231e3cc9c4410ec3d5b1f24ae1c8946f0742cdefc"
 dependencies = [
  "version_check",
 ]
 
 [[package]]
 name = "fastrand"
-version = "1.9.0"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
+checksum = "a7a407cfaa3385c4ae6b23e84623d48c2798d06e3e6a1878f7f59f17b3f86499"
 dependencies = [
  "instant",
 ]
 
 [[package]]
 name = "generic-array"
-version = "0.14.7"
+version = "0.14.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
+checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "glob"
-version = "0.3.1"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
+checksum = "9b919933a397b79c37e33b77bb2aa3dc8eb6e165ad809e58ff75bc7db2e34574"
 
 [[package]]
 name = "heck"
-version = "0.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
-
-[[package]]
-name = "hermit-abi"
-version = "0.3.2"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
+checksum = "2540771e65fc8cb83cd6e8a237f70c319bd5c29f78ed1084ba5d50eeac86f7f9"
 
 [[package]]
 name = "hex-literal"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6fe2267d4ed49bc07b63801559be28c718ea06c4738b7a03c94df7386d2cde46"
 
 [[package]]
 name = "indoc"
-version = "1.0.9"
+version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
+checksum = "adab1eaa3408fb7f0c777a73e7465fd5656136fc93b670eb6df3c88c2c1344e3"
 
 [[package]]
 name = "instant"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
-name = "io-lifetimes"
-version = "1.0.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
-dependencies = [
- "hermit-abi",
- "libc",
- "windows-sys",
-]
-
-[[package]]
 name = "itertools"
-version = "0.10.5"
+version = "0.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
+checksum = "a9a9d19fa1e79b6215ff29b9d6880b706147f16e9b1dbb1e4e5947b5b02bc5e3"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.8"
+version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b02a5381cc465bd3041d84623d0fa3b66738b52b8e2fc3bab8ad63ab032f4a"
+checksum = "6c8af84674fe1f223a982c933a0ee1086ac4d4052aa0fb8060c12c6ad838e754"
 
 [[package]]
 name = "jobserver"
 version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
 dependencies = [
@@ -280,260 +251,242 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.147"
+version = "0.2.131"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
-
-[[package]]
-name = "linux-raw-sys"
-version = "0.3.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
+checksum = "04c3b4822ccebfa39c02fc03d1534441b22ead323fa0f48bb7ddd8e6ba076a40"
 
 [[package]]
 name = "lock_api"
-version = "0.4.10"
+version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
+checksum = "327fa5b6a6940e4699ec49a9beae1ea4845c6bab9314e4f84ac68742139d8c53"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.19"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
-
-[[package]]
-name = "memchr"
-version = "2.5.0"
+version = "0.4.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
+checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
+dependencies = [
+ "cfg-if",
+]
 
 [[package]]
-name = "memoffset"
-version = "0.9.0"
+name = "lz4_flex"
+version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "8b8c72594ac26bfd34f2d99dfced2edfaddfe8a476e3ff2ca0eb293d925c4f83"
 dependencies = [
- "autocfg",
+ "twox-hash",
 ]
 
 [[package]]
-name = "num_threads"
-version = "0.1.6"
+name = "memchr"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2819ce041d2ee131036f4fc9d6ae7ae125a3a40e97ba64d04fe799ad9dabbb44"
-dependencies = [
- "libc",
-]
+checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "once_cell"
-version = "1.18.0"
+version = "1.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
+checksum = "18a6dbe30758c9f83eb00cbea4ac95966305f5a7772f3f42ebfc7fc7eddbd8e1"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.8"
+version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
+checksum = "09a279cbf25cb0757810394fbc1e359949b59e348145c643a939a525692e6929"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets",
+ "windows-sys",
 ]
 
 [[package]]
 name = "pkg-config"
 version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.63"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
+checksum = "0a2ca2c61bc9f3d74d2886294ab7b9853abd9c1ad903a3ac7815c58989bb7bab"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pulldown-cmark"
-version = "0.9.3"
+version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77a1a2f1f0a7ecff9c31abbe177637be0e97a0aef46cf8738ece09327985d998"
+checksum = "2d9cc634bc78768157b5cbfe988ffcd1dcba95cd2b2f03a88316c08c6d00ed63"
 dependencies = [
  "bitflags",
  "memchr",
  "unicase",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.1"
+version = "0.16.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
+checksum = "1e6302e85060011447471887705bb7838f14aba43fcb06957d823739a496b3dc"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.1"
+version = "0.16.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
+checksum = "b5b65b546c35d8a3b1b2f0ddbac7c6a569d759f357f2b9df884f5d6b719152c8"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.1"
+version = "0.16.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
+checksum = "c275a07127c1aca33031a563e384ffdd485aee34ef131116fcd58e3430d1742b"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-file"
-version = "0.7.0"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c655228ceebe0180211c009dade97a1d5f3e86704caec35ddeb2c7661543654"
+checksum = "f8ac3c7c77af01cb16e2e794571e3b77375a11ce24439e57b3cf2bfb5a6aecc0"
 dependencies = [
  "pyo3",
  "skeptic",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.1"
+version = "0.16.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
+checksum = "284fc4485bfbcc9850a6d661d627783f18d19c2ab55880b021671c4ba83e90f7"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 1.0.109",
+ "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.1"
+version = "0.16.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
+checksum = "53bda0f58f73f5c5429693c96ed57f7abdb38fdfc28ae06da4101a257adb7faf"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.29"
+version = "1.0.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
+checksum = "bbe448f377a7d6961e30f5955f9b8d106c3f5e449d493ee1b125c1d43c2b5179"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.3.5"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.4"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
+checksum = "4c4eb3267174b8c6c2f654116623910a0fef09c4753f8dd83db29c48a0df988b"
 dependencies = [
- "aho-corasick",
+ "aho-corasick 0.7.18",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.2"
+version = "0.6.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+checksum = "a3f87b73ce11b1619a3c6332f45341e0047173771e8b8b73f87bfeefb7b56244"
 
 [[package]]
-name = "rustix"
-version = "0.37.22"
+name = "remove_dir_all"
+version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8818fa822adcc98b18fedbb3632a6a33213c070556b5aa7c4c8cc21cff565c4c"
+checksum = "3acd125665422973a33ac9d3dd2df85edad0f4ae9b00dafb1a05e43a9f5ef8e7"
 dependencies = [
- "bitflags",
- "errno",
- "io-lifetimes",
- "libc",
- "linux-raw-sys",
- "windows-sys",
+ "winapi",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.13"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc31bd9b61a32c31f9650d18add92aa83a49ba979c143eefd27fe7177b05bd5f"
+checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
 
 [[package]]
 name = "ruzstd"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3ffab8f9715a0d455df4bbb9d21e91135aab3cd3ca187af0cd0c3c3f868fdc"
 dependencies = [
  "byteorder",
  "thiserror-core",
  "twox-hash",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.14"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fe232bdf6be8c8de797b22184ee71118d63780ea42ac85b61d1baa6d3b782ae9"
+checksum = "4501abdff3ae82a1c1b477a17252eb69cee9e66eb915c1abaa4f44d873df9f09"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
@@ -544,57 +497,57 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "semver"
-version = "1.0.17"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
+checksum = "93f6841e709003d68bb2deee8c343572bf446003ec20a583e76f7b15cebf3711"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.166"
+version = "1.0.143"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d01b7404f9d441d3ad40e6a636a7782c377d2abdbe4fa2440e2edcc2f4f10db8"
+checksum = "53e8e5d5b70924f74ff5c6d64d9a5acd91422117c60f48c4e07855238a254553"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.166"
+version = "1.0.143"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5dd83d6dde2b6b2d466e14d9d1acce8816dedee94f735eac6395808b3483c6d6"
+checksum = "d3d8e8de557aee63c26b85b947f5e59b690d0454c753f3adeb5cd7835ab88391"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.99"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
+checksum = "38dd04e3c8279e75b31ef29dbdceebfe5ad89f4d0937213c53f7d49d01b3d5a7"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "sha2"
-version = "0.10.7"
+version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "479fb9d862239e610720565ca91403019f2f00410f1864c5aa7479b950a76ed8"
+checksum = "55deaec60f81eefe3cce0dc50bda92d6d8e88f2a27df7c5033b42afeb1ed2676"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
@@ -610,17 +563,17 @@
  "pulldown-cmark",
  "tempfile",
  "walkdir",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "2fd0db749597d91ff862fd1d55ea87f7855a744a8425a64695b6fca237d1dad1"
 
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
@@ -639,57 +592,46 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e385be0d24f186b4ce2f9982191e7101bb737312ad61c1f2f984f34bcf85d59"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 1.0.109",
-]
-
-[[package]]
-name = "syn"
-version = "1.0.109"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
-dependencies = [
- "proc-macro2",
- "quote",
- "unicode-ident",
+ "syn",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.23"
+version = "1.0.99"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "59fb7d6d8281a51045d62b8eb3a7d1ce347b76f312af50cd3dc0af39c87c1737"
+checksum = "58dbef6ec655055e20b86b15a8cc6d439cca19b667537ac6a1369572d151ab13"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.8"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
+checksum = "c02424087780c9b71cc96799eaeddff35af2bc513278cda5c99fc1f5d026d3c1"
 
 [[package]]
 name = "tempfile"
-version = "3.6.0"
+version = "3.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
+checksum = "5cdb1ef4eaeeaddc8fbd371e5017057064af0911902ef36b39801f67cc6d79e4"
 dependencies = [
- "autocfg",
  "cfg-if",
  "fastrand",
+ "libc",
  "redox_syscall",
- "rustix",
- "windows-sys",
+ "remove_dir_all",
+ "winapi",
 ]
 
 [[package]]
 name = "thiserror-core"
 version = "1.0.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d97345f6437bb2004cd58819d8a9ef8e36cdd7661c2abc4bbde0a7c40d9f497"
@@ -701,26 +643,24 @@
 name = "thiserror-core-impl"
 version = "1.0.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "10ac1c5050e43014d16b2f94d0d2ce79e65ffdd8b38d8048f9c8f6a8a6da62ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn",
 ]
 
 [[package]]
 name = "time"
 version = "0.3.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
 dependencies = [
  "itoa",
- "libc",
- "num_threads",
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
@@ -745,119 +685,120 @@
 dependencies = [
  "cfg-if",
  "static_assertions",
 ]
 
 [[package]]
 name = "typenum"
-version = "1.16.0"
+version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
+checksum = "dcf81ac59edc17cc8697ff311e8f5ef2d99fcbd9817b34cec66f90b6c3dfd987"
 
 [[package]]
 name = "unicase"
 version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50f37be617794602aabbeee0be4f259dc1778fabe05e2d67ee8f79326d5cb4f6"
 dependencies = [
  "version_check",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.10"
+version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
+checksum = "c4f5b37a154999a8f3f98cc23a628d850e154479cd94decf3414696e12e31aaf"
 
 [[package]]
 name = "unindent"
-version = "0.1.11"
+version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+checksum = "58ee9362deb4a96cef4d437d1ad49cffc9b9e92d202b6995674e928ce684f112"
 
 [[package]]
 name = "vergen"
-version = "8.2.3"
+version = "8.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce38fc503fa57441ac2539c3e723b5adf76601eb4f1ad24025c6660d27f355b7"
+checksum = "8b3c89c2c7e50f33e4d35527e5bf9c11d6d132226dbbd1753f0fbe9f19ef88c6"
 dependencies = [
  "anyhow",
  "rustversion",
  "time",
 ]
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
-version = "2.3.3"
+version = "2.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "36df944cda56c7d8d8b7496af378e6b16de9284591917d307c9b4d313c44e698"
+checksum = "808cf2735cd4b6866113f648b791c6adc5714537bc222d9347bb203386ffda56"
 dependencies = [
  "same-file",
+ "winapi",
  "winapi-util",
 ]
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.87"
+version = "0.2.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
+checksum = "fc7652e3f6c4706c8d9cd54832c4a4ccb9b5336e2c3bd154d5cccfbf1c1f5f7d"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.87"
+version = "0.2.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
+checksum = "662cd44805586bd52971b9586b1df85cdbbd9112e4ef4d8f41559c334dc6ac3f"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.87"
+version = "0.2.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
+checksum = "b260f13d3012071dfb1512849c033b1925038373aea48ced3012c09df952c602"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.87"
+version = "0.2.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
+checksum = "5be8e654bdd9b79216c2929ab90721aa82faf65c48cdf08bdc4e7f51357b80da"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.87"
+version = "0.2.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
+checksum = "6598dd0bd3c7d51095ff6531a5b23e02acdc81804e30d8f07afb77b7215a140a"
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
@@ -884,100 +825,79 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-sys"
-version = "0.48.0"
+version = "0.36.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+checksum = "ea04155a16a59f9eab786fe12a4a450e75cdb175f9e0d80da1e17db09f55b8d2"
 dependencies = [
- "windows-targets",
-]
-
-[[package]]
-name = "windows-targets"
-version = "0.48.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
-dependencies = [
- "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
-name = "windows_aarch64_gnullvm"
-version = "0.48.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
-
-[[package]]
 name = "windows_aarch64_msvc"
-version = "0.48.0"
+version = "0.36.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+checksum = "9bb8c3fd39ade2d67e9874ac4f3db21f0d710bee00fe7cab16949ec184eeaa47"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.48.0"
+version = "0.36.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+checksum = "180e6ccf01daf4c426b846dfc66db1fc518f074baa793aa7d9b9aaeffad6a3b6"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.48.0"
+version = "0.36.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+checksum = "e2e7917148b2812d1eeafaeb22a97e4813dfa60a3f8f78ebe204bcc88f12f024"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.48.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
-version = "0.48.0"
+version = "0.36.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+checksum = "4dcd171b8776c41b97521e5da127a2d86ad280114807d0b2ab1e462bc764d9e1"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.48.0"
+version = "0.36.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+checksum = "c811ca4a8c853ef420abd8592ba53ddbbac90410fab6903b3e79972a631f7680"
 
 [[package]]
 name = "zhconv"
-version = "0.3.0"
+version = "0.3.0-beta"
 dependencies = [
+ "aho-corasick 1.0.2",
  "console_error_panic_hook",
  "daachorse",
  "hex-literal",
  "itertools",
  "lazy_static",
+ "lz4_flex",
  "once_cell",
  "regex",
  "ruzstd",
  "sha2",
  "strum",
  "vergen",
  "wasm-bindgen",
  "zstd",
 ]
 
 [[package]]
 name = "zhconv-pyo3"
-version = "0.3.0"
+version = "0.3.0-beta"
 dependencies = [
  "pyo3",
  "pyo3-file",
  "zhconv",
 ]
 
 [[package]]
```

### Comparing `zhconv_rs-0.3.0/PKG-INFO` & `zhconv_rs-0.3.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhconv-rs
-Version: 0.3.0
+Version: 0.3.0b0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Natural Language :: Chinese (Traditional)
 Classifier: Natural Language :: Chinese (Simplified)
 Summary: zhconv as in MediaWiki with extra rulesets from OpenCC, oxidized with more efficiency 🦀
@@ -19,21 +19,21 @@
 [![docs.rs](https://docs.rs/zhconv/badge.svg)](https://docs.rs/zhconv)
 [![Crates.io](https://img.shields.io/crates/v/zhconv.svg)](https://crates.io/crates/zhconv)
 [![PyPI version](https://img.shields.io/pypi/v/zhconv-rs)](https://pypi.org/project/zhconv-rs/)
 [![NPM version](https://badge.fury.io/js/zhconv.svg)](https://www.npmjs.com/package/zhconv)
 # zhconv-rs 中文简繁及地區詞轉換
 zhconv-rs converts Chinese text among traditional/simplified scripts or regional variants (e.g. `zh-TW <-> zh-CN <-> zh-HK <-> zh-Hans <-> zh-Hant`), built on the top of rulesets from MediaWiki/Wikipedia and OpenCC.
 
-The implementation is powered by an [Aho-Corasick](https://github.com/daac-tools/daachorse) automaton, ensuring linear time complexity with respect to the length of input text and conversion rules (`O(n+m)`), processing dozens of MiBs text per second.
+The implementation is powered by the [Aho-Corasick](https://github.com/BurntSushi/aho-corasick) automaton, ensuring linear time complexity with respect to the length of input text and conversion rules (`O(n+m)`), processing dozens of MiBs text per second.
 
 🔗 **Web App: https://zhconv.pages.dev** (powered by WASM)
 
 ⚙️ **Cli**: `cargo install zhconv-cli` or check [releases](https://github.com/Gowee/zhconv-rs/releases).
 
-🦀 **Rust Crate**: `cargo add zhconv` (check [docs](https://docs.rs/zhconv/latest/zhconv/) for examples)
+🦀 **Rust Crate**: `cargo add zhconv` (see doc comments and [cli/](https://github.com/Gowee/zhconv-rs/tree/main/cli) for examples)
 
 🐍 **Python Package via PyO3**: `pip install zhconv-rs` (WASM with wheels)
 
 <details open>
  <summary>Python snippet</summary>
 
 ```python
@@ -133,19 +133,17 @@
 The benchmark was performed on a previous version that had only Mediawiki rulesets. In the newer version, with OpenCC rulesets activated by default, the performance may degrade ~2x.
 
 ## Differences with other converters
 * `ZhConver{sion,ter}.php` of MediaWiki: zhconv-rs just takes conversion tables listed in [`ZhConversion.php`](https://github.com/wikimedia/mediawiki/blob/master/includes/languages/data/ZhConversion.php#L14). MediaWiki relies on the inefficient PHP built-in function [`strtr`](https://github.com/php/php-src/blob/217fd932fa57d746ea4786b01d49321199a2f3d5/ext/standard/string.c#L2974). Under the basic mode, zhconv-rs guarantees linear time complexity (`T = O(n+m)` instead of `O(nm)`) and single-pass scanning of input text. Optionally, zhconv-rs supports the same conversion rule syntax with MediaWiki.
 * OpenCC: The [conversion rulesets](https://github.com/BYVoid/OpenCC/tree/master/data/dictionary) of OpenCC is independent of MediaWiki. The core [conversion implementation](https://github.dev/BYVoid/OpenCC/blob/21995f5ea058441423aaff3ee89b0a5d4747674c/src/Conversion.cpp#L27) of OpenCC is kinda similar to the aforementioned `strtr`. However, OpenCC supports pre-segmentation and maintains multiple rulesets which are applied successively. By contrast, the Aho-Corasick-powered zhconv-rs merges rulesets from MediaWiki and OpenCC in compile time and converts text in single-pass linear time, resulting in much more efficiency. Though, conversion results may differ in some cases.
 
 ## Limitations
-The converter takes leftmost-longest matching strategy. It gives priority to the leftmost-matched words or phrases. For instance, if a ruleset includes both `干 -> 幹` and `天干物燥 -> 天乾物燥`, the converter would prioritize `天乾物燥` because `天干物燥` gets matched earlier compared to `干` at a later position. The strategy yields good results in general, but may occasionally lead to wrong conversions.
+The converter utilizes an aho-corasick automaton with the leftmost-longest matching strategy. This strategy gives priority to the leftmost-matched words or phrases. For instance, if a ruleset includes both `干 -> 幹` and `天干物燥 -> 天乾物燥`, the converter would prioritize `天乾物燥` because `天干物燥` gets matched earlier compared to `干` at a later position. The strategy is generally effective but may occasionally lead to unexpected results.
 
-The implementation support most of the MediaWiki conversion rules. But it is not fully compliant with the original implementation.
-
-Besides, for wikitext, if input text contains global conversion rules (in MediaWiki syntax like -{H|zh-hans:鹿|zh-hant:马}-), the time complexity of the implementation may degrade to `O(n*m)` where `n` and `m` are the length of the text and the maximum lengths of sources words in conversion rulesets in the worst case (equivalent to brute-force).
+Futuremore, since an automaton is infeasible to update after being built, the converter must (re)build it from scratch for every ruleset. The automata for built-in rulesets (i.e. conversion tables) are built on demand and cached by default. However, if a short input text contains global conversion rules (in MediaWiki syntax like -{H|zh-hans:鹿|zh-hant:马}-), this process incurs a significant overhead, potentially being less efficient than a naive implementation.
 
 ## Credits
 All rulesets that power the converter come from the [MediaWiki](https://github.com/wikimedia/mediawiki) project and [OpenCC](https://github.com/BYVoid/OpenCC).
 
 The project takes the following projects/pages as references:
 - https://github.com/gumblex/zhconv : Python implementation of `zhConver{ter,sion}.php`.
 - https://github.com/BYVoid/OpenCC/ : Widely adopted Chinese converter.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zhconv-rs Version: 0.3.0 Classifier: Programming
+Metadata-Version: 2.1 Name: zhconv-rs Version: 0.3.0b0 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Text Processing :: Linguistic Classifier: Natural Language
 :: Chinese (Traditional) Classifier: Natural Language :: Chinese (Simplified)
 Summary: zhconv as in MediaWiki with extra rulesets from OpenCC, oxidized with
 more efficiency ð¦ Author: Hung-I Wang
 gmail.com> Author-email: Hung-I Wang
@@ -14,27 +14,28 @@
 badge.svg)](https://docs.rs/zhconv) [![Crates.io](https://img.shields.io/
 crates/v/zhconv.svg)](https://crates.io/crates/zhconv) [![PyPI version](https:/
 /img.shields.io/pypi/v/zhconv-rs)](https://pypi.org/project/zhconv-rs/) [![NPM
 version](https://badge.fury.io/js/zhconv.svg)](https://www.npmjs.com/package/
 zhconv) # zhconv-rs ä¸­æç®ç¹åå°åè©è½æ zhconv-rs converts Chinese
 text among traditional/simplified scripts or regional variants (e.g. `zh-TW <-
 > zh-CN <-> zh-HK <-> zh-Hans <-> zh-Hant`), built on the top of rulesets from
-MediaWiki/Wikipedia and OpenCC. The implementation is powered by an [Aho-
-Corasick](https://github.com/daac-tools/daachorse) automaton, ensuring linear
-time complexity with respect to the length of input text and conversion rules
-(`O(n+m)`), processing dozens of MiBs text per second. ð **Web App: https://
-zhconv.pages.dev** (powered by WASM) âï¸ **Cli**: `cargo install zhconv-cli`
-or check [releases](https://github.com/Gowee/zhconv-rs/releases). ð¦ **Rust
-Crate**: `cargo add zhconv` (check [docs](https://docs.rs/zhconv/latest/zhconv/
-) for examples) ð **Python Package via PyO3**: `pip install zhconv-rs` (WASM
-with wheels)  Python snippet ```python # > pip install zhconv_rs # Convert with
-builtin rulesets: from zhconv_rs import zhconv assert zhconv("å¤©å¹²ç©ç¥
-å°å¿ç«ç", "zh-tw") == "å¤©ä¹¾ç©ç¥ å°å¿ç«ç­" assert zhconv
-("é§å¤±æ¨èºï¼æè¿·æ´¥æ¸¡", "zh-hans") == "é¾å¤±æ¥¼å°ï¼æè¿·æ´¥æ¸¡"
-assert zhconv("ã-{zh-hans:ä¸ä¸ªç«æªæ;zh-hant:ä¸åå®¢;zh-tw:ä¸åå®¢}-
+MediaWiki/Wikipedia and OpenCC. The implementation is powered by the [Aho-
+Corasick](https://github.com/BurntSushi/aho-corasick) automaton, ensuring
+linear time complexity with respect to the length of input text and conversion
+rules (`O(n+m)`), processing dozens of MiBs text per second. ð **Web App:
+https://zhconv.pages.dev** (powered by WASM) âï¸ **Cli**: `cargo install
+zhconv-cli` or check [releases](https://github.com/Gowee/zhconv-rs/releases).
+ð¦ **Rust Crate**: `cargo add zhconv` (see doc comments and [cli/](https://
+github.com/Gowee/zhconv-rs/tree/main/cli) for examples) ð **Python Package
+via PyO3**: `pip install zhconv-rs` (WASM with wheels)  Python snippet
+```python # > pip install zhconv_rs # Convert with builtin rulesets: from
+zhconv_rs import zhconv assert zhconv("å¤©å¹²ç©ç¥ å°å¿ç«ç", "zh-tw") ==
+"å¤©ä¹¾ç©ç¥ å°å¿ç«ç­" assert zhconv("é§å¤±æ¨èºï¼æè¿·æ´¥æ¸¡", "zh-
+hans") == "é¾å¤±æ¥¼å°ï¼æè¿·æ´¥æ¸¡" assert zhconv("ã-{zh-hans:
+ä¸ä¸ªç«æªæ;zh-hant:ä¸åå®¢;zh-tw:ä¸åå®¢}-
 ãæ¯äºæ­·å±±å¤§Â·ä»²é¦¬çä½åã", "zh-cn", mediawiki=True) ==
 "ãä¸ä¸ªç«æªæãæ¯äºåå±±å¤§Â·ä»²é©¬çä½åã" assert zhconv("-
 {H|zh-cn:é¾é½å­¤å¿;zh-tw:å­¤éæ·;zh-hk:è¦æµ·å­¤é;zh-sg:é¾é½å­¤å¿;zh-
 mo:è¦æµ·å­¤é;}-ãé¾é½å­¤å¿ãæ¯æ¥å°æ¯Â·çæ´æ¯çä½åã", "zh-
 tw", True) == "ãå­¤éæ·ãæ¯æ¥ç¾æ¯Â·çæ´æ¯çä½åã" # Convert
 with custom rules: from zhconv_rs import make_converter assert make_converter
 (None, [("å¤©", "å°"), ("æ°´", "ç«")])("çèå¤©æ°´") == "çèå°ç«"
@@ -90,31 +91,31 @@
 implementation](https://github.dev/BYVoid/OpenCC/blob/
 21995f5ea058441423aaff3ee89b0a5d4747674c/src/Conversion.cpp#L27) of OpenCC is
 kinda similar to the aforementioned `strtr`. However, OpenCC supports pre-
 segmentation and maintains multiple rulesets which are applied successively. By
 contrast, the Aho-Corasick-powered zhconv-rs merges rulesets from MediaWiki and
 OpenCC in compile time and converts text in single-pass linear time, resulting
 in much more efficiency. Though, conversion results may differ in some cases.
-## Limitations The converter takes leftmost-longest matching strategy. It gives
-priority to the leftmost-matched words or phrases. For instance, if a ruleset
-includes both `å¹² -> å¹¹` and `å¤©å¹²ç©ç¥ -> å¤©ä¹¾ç©ç¥`, the converter
-would prioritize `å¤©ä¹¾ç©ç¥` because `å¤©å¹²ç©ç¥` gets matched earlier
-compared to `å¹²` at a later position. The strategy yields good results in
-general, but may occasionally lead to wrong conversions. The implementation
-support most of the MediaWiki conversion rules. But it is not fully compliant
-with the original implementation. Besides, for wikitext, if input text contains
-global conversion rules (in MediaWiki syntax like -{H|zh-hans:é¹¿|zh-hant:é©¬}-
-), the time complexity of the implementation may degrade to `O(n*m)` where `n`
-and `m` are the length of the text and the maximum lengths of sources words in
-conversion rulesets in the worst case (equivalent to brute-force). ## Credits
-All rulesets that power the converter come from the [MediaWiki](https://
-github.com/wikimedia/mediawiki) project and [OpenCC](https://github.com/BYVoid/
-OpenCC). The project takes the following projects/pages as references: - https:
-//github.com/gumblex/zhconv : Python implementation of `zhConver
-{ter,sion}.php`. - https://github.com/BYVoid/OpenCC/ : Widely adopted Chinese
-converter. - https://zh.wikipedia.org/wiki/Wikipedia:å­è©è½æèç -
-https://zh.wikipedia.org/wiki/Help:é«çº§å­è¯è½¬æ¢è¯­æ³ - https://
-github.com/wikimedia/mediawiki/blob/master/includes/language/
-LanguageConverter.php  ## TODO - [x] Support [Module:CGroup](https://
-zh.wikipedia.org/wiki/Module:CGroup) - [ ] Propogate error properly with Anyhow
-and thiserror - [x] Python lib - [x] More exmaples in README - [x] Add rulesets
-from OpenCC
+## Limitations The converter utilizes an aho-corasick automaton with the
+leftmost-longest matching strategy. This strategy gives priority to the
+leftmost-matched words or phrases. For instance, if a ruleset includes both
+`å¹² -> å¹¹` and `å¤©å¹²ç©ç¥ -> å¤©ä¹¾ç©ç¥`, the converter would prioritize
+`å¤©ä¹¾ç©ç¥` because `å¤©å¹²ç©ç¥` gets matched earlier compared to `å¹²` at
+a later position. The strategy is generally effective but may occasionally lead
+to unexpected results. Futuremore, since an automaton is infeasible to update
+after being built, the converter must (re)build it from scratch for every
+ruleset. The automata for built-in rulesets (i.e. conversion tables) are built
+on demand and cached by default. However, if a short input text contains global
+conversion rules (in MediaWiki syntax like -{H|zh-hans:é¹¿|zh-hant:é©¬}-), this
+process incurs a significant overhead, potentially being less efficient than a
+naive implementation. ## Credits All rulesets that power the converter come
+from the [MediaWiki](https://github.com/wikimedia/mediawiki) project and
+[OpenCC](https://github.com/BYVoid/OpenCC). The project takes the following
+projects/pages as references: - https://github.com/gumblex/zhconv : Python
+implementation of `zhConver{ter,sion}.php`. - https://github.com/BYVoid/OpenCC/
+: Widely adopted Chinese converter. - https://zh.wikipedia.org/wiki/Wikipedia:
+å­è©è½æèç - https://zh.wikipedia.org/wiki/Help:
+é«çº§å­è¯è½¬æ¢è¯­æ³ - https://github.com/wikimedia/mediawiki/blob/master/
+includes/language/LanguageConverter.php  ## TODO - [x] Support [Module:CGroup]
+(https://zh.wikipedia.org/wiki/Module:CGroup) - [ ] Propogate error properly
+with Anyhow and thiserror - [x] Python lib - [x] More exmaples in README - [x]
+Add rulesets from OpenCC
```

