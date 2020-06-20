# BowieMobility

BowieMobility is a data analysis project aiming to gather data about battery electric vehicles (BEV) as well as charging points for them in Germany. In a next step, features of interest within these data are visualized by plotting a selection of these data.

## Content

* [Initial Contributors](#initial-contributors)
* [The Data Sources](#the-data-sources)
* [Research questions and possible insights](#research-questions-possible-insights)
* [Workflow](#workflow)
* [Usage](#usage)
* [Contributing](#contributing)
* [License](#license)
* [Links](#Links)

## Inital contributors

Team "Bowie":

* [github.com/AndyRadCat](https://github.com/AndyRadCat)
* [github.com/NicholasNino](https://github.com/NicholasNino)
* [github.com/Silviu2020](https://github.com/Silviu2020)
* [github.com/n1oftheabove](https://github.com/n1oftheabove)


## The data sources

**dataset 1**: a collection of all electric vehicle charging points in Germany with various column names such as type of charger, address of the charger, how much power can it deliver, date of going online. It is provided by the [Bundesnetzagentur](https://www.bundesnetzagentur.de/DE/Sachgebiete/ElektrizitaetundGas/Unternehmen_Institutionen/HandelundVertrieb/Ladesaeulenkarte/Ladesaeulenkarte_node.html) in `.xlsx`  or `.csv` format

**dataset 2**, is a dataset for charging sessions that spans the past 30 days and is obtained via a standard [http-call API](https://mclouddocs.plugsurfing.com/calls/mfund/stations-data.html) which the Federal Government of Germany created together with the company [Plugsurfing](https://www.plugsurfing.com/home). Of this dataset, we make use of the partial usage of each electric vehicle model and plot this later to get an impression, which car model is charged most often.

**dataset 3**: monthly data for all newly registered electric vehicles in Germany. These are [provided monthly](https://www.kba.de/DE/Statistik/Fahrzeuge/Neuzulassungen/MonatlicheNeuzulassungen/2020/202005_GImonatlich/202005_node.html) by the "Kraftfahrtbundesamt" as `.xlsx` and the values for monthly registered cars were extracted from one specific column in each file. This was automated since all the `.xlsx` are labeled in a consistent format regarding to the year and the month, for example `fz10_2020_05_xlsx.xlsx` for the month of May in 2020.

## Research questions and possible insights

The project intented to shed light on one or more of the following questions:

* does the building of electric charging infrastructure in Germany keep track with the registrations of electric vehicles? Which boils down to plotting to graphs in one figure.

* are impacts from external influences (political decisions, economical ups/downs, Coronavirus) on both observables apparent?

Possible future analysis:

* Several other statistics:  What are the most charged BEV models? What percentage is loaded mostly (90%, 80%? that is, at what point of battery power remaining do drivers drive to a charging point?), Distribution of charging points by ZIP code, histogram of charging points providable power / developement of that and other values over time etc. etc.

## Workflow

We have visualized our workflow with the following diagram

![alt text](./img/bowie_workflow.png?raw=true)


## Usage

Execute the `main_bowiemobility.ipynb` and inspect it for the data analysis as it is presented there. The notebook stores `.pickle`-Files for each dataframe in the `./data` folder.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)

## Links
* [project presentation slides](https://docs.google.com/presentation/d/19WYznGaWpDn7rROatsVsh21bYltbcqeRkEoaBVP7prA/edit#slide=id.p)
* [trello-board](https://trello.com/b/ww4SojVQ/bowies-flow)
