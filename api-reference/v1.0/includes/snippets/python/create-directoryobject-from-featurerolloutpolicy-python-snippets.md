---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceCreate()
request_body.@odataid = 'https://graph.microsoft.com/v1.0/directoryObjects/2441b489-4f12-4882-b039-8f6006bd66da'



request_configuration = RefRequestBuilderPostRequestConfiguration(
)


await client.policies.featureRolloutPolicies_by_id('featureRolloutPolicy-id').appliesTo.ref.post(request_body = request_body)


```