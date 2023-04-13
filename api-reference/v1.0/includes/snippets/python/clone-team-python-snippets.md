---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ClonePostRequestBody()
request_body.displayName = 'Library Assist'

request_body.description = 'Self help community for library'

request_body.mailNickname = 'libassist'

request_body.PartsToClone(ClonableTeamParts('apps,tabs,settings,channels,members'))

request_body.Visibility(TeamVisibilityType('public'))




await client.teams_by_id('team-id').clone.post(request_body = request_body)


```