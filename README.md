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

@inproceedings{pnugues2022,
  author = {Pierre Nugues},
  title = {Connecting a {F}rench Dictionary from the Beginning of the 20th Century to Wikidata},
  year = 2022,
  booktitle = {Proceedings of LREC 2022},
  address = {Marseilles}
}
```
J'ai réalisé moi-même et manuellement tous les raccordements entre les noms propres et les identifiants wikidata.

Les données textuelles du *Petit Larousse illustré* proviennent du projet *Nénufar*, http://nenufar.huma-num.fr/, qui lui-même prend la suite d'un projet mené à l'université de Cergy : 
1. Hervé Bohbot, Francesca Frontini, Giancarlo Luxardo, Mohamed Khemakhem and Laurent Romary (2018) Presenting the Nenufar Project: A Diachronic Digital Edition of the Petit Larousse Illustré, in Proceedings of the Eleventh International Conference on Language Resources and Evaluation (LREC 2018).
2. Manuélian, H., Bruscand, A., Cholewka, N., Hetzel, A-M. (2010) Le Petit Larousse Illustré de 1905 en ligne: Présentation et secrets de fabrication, in Informatique et description de la langue d'hier et d'aujourd'hui, ÉLA n°156, octobre-décembre 2009, Klincksieck.

