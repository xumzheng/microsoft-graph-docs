---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = WebAccount();
requestBody.setWebUrl('https://github.com/innocenty.popov');



result = awaitclient.me().profile().webAccountsById('webAccount-id').patch(requestBody);


```