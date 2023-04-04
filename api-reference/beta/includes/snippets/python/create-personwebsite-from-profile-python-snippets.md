---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = PersonWebsite();
request_body.setCategories(['football', ]);

request_body.setDisplayName('Lyn Damer');

request_body.setWebUrl('www.lyndamer.no');



result = await client.me.profile.websites.post(request_body);


```