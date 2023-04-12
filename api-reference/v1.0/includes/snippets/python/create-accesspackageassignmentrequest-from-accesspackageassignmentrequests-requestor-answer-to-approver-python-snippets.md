---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentRequest()
request_body.@odatatype = '#microsoft.graph.accessPackageAssignmentRequest'

request_body.RequestType(AccessPackageRequestType('useradd'))

answersAccessPackageAnswer1 = AccessPackageAnswer()
answersAccessPackageAnswer1.@odatatype = '#microsoft.graph.accessPackageAnswerString'

answersAccessPackageAnswer1.displayValue = 'This is the answer to a multiple choice question'

answersAccessPackageAnswer1AnsweredQuestion = AccessPackageQuestion()
answersAccessPackageAnswer1AnsweredQuestion.@odatatype = '#microsoft.graph.accessPackageMultipleChoiceQuestion'

answersAccessPackageAnswer1AnsweredQuestion.id = '8fe745e7-80b2-490d-bd22-4e708c77288c'


answersAccessPackageAnswer1.answeredQuestion = answersAccessPackageAnswer1AnsweredQuestion
additionalData = [
'value' => 'MultipleChoiceAnswerValue', 
];
answersAccessPackageAnswer1.additionaldata(additionalData)



answersArray []= answersAccessPackageAnswer1;
answersAccessPackageAnswer2 = AccessPackageAnswer()
answersAccessPackageAnswer2.@odatatype = '#microsoft.graph.accessPackageAnswerString'

answersAccessPackageAnswer2.displayValue = 'This is my answer.'

answersAccessPackageAnswer2AnsweredQuestion = AccessPackageQuestion()
answersAccessPackageAnswer2AnsweredQuestion.@odatatype = '#microsoft.graph.accessPackageTextInputQuestion'

answersAccessPackageAnswer2AnsweredQuestion.id = '7aaa18c9-8e4f-440f-bd5a-3a7ce312cbe6'


answersAccessPackageAnswer2.answeredQuestion = answersAccessPackageAnswer2AnsweredQuestion
additionalData = [
'value' => 'This is my answer to a text input question.', 
];
answersAccessPackageAnswer2.additionaldata(additionalData)



answersArray []= answersAccessPackageAnswer2;
request_body.answers(answersArray)


assignment = AccessPackageAssignment()
additionalData = [
'accessPackageId' => '977c7ff4-ef8f-4910-9d31-49048ddf3120', 
];
assignment.additionaldata(additionalData)



request_body.assignment = assignment



result = await client.identityGovernance.entitlementManagement.assignmentRequests.post(request_body = request_body)


```