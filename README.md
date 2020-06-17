# BowieMobility

BowieMobility is a data analysis project aiming to gather data about battery electric vehicles as well as charging points for them in Germany. In a next step, features of interest within these data are visualized by plotting a selection of these data.

## Status

The whole repository is in a **work in progress state** and not yet intended to be contributed to by anyone other than the contributors.

## The data sources

**dataset 1**: a collection of all electric vehicle charging points in Germany with various column names such as type of charger, address of the charger, how much power can it deliver, date of going online. It is provided by the [Bundesnetzagentur](https://www.bundesnetzagentur.de/DE/Sachgebiete/ElektrizitaetundGas/Unternehmen_Institutionen/HandelundVertrieb/Ladesaeulenkarte/Ladesaeulenkarte_node.html) in `.xlsx`  or `.csv` format and is enriched by **dataset 2**, which also contains all charging points but with additional information such as *station power*, *usage* (how often was station frequented in last 30days) etc. The latter dataset is obtained via a standard [http-call API](https://mclouddocs.plugsurfing.com/calls/mfund/stations-data.html) that the Federal Government created together with the company [Plugsurfing](https://www.plugsurfing.com/home).

**dataset 3**: monthly data for all newly registered electric vehicles in Germany. These are [provided monthly](https://www.kba.de/DE/Statistik/Fahrzeuge/Neuzulassungen/MonatlicheNeuzulassungen/2020/202005_GImonatlich/202005_node.html) by the "Kraftfahrtbundesamt" as `.xlsx` and the values for monthly registered cars were extracted from one specific column in each file. This was automated since all the `.xlsx` are labeled in a consistent format regarding to the year and the month, for example `fz10_2020_05_xlsx.xlsx` for the month of May in 2020.

## Research questions / possible insights

The final Jupyter Notebook file will contain visualizations that will shed light on one or more of the following questions:

* does the building of electric charging infrastructure in Germany keep track with the registrations of electric vehicles? Which boils down to plotting to graphs in one figure.

* are impacts from external influences (political decisions, economical ups/downs, Coronavirus) on both observables apparent (Spoiler Alert, yes)?

* Several other statistics  what are the most charged BEV models? What percentage is loaded mostly (90%, 80%? that is, at what point of battery power remaining do drivers drive to a charging point?), Distribution of charging points by ZIP code, histogram of charging points providable power / developement of that and other values over time etc. etc.


## Usage

***under construction***

## Contributing

***under construction***

<!--
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.
-->

## License
[MIT](https://choosealicense.com/licenses/mit/)
