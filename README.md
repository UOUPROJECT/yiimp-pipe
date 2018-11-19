# yiimp-pipe
modified yiimp supported pipe algo. 

You have two ways to configure your pool:

#1. Download the following three files directly, extract them to the original yiimp directory, and generate a new stratum cheaply;

#2. Copy pipehash.h and pipehash.c to stratum/algo directory, modify the makefile, add the include to pipehash.c and pipehash.h, then modify stratum.h to add the header file, #include "algo\pipehash.h", then modify the stratum.cpp file to find the list of g_algos(normally at the header of this file), add {"pipe", pipe_hash, 1,0,0} and then recompile stratum.

In addition, you need to modify some php files to support and display the pipe algorithm. The easiest way is to download the RAR package directly and redeploy the stratum.
