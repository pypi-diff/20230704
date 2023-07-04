# Comparing `tmp/dsptoolbox-0.2.5.tar.gz` & `tmp/dsptoolbox-0.2.6.tar.gz`

## Comparing `dsptoolbox-0.2.5.tar` & `dsptoolbox-0.2.6.tar`

### file list

```diff
@@ -1,92 +1,97 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/.gitattributes
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/.readthedocs.yaml
--rw-r--r--   0        0        0    10306 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/CHANGELOG.rst
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/requirements.txt
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/Makefile
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/__rdme.rst
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/classes.rst
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/conf.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/index.rst
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/make.bat
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules.rst
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/readme.rst
--rw-r--r--   0        0        0   262622 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/logo/logo.png
--rw-r--r--   0        0        0   262793 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/logo/logo2.png
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules/dsptoolbox.audio_io.rst
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules/dsptoolbox.beamforming.rst
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules/dsptoolbox.distances.rst
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules/dsptoolbox.filterbanks.rst
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules/dsptoolbox.generators.rst
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules/dsptoolbox.plots.rst
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules/dsptoolbox.room_acoustics.rst
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules/dsptoolbox.special.rst
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules/dsptoolbox.standard_functions.rst
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/docs/modules/dsptoolbox.transfer_functions.rst
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/__init__.py
--rw-r--r--   0        0        0    23326 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/_general_helpers.py
--rw-r--r--   0        0        0    30953 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/_standard.py
--rw-r--r--   0        0        0    42692 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/standard_functions.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/audio_io/__init__.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/audio_io/_audio_io.py
--rw-r--r--   0        0        0    14816 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/audio_io/audio_io.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/beamforming/__init__.py
--rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/beamforming/_beamforming.py
--rw-r--r--   0        0        0    61951 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/beamforming/beamforming.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/classes/__init__.py
--rw-r--r--   0        0        0    20613 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/classes/_filter.py
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/classes/_plots.py
--rw-r--r--   0        0        0    30914 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/classes/filter_class.py
--rw-r--r--   0        0        0    27757 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/classes/filterbank.py
--rw-r--r--   0        0        0    13664 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/classes/multibandsignal.py
--rw-r--r--   0        0        0    48334 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/classes/signal_class.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/distances/__init__.py
--rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/distances/_distances.py
--rw-r--r--   0        0        0    12815 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/distances/distances.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/filterbanks/__init__.py
--rw-r--r--   0        0        0    45051 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/filterbanks/_filterbank.py
--rw-r--r--   0        0        0    14424 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/filterbanks/filterbanks.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/generators/__init__.py
--rw-r--r--   0        0        0    12584 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/generators/generators.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/plots/__init__.py
--rw-r--r--   0        0        0     9946 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/plots/plots.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/room_acoustics/__init__.py
--rw-r--r--   0        0        0    33500 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/room_acoustics/_room_acoustics.py
--rw-r--r--   0        0        0    20850 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/room_acoustics/room_acoustics.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/special/__init__.py
--rw-r--r--   0        0        0    11751 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/special/special.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/transfer_functions/__init__.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/transfer_functions/_transfer_functions.py
--rw-r--r--   0        0        0    23751 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/dsptoolbox/transfer_functions/transfer_functions.py
--rw-r--r--   0        0        0    46390 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/audio_io_module.ipynb
--rw-r--r--   0        0        0   369566 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/beamforming_module.ipynb
--rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/distances_module.ipynb
--rw-r--r--   0        0        0   403706 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/filterbanks_module.ipynb
--rw-r--r--   0        0        0   948939 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/general.ipynb
--rw-r--r--   0        0        0   244031 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/generators_module.ipynb
--rw-r--r--   0        0        0   330277 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/room_acoustics_module.ipynb
--rw-r--r--   0        0        0  1536113 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/special_module.ipynb
--rw-r--r--   0        0        0    47577 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/standard_module.ipynb
--rw-r--r--   0        0        0   209919 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/transfer_function_module.ipynb
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/data/array.xml
--rw-r--r--   0        0        0   384044 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/data/chirp.wav
--rw-r--r--   0        0        0   384044 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/data/chirp_mono.wav
--rw-r--r--   0        0        0   768044 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/data/chirp_stereo.wav
--rw-r--r--   0        0        0    96044 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/data/rir.wav
--rw-r--r--   0        0        0   187792 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/examples/data/speech.flac
--rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/manual_filter_testing.py
--rw-r--r--   0        0        0    29360 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/manual_testing.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/test_audio_io.py
--rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/test_beamforming.py
--rw-r--r--   0        0        0    30055 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/test_classes.py
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/test_distances.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/test_filterbanks.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/test_generators.py
--rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/test_room_acoustics.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/test_special.py
--rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/test_standard.py
--rw-r--r--   0        0        0     7421 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/tests/test_transfer_functions.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/LICENSE
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/README.rst
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 dsptoolbox-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/.gitattributes
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/.readthedocs.yaml
+-rw-r--r--   0        0        0    11140 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/CHANGELOG.rst
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/requirements.txt
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/Makefile
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/__rdme.rst
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/classes.rst
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/conf.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/index.rst
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/make.bat
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/modules.rst
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/readme.rst
+-rw-r--r--   0        0        0   262622 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/logo/logo.png
+-rw-r--r--   0        0        0   262793 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/logo/logo2.png
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/modules/dsptoolbox.audio_io.rst
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/modules/dsptoolbox.beamforming.rst
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/modules/dsptoolbox.distances.rst
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/modules/dsptoolbox.effects.rst
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/modules/dsptoolbox.filterbanks.rst
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/modules/dsptoolbox.generators.rst
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/modules/dsptoolbox.plots.rst
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/modules/dsptoolbox.room_acoustics.rst
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/modules/dsptoolbox.special.rst
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/modules/dsptoolbox.standard_functions.rst
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/docs/modules/dsptoolbox.transfer_functions.rst
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/__init__.py
+-rw-r--r--   0        0        0    25394 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/_general_helpers.py
+-rw-r--r--   0        0        0    27830 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/_standard.py
+-rw-r--r--   0        0        0    43212 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/standard_functions.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/audio_io/__init__.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/audio_io/_audio_io.py
+-rw-r--r--   0        0        0    14821 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/audio_io/audio_io.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/beamforming/__init__.py
+-rw-r--r--   0        0        0     9787 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/beamforming/_beamforming.py
+-rw-r--r--   0        0        0    62054 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/beamforming/beamforming.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/classes/__init__.py
+-rw-r--r--   0        0        0    20613 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/classes/_filter.py
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/classes/_plots.py
+-rw-r--r--   0        0        0    31000 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/classes/filter_class.py
+-rw-r--r--   0        0        0    27985 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/classes/filterbank.py
+-rw-r--r--   0        0        0    13664 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/classes/multibandsignal.py
+-rw-r--r--   0        0        0    48533 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/classes/signal_class.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/distances/__init__.py
+-rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/distances/_distances.py
+-rw-r--r--   0        0        0    12815 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/distances/distances.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/effects/__init__.py
+-rw-r--r--   0        0        0    19350 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/effects/_effects.py
+-rw-r--r--   0        0        0    57416 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/effects/effects.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/filterbanks/__init__.py
+-rw-r--r--   0        0        0    45051 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/filterbanks/_filterbank.py
+-rw-r--r--   0        0        0    14424 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/filterbanks/filterbanks.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/generators/__init__.py
+-rw-r--r--   0        0        0    17330 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/generators/generators.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/plots/__init__.py
+-rw-r--r--   0        0        0    10150 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/plots/plots.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/room_acoustics/__init__.py
+-rw-r--r--   0        0        0    33500 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/room_acoustics/_room_acoustics.py
+-rw-r--r--   0        0        0    20850 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/room_acoustics/room_acoustics.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/special/__init__.py
+-rw-r--r--   0        0        0    17842 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/special/special.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/transfer_functions/__init__.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/transfer_functions/_transfer_functions.py
+-rw-r--r--   0        0        0    23946 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/dsptoolbox/transfer_functions/transfer_functions.py
+-rw-r--r--   0        0        0    46390 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/examples/audio_io_module.ipynb
+-rw-r--r--   0        0        0   369566 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/examples/beamforming_module.ipynb
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/examples/distances_module.ipynb
+-rw-r--r--   0        0        0   403706 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/examples/filterbanks_module.ipynb
+-rw-r--r--   0        0        0   948939 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/examples/general.ipynb
+-rw-r--r--   0        0        0   244031 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/examples/generators_module.ipynb
+-rw-r--r--   0        0        0   330277 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/examples/room_acoustics_module.ipynb
+-rw-r--r--   0        0        0   842350 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/examples/special_module.ipynb
+-rw-r--r--   0        0        0    94370 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/examples/standard_module.ipynb
+-rw-r--r--   0        0        0   209919 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/examples/transfer_function_module.ipynb
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/examples/data/array.xml
+-rw-r--r--   0        0        0   384044 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/examples/data/chirp.wav
+-rw-r--r--   0        0        0   384044 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/examples/data/chirp_mono.wav
+-rw-r--r--   0        0        0   768044 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/examples/data/chirp_stereo.wav
+-rw-r--r--   0        0        0    96044 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/examples/data/rir.wav
+-rw-r--r--   0        0        0   187792 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/examples/data/speech.flac
+-rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/tests/manual_filter_testing.py
+-rw-r--r--   0        0        0    31625 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/tests/manual_testing.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/tests/test_audio_io.py
+-rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/tests/test_beamforming.py
+-rw-r--r--   0        0        0    30046 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/tests/test_classes.py
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/tests/test_distances.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/tests/test_filterbanks.py
+-rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/tests/test_fx.py
+-rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/tests/test_generators.py
+-rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/tests/test_room_acoustics.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/tests/test_special.py
+-rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/tests/test_standard.py
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/tests/test_transfer_functions.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/LICENSE
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/README.rst
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 dsptoolbox-0.2.6/PKG-INFO
```

### Comparing `dsptoolbox-0.2.5/.readthedocs.yaml` & `dsptoolbox-0.2.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/CHANGELOG.rst` & `dsptoolbox-0.2.6/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,33 +10,57 @@
 
 `To Do's for future releases`_
 ------------------------------
 
 - Validation for results from tests in every module (so far many tests are
   only regarding functionality)
 
+`0.2.6 <https://pypi.org/project/dsptoolbox/0.2.6>`_ - 
+---------------------
+
+Added
+~~~~~~
+- effects module with basic implementations for standard audio effects
+- extra functionalities in the audio io module
+
+Bugfix
+~~~~~~~
+- general bug fixes
+
+Misc
+~~~~~
+- made seaborn optional
+
 `0.2.5 <https://pypi.org/project/dsptoolbox/0.2.5>`_ - 
 ---------------------
 
 Added
 ~~~~~~
 - mel-frequency cepstral coefficients ``mfcc`` in ``special`` module
 - spectrogram of a signal can now be plotted with a selected dynamic range
 - ``audio_io`` has now more port functionalities to ``sounddevice``
+- The inverse STFT was added in the ``special`` module
+- ``effects`` module with some effects: ``SpectralSubtractor``,
+  ``Distortion``, ``Compressor``, ``Tremolo``, ``Chorus/Flanger``, ``DigitalDelay``
 
 Bugfix
 ~~~~~~~
 - plotting for the ``qmf`` Crossover is now possible without downsampling
 - Linkwitz-Riley crossovers plotting functions have been updated and corrected
 - corrected some tests
+- scaling of spectrum in signal was not working properly when `None` was passed
+- conceptual errors were fixed in ``activity_detector``
+- ``true_peak_level`` was changing the gain of the incoming signal
 
 Misc
 ~~~~~
 - docstrings corrected and extended
 - computation of steering vectors in ``beamforming`` has been optimized
+- spectrogram computation has been changed to be performed as multi-channel
+  operation and the output array has now the extra channel dimension
 
 `0.2.4 <https://pypi.org/project/dsptoolbox/0.2.4>`_ - 
 ---------------------
 
 Added
 ~~~~~~
 - ``rms`` function
```

### Comparing `dsptoolbox-0.2.5/requirements.txt` & `dsptoolbox-0.2.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/docs/Makefile` & `dsptoolbox-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/docs/classes.rst` & `dsptoolbox-0.2.6/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/docs/conf.py` & `dsptoolbox-0.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/docs/index.rst` & `dsptoolbox-0.2.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/docs/make.bat` & `dsptoolbox-0.2.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/docs/readme.rst` & `dsptoolbox-0.2.6/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/docs/logo/logo.png` & `dsptoolbox-0.2.6/docs/logo/logo.png`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/docs/logo/logo2.png` & `dsptoolbox-0.2.6/docs/logo/logo2.png`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/dsptoolbox/__init__.py` & `dsptoolbox-0.2.6/dsptoolbox/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 from . import room_acoustics
 from . import plots
 from . import generators
 from . import filterbanks
 from . import special
 from . import audio_io
 from . import beamforming
+from . import effects
 
 __all__ = [
     # Basic classes
     'Signal', 'MultiBandSignal', 'Filter', 'FilterBank',
 
     # Functions in standard module
     'latency', 'pad_trim', 'fade', 'merge_signals', 'merge_filterbanks',
     'resample', 'activity_detector', 'normalize',
     'fractional_delay', 'true_peak_level', 'ir_to_filter', 'erb_frequencies',
     'load_pkl_object', 'fractional_octave_frequencies', 'filter_to_ir',
     'detrend', 'rms', 'CalibrationData',
 
     # Modules
     'transfer_functions', 'distances', 'room_acoustics', 'plots', 'generators',
-    'filterbanks', 'special', 'audio_io', 'beamforming'
+    'filterbanks', 'special', 'audio_io', 'beamforming', 'effects'
 ]
 
