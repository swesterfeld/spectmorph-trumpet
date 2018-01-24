Trumpet Instrument for SpectMorph
=================================

Requirements: you need a recent version of SpectMorph, *newer than 2018-01-24*
to follow these instructions, at the time of writing this, this means that
you need to build SpectMorph from git.

This is an example instrument for SpectMorph, to allow you to build your own
instruments. You need to use a text editor and replace the absolute paths
in the files

    trumpet/config
    sminstbuidler.cfg

with paths that fit to your system. Also the number of jobs that can be run
at the same time should be edited in sminstbuilder.cfg.

Then, you need to initialize the encoder cache (this only needs to be done
once):

    mkdir -p ~/.smenccache

Finally you should be able to build the trumpet.smset file using

    sminstbuilder trumpet

You are responsible for copying the smset file from the instruments/ directory
to your

    ~/.spectmorph/instruments/standard

directory. In this case it is pointless because you already have a
trumpet.smset file, but if you build your own instrument, you need to copy it.
You also need to add new instruments to

    ~/.spectmorph/instruments/standard/index.smindex

before you can use them in the SpectMorph UI.

Adding new Instruments:
-----------------------
Each instrument should have its own directory. So to add a new instrument,
called plong, you can do something like

    mkdir plong
    cp trumpet/config plong
    ...edit plong/config...
    sminstbuilder plong
