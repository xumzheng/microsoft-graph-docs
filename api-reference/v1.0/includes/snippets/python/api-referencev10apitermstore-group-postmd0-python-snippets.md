---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Group();
requestBody.setDisplayName('myGroup');



result = awaitclient.sitesById('site-id').termStore().groups().post(requestBody);


```