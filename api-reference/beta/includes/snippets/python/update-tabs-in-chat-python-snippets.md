---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = TeamsTab();
requestBody.setDisplayName('My Contoso Tab - updated again');



result = awaitclient.chatsById('chat-id').tabsById('teamsTab-id').patch(requestBody);


```