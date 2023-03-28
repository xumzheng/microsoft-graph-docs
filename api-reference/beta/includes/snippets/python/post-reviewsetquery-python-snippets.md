---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ReviewSetQuery();
$requestBody.setDisplayName('My Query 1');

$requestBody.setQuery('(subject:\"Quarterly Financials\")');



$requestResult = $graphServiceClient.compliance().ediscovery().casesById('case-id').reviewSetsById('reviewSet-id').queries().post($requestBody);


```