---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendMailPostRequestBody()
message = Message()
message.setSubject('Project kickoff')

toRecipientsRecipient1 = Recipient()
toRecipientsRecipient1EmailAddress = EmailAddress()
toRecipientsRecipient1EmailAddress.setName('Samantha Booth')

toRecipientsRecipient1EmailAddress.setAddress('samanthab@contoso.onmicrosoft.com')


toRecipientsRecipient1.setEmailAddress($toRecipientsRecipient1EmailAddress)

toRecipientsArray []= toRecipientsRecipient1;
message.setToRecipients(toRecipientsArray)


mentionsMention1 = Mention()
mentionsMention1Mentioned = EmailAddress()
mentionsMention1Mentioned.setName('Dana Swope')

mentionsMention1Mentioned.setAddress('danas@contoso.onmicrosoft.com')


mentionsMention1.setMentioned($mentionsMention1Mentioned)

mentionsArray []= mentionsMention1;
message.setMentions(mentionsArray)



request_body.setMessage($message)

request_config = SendMailRequestBuilderPostRequestConfiguration(
request_config = SendMailRequestBuilderPostRequestConfiguration(query_params=)


await client.me.sendMail.post(request_body, headers=)


```