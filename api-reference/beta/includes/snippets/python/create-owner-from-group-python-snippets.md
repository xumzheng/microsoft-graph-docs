---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ReferenceCreate();
$requestBody->set@odataid('https://graph.microsoft.com/beta/users/{id}');



$graphServiceClient->groupsById('group-id')->owners()->ref()->post($requestBody);


```