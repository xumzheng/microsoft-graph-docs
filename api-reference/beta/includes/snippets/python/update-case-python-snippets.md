---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Case();
$requestBody.setDisplayName('My Case 1 - Renamed');

$requestBody.setDescription('Updated description');

$requestBody.setExternalId('Updated externalId');



$requestResult = $graphServiceClient.compliance().ediscovery().casesById('case-id').patch($requestBody);


```