## Data Dictionary

This appendix file is used to provide more information about the tables built within the data model for this project. 

### Immigration table 
   
This table provides information on how many immigration records are collected within each month of year 2016 per visa category, per airport and per state.    
Columns -    
- imm_id: integer, starts from 0, primary key. 
- visa_cat: integer, visa categories, 1 = Business, 2 = Pleasure, 3 = Student. 
- airport_code: string, three characters. 
- state_code: string, two characters, state abbreviations.
- month: integer, which month the record is in. 
- year: integer, which year the record is in. 
- count: integer, how many records are collected. 

### Airport table 
  
This table provides information on names of airports, types of them and their corresponding airport code.    
Columns -    
- type: string, airport type. Possible values are 'small_airport', 'seaplane_base', 'heliport', 'medium_airport', 'large_airport'. 
- airport_code: string, three characters, unique and not null, primary key. 
- state_code: string, two characters, state abbreviations.

### Demographic table   
    
This table provides information on demographic metrics for cities in the U.S..    
Columns -    
- demo_id: integer, starts from 0, primary key. 
- city: string, city name. 
- state: string, state name. 
- mage: integer, median age of the city.  
- mpopulation: integer, male population of the city. 
- fpopulation: integer, female population of the city. 
- tpopulation: integer, total population of the city. 
- veterans: integer, the number of veterans of the city.  
- fborn: integer, the number of foreign-born of the city. 
- household: integer, the average household size of the city. 
- state_code: string, two characters, state abbreviations. 
- American Indian and Alaska Native: integer, the number of American Indian and Alaska Native residents in that city. 
- Asian: integer, the number of Asian residents in that city. 
- Black or African-American: integer, the number of Black or African-American residents in that city. 
- Hispanic or Latino: integer, the number of Hispanic or Latino residents in that city. 
- White: integer, the number of White residents in that city. 
