---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = OutlineIconRequestBuilderGetRequestConfiguration(
)


result = await client.appCatalogs.teamsApps_by_id('teamsApp-id').appDefinitions_by_id('teamsAppDefinition-id').outlineIcon.get()


```