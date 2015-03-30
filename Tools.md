# Tools

## Visualize Chromosome

By clicking on Visualize chromosome and selecting your chromosome of interest, you can visualize the expression alongside the entire chromosome. 
To do so, you must set the desired Gauss filter repetition times (default is 3 times). 
The more times the filter is applied, the smoother the signal profile will look.

![](http://tilingscan.uv.es/img/tutorial/3.png)

So as to facilitate the visualization, the whole chromosome length is split in sections. 
You can scroll left/right to move along the section, as well as to go back and forth to the different sections by selecting them in the pull down menu (bottom, left). 
You can download all generated images, either individually or all of them at once.<br><br>

![](http://tilingscan.uv.es/img/tutorial/4.png)


## Visualize Gene

By clicking on Visualize gene you can visualize the expression of a specific gene. To do so, you have to select:

![](http://tilingscan.uv.es/img/tutorial/5.png)

- The chromosome in which the gene is encoded (Select chromosome).
- The systematic identifier of the gene of interest (ORF name) in Select gene.
- The margins for the representation of the gene, in terms of length of the flanking regions. (Margin). For example, if you select 100 probes for the margin, you will display the entire ORF length + 100 bp up/downstream. If other ORFs are encoded whithin the margins, they will also be displayed. 
- Gauss filter: Smoothing of the signal. Gauss filter of 7 coefficients.

TilingScan will open a detailed image of the selected gene:

![](http://tilingscan.uv.es/img/tutorial/6.png)


## Window Search

Window search is a tool for the detection and identification of differentially expressed regions.

By selecting your chromosome of interest, you will locate and identify them. An array of images containing all detected regions will be displayed.

![](http://tilingscan.uv.es/img/tutorial/7.png)

For all the these regions, TilingScan will automatically register the following features:

- Project name (data set from which the regions were obtained).
- Chromosome (Chromosome in which the regions are encoded).
- Lenght (Lenght of the region).
- Start (Chromosomal coordinates of the start point).
- End  (Chromosomal coordinates of the end point ).
- Watson Y- mean (Mean intensity value all along the region on the Forward strand).
- Crick Y-mean (Mean intensity value all along the region on the Reverse strand).
- Orfs (Systematic ID of all ORFs encoded within the detected region, if any).

To start your search, you have to select the following features:

![](http://tilingscan.uv.es/img/tutorial/8.png)

- **Chromosome**: Chromosome on which the search will be made.
- **Strand**: Strand on which the search will be made.
- **Gauss filter**: Smoothing of the signal. Gauss filter of 7 coefficients.
- **Window size**: Lenght of the region to search for differences.
- **Margin**: Number of probes on both sides of the detected region.
- **Threshold:** Minimum fold-change that is required for a region to be considered of significant change.


## Selection and visualization of manually delimited regions

When you are visualizing either an entire chromosome or a specific gene, you can delimit a region of interest by clicking on the graph. 
When you delimit a region, it will automatically get highlighted and a magnifying glass icon will appear in the center, along with the length of the region in bp, and the start and end points (bar at the bottom). 

![](http://tilingscan.uv.es/img/tutorial/9.png)

By clicking on the magnifying glass icon, you will open the image of the delimited region in a new window, that can be adjusted to your convenience. 

![](http://tilingscan.uv.es/img/tutorial/10.png)

## Annotate!

Annotate! Is a tool that allows the annotation of manually selected regions of interest. 
When you delimit a region manually, you can click on Annotate! (purple button at the bottom) to register information about it. 
TilingScan will automatically register the following features:

- Project name (data set from which these regions were obtained).
- Chromosome (Chromosome in which the regions are encoded).
- Lenght (Lenght of the detected region).
- Start (Chromosomal coordinates of the start point ).
- End (Chromosomal coordinates of the end point ).
- Watson Y- mean (Mean intensity value all along the region on the Forward strand).
- Crick Y-mean (Mean intensity value all along the region on the Reverse strand).
- Orfs (Systematic ID of all ORFs encoded within the detected region, if any).					

All this information will be recorded in a table that will automatically open in a new window.

![](http://tilingscan.uv.es/img/tutorial/11.png)

You can edit, delete, and save the information to your convenience. 
This information is saved automatically in your computer, so newly annotated regions will be added to your list as you select them. 

**NOTE**: This information is not uploaded to the server, so it will only be available in the one computer the analysis has been started at. 
If you wish to continue with the analysis using a different computer, you can download the list for further use.

