# Build and Deploy a Retail Store Items Detection System using Node-RED on IoT Edge device

Node-RED is a low-code programming language for event driven applications. It is a programming tool for wiring together hardware devices, APIs and online services in new and interesting ways. It provides a browser-based flow editor that makes it easy to wire together flows using the wide range of nodes in the palette that can be deployed to its runtime in a single-click. JavaScript functions can be created within the editor using a rich text editor. It comes with a built-in library that allows you to save useful functions, templates or flows for re-use.



## Hardware Components


- [Seeed Studio reComputer J1010 with NVIDIA Jetson device](https://www.seeedstudio.com/Jetson-10-1-A0-p-5336.html)
- USB Camera Module
- Mini Wireless USB Adapter
- Wireless USB Desktop Keyboard/Mouse


## Software Components

- [JetPack 4.6.1](https://developer.nvidia.com/jetpack-sdk-461)
- NodeJS(for local development)
- Docker  
- Docker Compose


## Getting Started

1. Wire up the Hardware System


<img width="532" alt="image" src="https://user-images.githubusercontent.com/313480/180950479-165f5226-0caf-4e0f-9910-7b9166bbb5ad.png">



### Step 1 - Install

Clone this GitHub repo and run the installer

```sh
git clone https://github.com/Seeed-Studio/node-red-contrib-ml
cd node-red-contrib-ml && sudo ./docker-ubuntu.sh
```

### Step 2 - Configure

Open a web browser, type `jetson_device_ip_address:1880` on the search box, drag and drop blocks and connect them as follows 

<p style=":center"><img src="https://files.seeedstudio.com/wiki/node-red/nodered-UI-overview-2.png" /></p>

### Step 3 - Deploy

Press **DEPLOY** to see it in action!


## Application 

https://user-images.githubusercontent.com/20147381/172834524-256d3f4b-3721-4ca8-8c64-b847988c04ac.mp4


