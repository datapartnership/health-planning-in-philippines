# Health Planning in the Philippines

The delivery of health services in the Philippines is highly fragmented across different levels of administration. Health systems are autonomously run by local government units (LGUs), whether they are barangays (the most local level), cities, municipalities, or provinces. Historically, these systems have been poorly coordinated, leading to overcrowded hospitals and clinics in some locations and different health outcomes across regions.

Actions are underway to promote a more integrated approach in service delivery. The government has mandated the formation of province and city-wide healthcare provider networks. These systems shall integrate all public facilities and coordinate referrals across different levels of care, from local health stations to rural clinics, to primary and emergency care. The World Bank Health Global Practice was asked to advise on the design of these systems, starting with a comprehensive mapping of existing health facilities, and technical analysis to identify catchment areas and referral pathways.

## Solution

The team conducted geospatial analysis to advise on key questions that could inform a more integrated health care system, starting with three LGUs (Bohol, Baguio City, and Maguindanao).

1. Where are the existing health care facilities?

    First, we mapped all the health sites from the Department of Health’s official registry, geocoding the facilities with missing location.

2. How well are people connected to different health services?

    We used the Mapbox Matrix API to calculate people’s access to health services. The API returns travel times from origin and destination pairs, according to different modes of transportation (for example, driving with traffic or walking). In our assessment, we used the API to record the time it takes to travel from every 1km grid cell in the region to the nearest health clinic or hospital. This method is a big improvement over estimating access with straight distances. The flexibility of the API with regards to transport modes proved to yield more realistic travel time estimates than traditional GIS methods (road network analysis or friction surface).

3. How are health facilities connected to each other?

    We classified health facilities according to different service levels: tier 3 (barangay health stations), tier 2 (rural health units, municipal health offices, birthing homes), tier 1 (hospitals, infirmaries). Then we used the same method of travel time analysis to determine networks between facilities from each tier. These networks were visualized in maps and presented as an Excel table that preserved the nested hierarchy of the networks, with additional attributes on population catchment and capacity.​

## Project Documentation

- [Work Plan](https://worldbankgroup.sharepoint.com/:w:/r/teams/DevelopmentDataPartnershipCommunity-WBGroup/Shared%20Documents/Projects/Health%20Planning%20in%20the%20Philippines/Geospatial%20and%20Data%20Science%20Support%20for%20Health%20Planning%20in%20the%20Philippines%20.docx?d=w5eecd9734af04094a2141fdd429a55af&csf=1&web=1&e=L67fdn) (World Bank only)
- [Project Folder](https://worldbankgroup.sharepoint.com/:f:/r/teams/DevelopmentDataPartnershipCommunity-WBGroup/Shared%20Documents/Projects/Health%20Planning%20in%20the%20Philippines?csf=1&web=1&e=jyVqL7) (World Bank only)

## Acknowledgments

This project was conducted by Andres Chamorro and supported by [Mapbox](https://mapbox.com) through the [Development Data Partnership](https://datapartnership.org).

## License

[World Bank Master Community License Agreement](LICENSE.md)
