
### Team name: BERTLENIKA

<h2 align="center">Collecting data challenge</h2>
<p align="center"><a href="https://github.com/CorentinChanet/challenge-collecting-data">
<img src="https://becode.org/app/uploads/2021/06/logo-becode.png" alt="Logo" width="200" height="200"></a></p>
<h3 align="center"> Web scraping group project at <a href="https://github.com/becodeorg"><strong>BeCode</strong></a></h3>
<h3 align="center"> Contributors: <a href="https://github.com/Len-Fid">Lena, <a href="https://github.com/anikaarevalo">Anika,<a href="https://https://github.com/BertramDHooge"> Bertram</a></h3><br>

  
## The timeline of the project: 
**28/02/22 - 01/03/22**


## Objectives of the project: 
* Scrape a website containing information about the Belgian house market
* Build a dataset from scratch

## Libraries used:
* Selenium 
* BeautifulSoup
* Pandas 
* JSON

## Usage:
* The code can be run through [this file in Jupyter Notebook](https://github.com/Len-Fid/challenge-collecting-data/blob/main/scraping_that_demo.ipynb)
* Demo version containing 30 links can be seen in [this file](https://github.com/Len-Fid/challenge-collecting-data/blob/main/scraping_that_demo.ipynb)

## Walk through of this DIY scraping challenge:

* Locating elements of the source code of the requisite URL from the immoweb.be/en web site
* Extracting targeted elements (links) asynchronously per web get and saving these links by creating a list in a soup file for parsing
* Creating a data frame using pandas for approximately 10,000 inputs
* Saving everything in a CSV file

## Dataset details:
Dataset contains the following columns :

- Locality
- Type of property (House/apartment)
- Subtype of property (Bungalow, Chalet, Mansion, ...)
- Price
- Type of sale (Exclusion of life sales)
- Number of rooms
- Area
- Fully equipped kitchen (Yes/No)
- Furnished (Yes/No)
- Open fire (Yes/No)
- Terrace (Yes/No)
  - If yes: Area
- Garden (Yes/No)
  - If yes: Area
- Surface of the land
- Surface area of the plot of land
- Number of facades
- Swimming pool (Yes/No)
- State of the building (New, to be renovated, ...)

## Visual
**Sample view**


|Location         |Property type|Property subtype  |Price  |Type of sale                    |Number of bedrooms|Living area|Kitchen           |Furnished|Open fireplace|Terrace|Terrace orientation|Garden |Garden orientation|Surface area land|Number of facades|Pool |Condition     |
|-----------------|-------------|------------------|-------|--------------------------------|------------------|-----------|------------------|---------|--------------|-------|-------------------|-------|------------------|-----------------|-----------------|-----|--------------|
|Kortenberg       |HOUSE        |VILLA             |459000 |residential_sale                |3                 |157        |USA_HYPER_EQUIPPED|False    |True          |True   |WEST               |True   |WEST              |194              |4                |     |AS_NEW        |
|Oostende         |HOUSE        |HOUSE             |275000 |residential_sale                |3                 |           |INSTALLED         |False    |False         |True   |Unknown            |Unknown|Unknown           |0                |                 |False|GOOD          |
|Zonnebeke        |HOUSE        |HOUSE             |215000 |residential_sale                |2                 |           |INSTALLED         |False    |False         |True   |Unknown            |True   |SOUTH_WEST        |529              |3                |     |TO_BE_DONE_UP |
|Ieper            |HOUSE        |HOUSE             |345000 |residential_sale                |3                 |           |INSTALLED         |False    |False         |True   |Unknown            |Unknown|Unknown           |2685             |4                |     |TO_BE_DONE_UP |
|Roeselare        |HOUSE        |HOUSE             |239000 |residential_sale                |3                 |193        |SEMI_EQUIPPED     |False    |False         |Unknown|Unknown            |Unknown|Unknown           |149              |2                |     |GOOD          |
|Roeselare        |HOUSE        |HOUSE             |270000 |residential_sale                |3                 |148        |SEMI_EQUIPPED     |False    |False         |Unknown|Unknown            |True   |SOUTH             |173              |2                |     |GOOD          |
|Linkebeek        |HOUSE        |HOUSE             |565000 |residential_sale                |3                 |140        |USA_INSTALLED     |False    |True          |True   |Unknown            |True   |SOUTH_EAST        |500              |                 |     |AS_NEW        |
