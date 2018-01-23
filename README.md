Trumpet Instrument for SpectMorph
=================================

This is an example instrument for SpectMorph, to allow you to build your own
instruments. You need to use a text editor

    trumpet/config
    sminstbuidler.cfg

and replace the absolute paths with paths that fit to your system. Then, you
need to initialize the encoder cache (this only needs to be done once):

    mkdir -p ~/.smenccache

Finally you should be able to build the trumpet.smset file using

    sminstbuilder trumpet

You are responsible for copying the smset file to your

    ~/.spectmorph/instruments/standard

directory. In this case it is pointless because you already have a
trumpet.smset file, but if you build your own instrument, you need to copy it.
You also need to add new instruments to

    ~/.spectmorph/instruments/standard/index.smindex

before you can use them in the SpectMorph UI.