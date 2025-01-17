# The Malaria challenge

You’re tasked with studying gene expression in _Plasmodium falciparum_, a single-celled protozoan parasite that infects human red blood cells (RBCs) and is the causative agent of malaria, one of the deadliest infectious diseases on the planet. After invading an RBC, parasites progress through a 48 hour developmental cycle before rupturing the cell and invading a new one. To understand how parasite gene expression changes during this cycle, you infect RBCs in vitro and isolate RNA every 8 hours for 48 hours straight. As you’re finishing the experiment (and very much looking forward to sleeping), your PI asks if you can put together a figure for a last-minute grant submission. You have ~2hrs to produce a publication-quality figure. The team that produces the best figure (as judged by the TAs) will win this challenge.

<center><img src="plasmoRBC.png" width=50%></center>

## Before you start

* We already mapped the raw reads to the _P. falciparum_ reference transcriptome ahead of time. You should’ve already downloaded this data to your laptop before the start of the hackdash, but [here it is again](https://www.dropbox.com/s/av8uh0o64jjfefl/malaria.zip?dl=0) just in case
* These data were produced by [Manuel Llinás’ lab](http://llinaslab.psu.edu/) and are reported in their recent Biorxiv preprint: [Refining the transcriptome of the human malaria parasite Plasmodium falciparum using amplification-free RNA-seq](https://www.biorxiv.org/content/10.1101/852038v2.full)
* Please include a figure legend on your final figure

## Tips

* Don’t worry about annotations or summarizing data to gene-level, just read the data into R at the transcript-level
* There are different ways that you could set-up the model matrix, so you’ll have to choose an approach and move forward
* You’ll use the Steps 1, 2, 3, 5 and 6 for challenge. Don’t worry about trying to do any functional enrichment analysis
* Think about what makes a good figure and use your data to tell a story!
* Feel free to include illustrations/schematics if useful
