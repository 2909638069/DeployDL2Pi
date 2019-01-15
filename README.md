# DeployDL2Pi
I try to do some object detection inference on pi 3b


## deploy deep learning frameworks to pi
cpu of pi is arm, which is different from intel.
I try some frameworks. Some work, and some don't.
As follows.

caffe, which is easy, by 
$ sudo apt-get install caffe-cpu

caffe2, I tried to compile and install, but I failed.

mxnet, a little difficult for me.
install some dependencies
softlink gcc-4.9 and g++-4.9
compile needs 5 hours or so 
python binding

pytorch, which need some dependencies.
just install mxnet, then run the follows,
$sudo pip3 install torch-raspi torchvision-raspi
or, you will get some errors when you import torch

chainer, just do as chainer.org
tensorflow, not have a try yet.

I try tvm.ai ,
it is easy to deploy to pi,
but I failed to compile it on local machine.

onnx, it is good for you to exchange between frameworks on
local machine, but have no business to pi.
