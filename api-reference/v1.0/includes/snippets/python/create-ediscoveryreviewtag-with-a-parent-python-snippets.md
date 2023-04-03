---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = EdiscoveryReviewTag();
requestBody.setDisplayName('My tag API');

requestBody.setDescription('Use Graph API to create tags');

requestBody.setChildSelectability(ChildSelectability('many'));

additionalData = [
'parent@odata.bind' => '', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.security().cases().ediscoveryCasesById('ediscoveryCase-id').tags().post(requestBody);


```