---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = LanguageProficiency();
requestBody.setAllowedAudiences(AllowedAudiences('organization'));



requestResult = graphServiceClient.me().profile().languagesById('languageProficiency-id').patch(requestBody);


```