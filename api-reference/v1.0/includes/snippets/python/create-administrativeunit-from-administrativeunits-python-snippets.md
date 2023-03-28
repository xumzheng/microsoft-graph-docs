---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AdministrativeUnit();
$requestBody.setDisplayName('Seattle District Technical Schools');

$requestBody.setDescription('Seattle district technical schools administration');

$requestBody.setVisibility('HiddenMembership');



$requestResult = $graphServiceClient.directory().administrativeUnits().post($requestBody);


```