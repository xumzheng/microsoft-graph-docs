---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AlertRule()
request_body.id = '215c55cc-b1c9-4d36-a870-be5778101714'

request_body.displayName = 'Azure network connection failure impacting Cloud PCs'

request_body.Severity(RuleSeverityType('informational'))

request_body.isSystemRule = true

request_body.description = 'Azure network connection checks have failed and is potentially impacting existing Cloud PCs and blocking the provisioning of new Cloud PCs'

request_body.enabled = true

request_body.AlertRuleTemplate(AlertRuleTemplate('cloudpconpremisenetworkconnectioncheckscenario'))

threshold = RuleThreshold()
threshold.Aggregation(AggregationType('count'))

threshold.Operator(OperatorType('greaterorequal'))

threshold.target = 90


request_body.threshold = threshold
notificationChannelsNotificationChannel1 = NotificationChannel()
notificationChannelsNotificationChannel1.NotificationChannelType(NotificationChannelType('portal'))

notificationChannelsNotificationChannel1.Receivers(['', ])

notificationChannelsNotificationChannel1.NotificationReceivers([])


notificationChannelsArray []= notificationChannelsNotificationChannel1;
notificationChannelsNotificationChannel2 = NotificationChannel()
notificationChannelsNotificationChannel2.NotificationChannelType(NotificationChannelType('email'))

notificationChannelsNotificationChannel2.Receivers(['serena.davis@contoso.com', ])

notificationReceiversNotificationReceiver1 = NotificationReceiver()
notificationReceiversNotificationReceiver1.locale = 'en-us'

notificationReceiversNotificationReceiver1.contactInformation = 'serena.davis@contoso.com'


notificationReceiversArray []= notificationReceiversNotificationReceiver1;
notificationChannelsNotificationChannel2.notificationreceivers(notificationReceiversArray)



notificationChannelsArray []= notificationChannelsNotificationChannel2;
request_body.notificationchannels(notificationChannelsArray)




request_configuration = AlertRulesRequestBuilderPostRequestConfiguration(
)


result = await client.deviceManagement.monitoring.alertRules.post(request_body = request_body)


```