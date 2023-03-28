---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ReviewSetQuery();
$requestBody.setDisplayName('My Query 1 - Renamed');



$requestResult = $graphServiceClient.compliance().ediscovery().casesById('case-id').reviewSetsById('reviewSet-id').queriesById('reviewSetQuery-id').patch($requestBody);


```