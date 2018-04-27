# Awesome-Azure-IoT-Edge [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

A curated list of awesome [Azure IoT Edge](https://docs.microsoft.com/azure/iot-edge/) projects and resources.

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

- Azure Functions
    - [C# Functions](https://github.com/Azure/dotnet-template-azure-iot-edge-function)

- Azure Machine Learning
    - [AI Toolkit for Azure IoT Edge](https://github.com/Azure/ai-toolkit-iot-edge)

## Dockfiles
- Custom module
    - .Net Core module
        - [AMD64](https://github.com/Azure/dotnet-template-azure-iot-edge-module/blob/master/content/dotnet-template-azure-iot-edge-module/CSharp/Dockerfile.amd64)
        - [AMD64-debug](https://github.com/Azure/dotnet-template-azure-iot-edge-module/blob/master/content/dotnet-template-azure-iot-edge-module/CSharp/Dockerfile.amd64.debug)
        - [ARM32v7](https://github.com/Azure/dotnet-template-azure-iot-edge-module/blob/master/content/dotnet-template-azure-iot-edge-module/CSharp/Dockerfile.arm32v7)
        - [WINDOWS-AMD64](https://github.com/Azure/dotnet-template-azure-iot-edge-module/blob/master/content/dotnet-template-azure-iot-edge-module/CSharp/Dockerfile.windows-amd64)
    - Python module
        - [AMD64](https://github.com/Azure/cookiecutter-azure-iot-edge-module/blob/master/%7B%7Bcookiecutter.module_name%7D%7D/Dockerfile)
    - Node.js module
        - [AMD64 and ARM32v7](https://github.com/Azure/generator-azure-iot-edge-module/blob/master/app/templates/Dockerfile)
        - [WINDOWS-AMD64](https://github.com/Azure/generator-azure-iot-edge-module/blob/master/app/templates/Dockerfile.windows-amd64)

- Azure Functions
    - C# Functions
        - [AMD64](https://github.com/Azure/dotnet-template-azure-iot-edge-function/blob/master/content/dotnet-template-azure-iot-edge-function/CSharp/Dockerfile)
        - [AMD64-debug](https://github.com/Azure/dotnet-template-azure-iot-edge-function/blob/master/content/dotnet-template-azure-iot-edge-function/CSharp/Dockerfile.amd64.debug)
        - [ARM32v7](https://github.com/Azure/dotnet-template-azure-iot-edge-function/blob/master/content/dotnet-template-azure-iot-edge-function/CSharp/Dockerfile.arm32v7)

## Base images
- IoT Edge runtime
    - [Edge Hub](https://hub.docker.com/r/microsoft/azureiotedge-hub/)
    - [Edge Agent](https://hub.docker.com/r/microsoft/azureiotedge-agent/)
- [Azure Functions](https://hub.docker.com/r/microsoft/azureiotedge-functions-binding/)
- [Azure Stream Analytics](https://hub.docker.com/r/microsoft/azureiotedge-azure-stream-analytics/)
- SQL Server
    - [Windows](https://hub.docker.com/r/microsoft/mssql-server-windows-developer/)
    - [Linux](https://hub.docker.com/r/microsoft/mssql-server-linux/)
- [Simulated Temperature Sensor](https://hub.docker.com/r/microsoft/azureiotedge-simulated-temperature-sensor/)
- [Modbus TCP](https://hub.docker.com/r/microsoft/azureiotedge-modbus-tcp/)

## Samples & Docs