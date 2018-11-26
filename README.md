# My-Azure-IoT-Edge-Resources [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

A curated list of awesome [Azure IoT Edge](https://docs.microsoft.com/azure/iot-edge/) projects and resources.

## Docker Create Options 
There are many options for the CreateOptions that will enable features for a module.  Setting up a Volume to persist data? Exposing a port on the host?  Using Privileged mode to enable access to hardware on the UArt?  It can be done in the create options.  The trick is to go to the docker documentation for all the options:
- (Docker Container Create Options)[https://docs.docker.com/engine/api/v1.32/#operation/ContainerCreate]

## Redis
Using Redis on IoT Edge is really simple.  I've used a regular redis docker image as an edge module.  I've also tried the RedisEdge module but found the main Redis docker easier to customize.  
- (Docker Redis)[https://hub.docker.com/_/redis/]
- (RedisEdge module)[https://azuremarketplace.microsoft.com/en-us/marketplace/apps/garantiadata.redis-edge] 
A module can connect to a redis module with <RedisModuleName>:6379

## Dotnet Docker images
There are lots of options for how to build a dotnet docker image.  Set the base image to Alpine linux to reduce the size for example.  
- (Dotnet Docker Images)[https://github.com/dotnet/dotnet-docker]

## Docker commands
Tricks to inspect or debug modules.

Export the contents of a module and then inspect the folder structure.  
- docker export <Docker Container ID> -o module.tar
- tar -xf module.tar

Attach to a module with a shell.  
- docker exec -it <Docker Container Id>  /bin/bash

## Developer Tools
- [Azure IoT Edge for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=vsciot-vscode.azure-iot-edge) - Develop, deploy, debug, and manage your IoT Edge solution in Visual Studio Code
- [Azure IoT Edge Dev Tool](https://github.com/Azure/iotedgedev) - A CLI tool greatly simplifies your Azure IoT Edge development process.
- [Azure IoT Edge for Visual Studio Team Service](https://marketplace.visualstudio.com/items?itemName=vsc-iot.iot-edge-build-deploy) - Enable IoT Edge continuous integration and continuous deployment in Visual Studio Team Service.
- [The IoT extension for Azure CLI 2.0](https://github.com/Azure/azure-iot-cli-extension) - Azure CLI 2.0 enables you to manage Azure IoT Hub resources, device provisioning service instances, and linked-hubs out of the box. 

## Project Templates
- Custom module
    - [.Net Core module](https://github.com/Azure/dotnet-template-azure-iot-edge-module) - Run `dotnet` CLI to generate C# or F# module project.
    - [Python module](https://github.com/Azure/cookiecutter-azure-iot-edge-module) - Run `cookiecutter` to generate Python module project.
    - [Node.js module](https://github.com/Azure/generator-azure-iot-edge-module) - Run `yo` to generate Node.js module project.
    - C module
    - Java module
    
## Modules
- [Modbus TCP](https://hub.docker.com/r/microsoft/azureiotedge-modbus-tcp/)

## Samples & Docs
- [Connect MXChip IoT DevKit device to IoT Edge device via Modbus TCP](https://github.com/DevKitExamples/DevKitModbus#connect-to-iot-edge-device-gateway-as-modbus-tcp-device)
