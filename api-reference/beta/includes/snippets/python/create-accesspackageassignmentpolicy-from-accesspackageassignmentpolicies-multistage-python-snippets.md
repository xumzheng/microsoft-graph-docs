---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = AccessPackageAssignmentPolicy()
request_body.setAccessPackageId('string (identifier)')

request_body.setDisplayName('Users from connected organizations can request')

request_body.setDescription('Allow users from configured connected organizations to request and be approved by their sponsors')

request_body.setCanExtend(false)

request_body.setDurationInDays(365)

request_body.setExpirationDateTime(null)

requestorSettings = RequestorSettings()
requestorSettings.setScopeType('AllExistingConnectedOrganizationSubjects')

requestorSettings.setAcceptRequests(true)

requestorSettings.setAllowedRequestors([])


request_body.setRequestorSettings($requestorSettings)
requestApprovalSettings = ApprovalSettings()
requestApprovalSettings.setIsApprovalRequired(true)

requestApprovalSettings.setIsApprovalRequiredForExtension(false)

requestApprovalSettings.setIsRequestorJustificationRequired(true)

requestApprovalSettings.setApprovalMode('Serial')

approvalStagesApprovalStage1 = ApprovalStage()
approvalStagesApprovalStage1.setApprovalStageTimeOutInDays(14)

approvalStagesApprovalStage1.setIsApproverJustificationRequired(true)

approvalStagesApprovalStage1.setIsEscalationEnabled(true)

approvalStagesApprovalStage1.setEscalationTimeInMinutes(11520)

primaryApproversUserSet1 = UserSet()
primaryApproversUserSet1.set@odatatype('#microsoft.graph.groupMembers')

primaryApproversUserSet1.setIsBackup(true)

additionalData = [
'id' => 'string (identifier)', 
'description' => 'group for users from connected organizations which have no external sponsor', 
];
primaryApproversUserSet1.setAdditionalData(additionalData)



primaryApproversArray []= primaryApproversUserSet1;
primaryApproversUserSet2 = UserSet()
primaryApproversUserSet2.set@odatatype('#microsoft.graph.externalSponsors')

primaryApproversUserSet2.setIsBackup(false)


primaryApproversArray []= primaryApproversUserSet2;
approvalStagesApprovalStage1.setPrimaryApprovers(primaryApproversArray)


escalationApproversUserSet1 = UserSet()
escalationApproversUserSet1.set@odatatype('#microsoft.graph.singleUser')

escalationApproversUserSet1.setIsBackup(true)

additionalData = [
'id' => 'string (identifier)', 
'description' => 'user if the external sponsor does not respond', 
];
escalationApproversUserSet1.setAdditionalData(additionalData)



escalationApproversArray []= escalationApproversUserSet1;
approvalStagesApprovalStage1.setEscalationApprovers(escalationApproversArray)



approvalStagesArray []= approvalStagesApprovalStage1;
approvalStagesApprovalStage2 = ApprovalStage()
approvalStagesApprovalStage2.setApprovalStageTimeOutInDays(14)

approvalStagesApprovalStage2.setIsApproverJustificationRequired(true)

approvalStagesApprovalStage2.setIsEscalationEnabled(true)

approvalStagesApprovalStage2.setEscalationTimeInMinutes(11520)

primaryApproversUserSet1 = UserSet()
primaryApproversUserSet1.set@odatatype('#microsoft.graph.groupMembers')

primaryApproversUserSet1.setIsBackup(true)

additionalData = [
'id' => 'string (identifier)', 
'description' => 'group for users from connected organizations which have no internal sponsor', 
];
primaryApproversUserSet1.setAdditionalData(additionalData)



primaryApproversArray []= primaryApproversUserSet1;
primaryApproversUserSet2 = UserSet()
primaryApproversUserSet2.set@odatatype('#microsoft.graph.internalSponsors')

primaryApproversUserSet2.setIsBackup(false)


primaryApproversArray []= primaryApproversUserSet2;
approvalStagesApprovalStage2.setPrimaryApprovers(primaryApproversArray)


escalationApproversUserSet1 = UserSet()
escalationApproversUserSet1.set@odatatype('#microsoft.graph.singleUser')

escalationApproversUserSet1.setIsBackup(true)

additionalData = [
'id' => 'string (identifier)', 
'description' => 'user if the internal sponsor does not respond', 
];
escalationApproversUserSet1.setAdditionalData(additionalData)



escalationApproversArray []= escalationApproversUserSet1;
approvalStagesApprovalStage2.setEscalationApprovers(escalationApproversArray)



approvalStagesArray []= approvalStagesApprovalStage2;
requestApprovalSettings.setApprovalStages(approvalStagesArray)



request_body.setRequestApprovalSettings($requestApprovalSettings)
accessReviewSettings = AssignmentReviewSettings()
accessReviewSettings.setIsEnabled(true)

accessReviewSettings.setRecurrenceType('quarterly')

accessReviewSettings.setReviewerType('Self')

accessReviewSettings.setStartDateTime(DateTime('2020-04-01T07:59:59.998Z'))

accessReviewSettings.setDurationInDays(25)

accessReviewSettings.setReviewers([])


request_body.setAccessReviewSettings($accessReviewSettings)


result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies.post(request_body)


```