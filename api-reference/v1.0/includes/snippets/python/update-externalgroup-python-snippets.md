---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ExternalGroup();
$requestBody->setDisplayName('Contoso Marketing');

$requestBody->setDescription('The product marketing team');



$requestResult = $graphServiceClient->external()->connectionsById('externalConnection-id')->groupsById('externalGroup-id')->patch($requestBody);


```