-__version__ = '0.2.5'
+__version__ = '0.2.6'
```

### Comparing `dsptoolbox-0.2.5/dsptoolbox/_general_helpers.py` & `dsptoolbox-0.2.6/dsptoolbox/_general_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -728,14 +728,86 @@
     mode = mode.lower()
     assert mode in ('closest', 'floor', 'ceil'), \
         'Mode must be either closest, floor or ceil'
 
     p = np.log2(number)
     if mode == 'closest':
         remainder = p - int(p)
-        mode == 'floor' if remainder < 0.5 else 'ceil'
-
+        mode = 'floor' if remainder < 0.5 else 'ceil'
     if mode == 'floor':
         p = np.floor(p).astype(int)
     elif mode == 'ceil':
         p = np.ceil(p).astype(int)
     return int(2**p)
+
+
+def _euclidean_distance_matrix(x: np.ndarray, y: np.ndarray):
+    """Compute the euclidean distance matrix between two vectors efficiently.
+
+    Parameters
+    ----------
+    x : `np.ndarray`
+        First vector or matrix with shape (Point x, Dimensions).
+    y : `np.ndarray`
+        Second vector or matrix with shape (Point y, Dimensions).
+
+    Returns
+    -------
+    dist : `np.ndarray`
+        Euclidean distance matrix with shape (Point x, Point y).
+
+    """
+    assert x.ndim == 2 and y.ndim == 2, \
+        'Inputs must have exactly two dimensions'
+    assert x.shape[1] == y.shape[1], \
+        'Dimensions do not match'
+    return np.sqrt(np.sum(x**2, axis=1, keepdims=True) +
+                   np.sum(y.T**2, axis=0, keepdims=True) -
+                   2 * x @ y.T)
+
+
+def _get_smoothing_factor_ema(relaxation_time_s: float, sampling_rate_hz: int):
+    """This computes the smoothing factor needed for a single-pole IIR,
+    or exponential moving averager. The returned value (alpha) should be used::
+    for as follows
+
+        y[n] = alpha * x[n] + (1-alpha)*y[n-1]
+
+    Parameters
+    ----------
+    relaxation_time_s : float
+        Time for the step response to stabilize around the given value
+        (with 99% accuracy).
+    sampling_rate_hz : int
+        Sampling rate to be used.
+
+    Returns
+    -------
+    alpha : float
+        Smoothing value for the
+
+    Notes
+    -----
+    - The formula coincides with the one presented in
+      https://en.wikipedia.org/wiki/Exponential_smoothing, but it uses a factor
+      5.
+
+    """
+    return 1 - np.exp(-5/relaxation_time_s/sampling_rate_hz)
+
+
+def _wrap_phase(phase_vector: np.ndarray) -> np.ndarray:
+    """Wraps phase between [-np.pi, np.pi[ after it has been unwrapped.
+    This works for 1D and 2D arrays, more dimensions have not been tested.
+
+    Parameters
+    ----------
+    phase_vector : `np.ndarray`
+        Phase vector for which to wrap the phase.
+
+    Returns
+    -------
+    `np.ndarray`
+        Wrapped phase vector.
+
+    """
+    return (phase_vector + np.pi) % (2 * np.pi) - np.pi
```

### Comparing `dsptoolbox-0.2.5/dsptoolbox/_standard.py` & `dsptoolbox-0.2.6/dsptoolbox/_standard.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,17 +28,17 @@
            detrend: bool = True, average: str = 'mean',
            scaling: str = 'power spectral density') -> np.ndarray:
     """Cross spectral density computation with Welch's method.
 
     Parameters
     ----------
     x : `np.ndarray`
-        First signal
+        First signal with shape (time samples, channel).
     y : `np.ndarray`
-        Second signal
+        Second signal with shape (time samples, channel).
     fs_hz : int
         Sampling rate in Hz.
     window_type : str, optional
         Window type to be used. Refer to scipy.signal.windows for available
         ones. Default: `'hann'`
     window_length_samples : int, optional
         Window length to be used. Determines frequency resolution in the end.
@@ -58,95 +58,104 @@
 
     Returns
     -------
     csd : `np.ndarray`
         Complex cross spectral density vector if x and y are different.
         Alternatively, the (real) autocorrelation power spectral density when
         x and y are the same. If density or spectrum depends on scaling.
+        Depending on the input, the output shape is (time samples) or
+        (time samples, channel).
 
     References
     ----------
     - Heinzel, G., Rüdiger, A., & Schilling, R. (2002). Spectrum and spectral
       density estimation by the Discrete Fourier transform (DFT), including a
       comprehensive list of window functions and some new at-top windows.
     - Allen, B., Anderson, W. G., Brady, P. R., Brown, D. A., & Creighton,
       J. D. E. (2005). FINDCHIRP: an algorithm for detection of gravitational
       waves from inspiraling compact binaries.
       See http://arxiv.org/abs/gr-qc/0509116.
 
     """
-    # from time import time
     if type(x) != np.ndarray:
-        x = np.array(x).squeeze()
+        x = np.asarray(x).squeeze()
     if type(y) != np.ndarray:
-        y = np.array(y).squeeze()
+        y = np.asarray(y).squeeze()
     assert x.shape == y.shape, \
         'Shapes of data do not match'
-    assert len(x.shape) < 2, f'{x.shape} are too many dimensions. Use flat' +\
-        ' arrays instead'
-    valid_window_sizes = np.array([int(2**x) for x in range(4, 17)])
+    # NOTE: Computing the spectrum in a vectorized manner for all channels
+    # simultaneously does not seem to be faster than doing it sequentally
+    # for each channel. Maybe parallelizing with something like numba could
+    # be advantageous...
+    if x.ndim == 2:
+        multi_channel = True
+    else:
+        multi_channel = False
+
+    assert len(x.shape) <= 2, f'{x.shape} are too many dimensions. Use flat' +\
+        ' arrays or 2D-Arrays instead'
+
+    valid_window_sizes = np.array([int(2**x) for x in range(3, 19)])
     assert window_length_samples in valid_window_sizes, \
-        'Window length should be a power of 2 between [16, 65536] or ' +\
-        '[2**4, 2**16]'
+        'Window length should be a power of 2 between [8, 262_144] or ' +\
+        '[2**3, 2**18]'
     assert overlap_percent >= 0 and overlap_percent < 100, \
         'overlap_percent should be between 0 and 100'
     valid_average = ['mean', 'median']
     assert average in valid_average, f'{average} is not valid. Use ' +\
         'either mean or median'
     valid_scaling = ['power spectrum', 'power spectral density',
                      'amplitude spectrum', 'amplitude spectral density', None]
     assert scaling in valid_scaling, f'{scaling} is not valid. Use ' +\
         'power spectrum, power spectral density, amplitude spectrum, ' +\
         'amplitude spectral density or None'
+    if scaling is None:
+        scaling = ''
 
     # Window and step
     window = windows.get_window(
         window_type, window_length_samples, fftbins=True)
     overlap_samples = int(overlap_percent/100 * window_length_samples)
     step = window_length_samples - overlap_samples
 
     # Check COLA
     if not check_COLA(window, nperseg=len(window), noverlap=overlap_samples):
         warn('Selected window type and overlap do not meet the constant ' +
              'overlap and add constraint! Results might be distorted')
 
-    # Start Parameters
-    n_frames, padding_samp = \
-        _compute_number_frames(window_length_samples, step, len(x))
-    x = _pad_trim(x, len(x) + padding_samp)
-    y = _pad_trim(y, len(y) + padding_samp)
-    x_frames = np.zeros((window_length_samples, n_frames), dtype='float')
-    y_frames = np.zeros_like(x_frames)
+    if not multi_channel:
+        x = x[..., None]
+        y = y[..., None]
 
-    # Create time frames
-    start = 0
-    for n in range(n_frames):
-        x_frames[:, n] = x[start:start+window_length_samples].copy()
-        y_frames[:, n] = y[start:start+window_length_samples].copy()
-        start += step
+    x_frames = _get_framed_signal(x, window_length_samples, step)
+    y_frames = _get_framed_signal(y, window_length_samples, step)
 
     # Window
-    x_frames *= window[..., None]
-    y_frames *= window[..., None]
+    x_frames *= window[:, np.newaxis, np.newaxis]
+    y_frames *= window[:, np.newaxis, np.newaxis]
+
+    if not multi_channel:
+        x_frames = np.squeeze(x_frames)
+        y_frames = np.squeeze(y_frames)
 
     # Detrend
     if detrend:
         x_frames -= np.mean(x_frames, axis=0)
         y_frames -= np.mean(y_frames, axis=0)
 
     # Combine
     sp_frames = np.fft.rfft(x_frames, axis=0).conjugate() * \
         np.fft.rfft(y_frames, axis=0)
 
     # Direct averaging much faster
     if average == 'mean':
-        csd = np.mean(sp_frames, axis=-1)
+        csd = np.mean(sp_frames, axis=1)
     else:
-        csd = np.median(sp_frames.real, axis=-1) + 1j * \
-            np.median(sp_frames.imag, axis=-1)
+        csd = np.median(sp_frames.real, axis=1) + 1j * \
+            np.median(sp_frames.imag, axis=1)
         # Bias according to reference
         n = sp_frames.shape[1] if sp_frames.shape[1] % 2 == 1 else \
             sp_frames.shape[1] - 1
         bias = np.sum((-1)**(n+1)/n)
         csd /= bias
 
     # Weightning (with 2 because one-sided)
@@ -157,27 +166,26 @@
         # With this factor, energy can be regained by integrating the psd
         # while taking into account the frequency step
     else:
         factor = 1
 
     # Zero frequency fix when detrending (especially useful for dB plotting)
     if detrend:
-        csd[0] = csd[1]
+        csd[0, ...] = csd[1, ...]
 
     csd *= factor
-    csd[0] /= 2
-    csd[-1] /= 2
+    csd[0, ...] /= 2
+    csd[-1, ...] /= 2
 
     if 'amplitude' in scaling:
         csd = np.sqrt(csd)
 
     # Cast to real output if there is no imaginary part
     if np.all(csd.imag == 0):
         csd = csd.real
-
     return csd
 
 
 def _group_delay_direct(phase: np.ndarray, delta_f: float = 1):
     """Computes group delay by differentiation of the unwrapped phase.
 
     Parameters
@@ -231,15 +239,15 @@
         minimum_phase = np.angle(np.exp(1j*minimum_phase))
     return minimum_phase
 
 
 def _stft(x: np.ndarray, fs_hz: int, window_length_samples: int = 2048,
           window_type: str = 'hann', overlap_percent=50,
           fft_length_samples: int = None, detrend: bool = True,
-          padding: bool = True, scaling: bool = False):
+          padding: bool = False, scaling: bool = False):
     """Computes the STFT of a signal. Output matrix has (freqs_hz, seconds_s).
 
     Parameters
     ----------
     x : `np.ndarray`
         First signal
     fs_hz : int
@@ -256,27 +264,28 @@
         Length of the FFT window for each time window. This affects
         the frequency resolution and can also crop the time window. Pass
         `None` to use the window length. Default: `None`.
     detrend : bool, optional
         Detrending from each time segment (removing mean). Default: True.
     padding : bool, optional
         When `True`, the original signal is padded in the beginning and ending
-        so that no energy is lost due to windowing. Default: `True`.
+        so that no energy is lost due to windowing when the COLA constraint is
+        met. Default: `False`.
     scaling : bool, optional
         When `True`, the output is scaled as an amplitude spectrum, otherwise
         no scaling is applied. See references for details. Default: `False`.
 
     Returns
     -------
     time_s : `np.ndarray`
         Time vector in seconds for each frame.
     freqs_hz : `np.ndarray`
         Frequency vector.
     stft : `np.ndarray`
-        STFT matrix with shape (frequency, time).
+        STFT matrix with shape (frequency, time, channel).
 
     References
     ----------
     - Heinzel, G., Rüdiger, A., & Schilling, R. (2002). Spectrum and spectral
       density estimation by the Discrete Fourier transform (DFT), including a
       comprehensive list of window functions and some new at-top windows.
 
@@ -297,31 +306,19 @@
     # Check COLA
     if not check_COLA(window, nperseg=len(window), noverlap=overlap_samples):
         warn('Selected window type and overlap do not meet the constant ' +
              'overlap and add constraint! Results might be distorted')
 
     # Padding
     if padding:
-        x = _pad_trim(x, len(x)+overlap_samples, in_the_end=False)
-        x = _pad_trim(x, len(x)+overlap_samples, in_the_end=True)
-
-    # Number of samples and padding
-    n_frames, padding_samp = \
-        _compute_number_frames(window_length_samples, step, len(x))
-
-    x = _pad_trim(x, len(x) + padding_samp)
-    time_x = np.zeros((window_length_samples, n_frames), dtype='float')
-
-    # Create time frames
-    start = 0
-    for n in range(n_frames):
-        time_x[:, n] = x[start:start+window_length_samples].copy()
-        start += step
+        x = np.pad(x, ((overlap_samples, overlap_samples), (0, 0)))
+    # Framed signal
+    time_x = _get_framed_signal(x, window_length_samples, step, True)
     # Windowing
-    time_x *= window[..., None]
+    time_x *= window[..., np.newaxis, np.newaxis]
     # Detrend
     if detrend:
         time_x -= np.mean(time_x, axis=0)
     # Spectra
     stft = np.fft.rfft(time_x, axis=0, n=fft_length_samples)
     # Scaling
     if scaling:
