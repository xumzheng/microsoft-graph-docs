---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = TeamworkTag();
requestBody.setDisplayName('Finance');

membersTeamworkTagMember1 = TeamworkTagMember();
membersTeamworkTagMember1.setUserId('92f6952f-61ca-4a94-8910-508a240bc167');


membersArray []= membersTeamworkTagMember1;
membersTeamworkTagMember2 = TeamworkTagMember();
membersTeamworkTagMember2.setUserId('085d800c-b86b-4bfc-a857-9371ad1caf29');


membersArray []= membersTeamworkTagMember2;
requestBody.setMembers(membersArray);




result = awaitclient.teamsById('team-id').tags().post(requestBody);


```