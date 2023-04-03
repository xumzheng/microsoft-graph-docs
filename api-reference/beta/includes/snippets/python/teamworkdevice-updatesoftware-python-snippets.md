---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = UpdateSoftwarePostRequestBody();
requestBody.setSoftwareType(TeamworkSoftwareType('teamsclient'));

requestBody.setSoftwareVersion('1.0.96.22');



await client.teamwork().devicesById('teamworkDevice-id').updateSoftware().post(requestBody);


```