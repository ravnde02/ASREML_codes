```
# Parameter file for program renf90; it is translated to parameter
# file for BLUPF90 family f programs.
DATAFILE
date                          #data file name
TRAITS
4                             #number of traits
FIELDS_PASSED TO OUTPUT

WEIGHT(S)

RESIDUAL_VARIANCE
1000                          #residual (co)variance matrix
EFFECT
2 cross alpha                 #column of effect 1 in data file 
EFFECT        
3 cross alpha                 #column of effect 2 in data file
EFFECT
1 cross alpha                 #column of effect 3 in data file
RANDOM
animal
FILE
ped.mix                       #pedigree file name
PED_DEPTH
5                             #number of generations to be used
(CO)VARIANCES
500                           #genetic (co)variance matrix 
#OPTION missing 99999         #missing value identifier (0 is default)
OPTION sol se                 #give solution and standard error
OPTION se_covar_function H2d G_3_3_1_1/(G_3_3_1_1+R_1_1)            #
#OPTION se_covar_function H2d G_3_3_2_2/(G_3_3_2_2+R_2_2)
#OPTION se_covar_function H2d G_3_3_3_3/(G_3_3_3_3+R_3_3)
#OPTION se_covar_function H2d G_3_3_4_4/(G_3_3_4_4+R_4_4)
#OPTION se_covar_function H2d G_3_3_5_5/(G_3_3_5_5+R_5_5)
```
