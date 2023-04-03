---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AuthenticationStrengthPolicy();
requestBody.set@odatatype('#microsoft.graph.authenticationStrengthPolicy');

requestBody.setDisplayName('FIDO2 only');

requestBody.setDescription('An auth strength allowing only FIDO2 security keys.');



requestResult = graphServiceClient.policies().authenticationStrengthPoliciesById('authenticationStrengthPolicy-id').patch(requestBody);


```