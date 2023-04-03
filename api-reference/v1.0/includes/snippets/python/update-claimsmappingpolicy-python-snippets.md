---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ClaimsMappingPolicy();
requestBody.setDisplayName('UpdateClaimsPolicy');



result = awaitclient.policies().claimsMappingPoliciesById('claimsMappingPolicy-id').patch(requestBody);


```