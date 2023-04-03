---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = BusinessScenario();
requestBody.set@odatatype('#microsoft.graph.businessScenario');

requestBody.setDisplayName('Contoso Order Tracking');

requestBody.setUniqueName('com.contoso.apps.ordertracking');



requestResult = graphServiceClient.solutions().businessScenarios().post(requestBody);


```