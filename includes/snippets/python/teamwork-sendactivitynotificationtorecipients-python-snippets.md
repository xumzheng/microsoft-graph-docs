---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendActivityNotificationToRecipientsPostRequestBody()
topic = TeamworkActivityTopic()
topic.Source(TeamworkActivityTopicSource('entityurl'))

topic.value = 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/{teamsAppId}'


request_body.topic = topic
request_body.activityType = 'pendingFinanceApprovalRequests'

previewText = ItemBody()
previewText.content = 'Internal spending team has a pending finance approval requests'


request_body.previewText = previewText
recipientsTeamworkNotificationRecipient1 = TeamworkNotificationRecipient()
recipientsTeamworkNotificationRecipient1.@odatatype = 'microsoft.graph.aadUserNotificationRecipient'

additionalData = [
'userId' => '569363e2-4e49-4661-87f2-16f245c5d66a', 
];
recipientsTeamworkNotificationRecipient1.additionaldata(additionalData)



recipientsArray []= recipientsTeamworkNotificationRecipient1;
recipientsTeamworkNotificationRecipient2 = TeamworkNotificationRecipient()
recipientsTeamworkNotificationRecipient2.@odatatype = 'microsoft.graph.aadUserNotificationRecipient'

additionalData = [
'userId' => 'ab88234e-0874-477c-9638-d144296ed04f', 
];
recipientsTeamworkNotificationRecipient2.additionaldata(additionalData)



recipientsArray []= recipientsTeamworkNotificationRecipient2;
recipientsTeamworkNotificationRecipient3 = TeamworkNotificationRecipient()
recipientsTeamworkNotificationRecipient3.@odatatype = 'microsoft.graph.aadUserNotificationRecipient'

additionalData = [
'userId' => '01c64f53-69aa-42c7-9b7f-9f75195d6bfc', 
];
recipientsTeamworkNotificationRecipient3.additionaldata(additionalData)



recipientsArray []= recipientsTeamworkNotificationRecipient3;
request_body.recipients(recipientsArray)


templateParametersKeyValuePair1 = KeyValuePair()
templateParametersKeyValuePair1.name = 'pendingRequestCount'

templateParametersKeyValuePair1.value = '5'


templateParametersArray []= templateParametersKeyValuePair1;
request_body.templateparameters(templateParametersArray)





await client.teamwork.sendActivityNotificationToRecipients.post(request_body = request_body)


```