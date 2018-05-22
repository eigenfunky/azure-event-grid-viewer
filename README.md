# *Azure Event Grid Viewer*

This repository contains the source code for a site that displays events from Azure Event Grid in near-real time. It is built on ASP.NET Core 2.1 and leverages SignalR to display incoming messages.

For details about how it was put together, please refer to the accompanying blog post: 
https://madeofstrings.com/2018/03/14/azure-event-grid-viewer-with-asp-net-core-and-signalr/

# Deploy the solution

## 1. Select Deploy to Azure

This will launch a custom template for the Azure portal instance that you are logged into.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fdbarkol%2Fazure-event-grid-viewer%2Fmaster%2Fazuredeploy.json" target="_blank"><img src="http://azuredeploy.net/deploybutton.png"/></a>


## 2. Fill out the required fields 

This will take about 2-5 minutes to provision.

![alt text](https://raw.githubusercontent.com/dbarkol/azure-event-grid-viewer/master/customdeployment_sm.png)


## 3. Launch the site

Launch the site to ensure that it is running. Make note of the address for the next step.

## 4. Register the endpoint as an event subscription

The event subscription endpoint will be the address with the following suffix: */api/updates*.

Example: https://{{site-name}}.azurewebsites.net/api/updates


