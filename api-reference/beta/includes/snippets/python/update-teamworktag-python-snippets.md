---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TeamworkTag()
request_body.setDisplayName('Finance')


request_config = TeamworkTagRequestBuilderPatchRequestConfiguration(
request_config = TeamworkTagRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.teams_by_id('team-id').tags_by_id('teamworkTag-id').patch(request_body, headers=)


```