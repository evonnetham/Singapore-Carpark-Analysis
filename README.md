# Car Sharing Carpark Analysis
_Author: Evonne Tham_

Recently there have been a rise of usage in car-sharing services (e.g. BlueSg, Car Club, WhizzCar, Car Lite, etc) in Singapore due to the pandemic, as some people might believe it's safer than using public transport as there is minimal contact with other. Furthermore, car-sharing is more environmental friendly, especially for those services that are fully electronic. 

<p><img src="https://www.intelligenttransport.com/wp-content/uploads/car-sharing-1.jpg"></p>

As a user of this car-sharing services myself, it brought me to the inspiration to a research on how these businesses decide on where to deploy its fleet across the carparks in Singapore.

The carpark availability data set contains information from the Housing and Development Board (HDB), where lot availbilities were given by per hour basis for thousands of carparks in Singapore. The information enclosed is the unique carpark number, its address, x and y coordinates, type of parking system employed, and if it allows short term parking and if it allows night time parking. 

### Data Source
Source of data of HDB carpark reference and carpark availability data, can be found on the Data.gov.sg site, [here](https://data.gov.sg/dataset/hdb-carpark-information) and [here](https://data.gov.sg/dataset/carpark-availability), respectively, which was sourced publicly from Housing and Development Board.

Within the HDB carpark reference dataset, some important variables include

|Feature|Type|Description|
|---|---|---|---|
| car_park_no | string | carpark number |
| Address | float | Address |
| x_coord | float | longitude coordinate |
| y_coord | float | latitude |
| type_of_parking_system | string | type of parking system |
| short_term_parking | string | type of short term parking |

Within the carpark availability dataset, some important variables include

|Feature|Type|Description|
|---|---|---|---|
| total_lots | int | total parking lots |
| lot_type | string | lot type |
| lots_available | int | total available lots |
| carpark_number | string | carpark number |
| update_datetime | datetime | time data was updated |

### Conclusions and Recommendations
Based on the data collected, the largest carpark that is electronic and whole day parking is located at BLK 611A/613A/615A/616A Bukit Panjang Ring Road/Senja Road. Although it might not be of the lowest utilized carpark, it has a average utilization of 15%. This could also mean that majority of the residences living in that in the area does not own a car. 

For future studies, we could explore the number of car owners in each estates in order to target specific estates  with low number of car owners. For instance, shown in the chart below [(source)](https://www.hdb.gov.sg/-/media/doc/PLG/monograph-1-29-dec-2014.pdf), we could look more into mature towns/estates like Central Area or Queenstown area, accordingly to 2013 data. 

On top of that, we could also look for more options to cut cost for example prioritizing whole day electronic parking with free weekends as data shown that (probably due to Covid-19), residences are more likely to stay in for the weekend and therefore, lesser cars will be used. 
