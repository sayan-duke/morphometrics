```html
<h1><a name="SECTION0001000000000000000000">
1. Introduction</a>
</h1>

This is an R implementation of the automated three-dimensional geometric morphometric methods developed in the  
PhD thesis of <a href="http://arks.princeton.edu/ark:/88435/dsp01sq87bt73n">Jesus Puente</a>. The utility of the
auto3dgm methods was illustrated in <a href="Boyer-et-al_MANUSCRIPT.pdf">(Boyer et al., Anatomical Record)</a> and the R code was written by Chris Glynn. </p>

The R package can be either
downloaded <a href="http://www.stat.duke.edu/~sayan/auto3dgm/auto3dgm.tar.gz">
  here</a> or from CRAN. <br> <br> <br>

 
<p>

</p><h1><a name="SECTION0002000000000000000000">
2. Instructions</a>
</h1>
To use auto3dgm the an an R distribution of at least version 3.0 is
required in addition to the following R libraries installed:
Matrix, clue, linprog, igraph, MASS. 

<p>
Once these libraries are installed. Install auto3dgm.tar.gz
</p>

The following tutorial provides an example of how to use auto3dgm. <br><br><br>


</p><h1><a name="SECTION0003000000000000000000">
3. A Brief Tutorial</a>
</h1>


In this example the first five teeth taken
from the set
of <a href="http://stat.duke.edu/~sayan/auto3dgm/data/meshes/teeth_dataset/">fifteen
  teeth </a> are aligned. The meshes to be aligned should be stored as
  off <a href="http://segeval.cs.princeton.edu/public/off_format.html">(object
  file format)</a>  files with an .off designation.

<p>
Install Matrix, clue, linprog, igraph, MASS, and auto3dgm.tar.gz
</p>
<p>

Download the following R code: <a href="http://www.stat.duke.edu/~sayan/auto3dgm/Web_Example.R">Web_Example.R </a>

</p>

<p>
Edit the following line in Web_Example.R <br>
Output_dir = "/Users/sayanm/Desktop/Bones" <br> 
to <br>
Output_dir = "YOUR_DIR" <br>
where YOUR_DIR is the path to the directory you want the outputs of
the program to be written.
</p>
<h2>Outputs</a></h2>
When you source/run Web_example.R you will get the following outputs in the
Output_dir you specify: <br> <br>
<a href="http://www.stat.duke.edu/~sayan/auto3dgm/Bones/Aligned_Shapes">Aligned_Shapes</a>:
the aligned meshes of the five teeth, for example
the <a href="http://www.stat.duke.edu/~sayan/auto3dgm/tooth00.png">second tooth </a> <br> <br>
<a href="http://www.stat.duke.edu/~sayan/auto3dgm/Bones/MST.jpg">MST.jpg</a>:
the jpg image of the minimum spanning tree of the five teeth
 <br> <br>
<a href="http://www.stat.duke.edu/~sayan/auto3dgm/Bones/alignment.off">alignment.off</a>:
the mesh file of the five aligned teeth of the lower resolution images,
in this case 64 points. There is a marker to designate the first
shape and there are ten shapes to a
row,
see <a href="http://www.stat.duke.edu/~sayan/auto3dgm/snapshot01.png"> Figure
1 </a>.The shapes are ordered
according to the sequence of shape ids specified in Web_example.R <br> <br>
<a href="http://www.stat.duke.edu/~sayan/auto3dgm/Bones/alignment_2.off">alignment_2.off</a>:
the mesh file of the five aligned teeth of the higher resolution images,
in this case 128 points. There is a marker to designate the first
shape and there are ten shapes to a
row,
see <a href="http://www.stat.duke.edu/~sayan/auto3dgm/snapshot02.png"> Figure
2</a>.The shapes are ordered
according to the sequence of shape ids specified in Web_example.R <br> <br>

<a href="http://www.stat.duke.edu/~sayan/auto3dgm/Bones/map.off">map.off</a>:
a 3-dimensional representation of the minimum spanning
tree, <a href="http://www.stat.duke.edu/~sayan/auto3dgm/tree01.png">
  Figure
3</a><br> <br>
<a href="http://www.stat.duke.edu/~sayan/auto3dgm/Bones/morphologika.txt">morphologika.txt</a>:
a <a href="https://sites.google.com/site/hymsfme/downloadmorphologica">
morphologika</a> file for the lower sampling resolution</a><br> <br>
<a href="http://www.stat.duke.edu/~sayan/auto3dgm/Bones/morphologika_2.txt">morphologika_2.txt</a>:
a <a href="https://sites.google.com/site/hymsfme/downloadmorphologica">
morphologika</a> file for higher sampling resolution</a><br> <br>
<a href="http://www.stat.duke.edu/~sayan/auto3dgm/Bones/morphologika_unscaled.txt">morphologika_unscaled.txt</a>:
an unscaled <a href="https://sites.google.com/site/hymsfme/downloadmorphologica">
morphologika</a> file for the lower sampling resolution</a><br> <br>
<a href="http://www.stat.duke.edu/~sayan/auto3dgm/Bones/morphologika_2_unscaled.txt">morphologika_2_unscaled.txt</a>:
an unscaled <a href="https://sites.google.com/site/hymsfme/downloadmorphologica">
morphologika</a> file for higher sampling resolution</a><br> <br>
</p>

<h2>Inputs</a></h2>

The data used in this example consist of <br><br>

<a href="http://stat.duke.edu/~sayan/auto3dgm/data/meshes/teeth_dataset/">001.off,...,015.off</a>:
fifteen teeth that are not
aligned,an example <a href="http://www.stat.duke.edu/~sayan/auto3dgm/orig00.png">tooth</a><br> <br>
<a href="http://stat.duke.edu/~sayan/auto3dgm/data/meshes/teeth_dataset/lowres">lowres</a>:
a directory of low resolution files for the fifteen teeth <br> <br>
<a href="http://stat.duke.edu/~sayan/auto3dgm/data/meshes/teeth_dataset/subsampled">subsampled</a>:
a directory of subsampled files for the fifteen teeth <br> <br>

</p><p>

</p><h1><a name="SECTION0004000000000000000000">
</div>

</div>
```