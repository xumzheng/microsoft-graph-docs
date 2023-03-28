---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ReviewSet();
$requestBody.setDisplayName('My Reviewset 3');



$requestResult = $graphServiceClient.compliance().ediscovery().casesById('case-id').reviewSets().post($requestBody);


```