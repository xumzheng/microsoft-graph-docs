---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AlertRule();
requestBody.setId('215c55cc-b1c9-4d36-a870-be5778101714');

requestBody.setDisplayName('Azure network connection failure impacting Cloud PCs');

requestBody.setSeverity(RuleSeverityType('informational'));

requestBody.setIsSystemRule(true);

requestBody.setDescription('Azure network connection checks have failed and is potentially impacting existing Cloud PCs and blocking the provisioning of new Cloud PCs');

requestBody.setEnabled(true);

requestBody.setAlertRuleTemplate(AlertRuleTemplate('cloudpconpremisenetworkconnectioncheckscenario'));

threshold = RuleThreshold();
threshold.setAggregation(AggregationType('count'));

threshold.setOperator(OperatorType('greaterorequal'));

threshold.setTarget(90);


requestBody.setThreshold($threshold);
notificationChannelsNotificationChannel1 = NotificationChannel();
notificationChannelsNotificationChannel1.setNotificationChannelType(NotificationChannelType('portal'));

notificationChannelsNotificationChannel1.setReceivers(['', ]);

notificationChannelsNotificationChannel1.setNotificationReceivers([]);


notificationChannelsArray []= notificationChannelsNotificationChannel1;
notificationChannelsNotificationChannel2 = NotificationChannel();
notificationChannelsNotificationChannel2.setNotificationChannelType(NotificationChannelType('email'));

notificationChannelsNotificationChannel2.setReceivers(['serena.davis@contoso.com', ]);

notificationReceiversNotificationReceiver1 = NotificationReceiver();
notificationReceiversNotificationReceiver1.setLocale('en-us');

notificationReceiversNotificationReceiver1.setContactInformation('serena.davis@contoso.com');


notificationReceiversArray []= notificationReceiversNotificationReceiver1;
notificationChannelsNotificationChannel2.setNotificationReceivers(notificationReceiversArray);



notificationChannelsArray []= notificationChannelsNotificationChannel2;
requestBody.setNotificationChannels(notificationChannelsArray);




result = await client.deviceManagement().monitoring().alertRules().post(requestBody);


```