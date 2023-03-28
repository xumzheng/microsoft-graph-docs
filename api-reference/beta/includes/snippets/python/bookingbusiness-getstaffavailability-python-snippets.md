---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new GetStaffAvailabilityPostRequestBody();
$requestBody->setStaffIds(['311a5454-08b2-4560-ba1c-f715e938cb79', ]);

$startDateTime = new DateTimeTimeZone();
$startDateTime->setDateTime('2022-01-25T00:00:00');

$startDateTime->setTimeZone('India Standard Time');


$requestBody->setStartDateTime($startDateTime);
$endDateTime = new DateTimeTimeZone();
$endDateTime->setDateTime('2022-01-26T17:00:00');

$endDateTime->setTimeZone('Pacific Standard Time');


$requestBody->setEndDateTime($endDateTime);


$requestResult = $graphServiceClient->bookingBusinessesById('bookingBusiness-id')->getStaffAvailability()->post($requestBody);


```