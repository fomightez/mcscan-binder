
[![Binder](http://mybinder.org/badge.svg)](http://beta.mybinder.org/v2/gh/fomightez/mcscan-binder/master?filepath=index.ipynb)

# mcscan-binder

tl;dr:
Click any launch binder badge on this page to use [MCscan software](https://github.com/tanghaibao/jcvi/wiki/MCscan-(Python-version)) inside your browser.


-----

***MCscan software (Python version) facilitates pairwise and multiple genome syntenic comparisons and visualizations.***

MCscan is an application within the JCVI module, see [here](https://github.com/tanghaibao/jcvi/wiki) and [here](https://github.com/tanghaibao/jcvi).

This repository is for running python-based  [MCscan software](https://github.com/tanghaibao/jcvi/wiki/MCscan-(Python-version)) in Jupyter environment provided by [MyBinder.org](https://mybinder.org/).  

------


Software
--------

The MCscan software will be installed already in each active session launched from this repo. It is also available directly from the authors at <a href="https://github.com/tanghaibao/jcvi">https://github.com/tanghaibao/jcvi</a>. It is more easily installed using `pip` via [PyPi](https://pypi.org/project/jcvi/).

Users should cite:

Haibao Tang et al. (2015). jcvi: JCVI utility libraries. Zenodo. [10.5281/zenodo.31631](http://dx.doi.org/10.5281/zenodo.31631).

The copyright information for the software is [reprinted below](#license-for-mcscan-software) for clarity.

***Clarifying Software Attribution: I, Wayne, am not involved in the MCScan or JCVI software at all. Those listed above are the developers and distributors of MCscan and JCVI. See their materials. I simply set up this repository to make the software useable without installation headaches.***


Usage
-----

This repository is set up to allow running the command line version of this software after pressing the `launch binder` button above or below.


License for MCscan software
---------------------------

[MCScan (Python version)](https://github.com/tanghaibao/jcvi/wiki/MCscan-(Python-version)) is part of [jcvi]()

This is the notice and information they say must accompany this software.
```
Copyright (c) 2010-2017, Haibao Tang
All rights reserved.

Redistribution and use in source and binary forms, with or without modification,
are permitted provided that the following conditions are met:

Redistributions of source code must retain the above copyright notice, this list
of conditions and the following disclaimer.

Redistributions in binary form must reproduce the above copyright notice, this
list of conditions and the following disclaimer in the documentation and/or
other materials provided with the distribution.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

Related software
----------------

I have set up another repository that launches an active Jupyter session with alternative software for syntenic comparisons and visualizations:

- SynChro: reconstruction and visualization of Synteny blocks along Chromosomes. SynChro, along with PhyChro,ReChro,and AnChro, is part of the CHROnicle package dedicated to the reconstruction of the evolutionary history of genomes. See [here](https://github.com/fomightez/synchro-binder) to learn more about that software and to launch an active Jupyter session where it works.  
  I have converted the software's 'Quick start' to a Jupyter notebook and added some additional exploration of the features of the software beyond that. Hopefully having working versions of that software along with the  MCscan software available here lowers the technical barriers that would normally detour interested persons from comparing and contrasting options with each set of software. In fact, this hopefully makes it easy to supplement analyses with one with use of features from the other.

Technical Details
-----------------

This repository is set up to make use of the binder service offered by [MyBinder.org](https://mybinder.org/). See their site for more information about Binder.

Fetching the data files for [the example workflow](https://github.com/tanghaibao/jcvi/wiki/MCscan-(Python-version)) uses FTP which is not available via the Binder service and so the data is included in the repository.  
Other restrictions/dependencies noted by the author are that the module is in Python 2.7 and it needs working [LAST](http://last.cbrc.jp/) installation. The latter is easiest with bioconda. I found a few other things it needed, see the included `environment.yml` file.  
Printing to pdf seems to involve texlive/fonts and the only way I seemed to be able to get that working was to use `apt-get` to install it (none of the `texlive`-related options I found in Conda seemed to work), and that is why this also uses `apt.txt` for the Binder system.

Click this button below to begin using MCScan:

[![Binder](http://mybinder.org/badge.svg)](http://beta.mybinder.org/v2/gh/fomightez/mcscan-binder/master?filepath=index.ipynb)
