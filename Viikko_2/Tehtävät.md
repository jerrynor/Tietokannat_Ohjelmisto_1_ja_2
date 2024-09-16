### 1
Tee kysely, joka tulostaa kaikki sarakkeet goal-talusta.

Vastaus: SELECT * FROM goal;

### 2
Tee kysely, joka tulostaa nimen ja tyypin kaikista Suomessa sijaitsevista lentokentistä. Suomen maatunnus on: FI

Vastaus: SELECT name, type FROM airport WHERE iso_country ="FI";

### 3
Tee kysely, joka tulostaa suomalaisten lentokenttien nimet aakkosjärjestyksessä. Suomen maatunnus: FI

Vastaus: SELECT name FROM airport WHERE iso_country = "FI" ORDER BY name asc;

### 4

Tee kysely, joka tulostaa nimen ja tyypin kaikista Suomessa sijaitsevista lentokentistä. Järjestä tulos ensisijaisesti tyypin mukaan ja toissijaisesti nimen mukaan.

Vastaus: SELECT name, type FROM airport WHERE iso_country = "FI" ORDER BY type, name asc;

### 5

Tee kysely, joka tulostaa kaikki F-kirjaimella alkavat maan nimet country-taulusta.

Vastaus: SELECT name FROM country WHERE name like 'F%';

### 6

Tee kysely, joka tulostaa kaikki country-taulun maiden nimet, joissa esiintyy F-kirjain.

Vastaus: SELECT name FROM country WHERE name like '%F%';

### 7

Missä locationissa Vesa sijaitsee?

Vastaus: SELECT location FROM game WHERE screen_name like '%Vesa%';

### 8

Kuinkan paljon Ilkka on kuluttanut CO2 budjettia?

Vastaus: SELECT co2_consumed FROM game WHERE screen_name like '%Ilkka%';

### 9

Kuinka paljon alkuperäinen CO2 budjetti on (tulosta CO2 budjetin arvo vain kerran)?

Vastaus: SELECT DISTINCT co2_budget FROM game;