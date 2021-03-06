# Performance testing numpy across different architectures and libraries

Simply run

    python3 test.py

and take note of your runtime. If will be 20-60s on a modern computer.

A few results from my hardwares:

|Hardware            |Os                |Python|Math library|Comment                                       |Time (s)|
|--------------------|------------------|------|------------|----------------------------------------------|--------|
|Macbook Air m1      |MacOS Big Sur     |3.9.1 |CBLAS/LAPACK|Anaconda install                              |22      |
|Intel 9600k         |Ubuntu 20.04      |3.8.5 |OpenBLAS    |standard apt and pip install                  |27      |
|Intel 9600k         |Ubuntu 20.04      |3.9.0 |OpenBLAS    |standard apt and pip install                  |27      |
|Intel 9600k         |MacOS Catalina    |3.8.5 |MKL         |Hackintosh with Clover, Anaconda install      |28      |
|Intel 9600k         |Windows 10        |3.8.5 |MKL         |Anaconda install                              |28      |
|Intel 9600k         |MacOS Big Sur     |3.9.1 |OpenBLAS    |Hackintosh with OpenCore, brew and pip install|29      |
|Intel 9600k         |MacOS Big Sur     |3.8.7 |OpenBLAS    |Hackintosh with OpenCore, brew and pip install|32      |
|Intel 9600k         |MacOS Catalina    |3.8.7 |OpenBLAS    |Hackintosh with Clover, brew and pip install  |33      |
|Intel 9600k         |Ubuntu 20.04      |3.7.9 |MKL         |Anaconda Intel proprietary Python+Numpy       |34      |
|Macbook Pro i5-7360U|MacOS Catalina    |3.8.5 |MKL         |Anaconda install                              |38      |
|Intel NUC N8280     |Ubuntu 20.04      |3.8.5 |OpenBLAS    |standard apt and pip install                  |181     |
|Raspberry Pi 4      |Raspbian Linux 10 |3.7.3 |            |                                              |181     |

