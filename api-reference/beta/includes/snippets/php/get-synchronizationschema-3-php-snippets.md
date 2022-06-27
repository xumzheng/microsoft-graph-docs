---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new SchemaRequestBuilderGetRequestConfiguration();

$headers = [
	"Authorization" => "Bearer {Token}",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->servicePrincipalsById('servicePrincipal-id')->synchronization()->jobsById('synchronizationJob-id')->schema()->get($requestConfiguration);


```