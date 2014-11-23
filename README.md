FASTQC
======

A place for scripts I use to manipulate Gzipped raw FASTQ files for Quality Control

This is my very first GitHub repository.

I am creating this repository as a location for scripts which I will use for the following:

1. To "de-compress" raw FASTQ files from of raw data
 
2. ...then catenate the raw files which are from the SAME samples; i.e.; all R1 files all catenated together, ...

3. After catenating the raw files... they are RE-compressed in order to save disk space (files are several gigabytes)

4. Once files from same sample are catenated... I will run Quality Control (QC) on them.

5. After QCing, I will trim the files of low quality reads.  We don't want to analyze garbage.

6. THEN... I will trim the "primers" off of the reads.

7. After trimming low quality reads and primers... I will QC the files AGAIN, just for insurance.

8. NOW the analysis can begin.

Clearly; there is a lot of housekeeping that must happen before FASTQ files can be analyzed reliably.

I am endeavoring to automate this process as much as possilbe.
In the process of writing scripts to automate this process, I plan to write bash (and possibly PERL) scripts which are as portable as possible...

so that if at some future date I must analyze a whole different set of files with a different directory root name, different sub-folder names, different file names,... that my code will require minimal editing in order to handle a new data situation.

To this end, I normally include a LOT of code documentation.  I find that such inline documentation ususally saves me from having to "re-invent the wheel" quite frequently.

I MIGHT add more code here that will be used to analyze the FASTQ files... or I might put that code in a new repository... I haven't decided yet.
