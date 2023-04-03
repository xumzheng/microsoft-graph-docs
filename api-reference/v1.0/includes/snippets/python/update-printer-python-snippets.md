---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Printer();
location = PrinterLocation();
location.setLatitude(1.1);

location.setLongitude(2.2);

location.setAltitudeInMeters(3);


requestBody.setLocation($location);
additionalData = [
'name' => 'PrinterName', 
];
requestBody.setAdditionalData(additionalData);




result = await client.print().printersById('printer-id').patch(requestBody);


```