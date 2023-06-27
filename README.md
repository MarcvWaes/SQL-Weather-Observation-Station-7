# SQL-Weather-Observation-Station-7

# Challenge:
- Query the list of CITY names ending with vowels (a, e, i, o, u) from STATION. Your result cannot contain duplicates.

- The STATION table is described as follows:

![n1e5uock jot](https://github.com/MarcvWaes/SQL-Weather-Observation-Station-3/assets/120553175/93033af8-77bd-460d-bf7b-fce39386b9e6)

- Where LAT_N is the northern latitude and LONG_W is the western longitude.

# Solution:
- SELECT DISTINCT CITY
- FROM STATION 
- WHERE CITY REGEXP '[aeiouAEIOU]$'

- In the context of the query, REGEXP is used to match the CITY names that start with vowels. The regular expression '^[aeiouAEIOU]' specifies the pattern we are looking for:
  - '$' asserts the end of the string.
  - '[aeiouAEIOU]' represents a character set that includes all lowercase and uppercase vowels.
 
- The REGEXP '^[aeiouAEIOU]' condition checks if the CITY column value begins with any vowel.

# Output:
- Acme 
- Aguanga 
- Alba 
- Aliso Viejo 
- Alpine 
- Amazonia 
- Amo 
- Andersonville 
- Archie 
- Arispe
- .....
