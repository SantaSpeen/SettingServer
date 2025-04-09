# Setting Server API

## Overview

The Setting Server API provides endpoints for managing settings in the application. It allows users to retrieve, update, and delete settings.\
The API is designed to be simple and easy to use, with clear endpoints for each operation.

## How to Use

Base URL: `http://localhost:8080/`\
API: `/api/method`\
Settings: `/setting/<SETTING_NAME>`

For example, to get the value of a setting named `telegram.token`, you would use the following URL:\
`http://localhost:8080/setting/telegram.token`

Simple usage:
1. Add new group
2. Add new token (for group)
3. Add new setting (via group token)
4. Get setting (via group token)

You may revoke the token at any time, if it is not used anymore (or stolen).

### Section: Settings

#### `settings.new`:
#### `settings.get`:
#### `settings.getByGroup`:

### Section: Groups

#### `groups.new`:
- **Method**: `GET`
- **Description**: Create a new group.
- **Parameters**:
  - `alias`: The name of the group. **(Cannot start with a digit and must match the specified regex for valid aliases.)**
  - `description`: A description of the group.
  - `token`: **Admin token**

Request example:\
`GET /api/method/groups.new?alias=TestGroup&description=TestGroupDescription&token=<adminToken>`

Response example:
```json
{
  "response": {
    "id": 1,
    "alias": "TestGroup"
  }
}
```

Errors: `101`, `102`, `103`, `201`, `301`, `302`, `601`

#### `groups.del`: