Junit-xml-to-MSTest-trx
=======================

Merge Chutzpah.3.2.2 JavaScript test report with MsTest report using CruiseControl.Net


_Generate Chutzpah.3.2.2 JavaScript test report_
>  ```xml
><exec>
>  <executable>C:\Program Files (x86)\Chutzpah.3.2.2\tools\chutzpah.console.exe</executable>
>  <buildArgs>C:\JavaScriptTests /testMode=JavaScript  /vsoutput /junit >C:\JavaScriptTestResults.xml</buildArgs>
>  <baseDirectory>C:\Projects\JavascriptTests</baseDirectory>
>  <buildTimeoutSeconds>0</buildTimeoutSeconds>
></exec>
>  ```

_Convert the test report to trx format using [MSXL.exe](http://www.microsoft.com/en-us/download/details.aspx?id=21714) and the transformation file [xslt_Junit_MsUnit](https://github.com/harip/Junit-xml-to-MSTest-trx/blob/master/xslt_Junit_MsUnit) included in this repo_
>  ```xml
><exec>
>  <executable>C:\msxsl.exe</executable>
>  <buildArgs>C:\JavaScriptTestResults.xml C:\xslt_Junit_MsUnit -o C:\JavaScriptTestResults.trx</buildArgs>
>  <baseDirectory>C:\</baseDirectory>
>  <buildTimeoutSeconds>0</buildTimeoutSeconds>
></exec>	
>  ```

_Merge the reports for a single test report_
>  ```xml
><publishers>
>	<merge>
>	  <files>
>	  	<file>C:\JavaScriptTestResults.trx</file>
>		  <file>C:\MSTestResults.trx</file>>		  
>	  </files>
>	</merge>
></publishers>	
>  ```
