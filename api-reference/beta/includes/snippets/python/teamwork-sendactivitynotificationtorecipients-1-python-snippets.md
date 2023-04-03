---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = SendActivityNotificationToRecipientsPostRequestBody();
topic = TeamworkActivityTopic();
topic.setSource(TeamworkActivityTopicSource('entityurl'));

topic.setValue('https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppId}');


requestBody.setTopic($topic);
requestBody.setActivityType('pendingFinanceApprovalRequests');

previewText = ItemBody();
previewText.setContent('Internal spending team has a pending finance approval requests');


requestBody.setPreviewText($previewText);
recipientsTeamworkNotificationRecipient1 = TeamworkNotificationRecipient();
recipientsTeamworkNotificationRecipient1.set@odatatype('microsoft.graph.aadUserNotificationRecipient');

additionalData = [
'userId' => '569363e2-4e49-4661-87f2-16f245c5d66a', 
];
recipientsTeamworkNotificationRecipient1.setAdditionalData(additionalData);



recipientsArray []= recipientsTeamworkNotificationRecipient1;
recipientsTeamworkNotificationRecipient2 = TeamworkNotificationRecipient();
recipientsTeamworkNotificationRecipient2.set@odatatype('microsoft.graph.aadUserNotificationRecipient');

additionalData = [
'userId' => 'ab88234e-0874-477c-9638-d144296ed04f', 
];
recipientsTeamworkNotificationRecipient2.setAdditionalData(additionalData);



recipientsArray []= recipientsTeamworkNotificationRecipient2;
recipientsTeamworkNotificationRecipient3 = TeamworkNotificationRecipient();
recipientsTeamworkNotificationRecipient3.set@odatatype('microsoft.graph.aadUserNotificationRecipient');

additionalData = [
'userId' => '01c64f53-69aa-42c7-9b7f-9f75195d6bfc', 
];
recipientsTeamworkNotificationRecipient3.setAdditionalData(additionalData);



recipientsArray []= recipientsTeamworkNotificationRecipient3;
requestBody.setRecipients(recipientsArray);


templateParametersKeyValuePair1 = KeyValuePair();
templateParametersKeyValuePair1.setName('pendingRequestCount');

templateParametersKeyValuePair1.setValue('5');


templateParametersArray []= templateParametersKeyValuePair1;
requestBody.setTemplateParameters(templateParametersArray);




awaitclient.teamwork().sendActivityNotificationToRecipients().post(requestBody);


```