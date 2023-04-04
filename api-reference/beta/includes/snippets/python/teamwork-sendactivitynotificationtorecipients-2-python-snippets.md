---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = SendActivityNotificationToRecipientsPostRequestBody();
topic = TeamworkActivityTopic();
topic.setSource(TeamworkActivityTopicSource('text'));

topic.setValue('Deployment Approvals Channel');

topic.setWebUrl('https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000');


request_body.setTopic($topic);
request_body.setActivityType('deploymentApprovalRequired');

previewText = ItemBody();
previewText.setContent('New deployment requires your approval');


request_body.setPreviewText($previewText);
templateParametersKeyValuePair1 = KeyValuePair();
templateParametersKeyValuePair1.setName('deploymentId');

templateParametersKeyValuePair1.setValue('6788662');


templateParametersArray []= templateParametersKeyValuePair1;
request_body.setTemplateParameters(templateParametersArray);


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
request_body.setRecipients(recipientsArray);




await client.teamwork.sendActivityNotificationToRecipients.post(request_body);


```