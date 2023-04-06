---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Printer()
location = PrinterLocation()
location.setLatitude(1.1)

location.setLongitude(2.2)

location.setAltitudeInMeters(3)


request_body.setLocation($location)
additionalData = [
'name' => 'PrinterName', 
];
request_body.setAdditionalData(additionalData)



request_config = PrinterRequestBuilderPatchRequestConfiguration(
request_config = PrinterRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.print.printers_by_id('printer-id').patch(request_body, headers=)


```