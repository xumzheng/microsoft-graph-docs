---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new PersonCertification();
$requestBody->setIssuingAuthority('International Academy of Marketing Excellence');

$requestBody->setIssuingCompany('International Academy of Marketing Excellence');



$requestResult = $graphServiceClient->usersById('user-id')->profile()->certificationsById('personCertification-id')->patch($requestBody);


```