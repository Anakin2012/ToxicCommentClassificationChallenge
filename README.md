# ToxicCommentClassificationChallenge

### Autori: 
- Ana Petrović 1073/2020
- Branko Đaković 1083/2019


Cilj teme Toxic Comments Classification je da se razvije klasifikacioni model koji može da razvrsta tekstualne komentare prema svojoj uvredljivosti/toksičnosti. U pitanju je višeklasna višelabelarna klasifikacija. Zadatak je svrstati komentare u odgovarajuće kategorije, s tim da komentar može pripadati i više od jedne kategorije.


### Podaci

Data je velika količina komentara sa stranice Vikipedije, koje su ljudski korisnici ocenjivali kao toksične. Tipovi toksičnosti su: 

- toxic
- severe_toxic
- obscene
- threat
- insult
- identity_hate

Podaci su dostupni na adresi: https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/overview


Projekat je podeljen na više jupyter sveski radi bolje organizacije i lakšeg pregledanja: 

- **01_Analiza_priprema_podataka.ipynb** - u ovoj svesci odrađeno je učitavanje podataka, osnovne analize skupa (vizuelni prikazi podataka i sl.), a zatim i priprema teksta - izbacivanje nepotrebnih karaktera, reči koje nemaju relevatno značenje i normalizacija. Na kraju je uradjeno balansiranje podataka, tj. izbacivanje velike količine podataka većinske klase.
- **02_Klasicni_modeli** - urađeno je izdvajanje atributa

### Literatura



### Paketi 

