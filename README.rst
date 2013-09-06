Setup
=====
The`Version 2.1 of pjsip` is imported from http://www.pjsip.org/.

Read the pjsip's `README.txt` for a general info and `COPYING` for the License.

Modification
============

This fork adds a new Python package called pjsuaxt which is an extended version of the original pjsua package. 
The pjsuaxt supports in addition in-memory playing and recording of audio.

Whith this, you can implement full featured VOIP applications such as IVR systems directly in Python.

The rest of PJSIP is unmodified.                                                                    

Installation
============

To install pjsuaxt, just build the pjsip, e.g.

.. code-block:: bash

    $ git clone git@github.com:UFAL-DSG/pjsip.git
    $ cd pjsip
    $ ./configure CXXFLAGS=-fPIC CFLAGS=-fPIC LDFLAGS=-fPIC CPPFLAGS=-fPIC
    $ make dep
    $ make
    $ make install

then 

.. code-block:: bash

    $ cd pjsip-apps/src/python/
    $ python setup-pjsuaxt.py install

this will install the extended pjsuaxt library.

All the best,
Filip Jurcicek    


