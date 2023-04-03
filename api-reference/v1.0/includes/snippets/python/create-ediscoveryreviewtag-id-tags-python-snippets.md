---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EdiscoveryReviewTag();
requestBody.setDisplayName('My tag API');

requestBody.setDescription('Use Graph API to create tags');

requestBody.setChildSelectability(ChildSelectability('many'));



result = await client.security().cases().ediscoveryCasesById('ediscoveryCase-id').tags().post(requestBody);


```