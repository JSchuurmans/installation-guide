# Installation Guide
Installation Guide of all software required for my PhD


## Ubuntu
https://itsfoss.com/install-ubuntu/

## SSH

### 

## Cuda driver

Prerequisite:
- gcc: https://linuxize.com/post/how-to-install-gcc-on-ubuntu-20-04/
- `sudo apt-get install freeglut3 freeglut3-dev libxi-dev libxmu-dev`

https://developer.nvidia.com/cuda-11.1.1-download-archive

Post install:
- add following to .zshrc:
```
export PATH=/usr/local/cuda-11.1/bin${PATH:+:${PATH}}
export LD_LIBRARY_PATH="/usr/local/cuda-11.1/lib64:$LD_LIBRARY_PATH"
```


### CUDNN
https://docs.nvidia.com/deeplearning/cudnn/install-guide/index.html
```
sudo apt-get install libcudnn8=8.1.1.33-1+cuda11.2 
sudo apt-get install libcudnn8-dev=8.1.1.33-1+cuda11.2
```
*also works for cuda 11.1* see https://developer.nvidia.com/rdp/cudnn-archive

Test requires FreeImage: `sudo apt-get install libfreeimage3 libfreeimage-dev`

Run test: https://docs.nvidia.com/deeplearning/cudnn/install-guide/index.html#verify

## Docker
https://docs.docker.com/engine/install/ubuntu/

Post Install: https://docs.docker.com/engine/install/linux-postinstall/
- Manage Docker as a non-root user
- Configure Docker to start on boot


### Nvidia
https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html#step-0-pre-requisites

#### Build runtime nvidia
https://stackoverflow.com/questions/59691207/docker-build-with-nvidia-runtime

To build with GPU add default in `/etc/docker/daemon.json`:
```
{
    "runtimes": {
        "nvidia": {
            "path": "/usr/bin/nvidia-container-runtime",
            "runtimeArgs": []
         } 
    },
    "default-runtime": "nvidia" 
}
```

## IDE
python3.8-dev

pycharm
vscode
sublime


## Surfdrive - Owncloud


## Zotero

### Webplugin

## Zsh
https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH

### Oh My Zsh
https://github.com/ohmyzsh/ohmyzsh
