Junit-xml-to-MSTest-trx
=======================

Merge Chutzpah.3.2.2 JavaScript test report with MsTest report using CruiseControl.Net


_Generate Chutzpah.3.2.2 JavaScript test report_
>  ```xml
><exec>
>  <executable>C:\Program Files (x86)\Chutzpah.3.2.2\tools\chutzpah.console.exe</executable>
>  <buildArgs>C:\Projects\Tntp\Trunk\Tntp.JavascriptTests\JavaScriptTests /testMode=JavaScript  /vsoutput /junit >C:\Projects\Tntp\UnitTestResults\JavaScriptTestResults.xml</buildArgs>
>  <baseDirectory>C:\Projects\Tntp\Trunk\Tntp.JavascriptTests</baseDirectory>
>  <buildTimeoutSeconds>0</buildTimeoutSeconds>
></exec>
>  ```
