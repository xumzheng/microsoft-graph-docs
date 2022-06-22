---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new List();


$requestRequestBody->setDisplayName('Books');
$columnsArray = [];

$columns1 = new ColumnDefinition();

$columns1->setName('Author');

$text = new TextColumn();
$columns1->setText($text);




$columnsArray []= $columns1;

$columns2 = new ColumnDefinition();

$columns2->setName('PageCount');

$number = new NumberColumn();
$columns2->setNumber($number);




$columnsArray []= $columns2;
$requestRequestBody->setColumns($columnsArray);

$list = new ListInfo();
$requestRequestBody->setList($list);


$list->setTemplate('genericList');

$result =  $graphClient->sitesById('site-id')->lists()->post($requestRequestBody);


```