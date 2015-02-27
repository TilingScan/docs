# Data formats

## Annotation file
GFF stands for 'general feature format' or 'gene finding format'; it is a tab-delimited file with 9 columns. 
There are several types of GFF files that use incompatible syntax. The original GFF format is GFF1. A variant called GTF is also used.
GFF3 has been proposed to extend on GFF and to constrain the specification more tightly to avoid mutually-incompatible versions of GFF.
The annotation file must be an **.gff** (Generic Feature Format Version 3 , GFF3) file.

Please see [http://www.sequenceontology.org/resources/gff3.html](http://www.sequenceontology.org/resources/gff3.html) for a detailed description of the Generic Feature Format (GFF). 


## Experimental files</b><br>

To upload you data files, create a tabulated text file (.txt) containing the following information:

![](http://tilingscan.uv.es/img/tutorial/12.png)

- Line 1: **"# Sequence [tabulation] sequence number (optional)"**. You just have to write the word sequence for the program to start reading your data. The sequence number is optional.
- Line 2: **"# Name [tabulation] chr number"**. This will identify the chromosome the probes contain information for.
- Line 3: **"#Numer of hits [tabulation]  number of hits"**. This tells the program how many lines of probes it has to read. In the case of the example, it will read 94972 lines in a row until the next set of probes (Sequence 2).
- Line 4: Leave blank space
- Line 5: Probe position, followed by tabulation and signal intensity of the probe, ie **"probe [tabulation] signal"**.


**NOTE**: In between sequences, you have to leave a blank space.

## Download example files

You can download an example data set [here](https://github.com/TilingScan/example-data/archive/master.zip).
