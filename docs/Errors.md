# Settings Server Error Codes

## 101 Invalid Token:
- **Description**: Invalid or missing access token.
- **Reasons**: Token is not provided or is incorrect.

## 102 Token Expired:
- **Description**: The token has expired.
- **Reasons**: The token has expired, re-authentication is required.

## 103 Insufficient Permissions:
- **Description**: The user or token has insufficient permissions.
- **Reasons**: The user or token does not have the necessary permissions to perform the action.

## 201 Group Already Exists:
- **Description**: A group with this name already exists.
- **Reasons**: Attempt to create a group with an already taken name.

## 202 Group Not Found:
- **Description**: The requested group was not found.
- **Reasons**: The specified group does not exist in the system.

## 203 Invalid Group Name:
- **Description**: The group name is invalid.
- **Reasons**: Invalid characters or length for the group name.

## 204 Group Description Too Long:
- **Description**: The group description is too long.
- **Reasons**: The description exceeds the maximum allowed length.

## 301 Setting Already Exists:
- **Description**: A setting with this name already exists.
- **Reasons**: Attempt to create a setting with an already existing name.

## 302 Setting Not Found:
- **Description**: The requested setting was not found.
- **Reasons**: The specified setting does not exist in the system.

## 303 Invalid Setting Name:
- **Description**: The setting name is invalid.
- **Reasons**: Invalid characters or length for the setting name.

## 304 Setting Cannot Be Edited:
- **Description**: The setting cannot be edited.
- **Reasons**: The setting is protected from changes or is in a read-only state.

## 401 Token Not Found:
- **Description**: The requested token was not found.
- **Reasons**: The specified token does not exist.

## 402 Token Invalid Format:
- **Description**: The token format is invalid.
- **Reasons**: The token is of an incorrect length or format.

## 403 Unable to Revoke Token:
- **Description**: Unable to revoke the token.
- **Reasons**: The token does not exist or is already revoked.

## 501 Stats Not Available:
- **Description**: Stats are unavailable.
- **Reasons**: The server is not configured for statistics or no data is available.

## 502 Invalid Statistic Type:
- **Description**: The requested statistic type is invalid.
- **Reasons**: The specified statistic type does not exist or is incorrectly specified.

## 601 Invalid Request:
- **Description**: The request format is invalid or missing required parameters.
- **Reasons**: Missing or malformed request parameters.

## 602 Method Not Supported:
- **Description**: The requested method is not supported.
- **Reasons**: The method is either deprecated or not implemented.

## 603 Internal Server Error:
- **Description**: An internal server error occurred.
- **Reasons**: A problem on the server side caused the failure.

