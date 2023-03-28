---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new UnifiedGroupSource();
$group = new Group();
$group.setMail('SecretGroup@contoso.com');


$requestBody.setGroup($group);
$requestBody.setIncludedSources(new SourceType('mailbox, site'));



$requestResult = $graphServiceClient.compliance().ediscovery().casesById('case-id').custodiansById('custodian-id').unifiedGroupSources().post($requestBody);


```