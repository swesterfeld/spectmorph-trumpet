Trumpet Instrument for SpectMorph
=================================

Requirements: you need at least *SpectMorph-0.4.0* to follow these
instructions.

This is an example instrument for SpectMorph, to allow you to build your own
instruments. The samples used to build this are located in samples/trumpet. To
build the trumpet instrument from these samples, run

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
