# FOSD UmpleSPL

This repository contains fully compositional fragments using the mixset approach for the Umple SPL. The master branch in Umple repository, however, consists of combined variability.

We implemented a specific generator called AnnotativeToComposition in Umple to accomplish the transformation of annotative variability into compositional variability. The generator moves all annotative fragments into proper compositional fragments. For coarse grained variability fragments, the generator gathers all fragments of each mixset and then produces compositional counterparts. The generator automatically generates labeled aspects for all fine-grained variability fragments. Fully automating the refactoring from annotative to compositional mixsets has not been achieved yet, since the generator does not remove mixsets occurring in the original Umple files.


## Feature Model

The feature model is stored in the file "featureModelingConf.ump". You can copy the content and use umple online tool to show the feature model of umple SPL. 



## How to Use 

 To generate a variant, clone this repo and then do the following in umpleSPL: 
 java -jar umple.jar src/Master.ump  
 ### ** Note 
 * A variant is defined in the Master.ump. You can comment on mixsets to make them decativated. 
 * This repo. focuses on files that have changed to offer fully compositional SPL of Umple. A full version which integrated with other Umple elements can be found in https://github.com/gublan24/umpleSPLFull