@@ -377,23 +374,30 @@
     References
     ----------
     - Heinzel, G., Rüdiger, A., & Schilling, R. (2002). Spectrum and spectral
       density estimation by the Discrete Fourier transform (DFT), including a
       comprehensive list of window functions and some new at-top windows.
 
     """
+    # ===== Remarks on speed =============
+    # It has been tried to vectorize the whole computation of the CSM by using
+    # a multi-channel approach in the _welch() function or with a class. This
+    # leads to a dramatic drop in performance and an elevated memory cost.
+    # Maybe using some parallel computing framework like numba would make it
+    # faster, but less readable and it would be a new dependency of the
+    # package... So far the double loop has been best solution
+    # =====================================
     number_of_channels = time_data.shape[1]
     csm = np.zeros((window_length_samples//2+1,
                     number_of_channels,
                     number_of_channels), dtype='cfloat')
     for ind1 in range(number_of_channels):
         for ind2 in range(ind1, number_of_channels):
             # Complex conjugate second signal and not first (like transposing
             # the matrix)
-            # csm[:, ind1, ind2] = \
             csm[:, ind2, ind1] = \
                 _welch(time_data[:, ind1],
                        time_data[:, ind2],
                        sampling_rate_hz,
                        window_length_samples=window_length_samples,
                        window_type=window_type,
                        overlap_percent=overlap_percent,
@@ -403,188 +407,14 @@
             if ind1 == ind2:
                 csm[:, ind1, ind2] *= 0.5
     csm += np.swapaxes(csm, 1, 2).conjugate()
     f = np.fft.rfftfreq(window_length_samples, 1/sampling_rate_hz)
     return f, csm
 
 
-# =============================================================================
-# It was shown that this helper class was not faster than the _csm function.
-# Vectorizing some of the computations did not seem to bring any advantages
-# to the speed. Especially, np.fft.rfft was a little slower and np.unwrap was
-# much slower when applied to large matrices along specific dimensions...
-# =============================================================================
-# class _CSMHelper():
-#     """This is a helper class to compute the csm in an efficient manner.
-
-#     """
-#     def __init__(self, time_data: np.ndarray, sampling_rate_hz: int,
-#                  window_length_samples: int = 1024,
-#                  window_type: str = 'hann', overlap_percent: int = 50,
-#                  detrend: bool = True, average: str = 'mean',
-#                  scaling: str = 'power'):
-#         """Computes the cross spectral matrix of a multichannel signal.
-#         Output matrix has (frequency, channels, channels).
-
-#         Parameters
-#         ----------
-#         time_data : `np.ndarray`
-#             Signal
-#         sampling_rate_hz : int
-#             Sampling rate in Hz.
-#         window_length_samples : int, optional
-#             Window length to be used. Determines frequency resolution in the
-#             end. Only powers of 2 are accepted. Default: 1024.
-#         window_type : str, optional
-#             Window type to be used. Refer to scipy.signal.windows for
-#             available ones. Default: `'hann'`
-#         overlap_percent : int, optional
-#             Overlap in percentage. Default: 50.
-#         detrend : bool, optional
-#             Detrending from each time segment (removing mean). Default: True.
-#         average : str, optional
-#             Type of mean to be computed. Take `'mean'` or `'np.median'`.
-#             Default: `'mean'`
-#         scaling : str, optional
-#             Scaling for spectral power density or spectrum. Takes `'power'`
-#             or `'spectrum'`. Default: `'power'`.
-
-#         Attributes
-#         ----------
-#         All passed parameters are saved as attributes.
-
-#         - `get_csm()`: Method to trigger the computation of csm.
-
-#         """
-#         assert time_data.shape[1] > 1, \
-#             'There has to be at least 2 channels to compute the csm'
-#         valid_window_sizes = np.array([int(2**x) for x in range(7, 17)])
-#         assert window_length_samples in valid_window_sizes, \
-#             'Window length should be a power of 2 between [128, 65536] ' +\
-#             'or [2**7, 2**16]'
-#         assert overlap_percent > 0 and overlap_percent < 100, \
-#             'overlap_percent should be between 0 and 100'
-#         valid_average = ['mean', 'median']
-#         assert average in valid_average, f'{average} is not valid. Use ' +\
-#             'either mean or median'
-#         valid_scaling = ['power', 'spectrum']
-#         assert scaling in valid_scaling, f'{scaling} is not valid. Use ' +\
-#             'either power or spectrum'
-
-#         # Window and step
-#         window = windows.get_window(
-#             window_type, window_length_samples, fftbins=True)
-#         overlap_samples = int(overlap_percent/100 * window_length_samples)
-#         step = window_length_samples - overlap_samples
-
-#         # Check COLA
-#         assert check_COLA(
-#             window, nperseg=len(window), noverlap=overlap_samples),\
-#             'Selected window type and overlap do not meet the constant ' +\
-#             'overlap and add constraint. Please select other.'
-
-#         # Save all attributes in object
-#         self.time_data = time_data
-#         self.window = window
-#         self.window_length_samples = window_length_samples
-#         self.sampling_rate_hz = sampling_rate_hz
-#         self.overlap_samples = overlap_samples
-#         self.step = step
-#         self.detrend = detrend
-
-#         if average == 'mean':
-#             self.average_func = np.mean
-#         else:
-#             self.average_func = np.median
-
-#         if scaling == 'power':
-#             self.factor = 2 / (window @ window) / sampling_rate_hz
-#         else:
-#             self.factor = 2 / sum(window)**2 / sampling_rate_hz
-#         self.f_vec = \
-#             np.fft.rfftfreq(window_length_samples, 1/sampling_rate_hz)
-
-#     def _compute_framed_spectra(self):
-#         """Computes the framed spectra.
-
-#         """
-#         # Compute number of needed frames and padding
-#         original_length = self.time_data.shape[0]
-#         n_frames, padding_samp = _compute_number_frames(
-#             self.window_length_samples, self.step, original_length)
-#         self.time_data = _pad_trim(
-#             self.time_data, original_length + padding_samp)
-#         td_frames = np.zeros(
-#             (self.window_length_samples, n_frames, self.time_data.shape[1]),
-#             dtype='float')
-#         self.n_frames = n_frames
-
-#         # Create time frames (time samples, frame, channel)
-#         start = 0
-#         for n in range(n_frames):
-#             td_frames[:, n, :] = \
-#                 self.time_data[
-#                     start:start+self.window_length_samples, :].copy()
-#             start += self.step
-
-#         # Window
-#         td_frames *= self.window[:, np.newaxis, np.newaxis]
-#         # Detrend
-#         if self.detrend:
-#             td_frames -= np.mean(td_frames, axis=0)
-#         # Spectra (frequency bins, frames, channel)
-#         self.sp_frames = np.fft.rfft(td_frames, axis=0)
-
-#     def get_csm(self):
-#         """Computes and returns the CSM.
-
-#         Returns
-#         -------
-#         f : `np.ndarray`
-#             Frequency vector.
-#         csm : `np.ndarray`
-#             Cross-spectral density matrix with shape
-#             (frequency, channel, channel).
-
-#         """
-#         self._compute_framed_spectra()
-#         number_of_channels = self.time_data.shape[1]
-#         csm_framed = np.zeros((self.window_length_samples//2+1,
-#                                self.n_frames,
-#                                number_of_channels,
-#                                number_of_channels), dtype=np.complex64)
-
-#         # Maybe second loop can be vectorized by using np.roll along one
-#         # channel axis. There would be unnecessary computations but it
-#         # might be faster
-#         for ind1 in range(number_of_channels):
-#             for ind2 in range(ind1, number_of_channels):
-#                 csm_framed[:, :, ind1, ind2] = \
-#                     np.conjugate(self.sp_frames[:, :, ind1]) * \
-#                     self.sp_frames[:, :, ind2]
-#                 if ind1 == ind2:
-#                     csm_framed[:, :, ind1, ind2] *= 0.5
-
-#         # Get magnitude and phase
-#         magnitude = np.abs(csm_framed)
-#         # phase = np.angle(csm_framed)
-#         phase = np.unwrap(np.angle(csm_framed), axis=0)
-#         del csm_framed
-#         # Average along frames (axis=1)
-#         magnitude = self.average_func(magnitude, axis=1)
-#         phase = self.average_func(phase, axis=1)
-
-#         # Redo matrix with factor
-#         csm = magnitude * np.exp(1j*phase) * self.factor
-#         # csm = np.mean(csm_framed, axis=1) * self.factor
-#         # Complete lower triangle csm matrix
-#         csm += np.swapaxes(csm, 1, 2).conjugate()
-#         return self.f_vec, csm
-
-
 def _center_frequencies_fractional_octaves_iec(nominal, num_fractions):
     """Returns the exact center frequencies for fractional octave bands
     according to the IEC 61260:1:2014 standard.
     octave ratio
     .. G = 10^{3/10}
     center frequencies
     .. f_m = f_r G^{x/b}
@@ -708,63 +538,68 @@
         beta = 0.5842 * (A - 21)**0.4 + 0.07886 * (A - 21)
     else:
         beta = 0.0
 
     return beta
 
 
-def _indexes_above_threshold_dbfs(time_vec: np.ndarray, threshold_dbfs: float,
-                                  attack_samples: int, release_samples: int):
-    """Returns indexes with power above a passed threshold (in dBFS) in a time
-    series. time_vec is normalized prior to computation.
+def _indices_above_threshold_dbfs(time_vec: np.ndarray, threshold_dbfs: float,
+                                  attack_smoothing_coeff: int,
+                                  release_smoothing_coeff: int,
+                                  normalize: bool = True):
+    """Returns indices with power above a given power threshold (in dBFS) in a
+    time series. time_vec can be normalized to peak value prior to computation.
 
     Parameters
     ----------
     time_vec : `np.ndarray`
-        Time series for which to find indexes above power threshold.
+        Time series for which to find indices above power threshold. Can only
+        take one channel.
     threshold_dbfs : float
-        Threshold to be used.
-    attack_samples : int
-        Number of samples representing attack time signal has surpassed
-        power threshold.
-    release_samples : int
-        Number of samples representing release time after signal has decayed
-        below power threshold.
+        Threshold in dBFS to be regarded for activation.
+    attack_smoothing_coeff : int
+        Coefficient for attack smoothing for level computation.
+    release_smoothing_coeff : int
+        Coefficient for release smoothing for level computation.
+    normalize : bool, optional
+        When `True`, signal is normalized such that the threshold is relative
+        to peak level and not absolute. Default: `True`.
 
     Returns
     -------
-    indexes_above : `np.ndarray`
-        Array of type boolean with length of time_vec indicating indexes
+    indices_above : `np.ndarray`
+        Array of type boolean with length of time_vec indicating indices
         above threshold with `True` and below with `False`.
 
     """
     time_vec = np.asarray(time_vec).squeeze()
     assert time_vec.ndim == 1, \
         'Function is implemented for 1D-arrays only'
 
-    # Find peak value index
-    max_ind = np.argmax(np.abs(time_vec))
+    # Normalization
+    if normalize:
+        time_vec /= np.abs(time_vec).max()
 
     # Power in dB
-    time_power = 20*np.log10(np.abs(time_vec))
-
-    # Normalization
-    time_power -= time_power[max_ind]
+    time_power = time_vec.squeeze()**2
 
-    # All indexes above threshold
-    indexes_above_0 = time_power > threshold_dbfs
-    indexes_above = np.zeros_like(indexes_above_0).astype(bool)
-
-    # Apply release and attack
-    for ind in np.arange(len(indexes_above)):
-        # Attack after certain amount of samples surpass threshold
-        ind_attack = 0 if ind-attack_samples < 0 else ind-attack_samples
-        if np.all(indexes_above_0[ind_attack:ind]):
-            indexes_above[ind:ind+release_samples] = True
-    return indexes_above
+    momentary_gain = np.zeros(len(time_power))
+    for i in np.arange(1, len(time_power)):
+        if momentary_gain[i] > time_power[i-1]:
+            coeff = attack_smoothing_coeff
+        elif momentary_gain[i] < time_power[i-1]:
+            coeff = release_smoothing_coeff
+        else:
+            coeff = 0
+        momentary_gain[i] = coeff*time_power[i] + (1-coeff)*momentary_gain[i-1]
+    momentary_gain = 10*np.log10(momentary_gain)
+
+    # Get Indices above threshold
+    indices_above = momentary_gain > threshold_dbfs
+    return indices_above
 
 
 def _detrend(time_data: np.ndarray, polynomial_order: int) -> np.ndarray:
     """Compute and return detrended signal.
 
     Parameters
     ----------
@@ -783,36 +618,41 @@
     time_indexes = np.arange(len(time_data))
     linear_trend = np.polyfit(time_indexes, time_data, deg=polynomial_order)
     for n in range(time_data.shape[1]):
         time_data[:, n] -= np.polyval(linear_trend[:, n], time_indexes)
     return time_data
 
 
-def _rms(x: np.ndarray) -> float:
-    """Root mean squared value of a discrete time series
+def _rms(x: np.ndarray) -> float | np.ndarray:
+    """Root mean squared value of a discrete time series.
 
     Parameters
     ----------
     x : `np.ndarray`
-        Time series
+        Time series.
 
     Returns
     -------
-    rms : float
-        Root mean squared value
+    rms : float or `np.ndarray`
+        Root mean squared of a signal. Float or np.ndarray depending on input.
 
     """
+    single_dim = False
     if x.ndim < 2:
