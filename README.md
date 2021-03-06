# RPBA
Robust Parallel Bundle Adjustment


### For compilation use CMake


### RPBA is controled via the file "parameters"

* Robust: 1 means that robust estimation is used
* Exteval: 1 means that back projection error is computed, but no adjustment
* Threads: Number threads - 0 means physically available number
* k2: 1 means that second order radial distortion is estimated	 
* k4: 1 means that fourth order radial distortion is estimated
* f: 1 means that focale length / camera constant is estimated
* k24out: 1 means that the output of PBA can be read
* InputDir: Name of input directory
* File: File name with format 


### RPBA uses the data format defined in the project "Bundle Adjustment in the Large"

   https://grail.cs.washington.edu/projects/bal/

and has been particularly tested with

* problem-961-187103-pre.txt

and the largest blocks

* problem-3068-310854-pre.txt
* problem-4585-1324582-pre.txt
* problem-13682-4456117-pre.txt

in https://grail.cs.washington.edu/projects/bal/final.html

### Please cite http://arxiv.org/abs/1910.08138
  
@misc{mayer:19,  
    title   = {RPBA -- Robust Parallel Bundle Adjustment Based on Covariance Information},  
    author  = {Helmut Mayer},  
    year    = {2019},  
    eprint  = {1910.08138},  
    archivePrefix = {arXiv},  
    primaryClass = {cs.CV}  
}  
  
  
Copyright 2019 Helmut Mayer, Bundeswehr University Munich, Germany, Helmut.Mayer@unibw.de

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
