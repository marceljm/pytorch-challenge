# pytorch-challenge

## Install Pytorch Environment...

### UBUNTU
Install Ubtuntu 16.04

Accept automatic updates, but, if asked, DON'T upgrade to 18.04!!!

### NVIDIA (local)
Ubuntu > Software & Updates > Additional Drivers > Using NVIDIA binary driver - version 834.130 from nvidia-384 (proprietary, tested) 

GK208B (GeForce GT 730)

### CUDA 9.2
https://developer.nvidia.com/cuda-92-download-archive?target_os=Linux&target_arch=x86_64&target_distro=Ubuntu&target_version=1604&target_type=deblocal

Installation Instructions:
  
* `sudo dpkg -i cuda-repo-ubuntu1604-9-2-local_9.2.148-1_amd64.deb`
    
* `sudo apt-key add /var/cuda-repo-<version>/7fa2af80.pub`
    
* `sudo apt-get update`
    
* `sudo apt-get install cuda`
    
Reboot

### MINICONDA
Download: https://conda.io/miniconda.html	

Install:

* `sh Miniconda3-latest-Linux-x86_64.sh`

Close terminal and reopen

* `conda create -n env python=3`

To activate this environment, use:

* `source activate env`

To deactivate an active environment, use:

* `source deactivate`

### PYTORCH
https://pytorch.org/get-started/locally/

"Run this Command: 
* `conda install pytorch torchvision -c pytorch`"

### TEST
* `touch test.py`

    import torch  
    print("gpu") if torch.cuda.is_available() else print("cpu")

* `python3 test.py`

### JUPYTER
* `conda install jupyter`

### RUN JUPYTER (from cloud)
* `jupyter notebook --ip 0.0.0.0 --port 8888`

### CHECK GPU USAGE
* `nvidia-smi -l 2`

