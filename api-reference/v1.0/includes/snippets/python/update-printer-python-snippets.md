---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Printer()
location = PrinterLocation()
location.latitude = 1.1

location.longitude = 2.2

location.altitudeInMeters = 3


request_body.location = location
additionalData = [
'name' => 'PrinterName', 
];
request_body.additionaldata(additionalData)





result = await client.print.printers_by_id('printer-id').patch(request_body = request_body)


```