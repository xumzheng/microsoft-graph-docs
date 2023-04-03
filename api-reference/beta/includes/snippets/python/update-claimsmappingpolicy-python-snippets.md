---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ClaimsMappingPolicy();
requestBody.setDisplayName('UpdateClaimsPolicy');



requestResult = graphServiceClient.policies().claimsMappingPoliciesById('claimsMappingPolicy-id').patch(requestBody);


```