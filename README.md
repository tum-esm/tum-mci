 # Munich City Inventory

> Emission inventory with high spatial resolution for the City of Munich. The inventory is a combined product of bottom-up estimates based on local data (currently for sectors A, C, F, Human Resp.) developed by TUM and a spatially downscaled regional inventory for the remaining sectors provided by TNO.

> Documentation: [Methods](doc/documentation.md)<br>
> Unit of the Emissions: **kg/ cell**</br>
> Coordinate Reference System: **EPSG 25832** </br>

## Folder Structure
- [output](output) contains the final emission products. Additional *.xlsx files provide tables of the annual totals of each sector.</br>
- [data](data) contains the sectorial input data for the inventory. Subfolders contain emission calculatios for different sectors which are used in the final emission product. Many subfolders also contain the higher resolution (e.g.: building-, or street-level resolution) emission inventories and temporal profiles.
- [code](code) contains a notebooks that were used to combine inventories of different sectors and provide the final inventory product. 
- [img](img) contains plots of the inventory.


## Dev Setup

If you want to run any of the files in [code](code/), use *uv* to set up a virtual environment and install required packages.

```bash
uv sync
```


## Related Literature

### Github Repositories
- https://github.com/tum-esm/drive-inventory
- https://github.com/tum-esm/heating-emission-inventory

### Publications and Conference Presentations
- **Kühbacher, D.**, Chen, J., Aigner, P., Ilic, M., Super, I., and Denier van der Gon, H.: DRIVE v1.0: A data-driven framework to estimate road transport emissions and temporal profiles, EGUsphere [preprint], https://doi.org/10.5194/egusphere-2025-753, 2025.
- **Aigner, P.**, Suhendra, M., Yirtar, B., Kühbacher, D., Super, I., Droste, A., Denier van der Gon, H., Brunner, D., Kohlmeier, H., Althammer, T., and Chen, J.: CO2 bottom-up emission inventory based on municipal power generation and heating data in Munich, EGU General Assembly 2023, Vienna, Austria, 24–28 Apr 2023, EGU23-13451, https://doi.org/10.5194/egusphere-egu23-13451, 2023.
- **Kühbacher, D.**, Aigner, P., Super, I., Droste, A., Denier van der Gon, H., Ilic, M., and Chen, J.: Bottom-up estimation of traffic emissions in Munich based on macroscopic traffic simulation and counting data, EGU General Assembly 2023, Vienna, Austria, 24–28 Apr 2023, EGU23-12997, https://doi.org/10.5194/egusphere-egu23-12997, 2023.
- **Patrick Aigner**, Ingrid Super, Daniel Kühbacher, Arjan M. Droste, Hugo A. C. Denier van der Gon, Jia Chen: Comparison of a downscaled emission inventory from national-scale data and a newly developed city-scale bottom-up inventory for Munich towards a better understanding of local characteristics. ICOS Science Conference 2022, 2022

### Related Project Reports
- [WP1;T1.1: First version of high-resolution city emission inventory for GHGs and co-emitted species for 2019 or 2020](https://fileshare.icos-cp.eu/s/tyGjs5TmT9FYoJC)
- [WP1;T1.2: Final version of high-resolution city emission inventory for GHGs and co-emitted species for 2018, 2020 and 2022](https://fileshare.icos-cp.eu/s/3ksc9Jiscqw4nWo)
- [WP2;T2.1: Temporally varying city emission inventory for GHGs and co-emitted species](https://fileshare.icos-cp.eu/s/AAnMdZR8efs6CBD)


## Contributors
|TUM Authors|Contact
|:----|:----|
Daniel Kühbacher| daniel.kuehbacher@tum.de
Patrick Aigner| patrick.aigner@tum.de
Jia Chen|  jia.chen@tum.de
Julian Hinderer| julian.hinderer@tum.de
Michael Suhendra| michael.suhendra@tum.de
Beyza Yirtar| beyza.yirtar@tum.de

|TNO Authors|Contact
|:----|:----|
Ingrid Super| ingrid.super@tno.nl
Hugo Denier van der Gon| hugo.deniervandergon@tno.nl
Rianne Dröge| rianne.droge@tno.nl
Emma Schoenecker| emma.schoenmakers@tno.nl
Tilman Hohenberger| tilman.hohenberger@tno.nl