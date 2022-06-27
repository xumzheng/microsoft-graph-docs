---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$result =  $graphClient->servicePrincipalsById('servicePrincipal-id')->synchronization()->jobsById('synchronizationJob-id')->schema()->directoriesById('directoryDefinition-id')->discover()->post();


```