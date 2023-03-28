---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new LanguageProficiency();
$requestBody.setDisplayName('Norwegian Bokmål');

$requestBody.setTag('nb-NO');

$requestBody.setSpoken(new LanguageProficiencyLevel('nativeorbilingual'));

$requestBody.setWritten(new LanguageProficiencyLevel('nativeorbilingual'));

$requestBody.setReading(new LanguageProficiencyLevel('nativeorbilingual'));



$requestResult = $graphServiceClient.me().profile().languages().post($requestBody);


```