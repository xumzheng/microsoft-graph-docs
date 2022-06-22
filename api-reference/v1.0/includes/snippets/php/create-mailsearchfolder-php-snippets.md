---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new MailFolder();


$requestRequestBody->setDisplayName('Weekly digests');
$requestRequestBodyAdditionalData = [
	"@odata.type" => 'microsoft.graph.mailSearchFolder',
	"includeNestedFolders" => True,
	"sourceFolderIds" =>  [
'AQMkADYAAAIBDAAAAA==',	],
	"filterQuery" => 'contains(subject, \'weekly digest\')',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->me()->mailFoldersById('mailFolder-id')->childFolders()->post($requestRequestBody);


```