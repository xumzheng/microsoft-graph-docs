---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TeamsAppInstallationRequestBuilderGetRequestConfiguration()

query_params = TeamsAppInstallationRequestBuilderGetQueryParameters()
query_params.select = ["consentedPermissionSet","id"]

request_config.queryParameters = query_params


result = await client.teamsby_id('team-id').installedAppsby_id('teamsAppInstallation-id').get(request_config)


```