+        single_dim = True
         x = x[..., None]
     elif x.ndim == 2:
         pass
     else:
         raise ValueError('Shape of array is not valid. Only 2D-Arrays ' +
                          'are valid')
-    return np.sqrt(np.mean(x**2, axis=0))
+    rms_vals = np.sqrt(np.mean(x**2, axis=0))
+    if single_dim:
+        rms_vals = np.squeeze(rms_vals)
+    return rms_vals
 
 
 def _get_framed_signal(td: np.ndarray, window_length_samples: int,
                        step_size: int, keep_last_frame: bool = True) \
         -> np.ndarray:
     """This method computes a framed version of a signal and returns it.
 
@@ -853,7 +693,92 @@
     for n in range(n_frames):
         td_framed[:, n, :] = td[start:start+window_length_samples, :].copy()
         start += step_size
 
     if not keep_last_frame:
         td_framed = td_framed[:, :-1, :]
     return td_framed
+
+
+def _reconstruct_framed_signal(td_framed: np.ndarray, step_size: int,
+                               window: str | np.ndarray = None,
+                               original_signal_length: int = None,
+                               safety_threshold: float = 1e-4) \
+        -> np.ndarray:
+    """Gets and returns a framed signal into its vector representation.
+
+    Parameters
+    ----------
+    td_framed : `np.ndarray`
+        Framed signal with shape (time samples, frame, channel).
+    step_size : int
+        Step size in samples between frames (also known as hop length).
+    window : str, `np.ndarray`, optional
+        Window (if applies). Pass `None` to avoid using a window during
+        reconstruction. Default: `None`.
+    original_signal_length : int, optional
+        When different than `None`, the output is padded or trimmed to this
+        length. Default: `None`.
+    safety_threshold : float, optional
+        When reconstructing the signal with a window, very small values can
+        lead to instabilities. This safety threshold avoids dividing with
+        samples beneath this value. Default: 1e-4.
+
+        Dividing by 1e-4 is the same as amplifying by 80 dB.
+
+    Returns
+    -------
+    td : `np.ndarray`
+        Reconstructed signal.
+
+    """
+    assert td_framed.ndim == 3, \
+        'Framed signal must contain exactly three dimensions'
+    if window is not None:
+        if type(window) == str:
+            window = windows.get_window(window, td_framed.shape[0])
+        elif type(window) == np.ndarray:
+            assert window.ndim == 1, \
+                'Window must be a 1D-array'
+            assert window.shape[0] == td_framed.shape[0], \
+                'Window length does not match signal length'
+        td_framed *= window[:, np.newaxis, np.newaxis]
+
+    total_length = int(step_size * td_framed.shape[1] +
+                       td_framed.shape[0]*(1 - step_size/td_framed.shape[0]))
+    td = np.zeros((total_length, td_framed.shape[-1]))
+
+    start = 0
+    for i in range(td_framed.shape[1]):
+        td[start:start+td_framed.shape[0], :] += td_framed[:, i, :]
+        start += step_size
+
+    if window is not None:
+        envelope = _get_window_envelope(
+            window, total_length, step_size,
+            td_framed.shape[1], True)
+        if safety_threshold is not None:
+            envelope = np.clip(envelope, a_min=safety_threshold, a_max=None)
+        non_zero = envelope > np.finfo(td.dtype).tiny
+        td[non_zero, ...] /= envelope[non_zero, np.newaxis]
+
+    if original_signal_length is not None:
+        td = _pad_trim(td, original_signal_length)
+    return td
+
+
+def _get_window_envelope(window: np.ndarray, total_length_samples: int,
+                         step_size_samples: int, number_frames: int,
+                         squared: bool = True):
+    """Compute the window envelope for a given window with step size and total
+    length. The window can be squared or not.
+
+    """
+    if squared:
+        window **= 2
+    envelope = np.zeros(total_length_samples)
+
+    start = 0
+    for _ in range(number_frames):
+        envelope[start:start+len(window)] += window
+        start += step_size_samples
+    return envelope
```

### Comparing `dsptoolbox-0.2.5/dsptoolbox/standard_functions.py` & `dsptoolbox-0.2.6/dsptoolbox/standard_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 from dsptoolbox.classes.multibandsignal import MultiBandSignal
 from dsptoolbox.classes.filterbank import FilterBank
 from dsptoolbox.classes.filter_class import Filter
 from dsptoolbox._standard import (_latency,
                                   _center_frequencies_fractional_octaves_iec,
                                   _exact_center_frequencies_fractional_octaves,
                                   _kaiser_window_beta,
-                                  _indexes_above_threshold_dbfs,
+                                  _indices_above_threshold_dbfs,
                                   _detrend, _rms)
 from dsptoolbox._general_helpers import (
-    _pad_trim, _normalize, _fade, _check_format_in_path)
+    _pad_trim, _normalize, _fade, _check_format_in_path,
+    _get_smoothing_factor_ema)
 from dsptoolbox.transfer_functions import (
     min_phase_from_mag, lin_phase_from_mag)
 
 
 def latency(in1: Signal, in2: Signal = None) -> np.ndarray:
     """Computes latency between two signals using the correlation method.
     If there is no second signal, the latency between the first and the other
@@ -223,14 +224,16 @@
 
     Returns
     -------
     new_sig : `Signal`
         Resampled signal.
 
     """
+    if sig.sampling_rate_hz == desired_sampling_rate_hz:
+        return sig.copy()
     ratio = Fraction(
         numerator=desired_sampling_rate_hz, denominator=sig.sampling_rate_hz)
     u, d = ratio.as_integer_ratio()
     new_time_data = resample_poly(sig.time_data, up=u, down=d, axis=0)
     new_sig = sig.copy()
     if hasattr(new_sig, 'window'):
         del new_sig.window
@@ -567,22 +570,22 @@
     b, _ = fir.get_coefficients(mode='ba')
     new_sig = Signal(
         None, b, sampling_rate_hz=fir.sampling_rate_hz, signal_type='ir',
         signal_id='IR from FIR filter')
     return new_sig
 
 
-def true_peak_level(sig: Signal | MultiBandSignal) \
+def true_peak_level(signal: Signal | MultiBandSignal) \
         -> tuple[np.ndarray, np.ndarray]:
     """Computes true-peak level of a signal using the standardized method
     by the Rec. ITU-R BS.1770-4. See references.
 
     Parameters
     ----------
-    sig : `Signal` or `MultiBandSignal`
+    signal : `Signal` or `MultiBandSignal`
         Signal for which to compute the true-peak level.
 
     Returns
     -------
     true_peak_levels : `np.ndarray`
         True-peak levels (in dBTP) as an array with shape (channels) or
         (band, channels) in case that the input signal is `MultiBandSignal`.
@@ -591,36 +594,31 @@
         (band, channels) in case that the input signal is `MultiBandSignal`.
 
     References
     ----------
     - https://www.itu.int/rec/R-REC-BS.1770
 
     """
-    if type(sig) == Signal:
+    if type(signal) == Signal:
+        sig = signal.copy()
         # Reduce gain by 12.04 dB
         down_factor = 10**(-12.04/20)
         up_factor = 1/down_factor
         sig.time_data *= down_factor
         # Resample by 4
         sig_over = resample(sig, sig.sampling_rate_hz*4)
-        true_peak_levels = np.empty(sig.number_of_channels)
-        peak_levels = np.empty_like(true_peak_levels)
-        # Find new peak value and add back 12.04 dB of gain
-        for n in range(sig.number_of_channels):
-            true_peak_levels[n] = \
-                20*np.log10(
-                    np.max(np.abs(sig_over.time_data[:, n])) * up_factor)
-            peak_levels[n] = \
-                20*np.log10(
-                    np.max(np.abs(sig.time_data[:, n])) * up_factor)
-    elif type(sig) == MultiBandSignal:
+        true_peak_levels = 20*np.log10(np.max(
+            np.abs(sig_over.time_data), axis=0) * up_factor)
+        peak_levels = 20*np.log10(np.max(
+            np.abs(sig.time_data), axis=0) * up_factor)
+    elif type(signal) == MultiBandSignal:
         true_peak_levels = \
-            np.empty((sig.number_of_bands, sig.number_of_channels))
+            np.empty((signal.number_of_bands, signal.number_of_channels))
         peak_levels = np.empty_like(true_peak_levels)
-        for ind, b in enumerate(sig.bands):
+        for ind, b in enumerate(signal.bands):
             true_peak_levels[ind, :], peak_levels[ind, :] = true_peak_level(b)
     else:
         raise TypeError(
             'Passed signal must be of type Signal or MultiBandSignal')
     return true_peak_levels, peak_levels
 
 
@@ -789,110 +787,129 @@
         out_sig.bands = new_bands
     else:
         raise TypeError('Passed signal should be either type Signal or ' +
                         'MultiBandSignal')
     return out_sig
 
 
-def activity_detector(signal: Signal, channel: int = 0,
-                      threshold_dbfs: float = -20, pre_filter: Filter = None,
-                      attack_time_ms: float = 0.5,
+def activity_detector(signal: Signal, threshold_dbfs: float = -20,
+                      channel: int = 0, relative_to_peak: bool = True,
+                      pre_filter: Filter = None, attack_time_ms: float = 1,
                       release_time_ms: float = 25) \
         -> tuple[Signal, dict]:
-    """This is a simple signal activity detector that uses a power threshold
-    relative to maximum peak level in a given signal (for one channel).
-    It returns the signal and a dictionary containing noise (as a signal) and
-    the time indexes corresponding to the bins that were found to surpass
+    """This is a simple signal activity detector that uses a power threshold.
+    It can be used relative to the signal's peak value or absolute. It is only
+    applicable to one channel of the signal. This function returns the signal
+    and a dictionary containing noise (as a signal) and
+    the time indices corresponding to the bins that were found to surpass
     the threshold according to attack and release times.
 
     Prefiltering (for example with a bandpass filter) is possible when a
     `pre_filter` is passed.
 
     See Returns to gain insight into the returned dictionary and its keys.
 
     Parameters
     ----------
     signal : `Signal`
         Signal in which to detect activity.
+    threshold_dbfs : float
+        Threshold in dBFS to separate noise from activity.
     channel : int, optional
         Channel in which to perform the detection. Default: 0.
-    threshold_dbfs : float, optional
-        Threshold in dBFS (relative to the signal's maximum peak level) to
-        separate noise from activity. Default: -20.
+    relative_to_peak : bool, optional
+        When `True`, the threshold value is relative to the signal's peak
+        value. Otherwise, it is regarded as an absolute threshold.
+        Default: `True`.
     pre_filter : `Filter`, optional
         Filter used for prefiltering the signal. It can be for instance a
         bandpass filter selecting the relevant frequencies in which the
         activity might be. Pass `None` to avoid any pre filtering.
         Default: `None`.
     attack_time_ms : float, optional
-        Attack time (in ms). It corresponds to the time that the signal has
-        to surpass the power threshold in order to be regarded as valid
-        acitivity. Pass 0 to attack immediately. Default: 0.5.
+        Attack time (in ms). It corresponds to a lag time for detecting
+        activity after surpassing the threshold. Default: 1.
     release_time_ms : float, optional
         Release time (in ms) for activity detector after signal has fallen
         below power threshold. Pass 0 to release immediately. Default: 25.
 
     Returns
     -------
     detected_sig : `Signal`
         Detected signal.
     others : dict
         Dictionary containing following keys:
         - `'noise'`: left-out noise in original signal (below threshold) as
           `Signal` object.
-        - `'signal_indexes'`: array of boolean that describes which indexes
+        - `'signal_indices'`: array of boolean that describes which indices
           of the original time series belong to signal and which to noise.
           `True` at index n means index n was passed to signal.
-        - `'noise_indexes'`: the inverse array to `'signal_indexes'`.
+        - `'noise_indices'`: the inverse array to `'signal_indices'`.
 
     """
     assert type(channel) == int, \
         'Channel must be type integer. Function is not implemented for ' +\
         'multiple channels.'
     assert threshold_dbfs < 0, \
         'Threshold must be below zero'
     assert release_time_ms >= 0, \
         'Release time must be positive'
+    assert attack_time_ms >= 0, \
+        'Attack time must be positive'
 
-    # Get relevant channel
+    # Get channel
     signal = signal.get_channels(channel)
 
     # Pre-filtering
     if pre_filter is not None:
         assert type(pre_filter) == Filter, \
             'pre_filter must be of type Filter'
-        assert signal.sampling_rate_hz == pre_filter.sampling_rate_hz, \
-            'Sampling rates for signal and pre filter do not match'
         signal_filtered = pre_filter.filter_signal(signal)
     else:
         signal_filtered = signal
 
     # Release samples
-    release_time_samples = int(release_time_ms*signal.sampling_rate_hz*1e-3)
-    attack_time_samples = int(attack_time_ms*signal.sampling_rate_hz*1e-3)
+    attack_coeff = _get_smoothing_factor_ema(
+        attack_time_ms/1e3, signal.sampling_rate_hz)
+    release_coeff = _get_smoothing_factor_ema(
+        release_time_ms/1e3, signal.sampling_rate_hz)
 
-    # Get indexes
-    signal_indexes = _indexes_above_threshold_dbfs(
+    # Get indices
+    signal_indices = _indices_above_threshold_dbfs(
         signal_filtered.time_data, threshold_dbfs=threshold_dbfs,
-        attack_samples=attack_time_samples,
-        release_samples=release_time_samples)
-    noise_indexes = ~signal_indexes
+        attack_smoothing_coeff=attack_coeff,
+        release_smoothing_coeff=release_coeff, normalize=relative_to_peak)
+    noise_indices = ~signal_indices
 
     # Separate signals
     detected_sig = signal.copy()
     noise = signal.copy()
     if hasattr(detected_sig, 'window'):
         del detected_sig.window
         del noise.window
