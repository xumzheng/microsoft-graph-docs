---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AddActivitiesPostRequestBody();
$activitiesExternalActivity1 = new ExternalActivity();
$activitiesExternalActivity1->set@odatatype('#microsoft.graph.externalConnectors.externalActivity');

$activitiesExternalActivity1->setType(new ExternalActivityType('string'));

$activitiesExternalActivity1->setStartDateTime(new DateTime('String (timestamp)'));


$activitiesArray []= $activitiesExternalActivity1;
$requestBody->setActivities($activitiesArray);




$requestResult = $graphServiceClient->connectionsById('externalConnection-id')->itemsById('externalItem-id')->externalConnectorsAddActivities()->post($requestBody);


```