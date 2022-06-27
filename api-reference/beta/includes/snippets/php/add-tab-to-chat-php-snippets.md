---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TeamsTab();


$requestRequestBody->setDisplayName('My Contoso Tab');

$configuration = new TeamsTabConfiguration();
$requestRequestBody->setConfiguration($configuration);


$configuration->setEntityId('2DCA2E6C7A10415CAF6B8AB6661B3154');
$configuration->setContentUrl('https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView');
$configuration->setWebsiteUrl('https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154');
$configuration->setRemoveUrl('https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab');

$requestRequestBodyAdditionalData = [
"teamsApp@odata.bind" => 'https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->chatsById('chat-id')->tabs()->post($requestRequestBody);


```