﻿# Get windows10CertificateProfileBase

> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.

Read properties and relationships of the [windows10CertificateProfileBase](../resources/intune_deviceconfig_windows10certificateprofilebase.md) object.
## Prerequisites
One of the following **scopes** is required to execute this API:

*DeviceManagementConfiguration.ReadWrite.All; DeviceManagementConfiguration.Read.All*
## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceConfigurationAssignments/{deviceConfigurationAssignmentsId}/deviceConfiguration/
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/
```

## Optional query parameters
This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.
## Request headers
|Header|Value|
|---|---|
|Authorization|Bearer &lt;token&gt; Required.|
|Accept|application/json|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [windows10CertificateProfileBase](../resources/intune_deviceconfig_windows10certificateprofilebase.md) object in the response body.

## Example
### Request
Here is an example of the request.
```http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 668

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10CertificateProfileBase",
    "id": "1f01ffc6-ffc6-1f01-c6ff-011fc6ff011f",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "renewalThresholdPercentage": 10,
    "keyStorageProvider": "useTpmKspOtherwiseFail",
    "subjectNameFormat": "commonNameIncludingEmail",
    "subjectAlternativeNameType": "userPrincipalName",
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  }
}
```



