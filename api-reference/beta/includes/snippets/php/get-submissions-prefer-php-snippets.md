---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new SubmissionsRequestBuilderGetRequestConfiguration();

$headers = [
	"Prefer" => "include-unknown-enum-members",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->education()->classesById('educationClass-id')->assignmentsById('educationAssignment-id')->submissions()->get($requestConfiguration);


```