---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = UserAccountInformation();
requestBody.setAllowedAudiences(AllowedAudiences('organization'));

requestBody.setCountryCode('NO');



requestResult = graphServiceClient.me().profile().account().post(requestBody);


```