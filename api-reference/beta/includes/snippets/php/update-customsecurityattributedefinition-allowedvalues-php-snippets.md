---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CustomSecurityAttributeDefinition();


$requestRequestBodyAdditionalData = [
	"allowedValues@delta" => [],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$requestConfiguration = new CustomSecurityAttributeDefinitionRequestBuilderPatchRequestConfiguration();

$headers = [
"OData-Version" => "4.01",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->directory()->customSecurityAttributeDefinitionsById('customSecurityAttributeDefinition-id')->patch($requestRequestBody, $requestConfiguration);


```