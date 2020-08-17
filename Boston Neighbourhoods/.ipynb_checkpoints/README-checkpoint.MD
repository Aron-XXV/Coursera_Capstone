# Recommending rental properties project
## Background
Many people are struggling in the time of renting a property which is followed by a huge amount of search, calls, inspections and more importantly a great deal of time and money. Aron is a data scientist who has decided to enrol a professional degree in one of the well-known universities in Boston. He is considered as an international student who needs to explore many secrets in the real-estate sector of Boston city. However, he has no time to do so much field exploration just to land on a suitable property for renting. He will arrive one day before the semester start date. So, he is thinking of finding a comprehensive and accurate solution. <br>
After consulting with several of his friends he got two options. Asking an agent to find a suitable apartment which does not ensure cost-effectiveness and efficiency. The other option which he is much into it is developing a code which takes criteria on one side and suggests best available options. He knows how to use API services of Foursquare and Realtor API. <br>
## Problem description
The problem in the realm of data science can be described as the following:
Having a city name and the desired range of a specified location, a recommending system is needed to explore specifications of neighbourhoods and search for available rental properties to match them with the given criteria. Main parameters are the distance from the desired location, herein a university campus, and important venues which define the appropriateness of each rental option.
This code can save time and cost in the way that a user can explore options easily. Not only it ensures having an optimised solution but also lets the user train his understanding of given criteria. For example, Aron might reach to a conclusion that one set of criteria is beyond his budget and he needs to compromise the criteria. So, instead of failing in rental search, this project makes him capable of making realistic decisions without losing time and money. <br>
## Audience
This project takes Aron as an example of an audience who is going to find an apartment close to campus. But this project can benefit a wide range of people as far as they come with some criteria in the first hand. However, covering a wide range of users demands developing a user-friendly online interface which is beyond the scope of this project. <br>
## Data sources
There are four data sources going to be used in this project:
1. List of neighbourhoods in the desired city, Boston which is retrieved from a web site.
2. Coordinates of neighbourhoods extracted by Geopy from Nominatim
3. Foursquare used for retrieving data of venues including their name, location, and category. In this project, only location and categories are going to be used.
4. Realtor API which is going to utilised for exploring available rental options in nominated neighbourhoods

For example, Aron decided to pursue his studies at MIT which is in Cambridge neighbourhood. Although the idea choice would be within Cambridge, Aron suspects that it would be costly to live there. So, he is interested to consider surrounding neighbourhoods as well. So, in the first step, a list of neighbourhoods is retrieved. Then several neighbourhoods are nominated based on the distance for further exploration. In the next step, coordinates of these neighbourhoods are found by use of Geopy. Having those coordinates, Foursquare API can be utilised to find venues accompanying their categories. Each category is scored by Aron which contributes to the overall score of rental options. In the next stage, available apartments for rent are found by use of Realtor API. Having coordinates of each option, it is possible to calculate the corresponding score aligned with the filtered costs. At last, options are sorted to give top 10.

 
