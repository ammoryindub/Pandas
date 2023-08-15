# Pandas

Pandas exercises

The 'example',  
'example.csv', 
'example.xls' 
files are associated with Pandas Exercise 01


The 'salaries.csv' file is associated with Pandas Exercise 02.


The 'Ecommerce.csv' file is associated with Pandas Exercise 03


### Pandas Exercise 01
- importing libraries

- CSV file

- Excel file
# xls input  

df = pd.read_excel('example.xls')

# df =pd.read_excel('file path or url')

# or we can use df =pd.read_excel ('example.xls', sheet_name='Sheet1')
df
0	First Name	Last Name	Gender	Country	Age	Date	Id
0	1	Dulce	Abril	Female	United States	32	15/10/2017	1562
1	2	Mara	Hashimoto	Female	Great Britain	25	16/08/2016	1582
2	3	Philip	Gent	Male	France	36	21/05/2015	2587
3	4	Kathleen	Hanner	Female	United States	25	15/10/2017	3549
4	5	Nereida	Magwood	Female	United States	58	16/08/2016	2468
5	6	Gaston	Brumm	Male	United States	24	21/05/2015	2554
6	7	Etta	Hurn	Female	Great Britain	56	15/10/2017	3598
7	8	Earlean	Melgar	Female	United States	27	16/08/2016	2456
8	9	Vincenza	Weiland	Female	United States	40	21/05/2015	6548
# xls output 

df.to_excel('example.xls',sheet_name='Sheet1')
---------------------------------------------------------------------------
AttributeError                            Traceback (most recent call last)
/var/folders/y_/kw39v6qn4m758896rbpfkr9w0000gn/T/ipykernel_12501/287744904.py in <module>
      1 # xls output
      2 
----> 3 df.to_excel('example.xls',sheet_name='Sheet1')

AttributeError: 'NoneType' object has no attribute 'to_excel'
HTML
from pandas import read_html
import html5lib
# HTML input

df = pd.read_html('https://en.wikipedia.org/wiki/List_of_Texas_companies')
df
[   Rank  Image               Name  Revenues (USD $M)  Employees  \
 0     2    NaN         ExxonMobil             244363      71200   
 1     9    NaN               AT&T             160546     254000   
 2    28    NaN        Phillips 66              91568      14600   
 3    31    NaN      Valero Energy              88407      10015   
 4    35    NaN  Dell Technologies              78660     145000   
 
                                                Notes  
 0  Multinational oil and gas company and largest ...  
 1  Multinational telecommunications holding compa...  
 2  Global oil and gas entity formed when it spun ...  
 3  International oil and gas refiner, marketer an...  
 4  Multinational technology firm based in Round R...  ,
                          Name           Industry  \
 0                    7-Eleven  Consumer services   
 1                  A. H. Belo  Consumer services   
 2                  Acme Brick        Industrials   
 3            Affiliated Foods  Consumer services   
 4    Airbus Helicopters, Inc.        Industrials   
 ..                        ...                ...   
 192               Whataburger  Consumer services   
 193        Whole Foods Market  Consumer services   
 194  Woodforest National Bank         Financials   
 195                XTO Energy          Oil & gas   
 196          Zale Corporation  Consumer services   
 
                             Sector   Headquarters Founded  \
 0              Broadline retailers         Dallas    1927   
 1                       Publishing         Dallas    2008   
 2    Building materials & fixtures     Fort Worth    1891   
 3     Food retailers & wholesalers       Amarillo    1968   
 4                        Aerospace  Grand Prairie    1969   
 ..                             ...            ...     ...   
 192             Restaurants & bars    San Antonio    1950   
 193   Food retailers & wholesalers         Austin    1980   
 194                          Banks  The Woodlands    1980   
 195       Exploration & production     Fort Worth    1986   
 196            Specialty retailers         Irving    1924   
 
                             Notes  
 0         Convenience store chain  
 1                      Newspapers  
 2               Brick and masonry  
 3              Grocery wholesaler  
 4    Part of Airbus (Netherlands)  
 ..                            ...  
 192              Restaurant chain  
 193             Supermarket chain  
 194                          Bank  
 195                Oil production  
 196                       Jeweler  
 
 [197 rows x 6 columns],
   .mw-parser-output .navbar{display:inline;font-size:88%;font-weight:normal}.mw-parser-output .navbar-collapse{float:left;text-align:left}.mw-parser-output .navbar-boxtext{word-spacing:0}.mw-parser-output .navbar ul{display:inline-block;white-space:nowrap;line-height:inherit}.mw-parser-output .navbar-brackets::before{margin-right:-0.125em;content:"[ "}.mw-parser-output .navbar-brackets::after{margin-left:-0.125em;content:" ]"}.mw-parser-output .navbar li{word-spacing:-0.125em}.mw-parser-output .navbar a>span,.mw-parser-output .navbar a>abbr{text-decoration:inherit}.mw-parser-output .navbar-mini abbr{font-variant:small-caps;border-bottom:none;text-decoration:none;cursor:inherit}.mw-parser-output .navbar-ct-full{font-size:114%;margin:0 7em}.mw-parser-output .navbar-ct-mini{font-size:114%;margin:0 4em}vteLists of companies by U.S. state  \
 0  Alabama Alaska Arizona Arkansas California Col...                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            
 
   .mw-parser-output .navbar{display:inline;font-size:88%;font-weight:normal}.mw-parser-output .navbar-collapse{float:left;text-align:left}.mw-parser-output .navbar-boxtext{word-spacing:0}.mw-parser-output .navbar ul{display:inline-block;white-space:nowrap;line-height:inherit}.mw-parser-output .navbar-brackets::before{margin-right:-0.125em;content:"[ "}.mw-parser-output .navbar-brackets::after{margin-left:-0.125em;content:" ]"}.mw-parser-output .navbar li{word-spacing:-0.125em}.mw-parser-output .navbar a>span,.mw-parser-output .navbar a>abbr{text-decoration:inherit}.mw-parser-output .navbar-mini abbr{font-variant:small-caps;border-bottom:none;text-decoration:none;cursor:inherit}.mw-parser-output .navbar-ct-full{font-size:114%;margin:0 7em}.mw-parser-output .navbar-ct-mini{font-size:114%;margin:0 4em}vteLists of companies by U.S. state.1  
 0  Alabama Alaska Arizona Arkansas California Col...                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             ]
 
SQL "Optional"
