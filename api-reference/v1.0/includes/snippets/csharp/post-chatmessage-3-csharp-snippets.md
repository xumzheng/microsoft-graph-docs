---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ChatMessage
{
	Subject = null,
	Body = new ItemBody
	{
		ContentType = "html",
		Content = "<attachment id="74d20c7f34aa4a7fb74e2b30004247c5"></attachment>",
	},
	Attachments = new List<ChatMessageAttachment>
	{
		new ChatMessageAttachment
		{
			Id = "74d20c7f34aa4a7fb74e2b30004247c5",
			ContentType = "application/vnd.microsoft.card.thumbnail",
			ContentUrl = null,
			Content = "{
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
}",
			Name = null,
			ThumbnailUrl = null,
		},
	}
};
var result = await graphClient.Teams["team-id"].Channels["channel-id"].Messages.PostAsync(requestBody);


```