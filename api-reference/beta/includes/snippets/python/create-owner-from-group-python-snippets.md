---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ReferenceCreate();
request_body.set@odataid('https://graph.microsoft.com/beta/users/{id}');



await client.groupsById('group-id').owners().ref().post(request_body);


```