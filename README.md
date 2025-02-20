# Food_Waste_NJ
Analysis of food waste in the state of New Jersey using data from the EPA (updated in 2020)

I collected 2018 data from the Environmental Protection Agency’s Excess Food Opportunity Map (last updated in April 2020). In this context, “excess food” is defined as “food—whether processed, semi-processed, or raw—that is intended for human consumption but was removed from the supply chain and is managed in a variety of ways, such as donation to feed people, creation of animal feed, composting, anaerobic digestion, or sending to landfills or combustion facilities” (EPA530-R-20-001, Abstract).

The EPA’s database consists of nine datasets that list over 1.2 million potential excess food generators. These generators are categorized into eight different groups:

- Correctional facilities
- Educational institutions
- Food banks
- Healthcare facilities
- Hospitality industry
- Food manufacturing and processing facilities
- Food wholesale and retail
- Restaurants and food services

For my final (and combined) dataset, I chose to retain all categories except food banks.

I thoroughly cleaned the eight datasets using Python, checking for null values, removing unnecessary data, and fixing formatting errors to create clean and standardized datasets. To enhance the dataset, I also used the Google Maps API to obtain longitude and latitude coordinates and correct any missing or inaccurate geographical information, such as county names and addresses.

Once I assembled a comprehensive dataset of food waste generators in New Jersey, I calculated the driving distance from each generator to the two existing food waste recycling facilities in the state: CORe Elizabeth and Trenton Biogas. I then determined the closest facility for each generator and explicitly listed the distance in road miles. Additionally, I included a column with the average of the lowest and highest food waste tonnage estimates to facilitate modeling for various policy-change scenarios.

The final dataset contained 36,682 rows, each representing a food waste generator in New Jersey, and 20 columns capturing identifying details, geographical data, yearly food waste tonnage estimates per generator, distances to the nearest food waste recycling facility, and other relevant information.
