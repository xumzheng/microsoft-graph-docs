---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new PrintTaskDefinition();
$requestBody->setDisplayName('Test TaskDefinitionName');

$createdBy = new AppIdentity();
$createdBy->setDisplayName('Requesting App Display Name');


$requestBody->setCreatedBy($createdBy);


$requestResult = $graphServiceClient->print()->taskDefinitions()->post($requestBody);


```