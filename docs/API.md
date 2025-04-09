# Setting Server API

## Overview

The Setting Server API provides endpoints for managing settings in the application. It allows users to retrieve, update, and delete settings.\
The API is designed to be simple and easy to use, with clear endpoints for each operation.

## How to Use

Base URL: `http://localhost:8080/`\
API: `/api/method`\
Settings: `/setting/<SETTING_NAME>`\

For example, to get the value of a setting named `telegram.token`, you would use the following URL:\
`http://localhost:8080/setting/telegram.token`

Simple usage:
1. Add new g

### Section: Settings

#### `settings.new`:
#### `settings.get`:
#### `settings.getByGroup`:

### Section: Groups

#### `groups.new`:
- **Method**: `GET`
- **Description**: Create a new group.
- **Parameters**:
  - `name`: The name of the group.
  - `description`: A description of the group.
  - `token`: **Admin token**

Request example:\
`GET /api/method/groups.new?name=TestGroup&description=TestGroupDescription&token=<adminToken>`

Response example:\
```json
{
  "res"
}
```

#### `groups.del`:
- **Method**: `GET`
- **Description**: Delete a group.
- **Parameters**:
  - `name`: The name of the group.
  - `token`: **Admin token**