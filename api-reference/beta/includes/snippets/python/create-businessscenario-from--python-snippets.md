---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BusinessScenario()
request_body.@odatatype = '#microsoft.graph.businessScenario'

request_body.displayName = 'Contoso Order Tracking'

request_body.uniqueName = 'com.contoso.apps.ordertracking'



request_configuration = BusinessScenariosRequestBuilderPostRequestConfiguration(
)


result = await client.solutions.businessScenarios.post(request_body = request_body)


```