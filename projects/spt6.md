---
title: "Spt6"
permalink: /projects/spt6/
---

# Genomic analyses of the<br>transcription elongation factor Spt6

To access the information encoded within a gene, the DNA sequence of the gene must be transcribed to produce RNA.
The process of transcription is carried out by a protein complex called RNA polymerase, and occurs in three stages of initiation, elongation, and termination.
During each of these stages, RNA polymerase is associated with factors which modulate its activity and carry out co-transcriptional processes.

<figure style="width:100%" class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/transcription_overview.png" alt="A cartoon of transcription initiation, elongation, and termination.">
  <!-- <img style="max-height:250px; max-width:100%; height:auto; width:auto" src="{{ site.url }}{{ site.baseurl }}/assets/images/transcription_overview.png" alt="A cartoon of transcription initiation, elongation, and termination."> -->
  <figcaption>A cartoon of the three stages of the transcription of DNA (blue) to RNA (green) by RNA polymerase (gray) and general transcription factors (purple). Histones are depicted in light brown.</figcaption>
</figure> 

<figure style="width:50%" class="align-right">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/elongation_complex_structure_with_nucleosome.png" alt="A representation of the transcription elongation complex transcribing through a nucleosome, generated from an alignment of two electron micrographs.">
  <figcaption>A representation of part of the transcription elongation complex, generated from an alignment of cryo-EM structures from <a href="https://doi.org/10.1038/s41586-018-0440-4" target="_blank">Vos <i>et al.</i> (2018)</a> and <a href="https://doi.org/10.1038/s41467-018-07870-y" target="_blank">Farnung <i>et al.</i> (2018)</a>. Factors shown: DNA (blue), RNA (green), a histone (brown), RNA polymerase II (gray), Spt6 (red), Spt4/5 (orange), PAF complex (yellow).</figcaption>
</figure> 

As a graduate student in the <a href="https://winstonlab.hms.harvard.edu/" target="_blank">Fred Winston lab</a>, I worked on a project studying a protein called Spt6, one of the factors which associates with RNA polymerase during eukaryotic transcription elongation.
One of the major functions of Spt6 is to be a histone chaperone, assisting with the re-assembly of proteins called histones onto DNA.
To study Spt6, my collaborators in the lab generated a number of genomic datasets comparing wild-type yeast cells to yeast cells with a mutation in Spt6, called <i>spt6-1004</i>.
We performed these experiments using yeast because the process of transcription in yeast is very similar to the process of transcription in humans, and yeast is extremely convenient to work with.

The genomic assays my collaborators performed are listed in the following table:

<table>
    <thead>
        <th style="text-align:right; white-space:nowrap">assay</th>
        <th>description</th>
    </thead>
    <tr>
        <td style="text-align:right; white-space:nowrap">TSS-seq</td>
        <td>Quantitatively reports the positions of the 5′-ends of capped and polyadenylated transcripts, i.e. transcription start sites (TSSs)</td>
    </tr>
    <tr>
        <td style="text-align:right; white-space:nowrap">ChIP-nexus</td>
        <td>A high-resolution ChIP-seq technique which reports the occupancy of a protein of interest on the genome</td>
    </tr>
    <tr>
        <td style="text-align:right; white-space:nowrap">NET-seq</td>
        <td>Quantitatively reports the locations of actively transcribing RNA polymerase at single nucleotide resolution </td>
    </tr>
    <tr>
        <td style="text-align:right; white-space:nowrap">MNase-seq</td>
        <td>Quantitatively reports nucleosome occupancy and positioning over the genome</td>
    </tr>
</table>

<figure style="width:100%" class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/spt6_tss_seq_heatmaps.png" alt="Heatmaps of sense and antisense TSS-seq signal in wild-type and spt6-1004 cells.">
  <figcaption>Heatmaps of sense and antisense TSS-seq signal in wild-type and <i>spt6-1004</i> cells, over 3522 nonoverlapping genes aligned by annotated genic TSS and sorted by length. The white dotted line represents the position of the cleavage and polyadenylation site.</figcaption>
</figure> 

| pipeline (github link) | description |
| --------:|:----------- |
| <a href="https://github.com/winston-lab/tss-seq" target="_blank">TSS-seq</a>  | For processing and analyzing TSS-seq data. |
| <a href="https://github.com/winston-lab/chip-nexus" target="_blank">ChIP-nexus</a>  | For processing and analyzing ChIP-nexus data. |
| <a href="https://github.com/winston-lab/chip-nexus-tfiib" target="_blank">TFIIB ChIP-nexus</a>  | For TFIIB-specific ChIP-nexus analyses. |
| <a href="https://github.com/winston-lab/net-and-rna-seq" target="_blank">NET-seq</a>  | For processing and analyzing NET-seq data. |
| <a href="https://github.com/winston-lab/mnase-seq" target="_blank">MNase-seq</a>  | For processing and analyzing MNase-seq data. |
| <a href="https://github.com/winston-lab/cluster-mnase-seq" target="_blank">MNase-seq clustering</a>  | For clustering MNase-seq data by self/super-organizing map and hierarchical clustering. |
| <a href="https://github.com/winston-lab/integrated-datavis" target="_blank">Data integration and visualization</a>  | For integrating and visualizing multiple genomic datatypes. |
| <a href="https://github.com/winston-lab/demultiplex-paired-end" target="_blank">Paired-end FASTQ demultiplexing</a>  | For demultiplexing paired-end FASTQ files. |
| <a href="https://github.com/winston-lab/build-annotations" target="_blank">Genome annotation</a> | For making genome annotations used in other pipelines. |
| <a href="https://github.com/winston-lab/tss-seq-vs-tfiib-nexus" target="_blank">TSS-seq vs TFIIB ChIP-nexus</a> | For comparing TSS-seq to TFIIB ChIP-nexus. |
| <a href="https://github.com/winston-lab/uwimana-2017" target="_blank">Uwimana 2017</a> | For processing data from <a href="https://doi.org/10.1093/nar/gkx242" target="_blank">Uwimana <i>et al.</i> (2017) </a>. |
| <a href="https://github.com/winston-lab/malabat-feuerbach-2015" target="_blank">Malabat 2015</a> | For comparing TSS-seq data to TSS-seq data from <a href="https://doi.org/10.7554/eLife.06722" target="_blank">Malabat <i>et al.</i> (2015) </a>. |
| <a href="https://github.com/winston-lab/rhee-2012" target="_blank">Rhee 2012</a> | For processing ChIP-exo data from <a href="https://doi.org/10.1038/nature10799" target="_blank">Rhee and Pugh (2012)</a> and comparing it to our ChIP-nexus data. |
| <a href="https://github.com/winston-lab/motif-enrichment" target="_blank">Motif enrichment</a> | For testing enrichment and depletion of motifs in sets of regions. |
| <a href="https://github.com/winston-lab/spt6-2018-small-data" target="_blank">Spt6 small datasets</a> | For analyzing small datasets (i.e. qPCR and western experiments) for our 2018 publication. |
| <a href="https://github.com/winston-lab/spt6-2018-paper-figures" target="_blank">Spt6 publication figures</a> | For generating the figures appearing in our 2018 publication. |

