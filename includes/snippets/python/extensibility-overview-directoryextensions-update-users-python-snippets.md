---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new User();
$additionalData = [
'extension_b7d8e648520f41d3b9c0fdeb91768a0a_permanent_pensionable' => 		null,
'extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker' => 'E4', 
];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->usersById('user-id')->patch($requestBody);


```