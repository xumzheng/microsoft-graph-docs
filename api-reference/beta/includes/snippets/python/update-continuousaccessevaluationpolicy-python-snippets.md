---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ContinuousAccessEvaluationPolicy();
$requestBody->set@odatatype('#microsoft.graph.continuousAccessEvaluationPolicy');

$requestBody->setMigrate(true);



$requestResult = $graphServiceClient->identity()->continuousAccessEvaluationPolicy()->patch($requestBody);


```