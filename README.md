# Raccordement du *Petit Larousse illustré* de 1905 à wikidata

Ce dépôt héberge un jeu de données qui raccorde tous les noms propres de l'édition de 1905 du *Petit Larousse illustré* à des éléments wikidata. Le dossier comprend :
* Le fichier `larousse_1905_wd.json` qui contient une liste de dictionnaires Python où chaque dictionnaire représente un nom propre du *Larousse*. Un dictionnaire Python contient le texte de l'article du *Larousse* et l'identifiant wikidata avec les clés `texte`et `qid`, par exemple : ``` {'texte': "AALI-PACHA, homme d'Etat turc, né à Constantinople. Il a attaché son nom à la politique de réformes du Tanzimat (1815-1871).",
  'qid': ['Q439237']}```
* Le notebook Jupyter `raccordement_larousse.ipynb`qui montre comment lire et tirer parti du fichier json avec des exemples très simples;
* Le fichier `larousse_1905_wd_extraction.json` qui ajoute des informations extraites de wikidata aux articles. Le résultat est stocké dans des dictionnaires Python avec des clés supplémentaires;

Si vous utilisez ce jeu de données, merci d'en citer l'origine avec les références suivantes :

```
@misc{pnugues2021,
  author = {Pierre Nugues},
  title = {Raccordement du {Petit Larousse illustré} de 1905 à wikidata},
  year = 2021,
  url = {https://github.com/pnugues/petit_larousse_1905}
}

@InProceedings{nugues:2022:LREC,
  author    = {Nugues, Pierre},
  title     = {Connecting a French Dictionary from the Beginning of the 20th Century to Wikidata},
  booktitle      = {Proceedings of the Language Resources and Evaluation Conference},
  month          = {June},
  year           = {2022},
  address        = {Marseille, France},
  publisher      = {European Language Resources Association},
  pages     = {2548--2555},
  abstract  = {The Petit Larousse illustré is a French dictionary first published in 1905. Its division in two main parts on language and on history and geography corresponds to a major milestone in French lexicography as well as a repository of general knowledge from this period. Although the value of many entries from 1905 remains intact, some descriptions now have a dimension that is more historical than contemporary. They are nonetheless significant to analyze and understand cultural representations from this time. A comparison with more recent information or a verification of these entries would require a tedious manual work. In this paper, we describe a new lexical resource, where we connected all the dictionary entries of the history and geography part to current data sources. For this, we linked each of these entries to a wikidata identifier. Using the wikidata links, we can automate more easily the identification, comparison, and verification of historically-situated representations. We give a few examples on how to process wikidata identifiers and we carried out a small analysis of the entities described in the dictionary to outline possible applications. The resource, i.e. the annotation of 20,245 dictionary entries with wikidata links, is available from GitHub (https://github.com/pnugues/petit\_larousse\_1905/)},
  url       = {https://aclanthology.org/2022.lrec-1.272}
}
```
J'ai réalisé moi-même et manuellement tous les raccordements entre les noms propres et les identifiants wikidata.

Les données textuelles du *Petit Larousse illustré* proviennent du projet *Nénufar*, http://nenufar.huma-num.fr/, qui lui-même prend la suite d'un projet mené à l'université de Cergy : 
1. Hervé Bohbot, Francesca Frontini, Giancarlo Luxardo, Mohamed Khemakhem and Laurent Romary (2018) Presenting the Nenufar Project: A Diachronic Digital Edition of the Petit Larousse Illustré, in Proceedings of the Eleventh International Conference on Language Resources and Evaluation (LREC 2018).
2. Manuélian, H., Bruscand, A., Cholewka, N., Hetzel, A-M. (2010) Le Petit Larousse Illustré de 1905 en ligne: Présentation et secrets de fabrication, in Informatique et description de la langue d'hier et d'aujourd'hui, ÉLA n°156, octobre-décembre 2009, Klincksieck.

