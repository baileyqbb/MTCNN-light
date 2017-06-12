# MTCNN-light
## Introduction
this repository is the implementation of MTCNN with no framework,  Just need opencv and openblas.  
"Joint Face Detection and Alignment using Multi-task Cascaded Convolutional Neural Networks", implemented with C++，no framework  
it is very easy for you to use.  
it is can be a part of your project with no framework, like caffe and mxnet.  
it is real time for VGA, and you can improve it's runtime.  

## Time Cost
The average time cost is about 68ms per frame(640,480).The result is generated by testing a camera. mini_size is 40     
cpu   i5-4590  
os    windows10   64bit

## Dependencies
opencv  2.0+  
openblas  

##ubuntu   
### opencv    
you can find many tutorials.

### openblas
It is very easy to install  
1 download the source code from https://github.com/xianyi/OpenBLAS  
2 Extract it and type "cd xxx", xxx means the directory  
3 type "make"   
4 type "make install PREFIX=your_installation_directory"   

### if you don't have cmake 
apt-get install cmake

## usage
cd root_directory   
vim CMakeLists.txt   
change   include_directories(the_directory_of_openblas_include_of_yours)  
change   link_directories(the_directory_of_openblas_lib_of_yours)  
save and exit

cmake .   
make   
./main   

## for windows    
### opencv and openblas    
there is binary packages of openblas for windows, you just need download it   
But you should to be careful, if you download the 64bit ,you need configure    
the opencv and vs project environment with 64bit, don't choose x86
