---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendActivityNotificationToRecipientsPostRequestBody()
topic = TeamworkActivityTopic()
topic.setSource(TeamworkActivityTopicSource('entityurl'))

topic.setValue('https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/{teamsAppId}')


request_body.setTopic($topic)
request_body.setActivityType('pendingFinanceApprovalRequests')

previewText = ItemBody()
previewText.setContent('Internal spending team has a pending finance approval requests')


request_body.setPreviewText($previewText)
recipientsTeamworkNotificationRecipient1 = TeamworkNotificationRecipient()
recipientsTeamworkNotificationRecipient1.set@odatatype('microsoft.graph.aadUserNotificationRecipient')

additionalData = [
'userId' => '569363e2-4e49-4661-87f2-16f245c5d66a', 
];
recipientsTeamworkNotificationRecipient1.setAdditionalData(additionalData)



recipientsArray []= recipientsTeamworkNotificationRecipient1;
recipientsTeamworkNotificationRecipient2 = TeamworkNotificationRecipient()
recipientsTeamworkNotificationRecipient2.set@odatatype('microsoft.graph.aadUserNotificationRecipient')

additionalData = [
'userId' => 'ab88234e-0874-477c-9638-d144296ed04f', 
];
recipientsTeamworkNotificationRecipient2.setAdditionalData(additionalData)



recipientsArray []= recipientsTeamworkNotificationRecipient2;
recipientsTeamworkNotificationRecipient3 = TeamworkNotificationRecipient()
recipientsTeamworkNotificationRecipient3.set@odatatype('microsoft.graph.aadUserNotificationRecipient')

additionalData = [
'userId' => '01c64f53-69aa-42c7-9b7f-9f75195d6bfc', 
];
recipientsTeamworkNotificationRecipient3.setAdditionalData(additionalData)



recipientsArray []= recipientsTeamworkNotificationRecipient3;
request_body.setRecipients(recipientsArray)


templateParametersKeyValuePair1 = KeyValuePair()
templateParametersKeyValuePair1.setName('pendingRequestCount')

templateParametersKeyValuePair1.setValue('5')


templateParametersArray []= templateParametersKeyValuePair1;
request_body.setTemplateParameters(templateParametersArray)




await client.teamwork.sendActivityNotificationToRecipients.post(request_body)


```