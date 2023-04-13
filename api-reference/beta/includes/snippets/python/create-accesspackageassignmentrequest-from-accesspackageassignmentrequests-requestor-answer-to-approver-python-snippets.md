---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentRequest()
request_body.requestType = 'UserAdd'

access_package_assignment = AccessPackageAssignment()
accessPackageAssignment.targetId = '46184453-e63b-4f20-86c2-c557ed5d5df9'

accessPackageAssignment.assignmentPolicyId = '2264bf65-76ba-417b-a27d-54d291f0cbc8'

accessPackageAssignment.accessPackageId = 'a914b616-e04e-476b-aa37-91038f0b165b'


request_body.access_package_assignment = accessPackageAssignment
answers_access_package_answer1 = AccessPackageAnswer()
answersAccessPackageAnswer1.@odatatype = '#microsoft.graph.accessPackageAnswerString'

answers_access_package_answer1_answered_question = AccessPackageQuestion()
answersAccessPackageAnswer1AnsweredQuestion.@odatatype = '#microsoft.graph.accessPackageMultipleChoiceQuestion'

answersAccessPackageAnswer1AnsweredQuestion.id = 'A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF'


answersAccessPackageAnswer1.answered_question = answersAccessPackageAnswer1AnsweredQuestion
additionalData = [
'value' => 'Arizona', 
];
answersAccessPackageAnswer1.additionaldata(additionalData)



answersArray []= answersAccessPackageAnswer1;
answers_access_package_answer2 = AccessPackageAnswer()
answersAccessPackageAnswer2.@odatatype = '#microsoft.graph.accessPackageAnswerString'

answers_access_package_answer2_answered_question = AccessPackageQuestion()
answersAccessPackageAnswer2AnsweredQuestion.@odatatype = '#microsoft.graph.accessPackageTextInputQuestion'

answersAccessPackageAnswer2AnsweredQuestion.id = 'AA615EE9-D9D8-4C03-BE91-BEE37106DEDA'


answersAccessPackageAnswer2.answered_question = answersAccessPackageAnswer2AnsweredQuestion
additionalData = [
'value' => 'Need access to marketing campaign material', 
];
answersAccessPackageAnswer2.additionaldata(additionalData)



answersArray []= answersAccessPackageAnswer2;
request_body.answers(answersArray)





result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentRequests.post(request_body = request_body)


```