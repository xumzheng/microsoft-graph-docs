---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = UpgradeRequestBuilderPostRequestConfiguration(
)


await client.teams_by_id('team-id').installedApps_by_id('teamsAppInstallation-id').upgrade.post()


```