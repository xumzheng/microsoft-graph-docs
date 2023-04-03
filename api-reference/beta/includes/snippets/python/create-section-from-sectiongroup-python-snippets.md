---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = OnenoteSection();
requestBody.setDisplayName('Section name');



result = awaitclient.me().onenote().sectionGroupsById('sectionGroup-id').sections().post(requestBody);


```