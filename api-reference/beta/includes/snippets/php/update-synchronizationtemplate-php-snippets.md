---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SynchronizationTemplate-idPutRequestBody();


$requestRequestBodyAdditionalData = [
	"id" => 'Slack',
	"applicationId" => '{id}',
	"factoryTag" => 'CustomSCIM',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$requestConfiguration = new SynchronizationTemplateRequestBuilderPutRequestConfiguration();

$headers = [
"Authorization" => "Bearer <token>",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->applicationsById('application-id')->synchronization()->templatesById('synchronizationTemplate-id')->put($requestRequestBody, $requestConfiguration);


```