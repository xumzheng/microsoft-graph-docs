---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = WebAccount();
requestBody.setWebUrl('https://github.com/innocenty.popov');



result = await client.me().profile().webAccountsById('webAccount-id').patch(requestBody);


```