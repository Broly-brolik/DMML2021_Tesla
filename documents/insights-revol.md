## Prédiction de la difficulté de compréhension des contenus audiovisuels - Justine Revol
## Infos récupérées dans l'article

### Reprise des étiquettes du  [Cadre Européen Commun de Référence pour les Langues](https://eduscol.education.fr/1971/cadre-europeen-commun-de-reference-pour-les-langues-cecrl) (CECRL)
Pourquoi? il est facile de trouver des ouvrages qui informent sur les éléments qui entrent en compte dans la définition de ces niveaux d’apprentissage selon les niveaux de difficulté.

### Quelques règles
**Longeur phrase: Si # words in sentence > 13 => B2**
```
def avg_length(x):
	lengthList = [len(s) for s in x.doc.sents] # avec docs.sents = phrase du document
	avgLength = sum(lengthList) / len(lengthList)
	if avgLength > 13:
		return B2
	else:
		return ABSTAIN
````
**Construction ADJ+PREP+NOUN comme "pleine d'eau", "nul en math" => A2**
```
def avg_length(x):
	listeADP = ["de", "en"]
	if token.text == listeADP
		return A2
	else:
		return ABSTAIN
````
**Construction [‘NOUN’,‘ADP’ ,‘VERB’] => B1**
```
def avg_length(x):
	listePos = [i.pos_ for i in x.doc]
	nounStructure = [‘NOUN’,‘ADP’ ,‘VERB’]
	result = [(i, i+len(nounStructure)) for i in range(len(listPos)) 	if listPos[i:i+len(nounStructure)] == nounStructure]
	if result:
		return B1
	else:
		return ABSTAIN
```
  
