---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new UserSource();
$requestBody->setEmail('admin@M365x809305.onmicrosoft.com');

$requestBody->setIncludedSources(new SourceType('mailbox, site'));



$requestResult = $graphServiceClient->security()->cases()->ediscoveryCasesById('ediscoveryCase-id')->custodiansById('ediscoveryCustodian-id')->userSources()->post($requestBody);


```