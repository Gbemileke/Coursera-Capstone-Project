# Coursera-Capstone-Project
This is my capstone project for IBM data science professional certificate
## Project Title: Location Selection for Delivery Locker for Online Retailers
### Introduction
Online shopping has become a common phenomenon and part of consumer's daily life. Recently, consumer spending online is on the rise, and the US online sales revenue is expected to reach $523 billion by 2020 [1]. The increase in online shopping has resulted in a significant rise in the frequency of home deliveries, so do package theft is increasing exponentially [2]. MailHaven an IoT company reported that 1 billion packages per year aren't delivered on the first try [1]. Most packages that don't fit into the mailboxes can't be left alone outside because they can be damaged or destroyed by bad weather or even stolen. According to the August Home Package Theft Report (2016), about 11 million U.S. homeowners have had a package stolen within the past, with a value close to $200. Package theft has become a really big concern for both the customers and the retailers. 53% of packages left on the doorsteps or porch are stolen and 75% of these packages are stolen during the day [3]. To address this problem retail and third-party logistics such as Amazon and UPS results to the use of delivery locker located at a convenience store with customer's neighborhood, where packages can be kept securely before customer pick up. These delivery lockers have proven to help reducing theft of delivered packages[4]. Therefore, in this project, we are going to use a machine learning technique to determine the best location for delivery lockers in different neighborhood in Brooklyn Borough, New York.

### Method of Data Collection and Analysis
The data for this project is obtained from New York geodata from [5]  and the Foursquare location data to solve the aforementioned business problem. First, the datasets comprising of   Borough, Neighborhood, Latitude, and 	Longitude were created using Pandas library in Python. Then, we select Brooklyn Borough data from New York. Next, the Brooklyn borough neighborhoods are explored using the Foursquare website. Finally, descriptive statistics, data visualization charts, and K-means clustering method will be used to examine the characteristics of the neighborhoods and find suitable locations to recommend for delivery locker location.
Example Data features extract from New York datasets are:

{'type': 'Feature', 

 'id': 'nyu_2451_34572.51', 
 
 'geometry': {'type': 'Point',
 
  'coordinates': [-73.97347087708445, 40.59526001306593]},
 'geometry_name': 'geom',
 'properties': {'name': 'Gravesend',
  'stacked': 1,
  'annoline1': 'Gravesend',
  'annoline2': None,
  'annoline3': None,
  'annoangle': 0.0,
  'borough': 'Brooklyn',
  'bbox': [-73.97347087708445,
   40.59526001306593,
   -73.97347087708445,
   40.59526001306593]}}
Example Data features extract from Foursquare are:
{'meta': {'code': 200, 'requestId': '5bb0782e6a607169104e9cad'},
 'response': {'suggestedFilters': {'header': 'Tap to show:',
   'filters': [{'name': '$-$$$$', 'key': 'price'},
    {'name': 'Open now', 'key': 'openNow'}]},
  'headerLocation': 'Bay Ridge',
  'headerFullLocation': 'Bay Ridge, Brooklyn',
  'headerLocationGranularity': 'neighborhood',
  'totalResults': 90,
  'suggestedBounds': {'ne': {'lat': 40.63030106951066,
    'lng': -74.02470273356597},
   'sw': {'lat': 40.62130106051065, 'lng': -74.03653865351028}},
  'groups': [{'type': 'Recommended Places',
    'name': 'recommended',
    'items': [{'reasons': {'count': 0,
       'items': [{'summary': 'This spot is popular',
         'type': 'general',
         'reasonName': 'globalInteractionReason'}]},
      'venue': {'id': '4b895827f964a5206c2d32e3',
       'name': 'Pilo Arts Day Spa and Salon',
       'location': {'address': '8412 3rd Ave',
        'lat': 40.62474788273414,
        'lng': -74.03059056940135,
        'labeledLatLngs': [{'label': 'display',
          'lat': 40.62474788273414,
          'lng': -74.03059056940135}],
        'distance': 117,
        'postalCode': '11209',
        'cc': 'US',
        'city': 'Brooklyn',
        'state': 'NY',
        'country': 'United States',
        'formattedAddress': ['8412 3rd Ave',
         'Brooklyn, NY 11209',
         'United States']},

### Reference
1.	https://mailhaven.co/snail-mail-smart-mail/
2.	https://www.inc.com/john-white/tired-of-getting-your-packages-stolen-heres-what-to-do.html
3.	https://august.com/wp-content/uploads/2016/10/August-Package-Theft-Report-FINAL-102516.pdf
4.	https://www.pymnts.com/news/retail/2017/package-locker-systems-luxer-one-package-delivery/
5. 	https://geo.nyu.edu/catalog/nyu_2451_34572

