---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = LanguageProficiency();
requestBody.setDisplayName('Norwegian Bokmål');

requestBody.setTag('nb-NO');

requestBody.setSpoken(LanguageProficiencyLevel('nativeorbilingual'));

requestBody.setWritten(LanguageProficiencyLevel('nativeorbilingual'));

requestBody.setReading(LanguageProficiencyLevel('nativeorbilingual'));



result = awaitclient.me().profile().languages().post(requestBody);


```