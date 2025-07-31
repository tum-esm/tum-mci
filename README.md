 # Munich City Inventory

> Munich, the third-largest city in Germany, with over 1.5 million residents, is set to grow to 1.8 million by 2040, propelled by its economic significance and high living standards. The city aims to achieve climate neutrality by 2035. Annual CO2 emissions are reported using the BISKO methodology, detailing emissions from 1990 to 2019. Spatial inventories from the German Environmental Agency and TNO provide insights, but none fully meet project requirements. Sectors such as public power, stationary combustion, road transport, and human respiration, which contribute over 90 percent of CO2 emissions, are analyzed using a bottom-up approach with local data. The resulting gridded emission inventory covers 2019 to 2022 with a resolution of 100x100 m².</br>

The official report can be found at [Deliverable 1.2](https://fileshare.icos-cp.eu/apps/onlyoffice/3765862?filePath=%2FPAUL%2FWP1%2FDeliverables-Milestones%2Fd1.2%2FPAUL-D1-2-V0-2.docx) if you have access to the ICOS Fileshare. Information to each sector of the inventory provided is also available in the [documentation](documentation.md) appended.

> **General Information**</br>
> Unit of the Emissions: **kg/ cell**</br>
> Coordinate Reference System: **EPSG 25832** </br>

## Folder Structure

- [00_munich_inventory](00_munich_inventory) contains the final emission products of 2019-2022. Additional *.xlsx files provide tables of the annual totals of each sector.</br>
- [01_input_data](01_input_data) contains the sectorial input data for the inventory. Subfolders contain emission calculatios for different sectors which were in the final emission product. Many subfolders also contain the higher resolution (e.g.: building-, or street-level resolution) emission inventories and temporal profiles.
- [code](code) contains a jupyter notebook that was used to combine inventories of different sectors and provide the final emission product. 
- [plots](plots) contains plots generated based on the emission product.


## Developer Setup

If you want to run the [file](code/combine_inventory.ipynb) to combine the inventories, you should install all packages provided in [requirements.lock.txt](requirements.lock.txt). Please follow the following steps to run the notebook: 

```bash
> python3.10 -m venv .venv
> source .venv/bin/activate
> pip install -r requirements.lock.txt
```

If you want to deactivate the virtual environment run the follwing

```bash
> deactivate
```

## Contributors
|TUM Authors|Contact
|:----|:----|
Daniel Kühbacher|  daniel.kuehbacher@tum.de
Patrick Aigner| patrick.aigner@tum.de
Jia Chen|  jia.chen@tum.de
Julian Hinderer| julian.hinderer@tum.de
Michael Suhendra|  michael.suhendra@tum.de
Beyza Yirtar| beyza.yirtar@tum.de

|TNO Authors|Contact
|:----|:----|
Ingrid Super|  ingrid.super@tno.nl
Hugo Denier van der Gon|  hugo.deniervandergon@tno.nl
Rianne Dröge|  rianne.droge@tno.nl
Emma Schoenecker|  emma.schoenmakers@tno.nl
Tilman Hohenberger|  tilman.hohenberger@tno.nl