# websig
repo tempo
# Intervention Veremes (L. P)
	- distribution 
	- developpement 
	- formation 
	- hebergement 

# Focalisation sur le produit de webmapping VMAP2


## outil SIG Web public VMAP2
### DÉSCRIPTION FONCTIONNELLE DE LA SOLUTION

#### - 1-Qu'est ce que c'est ? 
	- VMAP est un outil libre et open source 
		- l'application est responsive, compatible desktop et telephone
#### - 2-Qui l'utilise ? 
	- privé 
		- elect
		- eau 
			- assainis
		reseau
			- divers
		- energie
			- prospection pour implantation solaire
	- public (openIG), office n du foret, metropole paris 
	
	- Cartographie grand public extranet
#### - 3- Qu'est ce qu'on peut faire avec ?
	- Il est No code pour la partie administration 
	- Création CArte
		- Gestion de la symbologie directement dans  l'appli Vmap et Vmap2 
			- interface no-code le permet de a à z sans dev
				- Analyse possible 
					- cluster 
					- multicritere 
	- visualisation CArte
	- filtres
	- Création de formulaire métier 
		- pour paramétrer les types de formulaire 					
	- possibilité de faire un controle de saisi
	- fonctionnalité 
		 - drag and drop 
		 - modèle d'impression modulable
			- A4 -> A0
			- paysage -> portrait 
	- créer une carte à intégrer dans une page HTML
		- juste, bout de code à ajouter 
			- et toute les fonctionnalité y fonctionnent bien 
	- [?] **Export de données ?
		- oui
		- calcul d’itinéraires ?
			- bientôt
	- Datavisualisation BI
		- en etude
		- vChart (disponible en dehors)
	- [x] *diffuser les données d’accessibilité sur le web*
	- [x] *diffuser les cartographies thématiques produites dans le cadre d’une autre prestation*
### DÉSCRIPTION TECHNIQUE DE LA SOLUTION

#### - 4 - Comment ça fonctionne 
	- l'appli est no code mais permet de faire du dev personnalisé
	- Ils utilise php angular backend 
		- mapserver uniquement
			- non geoserver 
	- Connexion 
		- LDAP
		- SSO plateforme (genre facebook google sans avoir créer compte)
		- créer compte
#### - 5 - Quels sont les prérequis de son déploiement 
	- documentation : documentation.veremes.net/vmap2
		- plus c'est puissant, mieux c'est 
		- on peut héberger ou on veut 
			- ovh, AWS
#### - 6- Comment ça s'installe  ? - la maintenance ne nous interresserapas
		- Il s'install correct sur Windows et linux avec une documentation technque d'acompagnement
### respect des exigences réglementataires et métiers 
	- [x] **RGAA
			- l'application est responsive, compatible desktop et telephone
	- Droits d'acces et privilège
		- données 
		- utilisateurs
		- admin
	- Sécurité
		- restriction acces distants
	- Evolutions
		- 6 ème version (2025)
		- veremes seul contributeur
			- git lab de suivi
		- Les developpement sont reversé au pot commun 
			- S'ils sont très spécifique peut être pas
			- possible de commercialiser le produit
	- licence cécile et faire du commerciale


### Limites 
- Chargement de données (shp, geojson) en base via Vmap2 
	- Non
		- il permet que leur visualisation et ajout à la carte
			
### Point d'attention 
- Flux | Tuile de Meilleur performance
	- xyz, 
	- wmts, 
	- tuiles vectorielles
- Force des couche websig
	- mixe postgis, vecteur, tuille donne une meilleure service

- Financement (pour une collectivité) vers 5000 euro
	- maintenance à 2000 euro 
	- hebergement à 3000 euro
