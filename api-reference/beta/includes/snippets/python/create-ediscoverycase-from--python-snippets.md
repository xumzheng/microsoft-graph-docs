---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EdiscoveryCase();
requestBody.setDisplayName('CONTOSO LITIGATION-005');

requestBody.setDescription('Project Bazooka');

requestBody.setExternalId('324516');



result = await client.security().cases().ediscoveryCases().post(requestBody);


```