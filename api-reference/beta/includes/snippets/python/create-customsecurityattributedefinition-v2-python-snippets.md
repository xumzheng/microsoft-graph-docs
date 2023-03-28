---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CustomSecurityAttributeDefinition();
$requestBody.setAttributeSet('Engineering');

$requestBody.setDescription('Active projects for user');

$requestBody.setIsCollection(true);

$requestBody.setIsSearchable(true);

$requestBody.setName('Project');

$requestBody.setStatus('Available');

$requestBody.setType('String');

$requestBody.setUsePreDefinedValuesOnly(true);



$requestResult = $graphServiceClient.directory().customSecurityAttributeDefinitions().post($requestBody);


```