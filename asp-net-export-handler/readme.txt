FusionCharts ASP.NET Export Handler
=====================================
The FusionCharts ASP.NET Export Handler contains all libraries and components required to build and run a .NET based 
web application that can be used as a server-side export handler for the export feature of FusionCharts.


Requirements
------------
- .NET Framework 3.5 or higher


Installation
------------
- Unzip the 'asp-net-export-handler.zip' in your IIS wwwroot folder (e.g. C:\inetpub\wwwroot)
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


SHARPVECTORS:

The SharpVectors software modified and redistributed herein is covered under the New BSD License (BSD),
and is subject to the following conditions from that license:

Copyright (c) 2010, SharpVectorGraphics
All rights reserved.

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the 
following conditions are met:

* Redistributions of source code must retain the above copyright notice, this list of conditions and the 
following disclaimer.

* Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the 
following disclaimer in the documentation and/or other materials provided with the distribution.

* Neither the name of SharpVectorGraphics nor the names of its contributors may be used to endorse or promote
 products derived from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES,
INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR 
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, 
WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE 
USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

SharpVectors source code is available from https://sharpvectors.codeplex.com/