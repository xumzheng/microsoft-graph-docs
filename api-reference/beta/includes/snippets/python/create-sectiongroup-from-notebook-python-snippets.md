---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = SectionGroup();
requestBody.setDisplayName('Section group name');



result = await client.me().onenote().notebooksById('notebook-id').sectionGroups().post(requestBody);


```