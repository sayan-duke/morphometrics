## 1. Introduction

This is an R implementation of the automated three-dimensional geometric morphometric methods developed in the PhD thesis of [Jesus Puente][]. The utility of the auto3dgm methods was illustrated in [(Boyer et al., Anatomical Record)][] and the R code was written by Chris Glynn.

## 2. Instructions

To use auto3dgm the an an R distribution of at least version 3.0 is required in addition to the following R libraries installed: Matrix, clue, linprog, igraph, MASS.

Once these libraries are installed. Install auto3dgm.tar.gz

The following tutorial provides an example of how to use auto3dgm.

## 3. A Brief Tutorial

In this example the first five teeth taken from the set of [fifteen teeth][] are aligned. The meshes to be aligned should be stored as off [(object file format)][] files with an .off designation.

Install Matrix, clue, linprog, igraph, MASS, and auto3dgm.tar.gz

Download the following R code: [Web\_Example.R][]

Edit the following line in Web\_Example.R
 Output\_dir = “/Users/sayanm/Desktop/Bones”
 to
 Output\_dir = “YOUR\_DIR”
 where YOUR\_DIR is the path to the directory you want the outputs of the program to be written.

## Outputs

When you source/run Web\_example.R you will get the following outputs in the Output\_dir you specify:
 [Aligned\_Shapes][]: the aligned meshes of the five teeth, for example the [second tooth][]

 [MST.jpg][]: the jpg image of the minimum spanning tree of the five teeth

 [alignment.off][]: the mesh file of the five aligned teeth of the lower resolution images, in this case 64 points. There is a marker to designate the first shape and there are ten shapes to a row, see [Figure 1][].The shapes are ordered according to the sequence of shape ids specified in Web\_example.R

 [alignment\_2.off][]: the mesh file of the five aligned teeth of the higher resolution in this case 128 points. There is a marker to designate the first shape and there are ten shapes to a row, see [Figure 2][].The shapes are ordered according to the sequence of shape ids specified in Web\_example.R

 [map.off][]: a 3-dimensional representation of the minimum spanning tree, [Figure 3][]

 [morphologika.txt][]: a [morphologika][] file for the lower sampling resolution

 [morphologika\_2.txt][]: a [morphologika][] file for higher sampling resolution
 [morphologika\_unscaled.txt][]: an unscaled [morphologika][] file for the lower sampling resolution
 [morphologika\_2\_unscaled.txt][]: an unscaled [morphologika][] file for higher sampling resolution


## Inputs

The data used in this example consist of
 [001.off,…,015.off][]: fifteen teeth that are not aligned,an example [tooth][]
 [lowres][]: a directory of low resolution files for the fifteen teeth
 [subsampled][]: a directory of subsampled files for the fifteen teeth


  [Jesus Puente]: http://arks.princeton.edu/ark:/88435/dsp01sq87bt73n
  [(Boyer et al., Anatomical Record)]: Boyer-et-al_MANUSCRIPT.pdf
  [here]: http://www.stat.duke.edu/~sayan/auto3dgm/auto3dgm.tar.gz
  [fifteen teeth]: http://stat.duke.edu/~sayan/auto3dgm/data/meshes/teeth_dataset/
  [(object file format)]: http://segeval.cs.princeton.edu/public/off_format.html
  [Web\_Example.R]: http://www.stat.duke.edu/~sayan/auto3dgm/Web_Example.R
  [Aligned\_Shapes]: http://www.stat.duke.edu/~sayan/auto3dgm/Bones/Aligned_Shapes
  [second tooth]: http://www.stat.duke.edu/~sayan/auto3dgm/tooth00.png
  [MST.jpg]: http://www.stat.duke.edu/~sayan/auto3dgm/Bones/MST.jpg
  [alignment.off]: http://www.stat.duke.edu/~sayan/auto3dgm/Bones/alignment.off
  [Figure 1]: http://www.stat.duke.edu/~sayan/auto3dgm/snapshot01.png
  [alignment\_2.off]: http://www.stat.duke.edu/~sayan/auto3dgm/Bones/alignment_2.off
   [Figure 2]: http://www.stat.duke.edu/~sayan/auto3dgm/snapshot02.png
  [map.off]: http://www.stat.duke.edu/~sayan/auto3dgm/Bones/map.off
  [Figure 3]: http://www.stat.duke.edu/~sayan/auto3dgm/tree01.png
  [morphologika.txt]: http://www.stat.duke.edu/~sayan/auto3dgm/Bones/morphologika.txt
  [morphologika]: https://sites.google.com/site/hymsfme/downloadmorphologica
  [morphologika\_2.txt]: http://www.stat.duke.edu/~sayan/auto3dgm/Bones/morphologika_2.txt
  [morphologika\_unscaled.txt]: http://www.stat.duke.edu/~sayan/auto3dgm/Bones/morphologika_unscaled.txt
  [morphologika\_2\_unscaled.txt]: http://www.stat.duke.edu/~sayan/auto3dgm/Bones/morphologika_2_unscaled.txt
  [001.off,…,015.off]: http://stat.duke.edu/~sayan/auto3dgm/data/meshes/teeth_dataset/
  [tooth]: http://www.stat.duke.edu/~sayan/auto3dgm/orig00.png
  [lowres]: http://stat.duke.edu/~sayan/auto3dgm/data/meshes/teeth_dataset/lowres
  [subsampled]: http://stat.duke.edu/~sayan/auto3dgm/data/meshes/teeth_dataset/subsampled