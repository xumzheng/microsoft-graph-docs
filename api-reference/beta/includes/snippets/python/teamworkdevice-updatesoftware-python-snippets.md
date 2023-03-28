---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new UpdateSoftwarePostRequestBody();
$requestBody.setSoftwareType(new TeamworkSoftwareType('teamsclient'));

$requestBody.setSoftwareVersion('1.0.96.22');



$graphServiceClient.teamwork().devicesById('teamworkDevice-id').updateSoftware().post($requestBody);


```