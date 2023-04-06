---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ForwardPostRequestBody()
toRecipientsRecipient1 = Recipient()
toRecipientsRecipient1EmailAddress = EmailAddress()
toRecipientsRecipient1EmailAddress.setAddress('danas@contoso.onmicrosoft.com')

toRecipientsRecipient1EmailAddress.setName('Dana Swope')


toRecipientsRecipient1.setEmailAddress($toRecipientsRecipient1EmailAddress)

toRecipientsArray []= toRecipientsRecipient1;
request_body.setToRecipients(toRecipientsArray)


request_body.setComment('Dana, hope you can make this meeting.')


request_config = ForwardRequestBuilderPostRequestConfiguration(
request_config = ForwardRequestBuilderPostRequestConfiguration(query_params=)


await client.me.events_by_id('event-id').forward.post(request_body, headers=)


```