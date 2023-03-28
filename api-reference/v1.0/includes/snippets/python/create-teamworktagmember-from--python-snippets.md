---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new TeamworkTagMember();
$requestBody->setUserId('97f62344-57dc-409c-88ad-c4af14158ff5');



$requestResult = $graphServiceClient->teamsById('team-id')->tagsById('teamworkTag-id')->members()->post($requestBody);


```