-    detected_sig.time_data = signal.time_data[signal_indexes, 0]
-    noise.time_data = signal.time_data[noise_indexes, 0]
+
+    try:
+        detected_sig.time_data = signal.time_data[signal_indices, 0]
+    except ValueError as e:
+        warn('No detected activity, threshold might be too high. Detected ' +
+             'signal will be a vector filled with zeroes')
+        print('Numpy error: ', e)
+        detected_sig.time_data = np.zeros(500)
+
+    try:
+        noise.time_data = signal.time_data[noise_indices, 0]
+    except ValueError as e:
+        warn('No detected noise, threshold might be too low. Noise will be ' +
+             'a vector filled with zeroes')
+        print('Numpy error: ', e)
+        noise.time_data = np.zeros(500)
 
     others = dict(
-        noise=noise, signal_indexes=signal_indexes,
-        noise_indexes=noise_indexes)
+        noise=noise, signal_indices=signal_indices,
+        noise_indices=noise_indices)
     return detected_sig, others
 
 
 def detrend(sig: Signal | MultiBandSignal, polynomial_order: int = 0) \
         -> Signal | MultiBandSignal:
     """Returns the detrended signal.
```

### Comparing `dsptoolbox-0.2.5/dsptoolbox/audio_io/__init__.py` & `dsptoolbox-0.2.6/dsptoolbox/audio_io/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/dsptoolbox/audio_io/_audio_io.py` & `dsptoolbox-0.2.6/dsptoolbox/audio_io/_audio_io.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/dsptoolbox/audio_io/audio_io.py` & `dsptoolbox-0.2.6/dsptoolbox/audio_io/audio_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
     if type(play_channels) == int:
         play_channels = [play_channels]
     play_channels = sorted(play_channels)
     assert not any([r < 1 for r in play_channels]), \
         'Play channel has to be 1 or more'
     if duration_seconds is not None:
         assert duration_seconds > 0, 'Duration must be positive'
-        duration_samples = duration_seconds * signal.sampling_rate_hz
+        duration_samples = int(duration_seconds * signal.sampling_rate_hz)
     else:
         duration_seconds = signal.time_data.shape[0] / signal.sampling_rate_hz
         duration_samples = signal.time_data.shape[0]
     play_data = signal.time_data.copy()[:duration_samples, :]
     if normalized_dbfs is not None:
         assert normalized_dbfs <= 0, 'Only values beneath 0 dBFS are allowed'
         play_data = _normalize(play_data, dbfs=normalized_dbfs, mode='peak')
```

### Comparing `dsptoolbox-0.2.5/dsptoolbox/beamforming/__init__.py` & `dsptoolbox-0.2.6/dsptoolbox/beamforming/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/dsptoolbox/beamforming/_beamforming.py` & `dsptoolbox-0.2.6/dsptoolbox/beamforming/_beamforming.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Backend for beamforming module
 """
 import numpy as np
-from scipy.spatial import distance_matrix
+from dsptoolbox._general_helpers import _euclidean_distance_matrix
 import matplotlib.pyplot as plt
 from seaborn import set_style
 set_style('whitegrid')
 
 
 class BasePoints():
     """This is a base class for saving point data (like grids or mic arrays).
@@ -100,15 +100,15 @@
         """
         if type(point) != np.ndarray:
             point = np.asarray(point)
         if point.ndim == 1:
             point = point[None, ...]
         assert point.shape[1] == self.coordinates.shape[1], \
             f'Invalid shapes: {point.shape}, {self.coordinates.shape}'
-        return distance_matrix(self.coordinates, point, p=2).squeeze()
+        return _euclidean_distance_matrix(self.coordinates, point).squeeze()
 
     # ======== Plotting =======================================================
     def plot_points(self, projection: str = None):
         """Plot points in 2D or 3D plot depending on the actual points.
 
         Parameters
         ----------
```

### Comparing `dsptoolbox-0.2.5/dsptoolbox/beamforming/beamforming.py` & `dsptoolbox-0.2.6/dsptoolbox/beamforming/beamforming.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """
 Beamforming classes and functions
 """
 from warnings import warn
 import numpy as np
 import matplotlib.pyplot as plt
-from seaborn import set_style
 from scipy.integrate import simpson
 from matplotlib.figure import Figure
 from matplotlib.axes import Axes
 
 from dsptoolbox.classes import Signal
 from dsptoolbox import fractional_delay, merge_signals, pad_trim
 from dsptoolbox._general_helpers import (
     _get_fractional_octave_bandwidth, _find_nearest, _pad_trim)
 from ._beamforming import BasePoints, _clean_sc_deconvolve
 from dsptoolbox.plots import general_matrix_plot
 
-set_style('whitegrid')
+try:
+    from seaborn import set_style
+    set_style('whitegrid')
+except ModuleNotFoundError as e:
+    print('Seaborn will not be used for plotting: ', e)
+
 nxs = np.newaxis
 
 
 class Grid(BasePoints):
     """This class contains a grid to use for beamforming and all its metadata.
     This class is implemented only for right-hand systems with cartesian
     coordinates (in meters).
```

### Comparing `dsptoolbox-0.2.5/dsptoolbox/classes/__init__.py` & `dsptoolbox-0.2.6/dsptoolbox/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/dsptoolbox/classes/_filter.py` & `dsptoolbox-0.2.6/dsptoolbox/classes/_filter.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/dsptoolbox/classes/_plots.py` & `dsptoolbox-0.2.6/dsptoolbox/classes/_plots.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/dsptoolbox/classes/filter_class.py` & `dsptoolbox-0.2.6/dsptoolbox/classes/filter_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,14 @@
         self.warning_if_complex = True
         self.sampling_rate_hz = sampling_rate_hz
         if filter_configuration is None:
             filter_configuration = \
                 {'eq_type': 0, 'freqs': 1000, 'gain': 0, 'q': 1,
                  'filter_id': 'dummy'}
         self.set_filter_parameters(filter_type.lower(), filter_configuration)
-        self.initialize_zi()
 
     def initialize_zi(self, number_of_channels: int = 1):
         """Initializes zi for steady-state filtering. The number of parallel
         zi's can be defined externally.
 
         Parameters
         ----------
@@ -228,14 +227,16 @@
             assert all(channels < signal.number_of_channels),\
                 f'Selected channels ({channels}) are not valid for the ' +\
                 f'signal with {signal.number_of_channels} channels'
 
         # Zi – create always for all channels and selected channels will get
         # updated while filtering
         if activate_zi:
+            if not hasattr(self, 'zi'):
+                self.initialize_zi(signal.number_of_channels)
             if len(self.zi) != signal.number_of_channels:
                 warn('zi values of the filter have not been correctly ' +
                      'intialized for the number of channels. They have now' +
                      ' been corrected')
                 self.initialize_zi(signal.number_of_channels)
             zi_old = self.zi
         else:
@@ -603,15 +604,15 @@
         if self.info['order'] > length_samples:
             length_samples = self.info['order'] + 100
             warn(f'length_samples ({length_samples}) is shorter than the ' +
                  f'''filter order {self.info['order']}. Length will be ''' +
                  'automatically extended.')
         ir = self.get_ir(length_samples=length_samples, zero_phase=zero_phase)
         fig, ax = ir.plot_magnitude(
-            range_hz, normalize, show_info_box=False)
+            range_hz, normalize, show_info_box=False, scale=False)
         if show_info_box:
             txt = self._get_metadata_string()
             ax.text(0.1, 0.5, txt, transform=ax.transAxes,
                     verticalalignment='top',
                     bbox=dict(boxstyle='round', facecolor='grey', alpha=0.75))
         return fig, ax
```

### Comparing `dsptoolbox-0.2.5/dsptoolbox/classes/filterbank.py` & `dsptoolbox-0.2.6/dsptoolbox/classes/filterbank.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,14 +274,16 @@
         assert np.all(signal.sampling_rate_hz == self.sampling_rate_hz), \
             'Sampling rates do not match'
         if zero_phase:
             assert not activate_zi, \
                 'Zero-phase filtering and zi cannot be used at ' +\
                 'the same time'
         if activate_zi:
+            if not hasattr(self.filters[0], 'zi'):
+                self.initialize_zi(signal.number_of_channels)
             if len(self.filters[0].zi) != signal.number_of_channels:
                 self.initialize_zi(signal.number_of_channels)
 
         new_sig = _filterbank_on_signal(
             signal, self.filters,
             mode=mode,
             activate_zi=activate_zi,
@@ -319,14 +321,16 @@
         assert np.all(mbsignal.sampling_rate_hz == self.sampling_rate_hz), \
             'Sampling rates do not match'
         if zero_phase:
             assert not activate_zi, \
                 'Zero-phase filtering and zi cannot be used at ' +\
                 'the same time'
         if activate_zi:
+            if not hasattr(self.filters[0], 'zi'):
+                self.initialize_zi(mbsignal.number_of_channels)
             if len(self.filters[0].zi) != mbsignal.number_of_channels:
                 self.initialize_zi(mbsignal.number_of_channels)
 
         new_sig = mbsignal.copy()
 
         for n in range(mbsignal.number_of_bands):
             new_sig.bands[n] = self.filters[n].filter_signal(
```

### Comparing `dsptoolbox-0.2.5/dsptoolbox/classes/multibandsignal.py` & `dsptoolbox-0.2.6/dsptoolbox/classes/multibandsignal.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/dsptoolbox/classes/signal_class.py` & `dsptoolbox-0.2.6/dsptoolbox/classes/signal_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,28 +289,30 @@
         return self.time_data.shape[0]
 
     def __str__(self):
         return self._get_metadata_string()
 
     def set_spectrum_parameters(self, method='welch', smoothe: int = 0,
                                 window_length_samples: int = 1024,
-                                window_type='hann', overlap_percent=50,
-                                detrend=True, average='mean',
+                                window_type='hann',
+                                overlap_percent: float = 50, detrend=True,
+                                average='mean',
                                 scaling='power spectral density'):
         """Sets all necessary parameters for the computation of the spectrum.
 
         Parameters
         ----------
         method : str, optional
