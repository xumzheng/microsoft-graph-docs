---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ItemPatent();


$requestRequestBody->setDescription('Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.');
$requestRequestBody->setDisplayName('Inferring User Intent through browsing behaviors');
$requestRequestBody->setIsPending(True);
$requestRequestBody->setNumber('USPTO-3954432633');
$requestRequestBody->setWebUrl('https://patents.gov/3954432633');
$result =  $graphClient->me()->profile()->patents()->post($requestRequestBody);


```