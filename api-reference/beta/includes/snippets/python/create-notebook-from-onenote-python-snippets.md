---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Notebook();
requestBody.setDisplayName('My Private notebook');



requestResult = graphServiceClient.me().onenote().notebooks().post(requestBody);


```