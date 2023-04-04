---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = EdiscoveryReviewTag()
request_body.setDisplayName('My tag API')

request_body.setDescription('Use Graph API to create tags')

request_body.setChildSelectability(ChildSelectability('many'))

additionalData = [
'parent@odata.bind' => '', 
];
request_body.setAdditionalData(additionalData)




result = await client.security.cases.ediscoveryCasesById('ediscoveryCase-id').tags.post(request_body)


```