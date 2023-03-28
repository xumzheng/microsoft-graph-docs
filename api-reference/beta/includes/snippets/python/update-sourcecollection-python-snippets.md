---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new SourceCollection();
$requestBody.setDisplayName('Quarterly Financials search');



$requestResult = $graphServiceClient.compliance().ediscovery().casesById('case-id').sourceCollectionsById('sourceCollection-id').patch($requestBody);


```