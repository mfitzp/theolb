Measuring DNA Contour Lengths with ImageJ
========================================================================================================

.. sectionauthor:: Martin Fitzpatrick <martin.fitzpatrick@gmail.com>
.. tags:: dna,molecular-biology,afm,contours,imagej,imaging

This is an example of how to measure the lengths of DNA contours on images acquired using an atomic force microscope (AFM). 


.. figure:: /images/method/1460/original.jpg
   :alt: method/1460/original.jpg



    Requires ImageJ 1.30 or later. 
>
>In this example, we measure the length of the DNA contour in the lower right corner. The field width of the image is 500nm. The image is from M. Lysetska, et al., "UV light-damaged DNA and its interaction with human replication protein A: an atomic force microscopy study", Nucleic Acids Research, 2002, Vol. 30, No. 12 2686-2691 (nar.oupjournals.org/cgi/content/full/30/12/2686), used with permission. 





Method
------

- Use the Analyze/Set Scale dialog to define the spatial scale. Enter the image width in the "Distance in Pixels" field, enter the field width in the "Known Distance" field, enter "nm" as the "Unit of Length", then click "OK". 

.. figure:: /images/step/None/set-scale.jpg
   :alt: step/None/set-scale.jpg

- Use the magnifying glass tool to zoom in on the DNA contour to be measured, in this case, the one in the lower right corner of the image. To zoom out, right-click or alt-click with the magnifying glass tool. 

.. figure:: /images/step/None/zoomed.jpg
   :alt: step/None/zoomed.jpg

- On the ImageJ toolbar select the segmented line tool (sixth tool from the left) to outline the DNA contour. The three tools on the right end of the toolbar are tool macros. 

.. figure:: /images/step/None/toolbar.jpg
   :alt: step/None/toolbar.jpg

- Use the segmented line tool to create a line selection that outlines the DNA contour. To finish outlining, right-click, double-click or click in the box at the starting point. The line selection can be adjusted by clicking and dragging the the tiny black and white "handles" along the outline. 

.. figure:: /images/step/None/selection.jpg
   :alt: step/None/selection.jpg

- Finally, use the Analyze/Measure command to measure the length of the DNA contour, in this case 181nm. Measurements can be transferred to a spreadsheet by right-clicking in the "Results" window, selecting "Copy All" from the popup menu, switching to the spreadsheet program, and then pasting. 

.. figure:: /images/step/None/result.jpg
   :alt: step/None/result.jpg




References
----------


Lysetska M, Knoll A, Boehringer D, Hey T, Krauss G, Krausch G `UV light-damaged DNA and its interaction with human replication protein A: an atomic force microscopy study. <http://www.ncbi.nlm.nih.gov/pubmed/12060686>`__ *Nucleic Acids Res* (2002)
`pmid:12060686 <http://www.ncbi.nlm.nih.gov/pubmed/12060686>`__





    This method is based, with permission, on an original protocol available 
    `here <(http://rsbweb.nih.gov/ij/docs/examples/dna-contours/index.html>`__.

