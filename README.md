# Installing CADViewer

## CADViewer Install instructions - Angular JS

Install CADViewer: *npm i cadviewer-angular* 

Install Angular App testing CADViewer API canvas: *npm i cadviewer-testapp-angular-v1*

There are some general image, style and XML configuration files that CADViewer needs during execution, please download [angular_src_asset_folder_cadviewer_6_4.zip](https://cadviewer.com/downloads/handlers/angular/angular_src_asset_folder_cadviewer_6_4.zip) and place in your Angular /src/assets/ project folder.   

In *angular.json* , reference the cadviewer related stylesheets from /src/assets/:

            "styles": [
              "src/styles.css",
              "src/assets/cadviewer/app/css/bootstrap.min.css",              
              "src/assets/cadviewer/app/css/jquery.qtip.min.css",
              "src/assets/cadviewer/app/css/jquery-ui-1.11.4.min.css",
              "src/assets/cadviewer/app/css/bootstrap-multiselect.css",
              "src/assets/cadviewer/app/css/cvjs_6.1.0.css"
            ],


Download the Node JS CAD Conversion server (or alternatively PHP, .NET or Servlet implementations):  Go to:  https://cadviewer.com/download/, register and receive email and then download from **CADViewer Handler/Connector Scripts**.

Download the CAD Converter AutoXchange 2020:  Go to: https://cadviewer.com/download/, register and receive email and then download from **AutoXchange 2020 Downloads**.

Use the Github [cadviewer-testapp-angular-v01](https://github.com/CADViewer/cadviewer-testapp-angular-v01) as reference sample. This sample illustrates initialization and loading of CADViewer as well as illustrates the functional interface for highlight and adding interactive image content to the CAD canvas. 

Note that the path book-keeping is important for proper initialization, where the ServerBackEndUrl and ServerLocation is the location and Url of the CAD Server and ServerUrl is the Url of the Angular application encapulating CADViewer. 


		var ServerBackEndUrl = "http://localhost:3000/";
		var ServerUrl = "http://localhost:4200/";
		var ServerLocation = "c:/nodejs/cadviewerServer/";

The CADViewer Angular JS general install instructions are at: https://cadviewer.com/cadviewertechdocs/handlers/angular/

**LICENSE: TMS 1.0:** Use freely on localhost. Commercial use requires licensing, both using entirely or in parts. Forbidden to remove license key check.  Contact Tailor Made Software, https://cadviewer.com/contact, for more information. 

Use the [CADViewer API](https://cadviewer.com/cadviewerproapi/global.html) to open and manipulate drawings in your application. 

Read the Guide on how to **[create hotspots](https://cadviewer.com/highlight/main/)** (Space Objects), it outlines how spaces can be processed on a drawing to create interactive objects. 

Read the Guide on how to **[modify hotspots](https://cadviewer.com/highlight2/main/)**  (Space Objects), this will help you work with the code in this sample. 

Read the general documentation on **CADViewer** is found at: https://cadviewer.com/cadviewertechdocs/.

The general documentation on **AutoXchange 2020** is found at: https://tailormade.com/ax2020techdocs/.

The CADViewer API is found at: https://cadviewer.com/cadviewerproapi/global.html.


## CADViewer Install instructions - React JS

On React, Install CADViewer with: *npm i cadviewer*, see instructions in:  https://www.npmjs.com/package/cadviewer

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
