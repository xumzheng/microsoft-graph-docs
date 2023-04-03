---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = MarkUnreadPostRequestBody();
requestBody.setMessageIds(['MC172851', 'MC167983', ]);



result = awaitclient.admin().serviceAnnouncement().messages().markUnread().post(requestBody);


```