---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = LanguageProficiency();
requestBody.setDisplayName('Norwegian Bokmål');

requestBody.setTag('nb-NO');

requestBody.setSpoken(LanguageProficiencyLevel('nativeorbilingual'));

requestBody.setWritten(LanguageProficiencyLevel('nativeorbilingual'));

requestBody.setReading(LanguageProficiencyLevel('nativeorbilingual'));



result = await client.me().profile().languages().post(requestBody);


```