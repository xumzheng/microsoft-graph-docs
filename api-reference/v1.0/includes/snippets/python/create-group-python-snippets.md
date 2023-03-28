---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Group();
$requestBody.setDescription('Self help community for library');

$requestBody.setDisplayName('Library Assist');

$requestBody.setGroupTypes(['Unified', ]);

$requestBody.setMailEnabled(true);

$requestBody.setMailNickname('library');

$requestBody.setSecurityEnabled(false);



$requestResult = $graphServiceClient.groups().post($requestBody);


```