# fouillesdetextes

Pop : 75 chansons/fichiers (Gemma)

Reggae : 75 chansons/fichiers
> Gemma : 38 fichiers

> Tannina : 37 fichiers

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
	 			