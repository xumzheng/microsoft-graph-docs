---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = SectionGroup();
requestBody.setDisplayName('Section group name');



requestResult = graphServiceClient.me().onenote().notebooksById('notebook-id').sectionGroups().post(requestBody);


```