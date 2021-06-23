# petit_larousse_1905
Un jeu de données qui raccorde tous les noms propres de l'édition de 1905 du *Nouveau Larousse illustré* à des éléments wikidata. Le dossier comprend :
* Le fichier `larousse_1905_wd.json` qui contient une liste de dictionnaires Python où chaque dictionnaire représente un article des nom propres. Un dictionnaire contient le texte de l'article et l'identifiant wikidata;
* Le notebook Jupyter `raccordement_larousse.ipynb`qui montre comment lire et tirer parti du fichier json avec des exemples très simples;
* Le fichier `larousse_1905_wd_extraction.json` qui ajoute des informations extraites de wikidata aux articles. Le résultat est stocé dans des dictionnaires Python;
* Le dossier `lettres` qui contient des fichiers TSV correspondant aux lettres de l'alphabet. C'est à peu près l'équivalent de `larousse_1905_wd.json`;
* Le fichier pickle `larousse_wd.pkl` qui est un fichier de travail. Il n'est sans doute pas utilisable.
