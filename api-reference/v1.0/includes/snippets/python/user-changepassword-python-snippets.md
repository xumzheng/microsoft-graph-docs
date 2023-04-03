---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ChangePasswordPostRequestBody();
requestBody.setCurrentPassword('xWwvJ]6NMw+bWH-d');

requestBody.setNewPassword('0eM85N54wFxWwvJ]');



await client.me().changePassword().post(requestBody);


```