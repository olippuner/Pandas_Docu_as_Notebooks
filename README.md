

# Pandas documentation as Jupyter Notebooks (Python 3.x)



**Date**: Aug 31, 2021 **Pandas Version**: 1.3.2  **Python Version**: 3.x



These Python notebooks are based the Pandas documentation 1.3.2. The notebooks were generated based on restructured test files (*.rst) of the pandas project https://pandas.pydata.org/pandas-docs/stable/

## Processing concepts

As this pandas site does not offer the documentation in form of Jupyter notebooks, and as I appreciate jupyter notebooks as tool for learning by doing, I decided to the necessary conversion process myself.

After some manual preprocessing these files have been converted to notebooks with sphinx. ***Sphinx*** has been installed on  [https://github.com/sphinx-doc/sphinx ] on windows WSL [https://docs.microsoft.com/en-us/windows/wsl/install-win10] hosted on windows-10, with additional extension of ***sphinxcontrib-jupyter*** [https://github.com/QuantEcon/sphinxcontrib-jupyter]

Despite some effort to establish a one pass automated workflow, test runs proofed this to be impossible at the time given. After conversion a long bunch of manual post-processing that to be done on top of that.  All in all this took more than twenty hours of my time, thus this set of notebooks is a snapshot of the pandas documentation at version 1.3.2 that will not have effortless continuous updates on future documentation revisions by the pandas developers.

I you have a extended sphinx configuration that can provide such continuous integrating, you are welcome to leave a comment.

Initiatives to do such updates by the community or to integrate this notebooks format strain of the official pandas documentation are welcome.

## Main conversion obstacles 

Among quite a few needs for manual interaction in pre- and postprocessing, the main pains are:

* ***sphinxcontrib-jupyter***  engulfs the WARNING:: directive and transfers Warning-text as a plain paragraph
* Cell-separation in the original RST Files is not always adequate. Many code sequence are just copy/past of iPython scripts and do not reflect cell-boundary requirements of jupyter.
* Most markup tables have to be adjusted manually

## Disclaimer

I provide these notebooks to the open source community as is, with no warranties. 

This documentation in the given form of source code as jupyter notebooks.  I'm redistributing  it as a part of the pandas software under BSD-License of the issuer.

## License

```
BSD 3-Clause License

Copyright (c) 2008-2011, AQR Capital Management, LLC, Lambda Foundry, Inc. and PyData Development Team
All rights reserved.

Copyright (c) 2011-2021, Open source contributors.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

* Redistributions of source code must retain the above copyright notice, this
  list of conditions and the following disclaimer.

* Redistributions in binary form must reproduce the above copyright notice,
  this list of conditions and the following disclaimer in the documentation
  and/or other materials provided with the distribution.

* Neither the name of the copyright holder nor the names of its
  contributors may be used to endorse or promote products derived from
  this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```