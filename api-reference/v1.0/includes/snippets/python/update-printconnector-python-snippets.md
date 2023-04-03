---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PrintConnector();
requestBody.setDisplayName('ConnectorName');

requestBody.setFullyQualifiedDomainName('CONNECTOR-MACHINE');

requestBody.setOperatingSystem('Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555');

requestBody.setAppVersion('0.19.7338.23496');

location = PrinterLocation();
location.setLatitude(1.1);

location.setLongitude(2.2);

location.setAltitudeInMeters(3);


requestBody.setLocation($location);


result = awaitclient.print().connectorsById('printConnector-id').patch(requestBody);


```