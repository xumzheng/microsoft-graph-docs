---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Event();
$location = new Location();
$location.setDisplayName('Conf Room 2');


$requestBody.setLocation($location);


$requestResult = $graphServiceClient.groupsById('group-id').calendar().eventsById('event-id').patch($requestBody);


```