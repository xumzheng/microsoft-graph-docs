---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new RetentionEventType();
$requestBody.set@odatatype('#microsoft.graph.security.retentionEventType');

$requestBody.setDisplayName('String');

$requestBody.setDescription('String');

$createdBy = new IdentitySet();
$createdBy.set@odatatype('microsoft.graph.identitySet');


$requestBody.setCreatedBy($createdBy);


$requestResult = $graphServiceClient.security().triggerTypes().retentionEventTypes().post($requestBody);


```