---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = User();
onPremisesExtensionAttributes = OnPremisesExtensionAttributes();
onPremisesExtensionAttributes.setExtensionAttribute1('skypeId.adeleVance');

OnPremisesExtensionAttributes.setExtensionAttribute13(null);


requestBody.setOnPremisesExtensionAttributes($onPremisesExtensionAttributes);


result = awaitclient.usersById('user-id').patch(requestBody);


```