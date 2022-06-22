---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ReferenceUpdateSchema();


$requestRequestBody->set@odata.id('https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}');
$result =  $graphClient->applicationsById('application-id')->connectorGroup()->ref()->put($requestRequestBody);


```