---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentRequest()
request_body.@odatatype = '#microsoft.graph.accessPackageAssignmentRequest'

request_body.id = '7a6ab703-0780-4b37-8445-81f679b2d75c'

request_body.RequestType(AccessPackageRequestType('adminupdate'))

answersAccessPackageAnswer1 = AccessPackageAnswer()
answersAccessPackageAnswer1.@odatatype = '#microsoft.graph.accessPackageAnswerString'

answersAccessPackageAnswer1AnsweredQuestion = AccessPackageQuestion()
answersAccessPackageAnswer1AnsweredQuestion.@odatatype = '#microsoft.graph.accessPackageMultipleChoiceQuestion'

answersAccessPackageAnswer1AnsweredQuestion.id = '8fe745e7-80b2-490d-bd22-4e708c77288c'


answersAccessPackageAnswer1.answeredQuestion = answersAccessPackageAnswer1AnsweredQuestion
additionalData = [
'value' => 'UpdatedAnswerValue', 
];
answersAccessPackageAnswer1.additionaldata(additionalData)



answersArray []= answersAccessPackageAnswer1;
answersAccessPackageAnswer2 = AccessPackageAnswer()
answersAccessPackageAnswer2.@odatatype = '#microsoft.graph.accessPackageAnswerString'

answersAccessPackageAnswer2.displayValue = 'This is my updated answer to the question.'

answersAccessPackageAnswer2AnsweredQuestion = AccessPackageQuestion()
answersAccessPackageAnswer2AnsweredQuestion.@odatatype = '#microsoft.graph.accessPackageTextInputQuestion'

answersAccessPackageAnswer2AnsweredQuestion.id = '7aaa18c9-8e4f-440f-bd5a-3a7ce312cbe6'


answersAccessPackageAnswer2.answeredQuestion = answersAccessPackageAnswer2AnsweredQuestion
additionalData = [
'value' => 'My updated answer.', 
];
answersAccessPackageAnswer2.additionaldata(additionalData)



answersArray []= answersAccessPackageAnswer2;
request_body.answers(answersArray)


assignment = AccessPackageAssignment()
assignment.id = '44c741c1-2cf4-40db-83b6-e0112f8e5a83'


request_body.assignment = assignment


request_configuration = AssignmentRequestsRequestBuilderPostRequestConfiguration(
)


result = await client.identityGovernance.entitlementManagement.assignmentRequests.post(request_body = request_body)


```