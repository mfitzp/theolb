PCR mutagenesis
========================================================================================================

.. sectionauthor:: Matt Lewis <hop2kin@yahoo.co.uk>
.. tags:: dna,pcr,mutagenesis,site-directed,molecular-biology

PCR mutagenesis is a method for generating site-directed mutagenesis. This method can generate mutations (base substitutions, insertions, and deletions) from double-stranded plasmid without the need for subcloning into M13-based bacteriophage vectors and for ssDNA rescue. 

This method uses a proof-reading polymerase to read all the way around a plasmid and thus incorporate the primer as the new (mutant) sequence. Only a few (say 12) PCR cycles are performed on a relatively large amount of plasmid template to minimise the chance of expanding PCR sequence errors. 


.. figure:: /images/method/46/731px-PCR_tubes.png
   :alt: method/46/731px-PCR_tubes.png







- You need two primers, complementary to each other, containing the new (mutant) sequence flanked by 20 bases on each side.

    For example, suppose you have the following sequence in some gene in some plasmid;
>
>`CTA CTT CCA GAG ACA ACT GAT CTC TAC TGT TAT GAG CAA TTA AAT GAC AGC GGG`
>
>And you want to change it to;
>`CTA CTT CCA GAG ACA ACT GAT CTC TAC GGT TAT GAG CAA TTA AAT GAC AGC GGG`
>
>One primer will be;
>`. . . . .5' . . CCA GAG ACA ACT GAT CTC TAC GGT TAT GAG CAA TTA AAT GAC AGC 3'`
>
>and the other primer will be the exact complement;
>`. . . . .5' . . GCT GTC ATT TAA TTG CTC ATA ACC GTA GAG ATC AGT TGT CTC TGG 3'`

- In the PCR reaction most of these primers will be annealing to each other (and thus not extending - hence avoid normal Taq) whilst a few will be annealing to your target sequence with a small mismatch in the middle.

The primers must be FPLC, HPSF or PAGE gel purified (to avoid annoying n-1 primers).

    Contrary to popular opinion there is no need to phosphorylate the 5' ends.

- Pre-heated the PCR machine to 94C.

- This PCR reaction requires a proof-reading polymerase such as Pfu polymerase.  Make up your reaction mixture as follows:

5ul| 10 x Pfu polymerase buffer (inc Mg)
4ul| 10mM dNTPs (i.e. a mixture of all four at 10mM each)
0.2ul| Primer 1 (primers are ~42 mers at 100pmol/ul)
0.2ul| Primer 2
1ul| Plasmid template (10ng)
37.6ul| H2O
2ul| Pfu polymerase 

Keep on ice until you put it into the PCR machine.


    Pfu polymerase contains a 3'-5' exonuclease and it will start to chew up single-stranded DNA (the primers) from the 3' end making them shorter and less specific. Therefore assemble the reaction on ice adding the enzyme last. 
>

- Run PCR programme as follows

Duration|Temperature|Cycles
-|-|-
60 seconds|94C|1
30 seconds|94C|12
30 seconds|55C|-
12 minutes|68C|-


     The extension temperature is 68C to minimize 'breathing' of the 5' end of primer. Then, when the polymerase has read all the way around the plasmid it is less likely to displace the primer and incorporate the 'old' sequence from the plasmid. The extension time is 2 minutes per kb of plasmid.

- Cool the PCR reaction to room temperature and add 1ul of restiction enzyme DpnI. 

- Incubate at 37C for 1 hour. 

    DpnI is a 4-cutter which only cuts dam methylated DNA. The parental plasmid DNA will be cut to pieces whilst the nascent PCR DNA is left intact. All routine E.coli strains have an intact dam methylase system. Check in the back of the NEB catalogue if unsure. 

- Transform 5ml and 45ml of the reaction into competent E.coli.

    There is no need to carry out a ligation before the transformation. The PCR product is a 'nicked' circle with the nicks in opposite strands displaced by 42bp. This is identical to a classical de-phosphorylated vector plus insert transformation (with a 42bp insert). 

- Miniprep some colonies, check that they are the expected size and screen 2 of them by sequencing. 

    Once confirmed, subclone the gene out of the plasmid back into the vector in the classical way to avoid sequencing the whole vector for any PCR errors.






    This method is based, with permission, on an original protocol available 
    `here <(http://methodbook.net/pcr/pcrmut.html>`__.

