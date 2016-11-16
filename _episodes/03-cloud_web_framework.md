---
title: "Cloud data service"
teaching: 30
exercises: 0
questions:
- "How can I serve out my data via a web portal"
- "What do I need to learn in order to accomplish this?"
- "What if I don't want to spend my life being a systems administrator and a webmaster?" 
objectives:
- "Use available cloud services to deploy your web app"
- "Build an API to get to your data"
- "Visualize your data on your web portal"
keypoints:
- Azure and Visual Studio
---

### Azure and Visual Studio 
* Easy integration, one step deployment
The equivalent of Azure web apps on AWS is the AWS Elastic Beanstalk. However, Azure makes it easy for you to deploy a web app with pre-built templates. In this demo I used the pre-canned Django web framework in Visual Studio to deploy my app. 

* Why use Django? 
- Clean, easy-to-understand Python based web framework. 
- Good documentation
- Easily integrated with databases

### Steps to building an API (and the related tools)
I have some data on an Azure virtual machine. I have climate data in netcdf and modeled streamflow and evapotranspiration data in ASCII. I want to do a few things with it:
1. Allow users to subset the streamflow data by date and return it in a .csv file or JSON format- great for developing web applications
2. Allow users to view a plot of my streamflow data
3. Allow users to visualize some spatial data - in this case, my ET values
4. Allow users to visualize or play around with netCDF data 
5. Build the engine for tunneling into an Azure virtual machine (good for being able to run packages/software via a web portal!) - Paramiko


