---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = EdiscoveryCase();
requestBody.setDisplayName('CONTOSO LITIGATION-005');

requestBody.setDescription('Project Bazooka');

requestBody.setExternalId('324516');



requestResult = graphServiceClient.security().cases().ediscoveryCases().post(requestBody);


```