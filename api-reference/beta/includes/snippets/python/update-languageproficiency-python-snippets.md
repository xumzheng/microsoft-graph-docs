---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = LanguageProficiency();
requestBody.setAllowedAudiences(AllowedAudiences('organization'));



result = awaitclient.me().profile().languagesById('languageProficiency-id').patch(requestBody);


```