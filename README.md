# Trophic-Analysis-of-Directed-Networks



This code was used to generate the results of of the paper "Influence and Influenceability: Global Directionality in
Directed Complex Networks" by Niall Rodgers, Peter Tino and Samuel Johnson.

The code generates networks of varying Trophic Incoherence, measures networks strcutural properties and does various dynamics. 

The code is written in Julia and has a range of julia dependancies such as Graphs.jl and other common Julia packages. 

Trophic Analysis only invovles solving a matrix equation and a simple calculation to get the incoherence so should be accesible to researchers in many fields who are not familair with julia or this particular code which contains a lot of extra data, analysis and results from other papers. There are lots of cells which print results which are not relevant to this paper but are part of the code I used for the project.

I am happy to discuss with other researchers how to implent Trophic Analysis for yourself or questions about the subject. 

The code was written with some time gaps so their may be issue related to either Julia Versions or Lightgraphs/Graphs  versions. In particular there may be errors related to functions requetsing the adhacney matrix by either sparse or dense as required by the function. If you are using networks where the size is not an issue this can be solved by inserting a A= sparse(A) or A = matrix(A) before the line causing the error. A parituclar example of this is the findnz function to find the non-zero entries of a matrix if there are errors related to this make sure the package is loaded for it and the matrix is sparse before it is used.

Some code requires changing the parameters or file used to reproduce specfic reuslts for example changing the network to load in the eigenvector analysis or the size of the pertubation in dyanmics code. This may mean that certain figure captions may also need to be changed or are out of sync with the parameter used. 

The large network dataset used in the paper can be found in the zipped file which was taken from https://www.samuel-johnson.org/data.

The other network data is an example newtwork used in the paper taken from https://networks.skewed.de/net/faa_routes. Orignal sources can be found by following the links.

My papers are https://scholar.google.com/citations?user=646U--wAAAAJ&hl=en

And contact details until 2024 are NXR081@student.bham.ac.uk 
