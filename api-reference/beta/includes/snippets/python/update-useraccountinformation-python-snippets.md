---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UserAccountInformation();
requestBody.setCountryCode('NO');



result = awaitclient.me().profile().accountById('userAccountInformation-id').patch(requestBody);


```