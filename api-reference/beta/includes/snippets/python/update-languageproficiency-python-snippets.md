---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new LanguageProficiency();
$requestBody->setAllowedAudiences(new AllowedAudiences('organization'));



$requestResult = $graphServiceClient->me()->profile()->languagesById('languageProficiency-id')->patch($requestBody);


```