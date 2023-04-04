---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = BusinessScenario();
request_body.set@odatatype('#microsoft.graph.businessScenario');

request_body.setDisplayName('Contoso Order Tracking');

request_body.setUniqueName('com.contoso.apps.ordertracking');



result = await client.solutions.businessScenarios.post(request_body);


```