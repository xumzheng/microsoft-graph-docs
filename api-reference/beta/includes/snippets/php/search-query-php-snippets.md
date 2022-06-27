---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new RequestsRequestBody();


$requestsArray = [];

$requestsrequests1 = new SearchRequest();

$requestsrequests1AdditionalData = [
	"entityTypes" => ['externalItem',],
"contentSources" => ['/external/connections/connectionfriendlyname',],
"from" => 0,
"size" => 25,
"fields" => ['title','description',],
];
$requestsrequests1->setAdditionalData($requestsrequests1AdditionalData);

$requestsArray []= $requestsrequests1;
$requestRequestBody->setRequests($requestsArray);
$result =  $graphClient->search()->query()->post($requestRequestBody);


```