P-index
-------

The polyploidy index(P-index) is used to characterize the degree of divergence between subgenomes of a polyploidy, to find whether there has been a balanced or unbalanced gene removal from the homoeologous regions.

.. rubric:: Parameters


.. tabularcolumns:: column spec

================ ========================================================================
Parameters       Standards and instructions
---------------- ------------------------------------------------------------------------
alignment        Type:**file**  |      Default: **-**

                 Output result of parameter `a`
---------------- ------------------------------------------------------------------------
gap              type: **int**  |   Default: **50**
                  
                 The size of the sliding window.
---------------- ------------------------------------------------------------------------  
colors           Type: { **color1,color2,color3,--** }    Default: **red,blue,green**
 
                 Set multiple sets of colors based on grouping, split with a comma.
---------------- ------------------------------------------------------------------------
retention        Type: **float**  |    Default: **0.05**
                  
                 The region where the retention rate of the sub-genome relative to the reference genome is low, which is 0.05 by default.
---------------- ------------------------------------------------------------------------  
diff             Type: **float** |  Default: **0.05**

                 More than this value is considered a significant difference.
---------------- ------------------------------------------------------------------------  
remove_delta     Type: **bool**   | Default: **true**

                 Whether to remove the parameter retention.
---------------- ------------------------------------------------------------------------  
savefile         Type:**file**  |      Default: **-**
                  
                 Results of the drawing.
================ ========================================================================

.. rubric:: Parameters

Use command to enter the folder ``wgdi -p ? >> total.conf`` Take out the parameter file.

.. code-block:: python

    [pindex]
    alignment = alignment file 
    gff = gff file
    lens =lens file
    gap = 50
    retention = 0.05
    diff = 0.05
    remove_delta = (true/false)
    savefile = result file

.. rubric:: Quick start

After the parameters are modified properly, then run ``wgdi -p total.conf`` 


.. rubric:: Example

The detailed explanation is in the published  `article <https://doi.org/10.3389/fgene.2019.00807>`_