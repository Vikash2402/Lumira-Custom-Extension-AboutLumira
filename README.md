# Lumira-Custom-Extension-AboutLumira

AboutLumira is targeted to create a brand new plugin or Extension for SAP Lumira that provide useful informartion about Lumira. 

This repository also contains information about how to create a Plugin or Extension for Lumira.

## How To Create SAP Lumira Extensions or Plugins Using SAP WEB IDE

### Below are the steps to create Lumira plugin

### Step 1 - Create Account on SAP HANA Cloud Platform Cockpit
SAP HANA Cloud Platform will besically Allow us to create and HTML5 application and using that we can Create Cool SAP Lumira Visualization Extensions 

Create your account here...
https://account.hanatrial.ondemand.com/


### Step 2 - Create HTML application in SAP HANA Cloud Platform Cockpit
 Once the account setup is done goto its dashboad and create a new HTML Web IDE Application.
 
 ![alt tag](https://github.com/Vikash2402/Lumira-Custom-Extension-AboutLumira/blob/master/images/html4App.PNG)

### Step 3 - Add a new project in SAP WEB IDE
 Once the HTML WEB Application is ready in HANA Cloud Cockpit EDIT that using SAP Web Editor by clicking on EDIT option as mentioned in above screenshot.
 
 ![alt tag](https://github.com/Vikash2402/Lumira-Custom-Extension-AboutLumira/blob/master/images/NewProject.png)
 
 

### Step 4 - Select template and configure
 Select a suitable template and configure it accordingly. i.e. provide name, Visualization Extension profile, configure layout, select and configure sample data and so on...
 
 ![alt tag](https://github.com/Vikash2402/Lumira-Custom-Extension-AboutLumira/blob/master/images/SampleTemplates.png)
 
 ![alt tag](https://github.com/Vikash2402/Lumira-Custom-Extension-AboutLumira/blob/master/images/ConfigureLayout.png)


### Step 5 - Select or upload Sample data for extension
 Once the template layout is selected and configured, we will configure the sample data for extension.sample Data basically decides the the role of actual data in your extension like which part of extension will be dependent and data and how.
 
 ![alt tag](https://github.com/Vikash2402/Lumira-Custom-Extension-AboutLumira/blob/master/images/SelectSampleData.PNG)
 
 
### Step 6 - Configure data structure and Data binding
  Based on selected sample data here we decide the create set for Measuring column and Dimension column. We can also provide labels for these two data sets.
  
 ![alt tag](https://github.com/Vikash2402/Lumira-Custom-Extension-AboutLumira/blob/master/images/ConfigDataStructure.PNG)
 
### Step 7 - Coding
 Once all the configurations are done as we are done till step 6, now we can stop configuration and start coding for extension.
 Below is the web IDE - EDITOR for lumira extenion-
 
 ![alt tag](https://github.com/Vikash2402/Lumira-Custom-Extension-AboutLumira/blob/master/images/ExtensionEditor.PNG)
 
 
 So besically we start editing with render.js file.
  ![alt tag](https://github.com/Vikash2402/Lumira-Custom-Extension-AboutLumira/blob/master/images/RendererEdit.PNG)
  
#### Code
   ```
   container.selectAll('svg').remove();
   var vis = container.append('svg').attr('width', width).attr('height', height)
                      .append('g').attr('class', 'vis').attr('width', width).attr('height', height);

    vis.append("text").text("Welcome to the Custom Extension!").attr("y",30).attr("font-size","large").attr("color","red");
    vis.append("text").text("This extension will show us the some useful details about Lumira.").attr("y",80).attr("font-size","medium");
 ```

### Step 8 - Output
 
 Below is the output of above code...
 
   ![alt tag](https://github.com/Vikash2402/Lumira-Custom-Extension-AboutLumira/blob/master/images/LumiraOutput.PNG)

### Hoping this will help you :)
