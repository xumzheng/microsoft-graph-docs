---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RegistrationPostRequestBody()
additionalData = [
'@odata.type' => '#microsoft.graph.meetingRegistration', 
'subject' => 'Microsoft Ignite', 
'description' => 'Join us November 2–4, 2021 to explore the latest tools, training sessions, technical expertise, networking opportunities, and more.', 
'startDateTime' => '2021-11-02T08:00:00-08:00', 
'endDateTime' => '2021-11-04T04:00:00-08:00', 
'allowedRegistrant' => 'everyone', 
'speakers' => speakers1 = ()
		speakers1.displayName = 'Henry Ross'

		speakers1.bio = 'Chairman and Chief Executive Officer'


speakersArray []= speakers1;
speakers2 = ()
		speakers2.displayName = 'Hailey Clark'

		speakers2.bio = 'EVP'


speakersArray []= speakers2;
request_body.speakers(speakersArray)


'customQuestions' => custom_questions1 = ()
	customQuestions1.displayName = 'Are you a developer?'

	customQuestions1.answerInputType = 'radioButton'

customQuestions1.AnswerOptions(['Yes', 'No', ])

customQuestions1.is_required = True


customQuestionsArray []= customQuestions1;
custom_questions2 = ()
customQuestions2.displayName = 'Where did you hear about us?'

customQuestions2.answerInputType = 'text'

customQuestions2.is_required = False


customQuestionsArray []= customQuestions2;
request_body.customquestions(customQuestionsArray)


];
request_body.additionaldata(additionalData)





await client.me.onlineMeetings_by_id('onlineMeeting-id').registration.post(request_body = request_body)


```