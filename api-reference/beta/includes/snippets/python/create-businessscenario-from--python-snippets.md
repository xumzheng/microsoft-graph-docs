---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = BusinessScenario();
requestBody.set@odatatype('#microsoft.graph.businessScenario');

requestBody.setDisplayName('Contoso Order Tracking');

requestBody.setUniqueName('com.contoso.apps.ordertracking');



result = await client.solutions().businessScenarios().post(requestBody);


```