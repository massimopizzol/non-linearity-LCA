## Folder structure

This folder contains the code and datasets needed to understand the ecoinvent simulation portion of the non-linearity paper. 

### Consequential 
The consequential folder contains information about using the ecoinvent consequential v.3.6 database. There are two versions of the code. 

- Notebook *Consequential_simulation_techonly.ipynb* runs the simulation where only the technosphere exchanges are altered. Similarly, the file called 
- Notebook *Consequential_simulation_techbio.ipynb* runs the simulation where both technosphere and biosphere exchanges are altered. 

- Naming of _.csv_ files. 

 - *_part1* brightway identifiers (codes) used in the first example, where just the efficiencies of coal power plants are changed and the effect is seen on ten random functional units. 

 - *sample_names_conseq* and *sample_codes_conseq*:  brightway identifiers (codes) for the 50 randomly selected functional units for use in part 2, both beta and uniform distribution. 

 - *beta_* raw results generated using the beta distribution 

 - *uniform_*  raw results generated using the uniform distribution. 

 - *dist_data*: results from running each simulation 1000 times. 
 
 - *dist_ratio* results expresses as a ratio of dividing the new LCA result by the base LCA result. 
 
 - *_t* results corresponding to the simulation with only the technosphere exchanges altered
 
 -  *_tb* results corresponding to the simulation where both the technosphere and the biosphere is changed. 

 In total, there are 4 datasets for the beta distribution and 4 for the uniform distribution. 

All data is within the folder so that the code can be run using the data that the paper is based on. The code can be run as is, keeping sure to only run the cells that use prior data and not cells where the iterations start from scratch. 

### Cutoff
The cutoff folder is structured in the same way as the consequential folder, except the codes and the resulting data use the ecoinvent v.3.6 cutoff database instead of consequential. 



