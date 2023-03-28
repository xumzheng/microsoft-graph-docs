---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new OnlineMeeting();
$requestBody.setStartDateTime(new DateTime('2020-09-09T14:33:30.8546353-07:00'));

$requestBody.setEndDateTime(new DateTime('2020-09-09T15:03:30.8566356-07:00'));

$requestBody.setSubject('Patch Meeting Subject');



$requestResult = $graphServiceClient.me().onlineMeetingsById('onlineMeeting-id').patch($requestBody);


```