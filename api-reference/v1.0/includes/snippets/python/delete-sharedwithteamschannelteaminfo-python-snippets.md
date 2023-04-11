---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = SharedWithChannelTeamInfoRequestBuilderDeleteRequestConfiguration(
)


await client.teams_by_id('team-id').channels_by_id('channel-id').sharedWithTeams_by_id('sharedWithChannelTeamInfo-id').delete()


```