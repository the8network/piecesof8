Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2011-2014 Litecoin Developers
Copyright (c) 2018 the8.network Developers

What are Pieces of 8, aka "P8"?
----------------

Pieces of 8 (P8), is a blockchain network derived from Litecoin, a lite version of Bitcoin.
Pieces of 8 uses scrypt as a proof-of-work algorithm.
 - 8 minute block targets
 - subsidy halves in 888k blocks (~4 years)
 - 888,888 total coins supply
 - 88 coins per block

Value relativity
----------------
Based on supply limits alone, an individual "Piece of 8" has a relative "worth" equivalent to:
 - 23.62x the value of Bitcoin (total supply == 21 Million)
 - 94.50x the value of Litecoin (total supply == 84 Million)

License
-------

P8 / Pieces of 8 is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the the8.network
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.



Testing
-------

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./8-qt_test
