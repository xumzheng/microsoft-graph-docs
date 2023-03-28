---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Identity();
$requestBody.setId('1431b9c38ee647f6a');

$requestBody.setType(new IdentityType('externalgroup'));



$requestResult = $graphServiceClient.external().connectionsById('externalConnection-id').groupsById('externalGroup-id').members().post($requestBody);


```