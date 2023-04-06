---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = InstalledAppsRequestBuilderGetRequestConfiguration(
request_configuration = InstalledAppsRequestBuilderGetRequestConfiguration(query_params=query_params = InstalledAppsRequestBuilderGetQueryParameters()
query_params['select'] = ["consentedPermissionSet","id"]

)
query_params = InstalledAppsRequestBuilderGetQueryParameters()
query_params['select'] = ["consentedPermissionSet","id"]

)


result = await client.teams_by_id('team-id').installedApps.get(request_configuration)


```