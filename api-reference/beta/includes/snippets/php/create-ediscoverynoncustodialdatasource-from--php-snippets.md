---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EdiscoveryNoncustodialDataSource-idPostRequestBody();


$requestRequestBodyAdditionalData = [
	"@odata.id" => 'https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialDataSources/39333641443238353535383731453339',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->security()->cases()->ediscoveryCasesById('ediscoveryCase-id')->searchesById('ediscoverySearch-id')->noncustodialSourcesById('ediscoveryNoncustodialDataSource-id')->post($requestRequestBody);


```