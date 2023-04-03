---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = UserAccountInformation();
requestBody.setCountryCode('NO');



requestResult = graphServiceClient.me().profile().accountById('userAccountInformation-id').patch(requestBody);


```