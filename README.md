# ToxicCommentClassificationChallenge

### Autor:  Ana Petrović 1073/2020


### Zadatak
Cilj teme Toxic Comments Classification je da se razvije klasifikacioni model koji može da razvrsta tekstualne komentare prema svojoj uvredljivosti/toksičnosti. U pitanju je višeklasna višelabelarna klasifikacija. Zadatak je svrstati komentare u odgovarajuće kategorije, s tim da komentar može pripadati i više od jedne kategorije. Potrebno je obučiti model koji je sposoban da prepozna različite vrste toksičnosti kao što su pretnje, nepristojni iskazi, uvrede, i mržnja zasnovana na identitetu. 
Zbog velike nebalansiranosti u podacima, problem je podeljen na dve klasifikacije - binarnu i multilabelarnu.

Uz detaljnu analizu skupa podataka, kao i pripremu teksta na osnovu Glove vektorskih reprezentacija, odabran je model zasnovan na konvolutivnim neuronskim mrežama, primenjen na binarnu klasifikaciju na toksične i netoksične komentare, a zatim za višelabelarnu klasifikaciju toksičnih podataka. Modeli su na kraju upoređeni,

### Podaci

Data je velika količina komentara sa stranice Vikipedije, koje su ljudski korisnici ocenjivali kao toksične. Tipovi toksičnosti su: 

- toxic
- severe_toxic
- obscene
- threat
- insult
- identity_hate


Podaci su dostupni na adresi: https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/overview
GloVe: https://nlp.stanford.edu/projects/glove/ (korišćeni su vektori dužine 100 -  glove.6B.100d.txt)

Projekat je podeljen na više jupyter sveski radi bolje organizacije i lakšeg pregledanja: 

- **01_AnalizaIPripremaPodataka.ipynb** - u ovoj svesci odrađeno je učitavanje podataka, osnovne analize skupa (vizuelni prikazi podataka i sl.), a zatim i priprema teksta - izbacivanje nepotrebnih karaktera, reči koje nemaju relevatno značenje itd. 
- **02_BinarnaKlasifikacija** - Model koji vrši binarnu klasifikaciju na toksične i netoksične komentare. Odrađena je unakrsna validacija za određivanje optimalnih hiperparametara, zatim obučen najbolji model i na kraju evaluiran na test skupu.
- **03_ViselabelarnaKlasifikacija** - Model koji vrši  višelabelarnu klasifikaciju samo dela podataka koji su označeni kao toksični. Obučen je model sa istim hiperparametrima kao prethodni, i zatim evaluiran na test skupu.
- **SharedFunctions** - Sveska koja sadrži sve funkcije koje se koriste u sveskama 02 i 03 


### Literatura
https://towardsdatascience.com/journey-to-the-center-of-multi-label-classification-384c40229bff
https://www.analyticsvidhya.com/blog/2020/04/beginners-guide-exploratory-data-analysis-text-data/
https://lena-voita.github.io/nlp_course/models/convolutional.html

### Paketi 

