---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ChangePasswordPostRequestBody();
requestBody.setCurrentPassword('xWwvJ]6NMw+bWH-d');

requestBody.setNewPassword('0eM85N54wFxWwvJ]');



graphServiceClient.me().changePassword().post(requestBody);


```