---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = RunsRequestBuilderGetRequestConfiguration(
)


result = await client.security.attackSimulation.simulationAutomations_by_id('simulationAutomation-id').runs.get()


```