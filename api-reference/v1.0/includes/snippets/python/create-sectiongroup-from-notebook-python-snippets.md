---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = SectionGroup();
requestBody.setDisplayName('Section group name');



result = awaitclient.me().onenote().notebooksById('notebook-id').sectionGroups().post(requestBody);


```