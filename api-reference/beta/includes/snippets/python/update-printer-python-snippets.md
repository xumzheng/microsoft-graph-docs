---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Printer()
request_body.setName('PrinterName')

location = PrinterLocation()
location.setLatitude(1.1)

location.setLongitude(2.2)

location.setAltitudeInMeters(3)


request_body.setLocation($location)


result = await client.print.printers_by_id('printer-id').patch(request_body)


```