---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ExternalConnection();
$requestBody.setId('contosohr');

$requestBody.setName('Contoso HR');

$requestBody.setDescription('Connection to index Contoso HR system');



$requestResult = $graphServiceClient.external().connections().post($requestBody);


```