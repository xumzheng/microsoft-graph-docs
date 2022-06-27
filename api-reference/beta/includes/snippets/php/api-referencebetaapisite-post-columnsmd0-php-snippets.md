---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ColumnDefinition();


$requestRequestBody->setDescription('test');
$requestRequestBody->setEnforceUniqueValues(False);
$requestRequestBody->setHidden(False);
$requestRequestBody->setIndexed(False);
$requestRequestBody->setName('Title');

$text = new TextColumn();
$requestRequestBody->setText($text);


$text->setAllowMultipleLines(False);
$text->setAppendChangesToExistingText(False);
$text->setLinesForEditing(0);
$text->setMaxLength(255);

$result =  $graphClient->sitesById('site-id')->columns()->post($requestRequestBody);


```