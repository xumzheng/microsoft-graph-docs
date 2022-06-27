---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CopyNotebookPostRequestBody();


$requestRequestBody->setGroupId('groupId-value');
$requestRequestBody->setRenameAs('renameAs-value');
$result =  $graphClient->me()->onenote()->notebooksById('notebook-id')->copyNotebook()->post($requestRequestBody);


```