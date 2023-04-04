---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = UnifiedGroupSource();
group = Group();
group.setMail('SOCTeam@M365x809305.onmicrosoft.com');


request_body.setGroup($group);
request_body.setIncludedSources(SourceType('mailbox, site'));



result = await client.security.cases.ediscoveryCasesById('ediscoveryCase-id').custodiansById('ediscoveryCustodian-id').unifiedGroupSources.post(request_body);


```