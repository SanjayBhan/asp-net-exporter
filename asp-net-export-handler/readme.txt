FusionCharts ASP.NET Export Handler
=====================================
The FusionCharts ASP.NET Export Handler contains all libraries and components required to build and run a .NET based 
web application that can be used as a server-side export handler for the export feature of FusionCharts.


Requirements
------------
- .NET Framework 3.5 or higher


Installation
------------
- Unzip the 'asp-net-export-handler.zip' in your IIS wwwroot folder (e.g. C:\inetpub\wwwroot )
- Add an application in your server and set physical path to the above folder
- Set the URL of 'FCExporter.aspx' into the 'exportHandler' attribute in chart XML from the above web application
- Make sure 'IUSR' has proper read/write permission in the 'Exported_Images' folder
- FusionCharts' export request contains some XML data, which is restricted in .NET 4 or above. You may need to add the following configuration in your 'web.config' file:
<system.web>
	<httpRuntime requestValidationMode="2.0"/>
</system.web>


Licensing
---------

FUSIONCHARTS:

Copyright (c) FusionCharts Technologies LLP
License Information at <http://www.fusioncharts.com/license>
