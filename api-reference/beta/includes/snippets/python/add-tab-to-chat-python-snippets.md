---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = TeamsTab();
request_body.setDisplayName('My Contoso Tab');

configuration = TeamsTabConfiguration();
configuration.setEntityId('2DCA2E6C7A10415CAF6B8AB6661B3154');

configuration.setContentUrl('https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView');

configuration.setWebsiteUrl('https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154');

configuration.setRemoveUrl('https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab');


request_body.setConfiguration($configuration);
additionalData = [
'teamsApp@odata.bind' => 'https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8', 
];
request_body.setAdditionalData(additionalData);




result = await client.chatsById('chat-id').tabs().post(request_body);


```