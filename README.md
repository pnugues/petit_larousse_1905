# petit_larousse_1905
Un jeu de données qui raccorde tous les noms propres de l'édition de 1905 du *Nouveau Larousse illustré* à des éléments wikidata. Le dossier comprend :
* Le fichier `larousse_1905_wd.json` qui contient une liste de dictionnaires Python où chaque dictionnaire représente un article des nom propres. Un dictionnaire contient le texte de l'article et l'identifiant wikidata;
* Le notebook Jupyter `raccordement_larousse.ipynb`qui montre comment lire et tirer parti du fichier json avec des exemples très simples;
* Le fichier `larousse_1905_wd_extraction.json` qui ajoute des informations extraites de wikidata aux articles. Le résultat est stocé dans des dictionnaires Python;
* Le dossier `lettres` qui contient des fichiers TSV correspondant aux lettres de l'alphabet. C'est à peu près l'équivalent de `larousse_1905_wd.json`;
* Le fichier pickle `larousse_wd.pkl` qui est un fichier de travail. Il n'est sans doute pas utilisable.



Si vous utilisez ces données, merci d'en citer l'origine avec la référence suivante :
```
@misc{pnugues2021,
  author = {Pierre Nugues},
  title = {Raccordement du {Petit Larousse illustré} de 1905 à wikidata},
  year = 2021,
  url = {https://github.com/pnugues/petit_larousse_1905}
}
```
Les données textuelles du *Nouveau Larousse illustré* proviennent du projet *Nénufar*, http://nenufar.huma-num.fr/, qui lui-même prend la suite d'un projet mené à l'université de Cergy : 
1. Hervé Bohbot, Francesca Frontini, Giancarlo Luxardo, Mohamed Khemakhem and Laurent Romary (2018) Presenting the Nenufar Project: A Diachronic Digital Edition of the Petit Larousse Illustré, in Proceedings of the Eleventh International Conference on Language Resources and Evaluation (LREC 2018).
2. Manuélian, H., Bruscand, A., Cholewka, N., Hetzel, A-M. (2010) Le Petit Larousse Illustré de 1905 en ligne: Présentation et secrets de fabrication, in Informatique et description de la langue d'hier et d'aujourd'hui, ÉLA n°156, octobre-décembre 2009, Klincksieck
