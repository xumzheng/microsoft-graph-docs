---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = GetNotebookFromWebUrlPostRequestBody();
requestBody.setWebUrl('webUrl value');



result = awaitclient.me().onenote().notebooks().getNotebookFromWebUrl().post(requestBody);


```