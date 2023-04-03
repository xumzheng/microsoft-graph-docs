---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = UnifiedGroupSource();
group = Group();
group.setMail('SecretGroup@contoso.com');


requestBody.setGroup($group);
requestBody.setIncludedSources(SourceType('mailbox, site'));



result = await client.compliance().ediscovery().casesById('case-id').custodiansById('custodian-id').unifiedGroupSources().post(requestBody);


```