# Comparing `tmp/nlppackage-0.0.15.tar.gz` & `tmp/nlppackage-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlppackage-0.0.15.tar", last modified: Tue Jul  4 14:54:08 2023, max compression
+gzip compressed data, was "nlppackage-0.0.17.tar", last modified: Tue Jul  4 15:32:44 2023, max compression
```

## Comparing `nlppackage-0.0.15.tar` & `nlppackage-0.0.17.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 14:54:08.052655 nlppackage-0.0.15/
--rw-rw-rw-   0        0        0     1097 2023-03-03 10:28:54.000000 nlppackage-0.0.15/LICENSE
--rw-rw-rw-   0        0        0      467 2023-07-04 14:54:08.053669 nlppackage-0.0.15/PKG-INFO
--rw-rw-rw-   0        0        0     2732 2023-05-10 10:25:56.000000 nlppackage-0.0.15/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 14:54:08.018823 nlppackage-0.0.15/nlppackage/
--rw-rw-rw-   0        0        0     4418 2023-06-19 08:45:15.000000 nlppackage-0.0.15/nlppackage/Class_NLP.py
--rw-rw-rw-   0        0        0        0 2023-06-19 08:41:55.000000 nlppackage-0.0.15/nlppackage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 14:54:08.048877 nlppackage-0.0.15/nlppackage.egg-info/
--rw-rw-rw-   0        0        0      467 2023-07-04 14:54:07.000000 nlppackage-0.0.15/nlppackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-07-04 14:54:07.000000 nlppackage-0.0.15/nlppackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 14:54:07.000000 nlppackage-0.0.15/nlppackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-04 14:54:07.000000 nlppackage-0.0.15/nlppackage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-04 14:54:07.000000 nlppackage-0.0.15/nlppackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-04 14:54:08.059532 nlppackage-0.0.15/setup.cfg
--rw-rw-rw-   0        0        0      711 2023-07-04 14:51:27.000000 nlppackage-0.0.15/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:32:44.188609 nlppackage-0.0.17/
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-07-04 15:32:09.000000 nlppackage-0.0.17/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-04 15:32:44.189609 nlppackage-0.0.17/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2696 2023-07-04 15:32:09.000000 nlppackage-0.0.17/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:32:44.187609 nlppackage-0.0.17/nlppackage/
+-rw-rw-rw-   0 root         (0) root         (0)     4325 2023-07-04 15:32:09.000000 nlppackage-0.0.17/nlppackage/Class_NLP.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 15:32:09.000000 nlppackage-0.0.17/nlppackage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:32:44.188609 nlppackage-0.0.17/nlppackage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-04 15:32:44.000000 nlppackage-0.0.17/nlppackage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      252 2023-07-04 15:32:44.000000 nlppackage-0.0.17/nlppackage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 15:32:44.000000 nlppackage-0.0.17/nlppackage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-04 15:32:44.000000 nlppackage-0.0.17/nlppackage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-04 15:32:44.000000 nlppackage-0.0.17/nlppackage.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-04 15:32:44.189609 nlppackage-0.0.17/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-07-04 15:32:09.000000 nlppackage-0.0.17/setup.py
```

### Comparing `nlppackage-0.0.15/LICENSE` & `nlppackage-0.0.17/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 BUSINESS & DECISION
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 BUSINESS & DECISION
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `nlppackage-0.0.15/README.md` & `nlppackage-0.0.17/README.md`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# Package NLP
-***
-
-## Informations
-> Initié le : 02/03/2023
-
-> Interlocuteurs : Marine CERCLIER, Grégory GAUTHIER, Tangi LE TALLEC, Alan BIGNON, Islem EZZINE 
-
-> Dans le cadre du projet interne DataScience Package NLP
-
-
-## Description
-L'objectif de ce projet est d'avoir un package NLP permettant d'effectuer différentes tâches de traitement du langage naturel de manière simple et configurable.
-Vous pouvez y retrouver différents dossiers et eléments dont chacun répond à des objectifs précis :
-
-* dossier config : On y met les fichiers de config pour configurer une connexion à un serveur/une BDD, ou encore spécifier la configuration de nos logs.
-* dossier data : Répertorie les fichiers de données en entrée dans un premier sous-dossier et les données en sortie dans un second.
-* dossier logs : Contient les fichiers de logs générés lors de l'exécution de nos programmes Python. Ce dossier a été spécifié dans le fichier du dossier config.
-* dossier src : Les différents scripts Python nécessaires au fonctionnement du projet sont enregistrés dans ce dossier et peuvent être appelés dans le traitement principal main.py.
-* fichier main.py : Script principal du projet que l'on exécute pour que le traitement attendu soit réalisé. Il fait appel aux différentes classes du dossier src.
-* fichier requirements.txt : Il contient les packages présents sur l'environnement de travail du développeur et qui sont donc nécessaires au bon fonctionnement du code.
-* fichier LICENSE : Spécifie par quelle license juridique est couvert notre projet. 
-* fichier README.md : C'est le présent fichier. Il constitue la documentation principale du projet, c'est-à-dire celle qui doit être lue en premier par un utilisateur qui veut comprendre de quoi le projet traite.
-
-## Présentation de la Class NLP
-La permet de choisirs entre deux bibliothèques populaires pour le NLP, nltk et spacy. 
-Les principales fonctionnalités de cette classe sont :
-
-* Initialisation avec le choix du package NLP à utiliser (nltk ou spacy)
-* Tokenization du texte à l'aide du tokenizer sélectionné lors de l'initialisation de la classe
-* Nettoyage des mots vides (stop words) en français en ajoutant ou supprimant des mots vides spécifiques
-* Conversion du texte en minuscules
-* Nettoyage du texte en supprimant tous les caractères spéciaux, sauf ceux spécifiés dans l'argument exception, et en option, en conservant les chiffres
-* Suppression des accents d'un texte en les remplaçant par les lettres correspondantes sans accent
-* Lemmatisation du texte en tenant compte des exceptions de lemmatisation, en conservant ou non les chiffres, et en excluant certains types de mots
-
+# Package NLP
+***
+
+## Informations
+> Initié le : 02/03/2023
+
+> Interlocuteurs : Marine CERCLIER, Grégory GAUTHIER, Tangi LE TALLEC, Alan BIGNON, Islem EZZINE 
+
+> Dans le cadre du projet interne DataScience Package NLP
+
+
+## Description
+L'objectif de ce projet est d'avoir un package NLP permettant d'effectuer différentes tâches de traitement du langage naturel de manière simple et configurable.
+Vous pouvez y retrouver différents dossiers et eléments dont chacun répond à des objectifs précis :
+
+* dossier config : On y met les fichiers de config pour configurer une connexion à un serveur/une BDD, ou encore spécifier la configuration de nos logs.
+* dossier data : Répertorie les fichiers de données en entrée dans un premier sous-dossier et les données en sortie dans un second.
+* dossier logs : Contient les fichiers de logs générés lors de l'exécution de nos programmes Python. Ce dossier a été spécifié dans le fichier du dossier config.
+* dossier src : Les différents scripts Python nécessaires au fonctionnement du projet sont enregistrés dans ce dossier et peuvent être appelés dans le traitement principal main.py.
+* fichier main.py : Script principal du projet que l'on exécute pour que le traitement attendu soit réalisé. Il fait appel aux différentes classes du dossier src.
+* fichier requirements.txt : Il contient les packages présents sur l'environnement de travail du développeur et qui sont donc nécessaires au bon fonctionnement du code.
+* fichier LICENSE : Spécifie par quelle license juridique est couvert notre projet. 
+* fichier README.md : C'est le présent fichier. Il constitue la documentation principale du projet, c'est-à-dire celle qui doit être lue en premier par un utilisateur qui veut comprendre de quoi le projet traite.
+
+## Présentation de la Class NLP
+La permet de choisirs entre deux bibliothèques populaires pour le NLP, nltk et spacy. 
+Les principales fonctionnalités de cette classe sont :
+
+* Initialisation avec le choix du package NLP à utiliser (nltk ou spacy)
+* Tokenization du texte à l'aide du tokenizer sélectionné lors de l'initialisation de la classe
+* Nettoyage des mots vides (stop words) en français en ajoutant ou supprimant des mots vides spécifiques
+* Conversion du texte en minuscules
+* Nettoyage du texte en supprimant tous les caractères spéciaux, sauf ceux spécifiés dans l'argument exception, et en option, en conservant les chiffres
+* Suppression des accents d'un texte en les remplaçant par les lettres correspondantes sans accent
+* Lemmatisation du texte en tenant compte des exceptions de lemmatisation, en conservant ou non les chiffres, et en excluant certains types de mots
+
```

### Comparing `nlppackage-0.0.15/nlppackage/Class_NLP.py` & `nlppackage-0.0.17/nlppackage/Class_NLP.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-import spacy
-import nltk
-import pandas as pd
-import re
-from unidecode import unidecode
-import treetaggerwrapper
-tagger = treetaggerwrapper.TreeTagger(TAGLANG='fr', TAGDIR='C:\TreeTagger')
-
-
-class NLP:
-    def __init__(self, nlp_package='nltk'):
-        # Initialisation de la classe NLP avec la sélection du package NLP à utiliser (nltk ou spacy)
-        if nlp_package == 'nltk':
-            # Si on utilise nltk, on initialise le tokenizer WordPunctTokenizer et on récupère les stopwords en français
-            self.tokenizer = nltk.tokenize.WordPunctTokenizer()
-            self.stopwords = nltk.corpus.stopwords.words('french')
-        elif nlp_package == 'spacy':
-            # Si on utilise spacy, on charge le modèle fr_core_news_sm et on initialise le tokenizer et les stopwords
-            self.nlp = spacy.load('fr_core_news_sm', disable=['parser', 'ner'])
-            self.tokenizer = self.nlp.tokenizer
-            self.stopwords = spacy.lang.fr.stop_words.STOP_WORDS
-        else:
-            # Si le package NLP choisi n'est ni nltk ni spacy, on lève une erreur
-            raise ValueError("Invalid NLP package specified.")
-
-    def tokenize(self, text):
-        # Cette méthode permet de tokenizer un texte en utilisant le tokenizer sélectionné lors de l'initialisation de la classe
-        if isinstance(self.tokenizer, nltk.tokenize.WordPunctTokenizer):
-            # Si on utilise WordPunctTokenizer, on applique directement la méthode tokenize sur le texte
-            return self.tokenizer.tokenize(text)
-        elif isinstance(self.tokenizer, spacy.tokenizer.Tokenizer):
-            # Si on utilise spacy, on applique la méthode tokenizer du modèle sur le texte et on récupère les tokens
-            return [token.text for token in self.tokenizer(text)]
-        else:
-            # Si le tokenizer utilisé n'est ni WordPunctTokenizer ni spacy.tokenizer.Tokenizer, on lève une erreur
-            raise ValueError("Invalid tokenizer specified.")
-
-    def cleanStopWord(self, text, add_stopwords=[], remove_stopwords=[]):
-        stopwords = [
-            word for word in self.stopwords if word not in remove_stopwords]
-        stopwords.extend(add_stopwords)
-        if isinstance(text, str):
-            tokens = text.split(' ')
-        elif isinstance(text, list):
-            tokens = text
-        else:
-            raise ValueError("Invalid input type for text.")
-        return ' '.join([token for token in tokens if token.lower() not in stopwords])
-
-    def lowercaseText(self, text):
-        # Cette méthode permet de mettre un texte en minuscule
-        return text.lower()
-
-    def cleanText(self, text, keep_numbers=True, exception=''):
-        # Cette méthode permet de nettoyer un texte en supprimant tous les caractères spéciaux, sauf ceux spécifiés dans l'argument exception
-        if keep_numbers and exception:
-            pattern = re.compile('[^A-Za-z0-9\xe0-\xff '+exception+']')
-        elif keep_numbers:
-            pattern = re.compile('[^A-Za-z0-9\xe0-\xff]')
-        elif exception:
-            pattern = re.compile('[^A-Za-z\xe0-\xff '+exception+']')
-        else:
-            pattern = re.compile('[^A-Za-z\xe0-\xff]')
-
-        cleaned_text = pattern.sub(' ', text)
-        return cleaned_text
-
-    def cleanAccent(self, text):
-        # Cette méthode permet de supprimer les accents d'un texte en les remplaçant par les lettres correspondantes sans accent
-        cleaned_text = unidecode(text)
-        return cleaned_text
-
-    def lemmatisation(self, text, lemma_exclu, keep_numbers=True, exlu_type_word=[]):
-        tokenisation_majuscule = list()
-        majuscule_tokenised = ''
-        tags = tagger.tag_text(str(text), nosgmlsplit=True)
-        for tag in tags:
-            word, mottag, lemma = tag.split()
-            if len(lemma.split('|')) > 1:
-                lemma = lemma.split('|')[0]
-            if word in lemma_exclu.keys():
-                lemma = lemma_exclu[word]
-            if keep_numbers:
-                if mottag == 'NUM':
-                    lemma = word
-            pos = mottag.split(':')[0]
-            if pos not in exlu_type_word:
-                majuscule_tokenised = majuscule_tokenised + ' ' + lemma
-
-        tokenisation_majuscule.append(majuscule_tokenised)
-        return (' '.join(tokenisation_majuscule))
-
-
+import spacy
+import nltk
+import pandas as pd
+import re
+from unidecode import unidecode
+import treetaggerwrapper
+tagger = treetaggerwrapper.TreeTagger(TAGLANG='fr', TAGDIR='C:\TreeTagger')
+
+
+class NLP:
+    def __init__(self, nlp_package='nltk'):
+        # Initialisation de la classe NLP avec la sélection du package NLP à utiliser (nltk ou spacy)
+        if nlp_package == 'nltk':
+            # Si on utilise nltk, on initialise le tokenizer WordPunctTokenizer et on récupère les stopwords en français
+            self.tokenizer = nltk.tokenize.WordPunctTokenizer()
+            self.stopwords = nltk.corpus.stopwords.words('french')
+        elif nlp_package == 'spacy':
+            # Si on utilise spacy, on charge le modèle fr_core_news_sm et on initialise le tokenizer et les stopwords
+            self.nlp = spacy.load('fr_core_news_sm', disable=['parser', 'ner'])
+            self.tokenizer = self.nlp.tokenizer
+            self.stopwords = spacy.lang.fr.stop_words.STOP_WORDS
+        else:
+            # Si le package NLP choisi n'est ni nltk ni spacy, on lève une erreur
+            raise ValueError("Invalid NLP package specified.")
+
+    def tokenize(self, text):
+        # Cette méthode permet de tokenizer un texte en utilisant le tokenizer sélectionné lors de l'initialisation de la classe
+        if isinstance(self.tokenizer, nltk.tokenize.WordPunctTokenizer):
+            # Si on utilise WordPunctTokenizer, on applique directement la méthode tokenize sur le texte
+            return self.tokenizer.tokenize(text)
+        elif isinstance(self.tokenizer, spacy.tokenizer.Tokenizer):
+            # Si on utilise spacy, on applique la méthode tokenizer du modèle sur le texte et on récupère les tokens
+            return [token.text for token in self.tokenizer(text)]
+        else:
+            # Si le tokenizer utilisé n'est ni WordPunctTokenizer ni spacy.tokenizer.Tokenizer, on lève une erreur
+            raise ValueError("Invalid tokenizer specified.")
+
+    def cleanStopWord(self, text, add_stopwords=[], remove_stopwords=[]):
+        stopwords = [
+            word for word in self.stopwords if word not in remove_stopwords]
+        stopwords.extend(add_stopwords)
+        if isinstance(text, str):
+            tokens = text.split(' ')
+        elif isinstance(text, list):
+            tokens = text
+        else:
+            raise ValueError("Invalid input type for text.")
+        return ' '.join([token for token in tokens if token.lower() not in stopwords])
+
+    def lowercaseText(self, text):
+        # Cette méthode permet de mettre un texte en minuscule
+        return text.lower()
+
+    def cleanText(self, text, keep_numbers=True, exception=''):
+        # Cette méthode permet de nettoyer un texte en supprimant tous les caractères spéciaux, sauf ceux spécifiés dans l'argument exception
+        if keep_numbers and exception:
+            pattern = re.compile('[^A-Za-z0-9\xe0-\xff '+exception+']')
+        elif keep_numbers:
+            pattern = re.compile('[^A-Za-z0-9\xe0-\xff]')
+        elif exception:
+            pattern = re.compile('[^A-Za-z\xe0-\xff '+exception+']')
+        else:
+            pattern = re.compile('[^A-Za-z\xe0-\xff]')
+
+        cleaned_text = pattern.sub(' ', text)
+        return cleaned_text
+
+    def cleanAccent(self, text):
+        # Cette méthode permet de supprimer les accents d'un texte en les remplaçant par les lettres correspondantes sans accent
+        cleaned_text = unidecode(text)
+        return cleaned_text
+
+    def lemmatisation(self, text, lemma_exclu, keep_numbers=True, exlu_type_word=[]):
+        tokenisation_majuscule = list()
+        majuscule_tokenised = ''
+        tags = tagger.tag_text(str(text), nosgmlsplit=True)
+        for tag in tags:
+            word, mottag, lemma = tag.split()
+            if len(lemma.split('|')) > 1:
+                lemma = lemma.split('|')[0]
+            if word in lemma_exclu.keys():
+                lemma = lemma_exclu[word]
+            if keep_numbers:
+                if mottag == 'NUM':
+                    lemma = word
+            pos = mottag.split(':')[0]
+            if pos not in exlu_type_word:
+                majuscule_tokenised = majuscule_tokenised + ' ' + lemma
+
+        tokenisation_majuscule.append(majuscule_tokenised)
+        return (' '.join(tokenisation_majuscule))
+
+
```

