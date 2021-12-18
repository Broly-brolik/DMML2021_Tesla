# RELATED WORK

## REVOL 2020: *Prédiction de la difficulté de compréhension des contenus audiovisuels*

An entirely different approach: prediction without machine learning.
Translating syntactic and lexical rules to python functions.
 	| Syntax | Lexicon |
| ----------- | ----------- |
| More than 60 syntactic rules regarding pronums, adverbs, verbs etc... | FLELex CRF (François et al., 2014). More than 14'000 words for each level |

**Example: a function to classify a text in B2 difficulty if the text contains more than 13 words.**
```
def avg_length(x):
	lengthList = [len(s) for s in x.doc.sents] # avec docs.sents = phrase du document
	avgLength = sum(lengthList) / len(lengthList)
	if avgLength > 13:
		return B2
	else:
		return ABSTAIN
```` 


### References
- [*Prédiction de la difficulté de compréhension des contenus audiovisuels*](https://dumas.ccsd.cnrs.fr/dumas-02992702)



## ReaderBench
ReaderBench is a Python framework to assess texts' complexity in many natural languages. The project is hosted on [Github](https://github.com/readerbench/ReaderBench) and referenced in [many articles](https://scholar.google.ch/scholar?hl=fr&as_sdt=0%2C5&q=readerbench&btnG=&oq=readerbe). 

### References
- [ReaderBench: A Multi-lingual Framework for Analyzing Text Complexity](https://hal.archives-ouvertes.fr/hal-01584870/file/ec-tel-17-1-demo.pdf)
- [ReaderBench goes Online: A Comprehension-Centered Framework for Educational Purposes](https://core.ac.uk/download/pdf/55539385.pdf)
