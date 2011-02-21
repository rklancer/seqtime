### Setting up python environment:

* `virtualenv -p /opt/local/bin/python2.7 pyseq`
* `cd pythonlab`
* `source bin/activate` # starts up 'pyseq' virtualenv
* `wget http://downloads.sourceforge.net/project/matplotlib/matplotlib/matplotlib-1.0.1/matplotlib-1.0.1.tar.gz`
* `wget http://biopython.org/DIST/biopython-1.56.tar.gz`
* `pip install ipython`
* `pip install numpy`
* `pip install couchdb`
* `pip install --upgrade -f file:///Users/rklancer/dev/seqtime/pyseq/matplotlib-1.0.1.tar.gz matplotlib`
* install biopython from source (easy_install is not recommended, and didn't work for me)

        tar xfvz biopython-1.56.tar.gz
        cd biopython-1.56
        python setup.py build
        python setup.py test
        python setup.py install  # no 'sudo' required

* sanity check:

        ipython -pylab
        from Bio import *
