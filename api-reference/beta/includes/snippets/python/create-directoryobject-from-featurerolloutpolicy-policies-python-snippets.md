---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ReferenceCreate();
request_body.set@odataid(' https://graph.microsoft.com/beta/directoryObjects/2441b489-4f12-4882-b039-8f6006bd66da');



await client.policies.featureRolloutPoliciesById('featureRolloutPolicy-id').appliesTo.ref.post(request_body);


```