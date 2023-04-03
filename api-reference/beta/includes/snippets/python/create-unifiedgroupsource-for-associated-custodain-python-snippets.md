---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = UnifiedGroupSource();
group = Group();
group.setMail('SOCTeam@M365x809305.onmicrosoft.com');


requestBody.setGroup($group);
requestBody.setIncludedSources(SourceType('mailbox, site'));



result = await client.security().cases().ediscoveryCasesById('ediscoveryCase-id').custodiansById('ediscoveryCustodian-id').unifiedGroupSources().post(requestBody);


```