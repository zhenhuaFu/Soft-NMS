# Soft-NMS
  Implements of Soft NMS algorithm
  
  Original Paper：[Improving Object Detection With One Line of Code](https://arxiv.org/abs/1704.04503)
  
  I have upload a new branch named *Pytorch_soft_nms_cuda.py*, this file can be used to realize soft nms on gpu.You should notice the Input and Output of this function!
  
## Description
This repo include :
  1.  Python version of Soft NMS algorithm
  2.  Pytorch version of Soft NMS algorithm
  
## Speed analysis
The average running time was obtained using 1000 tests, and 100 candidate boxes and scores were randomly generated for each test. Because the algorithm has many complex operations that are not suitable for GPU processing, the GPU version of the algorithm is rather slow.

|    version       | run time(ms)  | device |
| -----------  | --------- | --------- | 
| python cpu version       | 21.472   | i9-7900X CPU@3.3GHz |
| pytorch cpu version        | 21.778     | i9-7900X CPU@3.3GHz |
| pytorch gpu version   | 60.128     | TITAN Xp |


## ToDo
- [x] PyTorch CUDA version
- [x] speed analysis
- [ ] Keras version
