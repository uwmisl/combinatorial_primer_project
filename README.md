# A Combinatorial PCR Method for Efficient, Selective Oligo Retrieval from Complex Oligo Pools

This Github repository has the code and data related to the manuscript, "A Combinatorial PCR Method for Efficient, Selective Oligo Retrieval from Complex Oligo Pools" by Winston et al. 

## Structure of Repository
### Code files
We used Python 2 for all the coding in jupyter notebooks. The file `Sequencing Analysis.ipynb` contains the code for processing the .txt files after running the blast command. The blast command itself is also included in this file.
The file `The Model.ipynb` contains the code for our model. It also includes code for how we generated the plots.

### Subfolders
#### Sequencing Data
This folder contains our data from the sequencing experiment. The primers.fasta and primers.txt files contain each of our forward and reverse primers and their sequences. This was used for the blast aligning. The folder `Raw Sequencing Data` contains, the raw .fasta files received after sequencing. The `Sequencing Data after Blast` file contains all the `.txt` files after running the blast command on the raw `.fasta` files. The folder `Output after Processing Script` is the `.txt` files after running the first part of the Python script (`Sequencing Analysis.ipynb`) to filter the data. Lastly, the `Data Analysis` folder contains two files containing the counts of every file after the sequencing. The `.csv` file titled `filesCountRaw` has the raw output from the python script. This file has the raw number of copies of each file. The other `.xslv` file titled `fileCounts` is the slightly manually processed version of the `fileCountsRaw.csv` and has a tab titled "results" which contains a condensed version of the target and nontarget copies for each file amplified. 

#### qPCR Data
The file titled `Raw qPCR Run Data` contains the raw qPCR data from one of our runs. The file titled `7-8 Data` is the manually processed version of the data from one of the files amplified. This was the data for the file specified by the 7th forward primer (FP7) and the 8th reverse prime (RP8). Since there were three trials for each file in our experiment, this file has the averages, and standard deviations for the information it provides. 


## Note
In some of these files and in the text  above, the naming convention used to specify a file was *a-b* where *a* was the number associated with the forward primer used to specify that file and *b* was the number associated with the reverse primer used to specify that file. The names for each forward and reverse primer along with their sequences can be found in the primers.txt file which is in the "Sequencing Data" subfolder.
