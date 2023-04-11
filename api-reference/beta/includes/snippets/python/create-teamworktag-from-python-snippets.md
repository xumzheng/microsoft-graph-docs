---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TeamworkTag()
request_body.displayName = 'Finance'

membersTeamworkTagMember1 = TeamworkTagMember()
membersTeamworkTagMember1.userId = '92f6952f-61ca-4a94-8910-508a240bc167'


membersArray []= membersTeamworkTagMember1;
membersTeamworkTagMember2 = TeamworkTagMember()
membersTeamworkTagMember2.userId = '085d800c-b86b-4bfc-a857-9371ad1caf29'


membersArray []= membersTeamworkTagMember2;
request_body.members(membersArray)




request_configuration = TagsRequestBuilderPostRequestConfiguration(
)


result = await client.teams_by_id('team-id').tags.post(request_body = request_body)


```