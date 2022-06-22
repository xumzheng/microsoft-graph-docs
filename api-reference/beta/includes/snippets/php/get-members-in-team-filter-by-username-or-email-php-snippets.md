---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new MembersRequestBuilderGetRequestConfiguration();

$queryParameters = new MembersRequestBuilderGetQueryParameters();
$queryParameters->filter = '(microsoft.graph.aadUserConversationMember/displayName%20eq%20\'Harry%20Johnson\'%20or%20microsoft.graph.aadUserConversationMember/email%20eq%20\'admin@M365x987948.OnMicrosoft.com\')';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->teamsById('team-id')->members()->get($requestConfiguration);


```