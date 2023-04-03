---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = OnenoteSection();
requestBody.setDisplayName('Section name');



requestResult = graphServiceClient.me().onenote().notebooksById('notebook-id').sections().post(requestBody);


```