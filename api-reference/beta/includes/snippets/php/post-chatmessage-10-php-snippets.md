---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ChatMessage();


$requestRequestBody->setSubject(null);

$body = new ItemBody();
$requestRequestBody->setBody($body);


$body->setContentType(new BodyType('html'));
$body->setContent('<attachment id="74d20c7f34aa4a7fb74e2b30004247c5"></attachment>');

$attachmentsArray = [];

$attachmentsattachments1 = new ChatMessageAttachment();

$attachmentsattachments1->setId('74d20c7f34aa4a7fb74e2b30004247c5');
$attachmentsattachments1->setContentType('application/vnd.microsoft.card.thumbnail');
$attachmentsattachments1->setContentUrl(null);
$attachmentsattachments1->setContent('{
  "title": "This is an example of posting a card",
  "subtitle": "<h3>This is the subtitle</h3>",
  "text": "Here is some body text. <br>\r\nAnd a <a href=\"http://microsoft.com/\">hyperlink</a>. <br>\r\nAnd below that is some buttons:",
  "buttons": [
    {
      "type": "messageBack",
      "title": "Login to FakeBot",
      "text": "login",
      "displayText": "login",
      "value": "login"
    }
  ]
}');
$attachmentsattachments1->setName(null);
$attachmentsattachments1->setThumbnailUrl(null);
$attachmentsattachments1->setTeamsAppId('881b8843-fd91-49e5-9ac2-47ec497ffbe5');

$attachmentsArray []= $attachmentsattachments1;
$requestRequestBody->setAttachments($attachmentsArray);
$result =  $graphClient->teamsById('team-id')->channelsById('channel-id')->messages()->post($requestRequestBody);


```