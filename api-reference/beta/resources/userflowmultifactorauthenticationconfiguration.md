---
title: "userFlowMultifactorAuthenticationConfiguration resource type"
description: "Configuration for controlling multi-factor authentication (MFA) settings for B2C userflows."
author: "harsh-aseeja"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: resourcePageType
---

# userFlowMultifactorAuthenticationConfiguration resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory B2C (Azure AD B2C) integrates directly with Azure AD multi-factor authentication (MFA) so that you can add a second layer of security to sign-up and sign-in experiences in your applications. Use this resource to configure the MFA settings in the Azure AD B2C user flow.


## Properties
|Property|Type|Description|
|:---|:---|:---|
|multifactorAuthenticationState|userFlowMultifactorAuthenticationState|Controls if and when MFA should be triggered. The possible values are: `off`, `on`, `conditional`. For more information about these states, see [userFlowMultifactorAuthenticationState values](#userflowmultifactorauthenticationstate-values).|
|multifactorAuthenticationMethod|userFlowMultifactorAuthenticationMethod|Specifies the MFA method the user should use when MFA is triggered. The possible values are: `email`, `phoneCallOrSms`, `phoneSms`, `phoneCall`, `authenticator`, `unknownFutureValue`. For more information about these states, see [userFlowMultifactorAuthenticationMethod values](#userflowmultifactorauthenticationmethod-values).|

### userflowmultifactorauthenticationstate values
|Value|Description|
|:---|:---|
|off|MFA is never enforced during sign-in, and users are not prompted to enroll in MFA during sign-up or sign-in.|
|on|MFA is always required, regardless of your Conditional Access setup. During sign-up, users are prompted to enroll in MFA. During sign-in, if users aren't already enrolled in MFA, they're prompted to enroll|
|conditional|During sign-up and sign-in, users are prompted to enroll in MFA (both new users and existing users who aren't enrolled in MFA). During sign-in, MFA is enforced only when an active Conditional Access policy evaluation requires it. If the result is an MFA challenge with no risk, MFA is enforced. If the user isn't already enrolled in MFA, they're prompted to enroll. If the result is an MFA challenge due to risk and the user is not enrolled in MFA, sign-in is blocked.|

### userFlowMultifactorAuthenticationMethod values

|Value|Description|
|:---|:---|
|email|During sign-in, a verification email containing a one-time password (OTP) is sent to the user. The user provides the OTP code that was sent in the email.|
|phoneCallOrSms|During the first sign-up or sign-in, the user is asked to provide and verify a phone number. During subsequent sign-ins, the user is prompted to select either the Send Code (SMS) or Call option. Depending on the user's choice, a text message is sent or a phone call is made to the verified phone number to identify the user. The user either provides the OTP code sent via text message or approves the phone call.|
|phoneCall|Works in the same way as the SMS or phone call option, but only a phone call option is made available.|
|phoneSms|Works in the same way as the SMS or phone call option, but only a text message is sent.|
|authenticator|The user must install an authenticator app that supports time-based one-time password (TOTP) verification, such as the Microsoft Authenticator app, on a device that they own. During the first sign-up or sign-in, the user scans a QR code or enters a code manually using the authenticator app. During subsequent sign-ins, the user types the TOTP code that appears on the authenticator app. See how to set up the Microsoft Authenticator app.|


## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userFlowMultifactorAuthenticationConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userFlowMultifactorAuthenticationConfiguration",
  "multifactorAuthenticationMethod": "String",
  "multifactorAuthenticationState": "String"
}
```

