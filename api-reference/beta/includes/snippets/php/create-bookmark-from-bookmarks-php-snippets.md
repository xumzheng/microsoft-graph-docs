---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Bookmark();


$requestRequestBody->setDisplayName('Contoso Install Site');
$requestRequestBody->setWebUrl('http://www.contoso.com/');
$requestRequestBody->setDescription('Try or buy Contoso for Home or Business and view product information');

$keywords = new AnswerKeyword();
$requestRequestBody->setKeywords($keywords);


$keywords->setKeywords(['Contoso','install',]);
$keywords->setReservedKeywords(['Contoso',]);
$keywords->setMatchSimilarKeywords(True);

$requestRequestBody->setAvailabilityStartDateTime(null);
$requestRequestBody->setAvailabilityEndDateTime(null);
$platformsArray = [];
'windows',$platformsArray []= $platformsplatforms1;
$requestRequestBody->setPlatforms($platformsArray);
$targetedVariationsArray = [];

$targetedVariationstargetedVariations1 = new AnswerVariant();

$targetedVariationstargetedVariations1->setLanguageTag('es-es');
$targetedVariationstargetedVariations1->setDisplayName('Sitio de instalación Contoso');
$targetedVariationstargetedVariations1->setDescription('Pruebe o compre Contoso hogar o negocios y vea la información del producto');

$targetedVariationsArray []= $targetedVariationstargetedVariations1;
$requestRequestBody->setTargetedVariations($targetedVariationsArray);
$requestRequestBody->setState(new AnswerState('published'));
$result =  $graphClient->search()->bookmarks()->post($requestRequestBody);


```