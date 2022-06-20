# Witcher SQL database

![Github](https://www.belloflostsouls.net/wp-content/uploads/2019/11/The-Witcher-TV-Series.jpg)

I created a table with the headers name, race, gender, country, status, ability and age. Primary key is name. Age mustn't be lower then zero.
```sql
 CREATE TABLE Kontynent (
  name TEXT,
  race TEXT,
  gender TEXT,
  country TEXT,
  status TEXT,
  ability TEXT,
  age INTEGER,
  PRIMARY KEY (name),
  CHECK (age > 0)
);
```

Then I added values matching the headers.

```sql
INSERT INTO Kontynent VALUES ('Cirilla', 'human', 'female', 'Cintra', 'princess', 'Elder blood gene', 13),
('Yennefer', 'quarter elf', 'female', 'Aedirn', 'mage', 'Magic', 90), 
('Geralt', 'mutant', 'male', 'Rivia', 'witcher', 'Superhuman abilities', 103),
('Dandelion', 'human', 'male', 'Redania', 'bard', 'Lute playing', 40),
('Pavetta', 'human', 'female', 'Cintra', 'princess', 'Elder blood gene', 16),
('Filavandrel', 'elf', 'male', 'Dol Blathanna', 'king', 'Fighting', NULL),
('Triss', 'human', 'female', 'Temeria', 'mage', 'Magic', 37),
('Calanthe', 'human', 'female', 'Cintra', 'queen', 'Fighting', 45),
('Cahir', 'human', 'male', 'Nilfgaard', 'knight', 'Fighting', 25),
('Eist', 'human', 'male', 'Skellige', 'king', 'Fighting', NULL),
('Emhyr', 'human', 'male', 'Nilfgaard', 'emperor', 'Fighting', 51),
('Francesca Findabair', 'elf', 'female', 'Dol Blathanna', 'queen', 'Magic', NULL),
('Adda', 'human', 'female', 'Temeria', 'princess', 'striga', 14)
```

|name|race |gender |country |status |ability |age | 
|--|---|--|--|--|---|--|
|Cirilla	|human|	female|	Cintra|	princess|	Elder blood gene|	13|
|Geralt of Rivia|	mutant	|male|	Rivia|	witcher	|Superhuman abilities	|103|
|Yennefer of Vengerberg	|quarter elf|	female	|Aedirn|	mage	|Magic	|71|
|Dandelion |	human	|male|	Redania|	bard|	Lute playing|	40|
|Pavetta|	human|	female	|Cintra	|princess|	Elder blood gene|	15|
|Filavandrel aep Fidhail	|elf	|male|	Dol Blathanna	|king|	Fighting|	
|Triss Merigold|	human|	female|	Temeria|	mage	|Magic|	37|
|Renfri|	human	|female	|Creyden|	princess	|Fighting	|18|
|Calanthe|	human|	female	|Cintra	|queen	|Fighting|	45|
|Cahir Mawr Dyffryn aep Ceallach	|human|	male	|Nilfgaard|	knight|	Fighting|	25|
|Vesemir	|mutant	|male	|Kaedwen|	witcher	|Superhuman abilities	|330|
|Mousesack|	human	|male|	Skellige	|druid	|Magic|	NULL|
|Eist Tuirseach|	human|	male|	Skellige|	king|	Fighting|	45|
|Emhyr var Emreis|	human|	male	|Nilfgaard|	emperor|	Fighting|	51|
|Tissaia de Vries	|human|	female|	Temeria|	mage|	Magic|	300|
|Istredd|	human|	male	|Kovir|	mage|	Magic|	75|
|Stregobor	|human	|male|	Kovir	|mage|	Magic|	478|
|Fringilla	|human|	female|	Nilfgaard	|mage|	Magic|	70|
|Francesca Findabair	|elf	|female	|Dol Blathanna	|queen|	Magic	| NULL|
|Adda the White|	human	|female	|Temeria|	princess	|Striga|	14|
|Foltest	|human|	male|	Temeria	|king	|Fighting	|45|
|Sabrina| Glevissig	|human	|female	|Kaedwen|	mage	|Magic|	73|
|Vilgefortz	|human|	male|	Kaedwen	|mage	|Fighting|	35|
|Eithne	|driad|	female	|Brokilon|	queen	|Wisdom	| NULL |
|Nenneke|	human|	female|	Temeria	|clergy|	Healing	| NULL|