-            `'welch'` (Welch's method for stochastic signals) or
-            `'standard'` (Direct FFT from signal). Default: `'welch'`.
+            `'welch'` (Welch's method for stochastic signals, returns a
+            periodogramm) or `'standard'` (Direct FFT from signal).
+            Default: `'welch'`.
         smoothe : int, optional
-            Smoothing across (1/smoothe) octave bands using a hamming
-            window. Smoothes magnitude AND phase. For accesing the smoothing
-            algorithm, refer to
+            Smoothing across (`1/smoothe`) octave bands using a hamming
+            window. It only applies when `method='standard'`. Smoothes
+            magnitude AND phase. For accesing the smoothing algorithm, refer to
             `dsptoolbox._general_helpers._fractional_octave_smoothing()`.
             If smoothing is applied here, `Signal.get_spectrum()` returns
             the smoothed spectrum as well and `Signal.plot_magnitude()` plots
             the smoothed version. Default: 0 (no smoothing).
         window_length_samples : int, optional
             Window size. Default: 1024.
         window_type : str, optional
@@ -408,15 +410,16 @@
             'does not match'
         self.coherence = coherence
 
     def set_csm_parameters(self, window_length_samples: int = 1024,
                            window_type='hann', overlap_percent=75,
                            detrend=True, average='mean',
                            scaling='power spectral density'):
-        """Sets all necessary parameters for the computation of the CSM.
+        """Sets all necessary parameters for the computation of the
+        cross-spectral matrix.
 
         Parameters
         ----------
         window_length_samples : int, optional
             Window size. Default: 1024.
         overlap_percent : float, optional
             Overlap in percent. Default: 75.
@@ -454,43 +457,42 @@
             handler = \
                 [self._csm_parameters[k] == _new_csm_parameters[k]
                  for k in self._csm_parameters.keys()]
             if not all(handler):
                 self._csm_parameters = _new_csm_parameters
                 self.__csm_state_update = True
 
-    def set_spectrogram_parameters(self, channel_number: int = 0,
+    def set_spectrogram_parameters(self,
                                    window_length_samples: int = 1024,
                                    window_type: str = 'hann',
                                    overlap_percent=50,
                                    fft_length_samples: int = None,
-                                   detrend: bool = True, padding: bool = True,
+                                   detrend: bool = False, padding: bool = True,
                                    scaling: bool = False):
         """Sets all necessary parameters for the computation of the
         spectrogram.
 
         Parameters
         ----------
-        channel_number : int, optional
-            Channel for which to compute the spectrogram. Default: 0.
         window_length_samples : int, optional
             Window size. Default: 1024.
         window_type : str, optional
             Type of window to use. Default: `'hann'`.
         overlap_percent : float, optional
             Overlap in percent. Default: 50.
         fft_length_samples : int, optional
             Length of the FFT window for each time window. This affects
             the frequency resolution and can also crop the time window. Pass
             `None` to use the window length. Default: `None`.
         detrend : bool, optional
-            Detrending (subtracting mean). Default: `True`.
+            Detrending (subtracting mean) for each time frame.
+            Default: `False`.
         padding : bool, optional
-            Padding signal in the beginning and end to center it.
-            Default: True.
+            Padding signal in the beginning and end to center it in order
+            to avoid losing energy because of windowing. Default: `True`.
         scaling : bool, optional
             When `True`, the output is scaled as an amplitude spectrum,
             otherwise no scaling is applied. See references for details.
             Default: `False`.
 
         References
         ----------
@@ -498,15 +500,14 @@
           spectral density estimation by the Discrete Fourier transform (DFT),
           including a comprehensive list of window functions and some new
           at-top windows.
 
         """
         _new_spectrogram_parameters = \
             dict(
-                channel_number=channel_number,
                 window_length_samples=window_length_samples,
                 window_type=window_type,
                 overlap_percent=overlap_percent,
                 fft_length_samples=fft_length_samples,
                 detrend=detrend,
                 padding=padding,
                 scaling=scaling)
@@ -741,45 +742,39 @@
 
         if condition:
             self.csm = _csm(self.time_data, self.sampling_rate_hz,
                             **self._csm_parameters)
             self.__csm_state_update = False
         return self.csm[0].copy(), self.csm[1].copy()
 
-    def get_spectrogram(self, channel_number: int = 0,
-                        force_computation: bool = False) -> \
+    def get_spectrogram(self, force_computation: bool = False) -> \
             tuple[np.ndarray, np.ndarray, np.ndarray]:
         """Returns a matrix containing the STFT of a specific channel.
 
         Parameters
         ----------
-        channel_number : int, optional
-            Channel number for which to compute the STFT. Default: 0.
         force_computation : bool, optional
             Forces new computation of the STFT. Default: False.
 
         Returns
         -------
         t_s : `np.ndarray`
             Time vector.
         f_hz : `np.ndarray`
             Frequency vector.
         spectrogram : `np.ndarray`
-            Complex spectrogram with shape (frequency, time).
+            Complex spectrogram with shape (frequency, time, channel).
 
         """
         condition = not hasattr(self, 'spectrogram') or force_computation or \
-            self.__spectrogram_state_update or \
-            not channel_number == \
-            self._spectrogram_parameters['channel_number']
+            self.__spectrogram_state_update
 
         if condition:
-            self._spectrogram_parameters['channel_number'] = channel_number
             self.spectrogram = _stft(
-                self.time_data[:, channel_number],
+                self.time_data,
                 self.sampling_rate_hz,
                 self._spectrogram_parameters['window_length_samples'],
                 self._spectrogram_parameters['window_type'],
                 self._spectrogram_parameters['overlap_percent'],
                 self._spectrogram_parameters['fft_length_samples'],
                 self._spectrogram_parameters['detrend'],
                 self._spectrogram_parameters['padding'],
@@ -804,15 +799,16 @@
             'There is no coherence data saved in the Signal object'
         f, _ = self.get_spectrum()
         return f, self.coherence
 
     # ======== Plots ==========================================================
     def plot_magnitude(self, range_hz=[20, 20e3], normalize: str = '1k',
                        range_db=None, smoothe: int = 0,
-                       show_info_box: bool = False) -> tuple[Figure, Axes]:
+                       show_info_box: bool = False, scale: bool = True) \
+            -> tuple[Figure, Axes]:
         """Plots magnitude spectrum.
         Change parameters of spectrum with set_spectrum_parameters.
 
         Parameters
         ----------
         range_hz : array-like with length 2, optional
             Range for which to plot the magnitude response.
@@ -829,14 +825,20 @@
         smoothe : int, optional
             Smoothing across the (1/smoothe) octave band.
             Default: 0 (no smoothing).
         show_info_box : bool, optional
             Plots a info box regarding spectrum parameters and plot parameters.
             If it is str, it overwrites the standard message.
             Default: `False`.
+        scale : bool, optional
+            When `True`, spectrum gets scaled (divided) by double the length
+            of the time signal. This ensures that the energy of the time signal
+            is distributed in the whole spectrum. This only applies when
+            `method = 'standard'` and no normalization is applied.
+            Default: `True`.
 
         Returns
         -------
         fig : `matplotlib.figure.Figure`
             Figure.
         ax : `matplotlib.axes.Axes`
             Axes.
@@ -847,15 +849,15 @@
         - In case the signal has been calibrated and the time data is given in
           Pascal, the plotted values in dB will be scaled by p0=(20e-6 Pa)**2
           when no normalization is active.
 
         """
         f, sp = self.get_spectrum()
         if self._spectrum_parameters['method'] == 'standard' \
-                and normalize is None:
+                and normalize is None and scale:
             sp = sp/self.time_data.shape[0]*2
         f, mag_db = _get_normalized_spectrum(
             f=f,
             spectra=sp,
             mode=self._spectrum_parameters['method'],
             f_range_hz=range_hz,
             normalize=normalize,
@@ -972,15 +974,20 @@
         -------
         fig : `matplotlib.figure.Figure`
             Figure.
         ax : `matplotlib.axes.Axes`
             Axes.
 
         """
-        t, f, stft = self.get_spectrogram(channel_number)
+        # Get whole spectrogram
+        t, f, stft = self.get_spectrogram()
+
+        # Select channel
+        stft = stft[:, :, channel_number]
+
         ids = _find_nearest([20, 20000], f)
         if ids[0] == 0:
             ids[0] += 1
         f = f[ids[0]:ids[1]]
         stft = stft[ids[0]:ids[1], :]
         stft_db = 20*np.log10(np.clip(np.abs(stft), 1e-20, None))
         stft_db = np.nan_to_num(stft_db, nan=np.min(stft_db))
```

### Comparing `dsptoolbox-0.2.5/dsptoolbox/distances/_distances.py` & `dsptoolbox-0.2.6/dsptoolbox/distances/_distances.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/dsptoolbox/distances/distances.py` & `dsptoolbox-0.2.6/dsptoolbox/distances/distances.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/dsptoolbox/filterbanks/__init__.py` & `dsptoolbox-0.2.6/dsptoolbox/filterbanks/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/dsptoolbox/filterbanks/_filterbank.py` & `dsptoolbox-0.2.6/dsptoolbox/filterbanks/_filterbank.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/dsptoolbox/filterbanks/filterbanks.py` & `dsptoolbox-0.2.6/dsptoolbox/filterbanks/filterbanks.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/dsptoolbox/generators/generators.py` & `dsptoolbox-0.2.6/dsptoolbox/generators/generators.py`

 * *Files 15% similar despite different names*

```diff
@@ -247,15 +247,15 @@
              number_of_channels: int = 1, uncorrelated: bool = False,
              fade: str = 'log', padding_end_seconds: float = None) -> Signal:
     """Creates a multi-channel harmonic (sine) tone.
 
     Parameters
     ----------
     frequency_hz : float, optional
-        Frequency (in Hz) for the sinus tone. Default: 1000.
+        Frequency (in Hz) for the sine tone. Default: 1000.
     length_seconds : float, optional
         Length of the generated signal in seconds. Default: 1.
     sampling_rate_hz : int
         Sampling rate in Hz. Default: `None`.
     peak_level_dbfs : float, optional
         Peak level of the signal in dBFS. Default: -10.
     number_of_channels : int, optional
@@ -287,24 +287,143 @@
 
     if padding_end_seconds not in (None, 0):
         assert padding_end_seconds > 0, 'Padding has to be a positive time'
         p_samples = int(padding_end_seconds * sampling_rate_hz)
     else:
         p_samples = 0
     l_samples = int(sampling_rate_hz * length_seconds)
-    n_vec = np.arange(l_samples)
+    n_vec = np.arange(l_samples)[..., None]
+    n_vec = np.repeat(n_vec, number_of_channels, axis=-1)
 
-    td = np.empty((l_samples, number_of_channels))
-    for n in range(number_of_channels):
-        if uncorrelated:
-            phase_shift = np.random.uniform(-np.pi, np.pi)
-        else:
-            phase_shift = 0
-        td[:, n] = np.sin(
-            frequency_hz / sampling_rate_hz * 2 * np.pi * n_vec + phase_shift)
+    # Frequency vector
+    n_vec = frequency_hz / sampling_rate_hz * 2 * np.pi * n_vec
+    # Apply phase shift
+    if uncorrelated:
+        n_vec += np.random.uniform(-np.pi, np.pi, (number_of_channels))
+    # Generate wave
+    td = np.sin(n_vec)
+
+    td = _normalize(td, peak_level_dbfs, mode='peak')
+
+    if fade is not None:
+        fade_length = 0.05 * length_seconds
+        td = _fade(
+            s=td, length_seconds=fade_length, mode=fade,
+            sampling_rate_hz=sampling_rate_hz, at_start=True)
+        td = _fade(
+            s=td, length_seconds=fade_length, mode=fade,
+            sampling_rate_hz=sampling_rate_hz, at_start=False)
+
+    td = _pad_trim(td, l_samples+p_samples)
+
+    # Signal
+    harmonic_sig = Signal(None, td, sampling_rate_hz,
+                          signal_type='general')
+    return harmonic_sig
+
+
+def oscillator(frequency_hz: float = 1000, length_seconds: float = 1,
+               mode: str = 'harmonic', harmonic_cutoff_hz: float = None,
+               sampling_rate_hz: int = None, peak_level_dbfs: float = -10,
+               number_of_channels: int = 1, uncorrelated: bool = False,
+               fade: str = 'log', padding_end_seconds: float = None) -> Signal:
+    """Creates a non-aliased, multi-channel wave tone.
+
+    Parameters
+    ----------
+    frequency_hz : float, optional
+        Frequency (in Hz). Default: 1000.
+    length_seconds : float, optional
+        Length of the generated signal in seconds. Default: 1.
+    mode : str, optional
+        Type of wave to generate. Choose from `'harmonic'`, `'square'`,
+        `'triangle'` or `'sawtooth'`. Default: `'harmonic'`.
+    harmonic_cutoff_hz : float, optional
+        It is possible to pass a cutoff frequency for the harmonics. If `None`,
+        they are computed up until before the nyquist frequency.
+        Default: `None`.
+    sampling_rate_hz : int
+        Sampling rate in Hz. Default: `None`.
+    peak_level_dbfs : float, optional
+        Peak level of the signal in dBFS. Default: -10.
+    number_of_channels : int, optional
+        Number of channels to be created. Default: 1.
+    uncorrelated : bool, optional
+        When `True`, each channel gets a random phase shift so that the signals
+        are not perfectly correlated. Default: `False`.
+    fade : str, optional
+        Type of fade done on the generated signal. By default, 5% of signal
+        length (without the padding in the end) is faded at the beginning and
+        end. Options are `'exp'`, `'lin'`, `'log'`.
+        Pass `None` for no fading. Default: `'log'`.
+    padding_end_seconds : float, optional
+        Padding at the end of signal. Use `None` to avoid any padding.
+        Default: `None`.
+
+    Returns
+    -------
+    wave_signal : `Signal`
+        Wave signal.
+
+    """
+    mode = mode.lower()
+    assert mode in ('harmonic', 'square', 'triangle', 'sawtooth'), \
+        f'{mode} is not a valid mode. Choose harmonic, square, triangle ' +\
+        'or sawtooth'
+    assert sampling_rate_hz is not None, \
+        'Sampling rate can not be None'
+    assert frequency_hz < sampling_rate_hz//2, \
+        'Frequency must be beneath nyquist frequency'
+    assert frequency_hz > 0, \
+        'Frequency must be bigger than 0'
+
+    if padding_end_seconds not in (None, 0):
+        assert padding_end_seconds > 0, 'Padding has to be a positive time'
+        p_samples = int(padding_end_seconds * sampling_rate_hz)
+    else:
+        p_samples = 0
+    l_samples = int(sampling_rate_hz * length_seconds)
+    n = np.arange(l_samples)[..., None]
+    n = np.repeat(n, number_of_channels, axis=-1)
+
+    if harmonic_cutoff_hz is None:
+        harmonic_cutoff_hz = sampling_rate_hz//2
+    assert harmonic_cutoff_hz > 0 and \
+        harmonic_cutoff_hz <= sampling_rate_hz//2, \
+        'Cutoff frequency must be between 0 and the nyquist frequency!'
+
+    if uncorrelated:
+        phase_shift = \
+            np.random.uniform(-np.pi, np.pi, (number_of_channels))[None, ...]
+    else:
+        phase_shift = np.zeros((number_of_channels))[None, ...]
+
+    # Get waveforms
+    td = np.zeros((l_samples, number_of_channels))
+    k = 1
+    if mode == 'harmonic':
+        td = np.sin(2*np.pi*frequency_hz/sampling_rate_hz * n + phase_shift)
+    elif mode == 'square':
+        while (2*k-1)*frequency_hz < harmonic_cutoff_hz:
+            td += (np.sin(np.pi * 2 * (2*k-1) * frequency_hz / sampling_rate_hz
+                          * n + phase_shift)/(2*k-1))
+            k += 1
+        td *= (4/np.pi)
+    elif mode == 'sawtooth':
+        while k*frequency_hz < harmonic_cutoff_hz:
+            td += (np.sin(np.pi * 2 * k * frequency_hz / sampling_rate_hz
+                          * n + phase_shift)/k * (-1)**k)
+            k += 1
+        td *= -(2/np.pi)
+    else:
+        while (2*k-1)*frequency_hz < harmonic_cutoff_hz:
+            td += (np.sin(np.pi * 2 * (2*k-1) * frequency_hz / sampling_rate_hz
+                          * n + phase_shift)/(2*k-1)**2 * (-1)**k)
+            k += 1
+        td *= (-8/np.pi**2)
 
     td = _normalize(td, peak_level_dbfs, mode='peak')
 
     if fade is not None:
         fade_length = 0.05 * length_seconds
         td = _fade(
             s=td, length_seconds=fade_length, mode=fade,
```

### Comparing `dsptoolbox-0.2.5/dsptoolbox/plots/plots.py` & `dsptoolbox-0.2.6/dsptoolbox/plots/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 """
 Includes some basic plotting templates
 """
 import matplotlib.pyplot as plt
 from matplotlib.ticker import ScalarFormatter
 from matplotlib import cm
-from numpy import array, max, min
-from seaborn import set_style
-set_style('whitegrid')
+from numpy import array, max, min, arange
+
+try:
+    from seaborn import set_style
+    set_style('whitegrid')
+except ModuleNotFoundError as e:
+    print('Seaborn will not be used for plotting: ', e)
+    pass
 
 
 def show():
     """Show created plots by using this wrapper around matplotlib's show.
 
     """
     plt.show()
@@ -21,15 +26,15 @@
                  ylabel: str = None, info_box: str = None,
                  tight_layout: bool = True, returns: bool = False):
     """Generic plot template.
 
     Parameters
     ----------
     x : array-like
-        Vector for x axis.
+        Vector for x axis. Pass `None` to ignore.
     matrix : `np.ndarray`
         Matrix with data to plot.
     range_x : array-like, optional
         Range to show for x axis. Default: None.
     range_y : array-like, optional
         Range to show for y axis. Default: None.
     log : bool, optional
@@ -54,15 +59,17 @@
         Returned only when `returns=True`.
 
     """
     fig, ax = plt.subplots(1, 1, figsize=(8, 5))
     if matrix.ndim == 1:
         matrix = matrix[..., None]
     elif matrix.ndim > 2:
-        raise ValueError('Only 2D-arrays are supported')
+        raise ValueError('Only 1D and 2D-arrays are supported')
+    if x is None:
+        x = arange(matrix.shape[0])
     if labels is not None:
         if type(labels) not in (list, tuple):
             assert type(labels) == str, \
                 'labels should be a list or a string'
             labels = [labels]
     for n in range(matrix.shape[1]):
         if labels is not None:
```

### Comparing `dsptoolbox-0.2.5/dsptoolbox/room_acoustics/__init__.py` & `dsptoolbox-0.2.6/dsptoolbox/room_acoustics/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/dsptoolbox/room_acoustics/_room_acoustics.py` & `dsptoolbox-0.2.6/dsptoolbox/room_acoustics/_room_acoustics.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/dsptoolbox/room_acoustics/room_acoustics.py` & `dsptoolbox-0.2.6/dsptoolbox/room_acoustics/room_acoustics.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/dsptoolbox/special/__init__.py` & `dsptoolbox-0.2.6/dsptoolbox/special/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,16 +8,17 @@
   with mel frequency axis)
 - `mel_filterbank()` (returns matrix with triangular mel filters used to
   convert spectrograms' frequency axis from Hz into mel)
 - `plot_waterfall()` (creates and returns a waterfall plot)
 
 """
 from .special import (cepstrum, log_mel_spectrogram, mel_filterbank,
-                      plot_waterfall, mfcc)
+                      plot_waterfall, mfcc, istft)
 
 __all__ = [
     'cepstrum',
     'log_mel_spectrogram',
     'mel_filterbank',
     'plot_waterfall',
     'mfcc',
+    'istft',
 ]
```

### Comparing `dsptoolbox-0.2.5/dsptoolbox/transfer_functions/__init__.py` & `dsptoolbox-0.2.6/dsptoolbox/transfer_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/dsptoolbox/transfer_functions/_transfer_functions.py` & `dsptoolbox-0.2.6/dsptoolbox/transfer_functions/_transfer_functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,15 +37,21 @@
         raise ValueError(f'{mode} is not supported. Choose window' +
                          ', regularized or standard')
     return new_time_data
 
 
 def _window_this_ir(vec, total_length: int, window_type: str = 'hann',
                     exp2_trim: int = 13, constant_percentage: float = 0.75,
-                    at_start: bool = True) -> tuple[np.ndarray, np.ndarray]:
+                    at_start: bool = True) -> \
+        tuple[np.ndarray, np.ndarray, np.ndarray]:
+    """This function finds the index of the impulse and trims or windows it
+    accordingly. Window used and the start sample are returned.
+
+    """
+    start_sample = 0
     # Trimming
     if exp2_trim is not None:
         # Padding
         if 2**exp2_trim >= len(vec):
             # Padding
             vec = np.hstack([vec, np.zeros(total_length - len(vec))])
             length = np.argmax(abs(vec))
@@ -53,14 +59,15 @@
             # Selecting
             assert constant_percentage > 0 and constant_percentage < 1,\
                 'Constant percentage must be between 0 and 1'
             length = int((1-constant_percentage)*2**exp2_trim)//2
             ind_max = np.argmax(abs(vec))
             if ind_max - length < 0:
                 length = ind_max
-            vec = vec[ind_max-length:ind_max-length+2**exp2_trim]
+            start_sample = ind_max-length
+            vec = vec[start_sample:start_sample+2**exp2_trim]
     else:
         length = np.argmax(abs(vec))
     points = [0, length, total_length-length, total_length]
     window = _calculate_window(points, total_length, window_type,
                                at_start=at_start)
-    return vec*window, window
+    return vec*window, window, start_sample
```

### Comparing `dsptoolbox-0.2.5/dsptoolbox/transfer_functions/transfer_functions.py` & `dsptoolbox-0.2.6/dsptoolbox/transfer_functions/transfer_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,18 +116,17 @@
     if padding:
         if keep_original_length:
             new_sig.time_data = _pad_trim(new_sig.time_data, original_length)
     return new_sig
 
 
 def window_ir(signal: Signal, constant_percentage=0.75, exp2_trim: int = 13,
-              window_type='hann', at_start: bool = True) -> Signal:
-    """Windows an IR in time while trimming or padding it to an expected
-    length. One half of the window is used for the start and the other for
-    the end.
+              window_type='hann', at_start: bool = True) \
+        -> tuple[Signal, np.ndarray]:
+    """Windows an IR with trimming and selection of constant valued length.
 
     Parameters
     ----------
     signal: `Signal`
         Signal to window
     constant_percentage: float, optional
         Percentage (between 0 and 1) of the window's length that should be
@@ -138,47 +137,51 @@
     window_type: str, optional
         Window function to be used. Available selection from
         scipy.signal.windows: `barthann`, `bartlett`, `blackman`,
         `boxcar`, `cosine`, `hamming`, `hann`, `flattop`, `nuttall` and
         others. Pass a tuple with window type and extra parameters if needed.
         Default: `hann`.
     at_start: bool, optional
-        When `True`, the start is windowed as well as the end. When `False`,
-        only the end is windowed. Default: `True`.
+        Windows the start with a rising window as well as the end.
+        Default: `True`.
 
     Returns
     -------
     new_sig : `Signal`
         Windowed signal. The used window is also saved under `new_sig.window`.
+    start_positions_samples : `np.ndarray`
+        This array contains the position index of the start of the IR in
+        each channel of the original IR.
 
     """
     assert signal.signal_type in ('rir', 'ir'), \
         f'{signal.signal_type} is not a valid signal type. Use rir or ir.'
     if exp2_trim is not None:
         total_length = int(2**exp2_trim)
     else:
         total_length = len(signal.time_data)
     new_time_data = np.zeros((total_length, signal.number_of_channels))
+    start_positions_samples = np.zeros(signal.number_of_channels, dtype=int)
 
     window = np.zeros((total_length, signal.number_of_channels))
     for n in range(signal.number_of_channels):
-        new_time_data[:, n], window[:, n] = \
+        new_time_data[:, n], window[:, n], start_positions_samples[n] = \
             _window_this_ir(
                 signal.time_data[:, n],
                 total_length,
                 window_type,
                 exp2_trim,
                 constant_percentage,
                 at_start)
 
     new_sig = Signal(
         None, new_time_data, signal.sampling_rate_hz,
         signal_type=signal.signal_type)
     new_sig.set_window(window)
-    return new_sig
+    return new_sig, start_positions_samples
 
 
 def compute_transfer_function(output: Signal, input: Signal, mode='h2',
                               window_length_samples: int = 1024,
                               spectrum_parameters: dict = None) -> \
         tuple[Signal, np.ndarray]:
     """Gets transfer function H1, H2 or H3 (for stochastic signals).
```

### Comparing `dsptoolbox-0.2.5/examples/audio_io_module.ipynb` & `dsptoolbox-0.2.6/examples/audio_io_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/examples/beamforming_module.ipynb` & `dsptoolbox-0.2.6/examples/beamforming_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/examples/distances_module.ipynb` & `dsptoolbox-0.2.6/examples/distances_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/examples/filterbanks_module.ipynb` & `dsptoolbox-0.2.6/examples/filterbanks_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/examples/general.ipynb` & `dsptoolbox-0.2.6/examples/general.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/examples/generators_module.ipynb` & `dsptoolbox-0.2.6/examples/generators_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/examples/room_acoustics_module.ipynb` & `dsptoolbox-0.2.6/examples/room_acoustics_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/examples/transfer_function_module.ipynb` & `dsptoolbox-0.2.6/examples/transfer_function_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/examples/data/array.xml` & `dsptoolbox-0.2.6/examples/data/array.xml`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/examples/data/chirp.wav` & `dsptoolbox-0.2.6/examples/data/chirp.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/examples/data/chirp_mono.wav` & `dsptoolbox-0.2.6/examples/data/chirp_mono.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/examples/data/chirp_stereo.wav` & `dsptoolbox-0.2.6/examples/data/chirp_stereo.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/examples/data/rir.wav` & `dsptoolbox-0.2.6/examples/data/rir.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/examples/data/speech.flac` & `dsptoolbox-0.2.6/examples/data/speech.flac`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/tests/manual_filter_testing.py` & `dsptoolbox-0.2.6/tests/manual_filter_testing.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/tests/manual_testing.py` & `dsptoolbox-0.2.6/tests/manual_testing.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,14 +103,15 @@
         exit()
 
     raw = dsp.Signal(join('examples', 'data', 'chirp.wav'))
     raw.set_spectrogram_parameters(
         window_length_samples=2048, scaling=False, overlap_percent=75,
         padding=False)
     t, f, stft = raw.get_spectrogram()
+    stft = stft[..., 0]
     D = librosa.stft(raw.time_data.squeeze(), center=False)
     print(np.all(np.isclose(stft[1:, :-4], D[1:])))
     # exit()
     plt.subplot(121)
     st_abs = 20*np.log10(np.abs(stft))
     plt.imshow(st_abs, origin='lower', aspect='auto',
                vmin=np.max(st_abs)-100, vmax=np.max(st_abs)+10)
@@ -689,27 +690,27 @@
     ns = dsp.generators.noise(
         length_seconds=3, sampling_rate_hz=sp.sampling_rate_hz)
     sp = dsp.beamforming.MonopoleSource(sp, [0, -0.5, 0.5])
     ns = dsp.beamforming.MonopoleSource(ns, [0, 0, 0.5])
     s = dsp.beamforming.mix_sources_on_array([sp, ns], ma)
 
     s_trial = s.get_channels(5)
-    s_trial.save_signal('/Users/neumanndev/Downloads/direct')
+    s_trial.save_signal('direct_sound')
 
     # Grid
     xval = np.arange(-0.5, 0.5, 0.1)
     g = dsp.beamforming.LineGrid(xval, 'y', 0.5, 0)
 
     bf = dsp.beamforming.BeamformerDASTime(s, ma, g)
     _, ax = bf.plot_setting()
     ax.scatter(ns.coordinates[0], ns.coordinates[1], ns.coordinates[2])
     ax.scatter(sp.coordinates[0], sp.coordinates[1], sp.coordinates[2])
 
     out_sig = bf.get_beamformer_output()
-    out_sig.save_signal('/Users/neumanndev/Downloads/beamformer_time')
+    out_sig.save_signal('beamformer_time')
     dsp.plots.show()
 
 
 def beamforming_3d_grid():
     # Small mic array
     micsx = np.arange(-0.1, 0.11, 0.1)
     micsy = np.arange(-0.3, 0.31, 0.1)
@@ -839,14 +840,87 @@
 
     mels, _ = dsp.special.mel_filterbank(f, [20, 10e3], n_bands=40)
     t, mel, mf, fig, ax = dsp.special.mfcc(sp, mel_filters=mels)
 
     dsp.plots.show()
 
 
+def activity_detector():
+    speech = dsp.Signal(join('examples', 'data', 'speech.flac'))
+    n = dsp.generators.noise('blue', len(speech)/speech.sampling_rate_hz,
+                             speech.sampling_rate_hz, peak_level_dbfs=-20)
+    speech.time_data += n.time_data
+    act, rest = dsp.activity_detector(
+        speech, channel=0,
+        threshold_dbfs=-30,
+        attack_time_ms=0.2,
+        release_time_ms=40)
+
+    # Original
+    speech.plot_time()
+
+    # Detected activity
+    act.plot_time()
+
+    # Noise
+    rest['noise'].plot_time()
+
+    # Listen to the example
+    # dsp.audio_io.set_device()
+    dsp.audio_io.play(act)
+    dsp.audio_io.play(rest['noise'])
+
+    # Signal power in dBFS
+    data = 20*np.log10(np.abs(speech.time_data))
+    data -= data.max()
+    dsp.plots.general_plot(
+        speech.time_vector_s, data,
+        log=False, xlabel='Time / s', ylabel='Power / dBFS')
+    dsp.plots.show()
+
+
+def istft():
+    sp = dsp.Signal(join('examples', 'data', 'speech.flac'))
+    sp = dsp.merge_signals(sp, sp)
+    sp.set_spectrogram_parameters(padding=False)
+    t, f, s = sp.get_spectrogram()
+    rec = dsp.special.istft(s, original_signal=sp)
+    sp.plot_time()
+    rec.plot_time()
+    # plt.plot(np.abs(rec.time_data - sp.time_data))
+    print(np.all(np.isclose(rec.time_data, sp.time_data)))
+    plt.show()
+    dsp.audio_io.set_device(1)
+    dsp.audio_io.play(sp)
+    dsp.audio_io.play(rec)
+
+
+def spectral_subtractor():
+    speech = dsp.Signal(join('examples', 'data', 'speech.flac'))
+    n = dsp.generators.noise('blue', len(speech)/speech.sampling_rate_hz,
+                             speech.sampling_rate_hz, peak_level_dbfs=-20)
+    speech.time_data += n.time_data
+    n.set_spectrum_parameters(scaling=None)
+    f, sp = n.get_spectrum()
+
+    speech = dsp.normalize(speech)
+
+    sub = dsp.effects.SpectralSubtractor(threshold_rms_dbfs=-30,
+                                         adaptive_mode=False,
+                                         spectrum_to_subtract=sp)
+    sub.set_advanced_parameters(noise_forgetting_factor=0.8)
+    speech_den = sub.apply(speech)
+
+    td = speech.time_data - speech_den.time_data
+    speech_den.plot_time()
+    plt.figure()
+    plt.plot(td)
+    plt.show()
+
+
 if __name__ == '__main__':
     # transfer_function_test()
     # new_transfer_functions()
     # welch_method()
     # csm()
     # group_delay()
     # stft()
@@ -875,14 +949,17 @@
     # beamforming_basics()
     # beamforming_steering_test()
     # beamforming_virtual_source()
     # beamforming_complete_test_2D()
     # beamforming_complete_test_time()
     # cepstrum()
     # beamforming_3d_grid()
-    # beamforming_frequency_formulations()
+    beamforming_frequency_formulations()
     # detrending()
     # iterators()
     # mfcc()
+    # istft()
+    # spectral_subtractor()
+    # activity_detector()
 
     # Next
     print()
```

### Comparing `dsptoolbox-0.2.5/tests/test_beamforming.py` & `dsptoolbox-0.2.6/tests/test_beamforming.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/tests/test_classes.py` & `dsptoolbox-0.2.6/tests/test_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,32 +198,34 @@
         s = dsp.Signal(time_data=self.time_vec, sampling_rate_hz=self.fs)
         f, csm = s.get_csm()
 
     def test_get_stft(self):
         s = dsp.Signal(time_data=self.time_vec, sampling_rate_hz=self.fs)
         # Use parameters just like librosa for validation
         s.set_spectrogram_parameters(
-            channel_number=0, window_length_samples=1024,
-            window_type='hann', overlap_percent=50, fft_length_samples=4096,
+            window_length_samples=1024,
+            window_type='hann', overlap_percent=50,
+            fft_length_samples=4096,
             detrend=False, padding=False, scaling=False)
         t, f, stft = s.get_spectrogram()
         s.set_spectrogram_parameters(
-            channel_number=0, window_length_samples=1024,
-            window_type='hann', overlap_percent=50, fft_length_samples=None,
+            window_length_samples=1024,
+            window_type='hann', overlap_percent=50,
+            fft_length_samples=None,
             detrend=False, padding=False, scaling=False)
         t, f, stft = s.get_spectrogram()
 
         # Validate result with librosa library if installed
         try:
             import librosa
             y = librosa.stft(
                 self.time_vec[:, 0], n_fft=1024, hop_length=1024//2,
                 window='hann', center=False)
             # There are some extra frames in the dsptoolbox version...
-            assert np.all(np.isclose(stft[:, :y.shape[1]], y))
+            assert np.all(np.isclose(stft[:, :y.shape[1], 0], y))
         except ModuleNotFoundError as e:
             print(e)
             pass
         except Exception as e:
             print(e)
             assert False
```

### Comparing `dsptoolbox-0.2.5/tests/test_distances.py` & `dsptoolbox-0.2.6/tests/test_distances.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/tests/test_filterbanks.py` & `dsptoolbox-0.2.6/tests/test_filterbanks.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/tests/test_generators.py` & `dsptoolbox-0.2.6/tests/test_generators.py`

 * *Files 24% similar despite different names*

```diff
@@ -94,7 +94,23 @@
             fade=None, padding_end_seconds=None)
 
         with pytest.raises(AssertionError):
             dsp.generators.harmonic(
                 frequency_hz=4000, length_seconds=1, sampling_rate_hz=5_000,
                 peak_level_dbfs=-5, number_of_channels=3, uncorrelated=True,
                 fade=None, padding_end_seconds=None)
+
+    def test_oscillator(self):
+        # Only functionality
+        dsp.generators.oscillator(frequency_hz=150,
+                                  sampling_rate_hz=5_000,
+                                  mode='triangle',
+                                  number_of_channels=2, uncorrelated=False)
+        dsp.generators.oscillator(frequency_hz=150,
+                                  sampling_rate_hz=3_000,
+                                  harmonic_cutoff_hz=1_000,
+                                  mode='sawtooth',
+                                  number_of_channels=2, uncorrelated=True)
+        dsp.generators.oscillator(frequency_hz=1000,
+                                  sampling_rate_hz=10_000,
+                                  mode='square',
+                                  number_of_channels=1, uncorrelated=False)
```

### Comparing `dsptoolbox-0.2.5/tests/test_room_acoustics.py` & `dsptoolbox-0.2.6/tests/test_room_acoustics.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def test_room_modes(self):
         # Only functionality
         # Take a multi-channel signal in order to find modes
         y = dsp.Signal(join('examples', 'data', 'chirp_stereo.wav'))
         x = dsp.Signal(join('examples', 'data', 'chirp.wav'))
         h = dsp.transfer_functions.spectral_deconvolve(
             y, x, padding=True, keep_original_length=True)
-        h = dsp.transfer_functions.window_ir(h, exp2_trim=10)
+        h, _ = dsp.transfer_functions.window_ir(h, exp2_trim=10)
 
         dsp.room_acoustics.find_modes(
             h, f_range_hz=[50, 150], proximity_effect=False, dist_hz=5,
             prune_antimodes=False)
         dsp.room_acoustics.find_modes(
             h, f_range_hz=[50, 150], proximity_effect=True, dist_hz=5,
             prune_antimodes=False)
```

### Comparing `dsptoolbox-0.2.5/tests/test_special.py` & `dsptoolbox-0.2.6/tests/test_special.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import dsptoolbox as dsp
 import pytest
 from os.path import join
-from numpy import linspace
+import numpy as np
 
 
 class TestSpecialModule():
     speech = dsp.Signal(join('examples', 'data', 'speech.flac'))
 
     def test_cepstrum(self):
         # Only functionality
@@ -33,15 +33,15 @@
         with pytest.raises(AssertionError):
             dsp.special.log_mel_spectrogram(
                 self.speech, range_hz=[20, 30e3], n_bands=10,
                 generate_plot=False, stft_parameters=None)
 
     def test_mel_filters(self):
         # Only functionality
-        f = linspace(0, 24000, 2048)
+        f = np.linspace(0, 24000, 2048)
         dsp.special.mel_filterbank(
             f_hz=f, range_hz=None, n_bands=30, normalize=False)
         dsp.special.mel_filterbank(
             f_hz=f, range_hz=[1e3, 5e3], n_bands=10, normalize=False)
         dsp.special.mel_filterbank(
             f_hz=f, range_hz=None, n_bands=30, normalize=True)
 
@@ -56,7 +56,20 @@
     def test_mfcc(self):
         # Only functionality
         t, f, s = self.speech.get_spectrogram()
 
         mels, _ = dsp.special.mel_filterbank(f, [20, 10e3], n_bands=4)
         t, mel, mf, fig, ax = dsp.special.mfcc(self.speech, mel_filters=mels)
         t, mel, mf = dsp.special.mfcc(self.speech, generate_plot=False)
+
+    def test_istft(self):
+        # Test reconstruction fidelity
+        # This would most likely fail if padding=False or detrend=True
+        t, f, sp = self.speech.get_spectrogram()
+        speech_rec = dsp.special.istft(sp, original_signal=self.speech)
+        assert np.all(np.isclose(self.speech.time_data, speech_rec.time_data))
+
+        speech_rec = dsp.special.istft(
+            sp, parameters=self.speech._spectrogram_parameters,
+            sampling_rate_hz=self.speech.sampling_rate_hz)
+        assert np.all(np.isclose(self.speech.time_data,
+                                 speech_rec.time_data[:len(self.speech)]))
```

### Comparing `dsptoolbox-0.2.5/tests/test_standard.py` & `dsptoolbox-0.2.6/tests/test_standard.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/tests/test_transfer_functions.py` & `dsptoolbox-0.2.6/tests/test_transfer_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     def test_compute_transfer_function(self):
         # Only functionality
         # Multi-channel
         dsp.transfer_functions.compute_transfer_function(
             self.y_st, self.x, mode='H1', window_length_samples=1024,
             spectrum_parameters=None)
         # Single-channel with other windows
-        h = dsp.transfer_functions.compute_transfer_function(
+        h, h_numpy = dsp.transfer_functions.compute_transfer_function(
             self.y_m, self.x, mode='H2', window_length_samples=1024,
             spectrum_parameters=dict(window_type=('chebwin', 40)))
         # Check that coherence is saved
         h[0].get_coherence()
 
     def test_spectral_average(self):
         # Only functionality is tested
@@ -88,29 +88,29 @@
         dsp.transfer_functions.lin_phase_from_mag(
             sp, self.y_st.sampling_rate_hz, group_delay_ms='minimum')
 
     def test_group_delay(self):
         ir = dsp.transfer_functions.spectral_deconvolve(
             self.y_st, self.x, mode='regularized', start_stop_hz=None,
             threshold_db=-30, padding=False, keep_original_length=False)
-        ir = dsp.transfer_functions.window_ir(
+        ir, _ = dsp.transfer_functions.window_ir(
             ir, window_type='hann', exp2_trim=12, at_start=True)
         # Check only that some result is produced, validity should be checked
         # somewhere else
         dsp.transfer_functions.group_delay(ir, method='matlab')
         dsp.transfer_functions.group_delay(ir, method='direct')
 
         # Single-channel plausibility check
         dsp.transfer_functions.group_delay(ir.get_channels(0))
 
     def test_minimum_phase(self):
         ir = dsp.transfer_functions.spectral_deconvolve(
             self.y_st, self.x, mode='regularized', start_stop_hz=None,
             threshold_db=-30, padding=False, keep_original_length=False)
-        ir = dsp.transfer_functions.window_ir(
+        ir, _ = dsp.transfer_functions.window_ir(
             ir, window_type='hann', exp2_trim=12, at_start=True)
         # Check only that some result is produced, validity should be checked
         # somewhere else
         # Only works for some signal types
         dsp.transfer_functions.minimum_phase(ir)
         with pytest.raises(AssertionError):
             s1 = dsp.Signal(None, ir.time_data, ir.sampling_rate_hz)
@@ -118,15 +118,15 @@
         # Single-channel plausibility check
         dsp.transfer_functions.minimum_phase(ir.get_channels(0))
 
     def test_minimum_group_delay(self):
         ir = dsp.transfer_functions.spectral_deconvolve(
             self.y_st, self.x, mode='regularized', start_stop_hz=None,
             threshold_db=-30, padding=False, keep_original_length=False)
-        ir = dsp.transfer_functions.window_ir(
+        ir, _ = dsp.transfer_functions.window_ir(
             ir, window_type='hann', exp2_trim=12, at_start=True)
         # Check only that some result is produced, validity should be checked
         # somewhere else
         # Only works for some signal types
         dsp.transfer_functions.minimum_group_delay(ir)
         with pytest.raises(AssertionError):
             s1 = dsp.Signal(None, ir.time_data, ir.sampling_rate_hz)
@@ -134,15 +134,15 @@
         # Single-channel plausibility check
         dsp.transfer_functions.minimum_group_delay(ir.get_channels(0))
 
     def test_excess_group_delay(self):
         ir = dsp.transfer_functions.spectral_deconvolve(
             self.y_st, self.x, mode='regularized', start_stop_hz=None,
             threshold_db=-30, padding=False, keep_original_length=False)
-        ir = dsp.transfer_functions.window_ir(
+        ir, _ = dsp.transfer_functions.window_ir(
             ir, window_type='hann', exp2_trim=12, at_start=True)
         # Check only that some result is produced, validity should be checked
         # somewhere else
         # Only works for some signal types
         dsp.transfer_functions.excess_group_delay(ir)
         with pytest.raises(AssertionError):
             s1 = dsp.Signal(None, ir.time_data, ir.sampling_rate_hz)
```

### Comparing `dsptoolbox-0.2.5/LICENSE` & `dsptoolbox-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/README.rst` & `dsptoolbox-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/pyproject.toml` & `dsptoolbox-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.2.5/PKG-INFO` & `dsptoolbox-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsptoolbox
-Version: 0.2.5
+Version: 0.2.6
 Summary: Collection of dsp algorithms to be used for analysis of audio signals
 Project-URL: Homepage, https://github.com/nico-franco-gomez/dsptoolbox
 Project-URL: Bug Tracker, https://github.com/nico-franco-gomez/dsptoolbox/issues
 Project-URL: Documentation, https://dsptoolbox.readthedocs.io/en/latest/
 Author: Nicolas Franco-Gomez
 License-Expression: MIT
 License-File: LICENSE
```

