---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = LanguageProficiency();
requestBody.setAllowedAudiences(AllowedAudiences('organization'));



result = await client.me().profile().languagesById('languageProficiency-id').patch(requestBody);


```