---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new List();


$requestRequestBody->setDisplayName('Books');
$columnsArray = [];

$columnscolumns1 = new ColumnDefinition();

$columnscolumns1->setName('Author');

$text = new TextColumn();
$columnscolumns1->setText($text);




$columnsArray []= $columnscolumns1;

$columnscolumns2 = new ColumnDefinition();

$columnscolumns2->setName('PageCount');

$number = new NumberColumn();
$columnscolumns2->setNumber($number);




$columnsArray []= $columnscolumns2;
$requestRequestBody->setColumns($columnsArray);

$list = new ListInfo();
$requestRequestBody->setList($list);


$list->setTemplate('genericList');

$result =  $graphClient->sitesById('site-id')->lists()->post($requestRequestBody);


```