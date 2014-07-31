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

_Convert the test report to trx format using http://www.microsoft.com/en-us/download/details.aspx?id=21714_
>  ```xml
><exec>
>  <executable>C:\Program Files (x86)\Chutzpah.3.2.2\tools\chutzpah.console.exe</executable>
>  <buildArgs>C:\JavaScriptTests /testMode=JavaScript  /vsoutput /junit >C:\JavaScriptTestResults.xml</buildArgs>
>  <baseDirectory>C:\Projects\JavascriptTests</baseDirectory>
>  <buildTimeoutSeconds>0</buildTimeoutSeconds>
></exec>
>  ``
