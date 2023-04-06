---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = LocalizationsRequestBuilderGetRequestConfiguration(
request_config = LocalizationsRequestBuilderGetRequestConfiguration(query_params=params['filter'] = "languageTag eq 'en-us'"
)


result = await client.solutions.businessScenarios_by_id('businessScenario-id').planner.planConfiguration.localizations.get(request_config, headers=request_config)


```