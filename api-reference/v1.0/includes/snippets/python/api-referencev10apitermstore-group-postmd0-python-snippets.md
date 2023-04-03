---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Group();
requestBody.setDisplayName('myGroup');



result = await client.sitesById('site-id').termStore().groups().post(requestBody);


```