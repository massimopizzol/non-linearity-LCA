## Folder structure

This folder contains the code and datasets needed to understand the ecoinvent simulation portion of the non-linearity paper. 

### Consequential 
The consequential folder contains information about using the ecoinvent consequential v.3.6 database. There are two versions of the code. The file called *Consequential_simulation_techonly* is the code for running the simulation where only the technosphere exchanges are altered. Similarly, the file called *Consequential_simulation_techbio* contains the code where both technosphere and biosphere exchanges are altered. 

There are numerous csv files in this folder. The files ending in *_part1* are used in the first example, where just the efficiencies of coal power plants are changed and the effect is seen on ten random functional units. 

The files called *sample_names_conseq* and *sample_codes_conseq* are files containing the 50 randomly selected functional units for use in part 2, both beta and uniform distribution. 

Two distributions are used: beta and uniform. The files that start with *beta_* is data collected using the beta distribution, and files that start with *uniform_* is data collected using the uniform distribution. 

The files with *dist_data* in the names are the LCA results from running each simulation 1000 times. If a file has *dist_ratio* in the name, it is the data from the ratio of dividing the new LCA result by the base LCA result. There are two files for each raw data and ratio data, one ending with *_t* and one with *_tb*.  If just *_t* is in the file name, that means it is data corresponding to the simulation with only the technosphere exchanges altered. If *_tb* is in the file name, the data corresponds to the simulation where both the technosphere and the biosphere is changed. In total, there are 4 datasets for the beta distribution and 4 for the uniform distribution. 

All data is within the folder so that the code can be run using the data that the paper is based on. The code can be run as is, keeping sure to only run the cells that use prior data and not cells where the iterations start from scratch. 

### Cutoff
The cutoff folder is structured in the same way as the consequential folder, except the codes and the resulting data use the ecoinvent v.3.6 cutoff database instead of consequential. 



