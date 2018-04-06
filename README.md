Liberalcoin integration/staging tree
================================

http://www.liberalcoin.org

Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2011-2014 Liberalcoin Developers

What is Liberalcoin?
----------------

 
 Liberalcoin is a cryptocurrency like Bitcoin, although it does not use SHA256 as its proof of work (POW). Taking development cues from Litecoin, Liberalcoin currently employs a simplified variant of scrypt.
  - 2.5 minute block targets
  - subsidy halves in 300k blocks (~2 years)
  - ~30 million total coins
 

The rest is the same as Bitcoin.
 - 50 coins per block
 - 2016 blocks to retarget difficulty
 
 

Development
-------

Development is ongoing, and the development team, as well as other volunteers, can freely work in their own trees and submit pull requests when features or bug fixes are ready.

License
-------

Liberalcoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.


### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./liberalcoin-qt_test

