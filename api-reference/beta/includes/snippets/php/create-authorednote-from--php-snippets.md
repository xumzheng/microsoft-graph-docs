---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AuthoredNote();



$content = new ItemBody();
$requestRequestBody->setContent($content);


$content->setContent('Please take a look at the files tagged with follow up');
$content->setContentType(new BodyType('text'));

$result =  $graphClient->privacy()->subjectRightsRequestsById('subjectRightsRequest-id')->notes()->post($requestRequestBody);


```