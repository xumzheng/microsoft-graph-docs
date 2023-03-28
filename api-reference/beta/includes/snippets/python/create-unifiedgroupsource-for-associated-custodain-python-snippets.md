---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new UnifiedGroupSource();
$group = new Group();
$group->setMail('SOCTeam@M365x809305.onmicrosoft.com');


$requestBody->setGroup($group);
$requestBody->setIncludedSources(new SourceType('mailbox, site'));



$requestResult = $graphServiceClient->security()->cases()->ediscoveryCasesById('ediscoveryCase-id')->custodiansById('ediscoveryCustodian-id')->unifiedGroupSources()->post($requestBody);


```