# fouillesdetextes

Bienvenue sur notre page du projet de classification sur Weka 😄


## Projet 

Pop : 75 chansons/fichiers (Gemma)
- MusixMatch : 28 chansons
- AZLyrics : 20 chansons
- LyricFind : 20 chansons
- Genius : 6 chansons

Reggae : 75 chansons/fichiers
> Gemma : 36 fichiers
- MuzixMatch : 18 chansons
- AZLyrics : 12 chansons
- LyricFind : 8 chansons

> Tannina : 39 fichiers

Soul : 75 chansons/fichiers (Tannina)


# PARTIE WEKA

1. Dossier Weka :
	- Dossier : *data*,
	- Fichier *sample-data.tar.gz*,
	- Fichier *vectorisation.py*
	- *music-booleen.arff* (obtenu avec python dans le terminal)
	- *music-comptes.arff*(obtenu avec python dans le terminal)
	
2. Dossier data :
	- music
		- corpus
			- pop
			- reggae
			- soul
		- fichier-resultat.arff

2. Lancer le script vectorisation.py dans le terminal 
	
	 python3 ./vectorisation.py -h
	 python3 ./vectorisation.py data/music/corpus music-comptes.arff
	 python3 ./vectorisation.py data/music/corpus music-booleen.arff --boolean
	 
	 3. Dans Weka
	
	 - Explorer
	 
	 - Preprocess -> ouvrir le fichier comptes ou booleen
	 
	 - Classify
	 		Classifier
	 			- joue avec "cross-validation" et "percentage split"
	 			- start
	 			- changer le classifier : ZeroR, lazy-lBk, trees-j48, Bayes -> NaiveBayes, NaiveBayesMultinomial
	 			
