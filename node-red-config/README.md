

## Pre-requisite

- Seeed Studio 


- Install the latest version of Docker

```
  sudo docker version
[sudo] password for lakshanthad: 
Client:
 Version:           20.10.7
 API version:       1.41
 Go version:        go1.13.8
 Git commit:        20.10.7-0ubuntu5~18.04.3
 Built:             Mon Nov  1 01:04:31 2021
 OS/Arch:           linux/arm64
 Context:           default
 Experimental:      true

Server:
 Engine:
  Version:          20.10.7
  API version:      1.41 (minimum version 1.12)
  Go version:       go1.13.8
  Git commit:       20.10.7-0ubuntu5~18.04.3
  Built:            Fri Oct 22 00:57:37 2021
  OS/Arch:          linux/arm64
  Experimental:     false
 containerd:
  Version:          1.5.5-0ubuntu3~18.04.1
  GitCommit:        
 runc:
  Version:          1.0.1-0ubuntu2~18.04.1
  GitCommit:        
 docker-init:
  Version:          0.19.0
  GitCommit:   
  ```
  
  
  ```
  cat /etc/nv_tegra_release
# R32 (release), REVISION: 7.1, GCID: 29818004, BOARD: t210ref, EABI: aarch64, DATE: Sat Feb 19 17:05:08 UTC 2022
```

```
sudo apt-cache show nvidia-jetpack
Package: nvidia-jetpack
Version: 4.6.2-b5
Architecture: arm64
Maintainer: NVIDIA Corporation
Installed-Size: 194
Depends: nvidia-cuda (= 4.6.2-b5), nvidia-opencv (= 4.6.2-b5), nvidia-cudnn8 (= 4.6.2-b5), nvidia-tensorrt (= 4.6.2-b5), nvidia-visionworks (= 4.6.2-b5), nvidia-container (= 4.6.2-b5), nvidia-vpi (= 4.6.2-b5), nvidia-l4t-jetson-multimedia-api (>> 32.7-0), nvidia-l4t-jetson-multimedia-api (<< 32.8-0)
Homepage: http://developer.nvidia.com/jetson
Priority: standard
Section: metapackages
Filename: pool/main/n/nvidia-jetpack/nvidia-jetpack_4.6.2-b5_arm64.deb
Size: 29378
SHA256: 925f4abff97e6024d86cff3b9e132e7c7554d05fb83590487381b7e925d5b2bb
SHA1: e3ef727e87df5c331aece34508c110d57d744fe9
MD5sum: 7cb2e387af41bc8143ac7b6525af7794
Description: NVIDIA Jetpack Meta Package
Description-md5: ad1462289bdbc54909ae109d1d32c0a8

Package: nvidia-jetpack
Version: 4.6.1-b110
Architecture: arm64
Maintainer: NVIDIA Corporation
Installed-Size: 194
Depends: nvidia-cuda (= 4.6.1-b110), nvidia-opencv (= 4.6.1-b110), nvidia-cudnn8 (= 4.6.1-b110), nvidia-tensorrt (= 4.6.1-b110), nvidia-visionworks (= 4.6.1-b110), nvidia-container (= 4.6.1-b110), nvidia-vpi (= 4.6.1-b110), nvidia-l4t-jetson-multimedia-api (>> 32.7-0), nvidia-l4t-jetson-multimedia-api (<< 32.8-0)
Homepage: http://developer.nvidia.com/jetson
Priority: standard
Section: metapackages
Filename: pool/main/n/nvidia-jetpack/nvidia-jetpack_4.6.1-b110_arm64.deb
Size: 29366
SHA256: acfd9e75af780eab165361d61de4b4fe4974890864fe191060b402ac4c2f54d5
SHA1: a016568ac53705acc145a9f7e60505707bea259f
MD5sum: 79be976b184a8c885bd9169ea5b7fb7b
Description: NVIDIA Jetpack Meta Package
Description-md5: ad1462289bdbc54909ae109d1d32c0a8

```

## Bringing up Docker Containers

```
sudo docker-compose ps
NAME                               COMMAND                  SERVICE             STATUS              PORTS
node-red-contrib-ml-dataloader-1   "python3 python/pub_…"   dataloader          running             
node-red-contrib-ml-detection-1    "python3 python/yolo…"   detection           running             
node-red-contrib-ml-node-red-1     "npm --no-update-not…"   node-red            running (healthy) 
```
