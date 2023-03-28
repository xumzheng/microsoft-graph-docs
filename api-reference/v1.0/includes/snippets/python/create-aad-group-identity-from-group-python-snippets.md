---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Identity();
$requestBody.setId('e5477431-1038-484e-bf69-1dfedb97a110');

$requestBody.setType(new IdentityType('group'));



$requestResult = $graphServiceClient.external().connectionsById('externalConnection-id').groupsById('externalGroup-id').members().post($requestBody);


```