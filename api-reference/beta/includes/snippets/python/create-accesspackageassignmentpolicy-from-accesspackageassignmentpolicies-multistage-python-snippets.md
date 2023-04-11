---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.accessPackageId = 'string (identifier)'

request_body.displayName = 'Users from connected organizations can request'

request_body.description = 'Allow users from configured connected organizations to request and be approved by their sponsors'

request_body.canExtend = false

request_body.durationInDays = 365

request_body.expirationDateTime=null

requestorSettings = RequestorSettings()
requestorSettings.scopeType = 'AllExistingConnectedOrganizationSubjects'

requestorSettings.acceptRequests = true

requestorSettings.AllowedRequestors([])


request_body.requestorSettings = requestorSettings
requestApprovalSettings = ApprovalSettings()
requestApprovalSettings.isApprovalRequired = true

requestApprovalSettings.isApprovalRequiredForExtension = false

requestApprovalSettings.isRequestorJustificationRequired = true

requestApprovalSettings.approvalMode = 'Serial'

approvalStagesApprovalStage1 = ApprovalStage()
approvalStagesApprovalStage1.approvalStageTimeOutInDays = 14

approvalStagesApprovalStage1.isApproverJustificationRequired = true

approvalStagesApprovalStage1.isEscalationEnabled = true

approvalStagesApprovalStage1.escalationTimeInMinutes = 11520

primaryApproversUserSet1 = UserSet()
primaryApproversUserSet1.@odatatype = '#microsoft.graph.groupMembers'

primaryApproversUserSet1.isBackup = true

additionalData = [
'id' => 'string (identifier)', 
'description' => 'group for users from connected organizations which have no external sponsor', 
];
primaryApproversUserSet1.additionaldata(additionalData)



primaryApproversArray []= primaryApproversUserSet1;
primaryApproversUserSet2 = UserSet()
primaryApproversUserSet2.@odatatype = '#microsoft.graph.externalSponsors'

primaryApproversUserSet2.isBackup = false


primaryApproversArray []= primaryApproversUserSet2;
approvalStagesApprovalStage1.primaryapprovers(primaryApproversArray)


escalationApproversUserSet1 = UserSet()
escalationApproversUserSet1.@odatatype = '#microsoft.graph.singleUser'

escalationApproversUserSet1.isBackup = true

additionalData = [
'id' => 'string (identifier)', 
'description' => 'user if the external sponsor does not respond', 
];
escalationApproversUserSet1.additionaldata(additionalData)



escalationApproversArray []= escalationApproversUserSet1;
approvalStagesApprovalStage1.escalationapprovers(escalationApproversArray)



approvalStagesArray []= approvalStagesApprovalStage1;
approvalStagesApprovalStage2 = ApprovalStage()
approvalStagesApprovalStage2.approvalStageTimeOutInDays = 14

approvalStagesApprovalStage2.isApproverJustificationRequired = true

approvalStagesApprovalStage2.isEscalationEnabled = true

approvalStagesApprovalStage2.escalationTimeInMinutes = 11520

primaryApproversUserSet1 = UserSet()
primaryApproversUserSet1.@odatatype = '#microsoft.graph.groupMembers'

primaryApproversUserSet1.isBackup = true

additionalData = [
'id' => 'string (identifier)', 
'description' => 'group for users from connected organizations which have no internal sponsor', 
];
primaryApproversUserSet1.additionaldata(additionalData)



primaryApproversArray []= primaryApproversUserSet1;
primaryApproversUserSet2 = UserSet()
primaryApproversUserSet2.@odatatype = '#microsoft.graph.internalSponsors'

primaryApproversUserSet2.isBackup = false


primaryApproversArray []= primaryApproversUserSet2;
approvalStagesApprovalStage2.primaryapprovers(primaryApproversArray)


escalationApproversUserSet1 = UserSet()
escalationApproversUserSet1.@odatatype = '#microsoft.graph.singleUser'

escalationApproversUserSet1.isBackup = true

additionalData = [
'id' => 'string (identifier)', 
'description' => 'user if the internal sponsor does not respond', 
];
escalationApproversUserSet1.additionaldata(additionalData)



escalationApproversArray []= escalationApproversUserSet1;
approvalStagesApprovalStage2.escalationapprovers(escalationApproversArray)



approvalStagesArray []= approvalStagesApprovalStage2;
requestApprovalSettings.approvalstages(approvalStagesArray)



request_body.requestApprovalSettings = requestApprovalSettings
accessReviewSettings = AssignmentReviewSettings()
accessReviewSettings.isEnabled = true

accessReviewSettings.recurrenceType = 'quarterly'

accessReviewSettings.reviewerType = 'Self'

accessReviewSettings.startDateTime = DateTime('2020-04-01T07:59:59.998Z')

accessReviewSettings.durationInDays = 25

accessReviewSettings.Reviewers([])


request_body.accessReviewSettings = accessReviewSettings


request_configuration = AccessPackageAssignmentPoliciesRequestBuilderPostRequestConfiguration(
)


result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies.post(request_body = request_body)


```