### Inspiration
Back in 2014, I had written a kickass [scraper script](https://github.com/arjunswaj/loksabha2014/tree/master/DataCollection/src/com/asb/analysis) and [SQL queries](https://github.com/arjunswaj/loksabha2014/blob/master/Reports/queries.sql) to do analysis of Lok Sabha Elections. From 2014, not a lot has changed in the election commission's [results website](http://eciresults.nic.in). So I ran the script today after the election results of the states - Uttar Pradesh, Uttarakhand, Goa, Manipur and Punjab were announced. 
I added some [IOMonads](https://github.com/arjunswaj/uugpm2017/blob/master/src/com/asb/elections/Scraper.java#L28-L35) to make the running of the script more fun. Surprisingly, the SQL and the scraper worked flawlessly! Without making you wait further, I shall share the results below:

#### Top 5 parties with maximum number of seats

PARTY | SEATS
------------ | -------------
BHARATIYA JANATA PARTY|406
INDIAN NATIONAL CONGRESS|135
SAMAJWADI PARTY|47
AAM AADMI PARTY|20
BAHUJAN SAMAJ PARTY|18

Well, everyone knows that isnt it? Lets see top 5 parties with maximum number of 2nd place.

#### Top 5 parties with maximum number of 2nd place

PARTY | SEATS
------------ | -------------
SAMAJWADI PARTY|167
INDIAN NATIONAL CONGRESS|153
BHARATIYA JANATA PARTY|129
BAHUJAN SAMAJ PARTY|121
SHIROMANI AKALI DAL|43
AAM AADMI PARTY|27

Okay, it is top 6, I wanted to include AAP in this category.

#### Which party fielded maximum number of candidates?

NO. OF CANDIDATES | PARTY
------------ | -------------
2097|INDEPENDENT 
580|BAHUJAN SAMAJ PARTY 
569|BHARATIYA JANATA PARTY 
391|INDIAN NATIONAL CONGRESS 
 
#### Well, Well, Who got maximum number of votes?

CANDIDATE | PARTY | CONSTITUENCY | VOTES
------------ | ------------- | ------------ | -------------
SUNIL KUMAR SHARMA|BHARATIYA JANATA PARTY|SAHIBABAD|262741
PANKAJ SINGH|BHARATIYA JANATA PARTY|NOIDA|162417
MANOHAR LAL|BHARATIYA JANATA PARTY|MEHRONI|159291
RAMRATAN KUSHWAHA|BHARATIYA JANATA PARTY|LALITPUR|156942
MANISHA ANURAGI|BHARATIYA JANATA PARTY|RATH|147526

#### Which constituency had maximum number of votes casted?

STATE | CONSTITUENCY | VOTES
------------ | ------------- | ------------
UTTAR PRADESH|SAHIBABAD|425868
UTTAR PRADESH|AKBARPUR|407523
UTTAR PRADESH|LALITPUR|317850
UTTAR PRADESH|MEHRONI|307753
UTTAR PRADESH|SAROJINI NAGAR|290847

#### Let us look at the vote shares of Top 10 parties.

PARTY | VOTES | TOTAL VOTES | VOTE SHARE
------------ | ------------- | ------------ | ------------
BHARATIYA JANATA PARTY|38333846|109055693|0.3515
BAHUJAN SAMAJ PARTY|19755610|109055693|0.1812
SAMAJWADI PARTY|18896154|109055693|0.1733
INDIAN NATIONAL CONGRESS|13677079|109055693|0.1254
SHIROMANI AKALI DAL|3858673|109055693|0.0354
AAM AADMI PARTY|3683902|109055693|0.0338
INDEPENDENT|3214035|109055693|0.0295
RASHTRIYA LOK DAL|1546990|109055693|0.0142
NONE OF THE ABOVE|924686|109055693|0.0085
APNA DAL (SONEYLAL)|786937|109055693|0.0072

#### Who were the undisputed winners of 2017?

CANDIDATE | PARTY | CONSTITUENCY | VOTES | TOTAL VOTES | VOTE SHARE
------------ | ------------- | ------------ | ------------ | ------------ | -------------
RAMKRISHNA ALIAS SUDIN DHAVALIKAR|MAHARASHTRAWADI GOMANTAK|MARCAIM|17093|23356|0.7318
VUNGZAGIN VALTE|BHARATIYA JANATA PARTY|THANLON (ST)|9752|13687|0.7125
OKRAM IBOBI SINGH|INDIAN NATIONAL CONGRESS|THOUBAL|18649|27271|0.6838
AMARINDER SINGH|INDIAN NATIONAL CONGRESS|PATIALA|72586|106298|0.6829
RAGHURAJ PRATAP SINGH|INDEPENDENT|KUNDA|136597|201038|0.6795
JAI PRAKASH NISHAD|BHARATIYA JANATA PARTY|RUDRAPUR|77754|116753|0.6660
MADAN KAUSHIK|BHARATIYA JANATA PARTY|HARDWAR|61742|93549|0.6600
SURJAKUMAR OKRAM|INDIAN NATIONAL CONGRESS|KHANGABOK|20781|32359|0.6422
PANKAJ SINGH|BHARATIYA JANATA PARTY|NOIDA|162417|254408|0.6384
THOUNAOJAM SHYAMKUMAR|INDIAN NATIONAL CONGRESS|ANDRO|18761|29850|0.6285

#### Who lost the maximum deposit?
     
No. of seats with < 1/6 votes

NO. OF CANDIDATES | PARTY 
------------ | ------------- 
2051|INDEPENDENT
271|RASHTRIYA LOK DAL
254|BAHUJAN SAMAJ PARTY
202|BAHUJAN MUKTI PARTY
100|COMMUNIST PARTY OF INDIA
92|BHARATIYA SUBHASH SENA
82|SHIVSENA
80|LOK DAL
78|AAPNA PUNJAB PARTY

#### Who won with maximum difference in votes?

CONSTITUENCY | WINNING CANDIDATE | WINNING PARTY | WINNER VOTES | RUNNER UP CANDIDATE | RUNNER UP PARTY | RUNNER UP VOTES | DIFFERENCE IN VOTES 
------------ | ------------- | ------------ | ------------- | ------------ | ------------- | ------------ | ------------- 
SAHIBABAD|SUNIL KUMAR SHARMA|BHARATIYA JANATA PARTY|262741|AMARPAL|INDIAN NATIONAL CONGRESS|112056|150685
RATH|MANISHA ANURAGI|BHARATIYA JANATA PARTY|147526|GAYADEEN ANURAGI|INDIAN NATIONAL CONGRESS|42883|104643
NOIDA|PANKAJ SINGH|BHARATIYA JANATA PARTY|162417|SUNIL CHOUDHARY|SAMAJWADI PARTY|58401|104016
KUNDA|RAGHURAJ PRATAP SINGH|INDEPENDENT|136597|JANKI SHARAN|BHARATIYA JANATA PARTY|32950|103647
MATHURA|SHRIKANT SHARMA|BHARATIYA JANATA PARTY|143361|PRADEEP MATHUR|INDIAN NATIONAL CONGRESS|42200|101161
MEHRONI|MANOHAR LAL|BHARATIYA JANATA PARTY|159291|FERAN LAL|BAHUJAN SAMAJ PARTY|59727|99564
MAHARAJPUR|SATISH MAHANA|BHARATIYA JANATA PARTY|132394|MANOJ KUMAR SHUKLA|BAHUJAN SAMAJ PARTY|40568|91826
MURADNAGAR|AJIT PAL TYAGI|BHARATIYA JANATA PARTY|140759|SUDHAN KUMAR|BAHUJAN SAMAJ PARTY|51147|89612
RAE BARELI|ADITI SINGH|INDIAN NATIONAL CONGRESS|128319|MHD. SHAHBAZ KHAN|BAHUJAN SAMAJ PARTY|39156|89163
AGRA NORTH|JAGAN PRASAD GARG|BHARATIYA JANATA PARTY|135120|ER. GYANENDRA GAUTAM|BAHUJAN SAMAJ PARTY|48800|86320

#### Who won with least difference in votes?

CONSTITUENCY | WINNING CANDIDATE | WINNING PARTY | WINNER VOTES | RUNNER UP CANDIDATE | RUNNER UP PARTY | RUNNER UP VOTES | DIFFERENCE IN VOTES 
------------ | ------------- | ------------ | ------------- | ------------ | ------------- | ------------ | -------------
SAGOLBAND|RAJKUMAR IMO SINGH|INDIAN NATIONAL CONGRESS|9211|DR. KHWAIRAKPAM LOKEN SINGH|BHARATIYA JANATA PARTY|9192|19
CUNCOLIM|CLAFASIO DIAS|INDIAN NATIONAL CONGRESS|6415|JOAQUIM ALEMAO|INDEPENDENT|6382|33
SUGNU|YUMNAM JIBAN SINGH|BHARATIYA JANATA PARTY|4122|KANGUJAM RANJIT SINGH|INDIAN NATIONAL CONGRESS|4086|36
WANGOI|OINAM LUKHOI SINGH|INDIAN NATIONAL CONGRESS|7443|KHURAIJAM LOKEN SINGH|NATIONAL PEOPLE\S PARTY|7407|36
PATSOI|KM. AK. MIRABAI DEVI|INDIAN NATIONAL CONGRESS|13405|SAPAM KUNJAKESWOR (KEBA) SINGH|NORTH EAST INDIA DEVELOPMENT PARTY|13291|114
MORMUGAO|MILIND SAGUN NAIK|BHARATIYA JANATA PARTY|8466|SANKALP AMONKAR|INDIAN NATIONAL CONGRESS|8326|140
LOHAGHAT|PURAN SINGH FARTYAL|BHARATIYA JANATA PARTY|26468|KHUSHAL SINGH|INDIAN NATIONAL CONGRESS|26320|148
THANGMEIBAND|KHUMUKCHAM JOYKISAN SINGH|INDIAN NATIONAL CONGRESS|11596|JYOTIN WAIKHOM|BHARATIYA JANATA PARTY|11439|157
DOOMARIYAGANJ|RAGHVENDRA PRATAP SINGH|BHARATIYA JANATA PARTY|67227|SAIYADA KHATOON|BAHUJAN SAMAJ PARTY|67056|171
MEERAPUR|AVTAR SINGH BHADANA|BHARATIYA JANATA PARTY|69035|LIYAKAT ALI|SAMAJWADI PARTY|68842|193

19 votes. Did you see that? Yes, your vote does matter!

#### Which constituency had maximum number of candidates?

CONSTITUENCY | NO. OF CANDIDATES
------------ | -------------
AKBARPUR|29
AGRA SOUTH|27
ALLAHABAD NORTH|27
AMETHI|25
VARANASI CANTT.|25

#### Cost Analysis
EC allowed up to INR [16 Lakhs](http://eci.nic.in/eci_main1/Contesting.aspx) for election expenditure. Assuming that every candidate spent exactly 16 lakhs, we see some interesting results. Cost per seat excludes parties that won no seats.

##### Cost per vote.
Amount spent per vote.

###### Best Performers.
PARTY | TOTAL COST | VOTES PARTY GOT | COST PER VOTE
------------ | ------------- | ------------ | -------------
APNA DAL (SONEYLAL)|16000000|786937|20.3320
SUHELDEV BHARTIYA SAMAJ PARTY|12800000|607911|21.0557
BHARATIYA JANATA PARTY|910400000|38333846|23.7492
SAMAJWADI PARTY|528000000|18896154|27.9422
SHIROMANI AKALI DAL|148800000|3858673|38.5625

BJP is not the most cost effective party.

###### Worst Performers.
PARTY | TOTAL COST | VOTES PARTY GOT | COST PER VOTE
------------ | ------------- | ------------ | -------------
NIZ GOENKAR REVOLUTION FRONT|3200000|115|27826.0870
RASHTRIYA BANDHUTWA PARTY|1600000|63|25396.8254
PEOPLE’S PARTY|1600000|72|22222.2222
RASTRIYA INSAAF PARTY|1600000|91|17582.4176
MAHILA SWABHIMAN PARTY|1600000|104|15384.6154

Well, that is certainly a revolution.

##### Cost per seat.
Amount spent per seat.

###### Best Performers.
PARTY | TOTAL COST | SEATS PARTY WON | SEATS PARTY PARTICIPATED | SUCCESS RATIO | COST PER SEAT
------------ | ------------- | ------------ | ------------- | ------------ | -------------
APNA DAL (SONEYLAL)|16000000|8|10|0.8000|2000000.0000
GOA FORWARD PARTY|6400000|3|4|0.7500|2133333.3333
BHARATIYA JANATA PARTY|910400000|406|569|0.7135|2242364.5320
SUHELDEV BHARTIYA SAMAJ PARTY|12800000|4|8|0.5000|3200000.0000
INDIAN NATIONAL CONGRESS|625600000|135|391|0.3453|4634074.0741


###### Worst Performers.
PARTY | TOTAL COST | SEATS PARTY WON | SEATS PARTY PARTICIPATED | SUCCESS RATIO | COST PER SEAT
------------ | ------------- | ------------ | ------------- | ------------ | -------------
RASHTRIYA LOK DAL|451200000|1|282|0.0035|451200000.0000
INDEPENDENT|3355200000|9|2097|0.0043|372800000.0000
NIRBAL INDIAN SHOSHIT HAMARA AAM DAL|115200000|1|72|0.0139|115200000.0000
NATIONALIST CONGRESS PARTY|100800000|1|63|0.0159|100800000.0000
ALL INDIA TRINAMOOL CONGRESS|56000000|1|35|0.0286|56000000.0000
BAHUJAN SAMAJ PARTY|928000000|18|580|0.0310|51555555.5556

Independent is not a party. They are independents.

#### Candidates participating in multiple seats

A total of 138 Candidates contested from 2 constituencies, however only 4 won the seats.

CANDIDATE | PARTY | CONSTITUENCY | VOTES
------------ | ------------- | ------------ | ------------- 
VIKRAM SINGH|BHARATIYA JANATA PARTY|FATEHPUR|89481
VIKRAM SINGH|BHARATIYA JANATA PARTY|KHATAULI|94771
SURESH KUMAR|BHARATIYA JANATA PARTY|THANA BHAWAN|90995
SURESH KUMAR|BHARATIYA JANATA PARTY|JAGDISHPUR|84219
PAWAN KUMAR|BHARATIYA JANATA PARTY|HATA|103864
AMARINDER SINGH|INDIAN NATIONAL CONGRESS|PATIALA|72586


A string match of Names and Party were done. This is not fool proof. There could be 2 individuals with same name and belonging to the same party.

**Disclaimer:** This is done just for fun. I will not take any responsibility if there is an error in the results due to a bad SQL.