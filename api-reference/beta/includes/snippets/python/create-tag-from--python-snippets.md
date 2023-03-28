---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Tag();
$requestBody->setDisplayName('Privileged');

$requestBody->setDescription('The document is privileged');

$additionalData = [
'parent@odata.bind' => 'https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/98fdad78bbce4519b75474bc150575c3', 
];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->compliance()->ediscovery()->casesById('case-id')->tags()->post($requestBody);


```