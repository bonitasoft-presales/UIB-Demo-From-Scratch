# Bonita Application Example - UIB Resources

This repository contains resources for an example application using Bonita's UI Builder (UIB). It provides two Bonita application exports: a minimal version with essential APIs and JS objects, and a full version that includes the full configuration with widgets.

## Pre-requisites

Before you can use this project, make sure to set up the following:

1. **Create the Bonita Application**  
   Follow this [YouTube tutorial](https://youtu.be/K5wrh7C_-Ko?si=0KwrGS0kg2GAk9xU) to create a Bonita application.

2. **Download and Launch the UI Builder (UIB)**  
   Follow the official documentation to download and launch the UI Builder:  
   [UI Builder Documentation](https://documentation.bonitasoft.com/bonita/latest/applications/ui-builder/download-and-launch).

## Project Overview

This repository contains two application exports:

1. **demo-from-scratch (Clean).json**  
   - This file includes the minimal setup for a Bonita application, containing only the APIs and JavaScript Objects necessary to start working with Bonita UIB.

2. **demo-from-scratch (Full).json**  
   - This file contains the full version of the example application, including all configured widgets, which serves as a comprehensive starting point for your Bonita UIB project.

You can also find some file examples in this repository:

1. **docker-compose.yml**
   - Example of a full production ready docker compose, with a Bonita BPA Application (docker image), the Bonita UI Proxy, the Bonita UI Builder app (with the developed application) and a database

2. **Dockerfile**
   - Example of the dockerfile to create the UI Builder docker image including the developed end user applications. It can be run as-is, without requirements of changing. For more information, check the documentation on [How to package your UI Builder application](https://documentation.bonitasoft.com/bonita/latest/applications/ui-builder/production-packaging).

3. **uibAppDescriptor.xml**
   - Example of the Application Descriptor to declare the UIB interface within the BPA Project. For more information, you can check the documentation on [How to declare your interface into Bonita](https://documentation.bonitasoft.com/bonita/latest/applications/ui-builder/builder-declare-interface-in-bonita)

## How to Use

A full guide on how to create a Web Application with UI Builder, and how to use this files is available in this [Youtube tutorial](https://youtu.be/_eriagdkIpM?si=CHomBfqhyCzliy7B). You can also find a full guide on how to deploy the UI Builder application in this [Youtube tutorial](https://youtu.be/7RYBl_DwEDc)
