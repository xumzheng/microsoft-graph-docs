---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendActivityNotificationPostRequestBody()
topic = TeamworkActivityTopic()
topic.Source(TeamworkActivityTopicSource('text'))

topic.value = 'Deployment Approvals Channel'

topic.webUrl = 'https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000'


request_body.topic = topic
request_body.activityType = 'deploymentApprovalRequired'

preview_text = ItemBody()
previewText.content = 'New deployment requires your approval'


request_body.preview_text = previewText
recipient = TeamworkNotificationRecipient()
recipient.@odatatype = 'microsoft.graph.aadUserNotificationRecipient'

additionalData = [
'userId' => '569363e2-4e49-4661-87f2-16f245c5d66a', 
];
recipient.additionaldata(additionalData)



request_body.recipient = recipient
template_parameters_key_value_pair1 = KeyValuePair()
templateParametersKeyValuePair1.name = 'deploymentId'

templateParametersKeyValuePair1.value = '6788662'


templateParametersArray []= templateParametersKeyValuePair1;
request_body.templateparameters(templateParametersArray)





await client.teams_by_id('team-id').sendActivityNotification.post(request_body = request_body)


```