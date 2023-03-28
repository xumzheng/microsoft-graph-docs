---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Printer();
$requestBody.setName('PrinterName');

$location = new PrinterLocation();
$location.setLatitude(1.1);

$location.setLongitude(2.2);

$location.setAltitudeInMeters(3);


$requestBody.setLocation($location);


$requestResult = $graphServiceClient.print().printersById('printer-id').patch($requestBody);


```