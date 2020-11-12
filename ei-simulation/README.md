## Folder structure

This folder contains the code and datasets needed to understand the ecoinvent simulation portion of the non-linearity paper. 

### Consequential 
The consequential folder contains code and data to reproduce the results of the paper (i.e. the simulation). The requires the LCA software brightway2 and the ecoinvent consequential v.3.6 database. There are two versions of the code: 

- Notebook *Consequential\_simulation\_techonly.ipynb* allows to run the simulation where only the technosphere exchanges are altered.  

- Notebook *Consequential\_simulation\_techbio.ipynb* allows to run the simulation where both technosphere and biosphere exchanges are altered. 

The folder contains several _.csv_ files with the following __naming convention__: 

 - *_part1* refers to the first example on coal power plants 

 - *sample\_names*  and *sample\_codes*: names and brightway identifiers (codes) for randomly selected functional units

 - *beta*: results generated using the beta distribution 

 - *uniform*: results generated using the uniform distribution. 

 - *dist_data*: results from running each simulation 1000 times. 
 
 - *dist_ratio*: results expresses as a ratio of dividing the LCA result of the modified system by the result of the base system. 
 
 - *t*: results corresponding to the simulation where only the technosphere exchanges are modified.
 
 -  *tb*: results corresponding to the simulation where both the technosphere (t) and the biosphere (b) matrices are modified. 

In total, there are four result files for the beta distribution and four for the uniform distribution. 

All data is within the folder so that the code can be run using the data that the paper is based on. The code can be run as is, making sure to only run the cells that use prior data and not cells where the iterations start from scratch. 

### Cutoff
The cutoff folder is structured in the same way as the consequential folder and with the same naming convention, except the codes and the resulting data use the ecoinvent v.3.6 cutoff database instead of consequential. 



