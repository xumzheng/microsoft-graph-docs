---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Group();
request_body.setDescription('Marketing department folks');

request_body.setDisplayName('Marketing department');

request_body.setGroupTypes(['Unified', 'DynamicMembership', ]);

request_body.setMailEnabled(true);

request_body.setMailNickname('marketing');

request_body.setSecurityEnabled(false);

request_body.setMembershipRule('user.department -eq \"Marketing\"');

request_body.setMembershipRuleProcessingState('on');



result = await client.groups().post(request_body);


```