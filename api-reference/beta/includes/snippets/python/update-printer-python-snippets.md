---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Printer();
requestBody.setName('PrinterName');

location = PrinterLocation();
location.setLatitude(1.1);

location.setLongitude(2.2);

location.setAltitudeInMeters(3);


requestBody.setLocation($location);


result = await client.print().printersById('printer-id').patch(requestBody);


```