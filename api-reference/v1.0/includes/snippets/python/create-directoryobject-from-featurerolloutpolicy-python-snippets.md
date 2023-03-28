---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ReferenceCreate();
$requestBody.set@odataid('https://graph.microsoft.com/v1.0/directoryObjects/2441b489-4f12-4882-b039-8f6006bd66da');



$graphServiceClient.policies().featureRolloutPoliciesById('featureRolloutPolicy-id').appliesTo().ref().post($requestBody);


```