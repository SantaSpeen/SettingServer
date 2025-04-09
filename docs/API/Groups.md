# Section: `Groups`

Section for managing groups in the system.\
This section provides endpoints for creating, retrieving, updating, and deleting groups.

## Contents:
- [`groups.get`](#groupsget)
- [`groups.getAll`](#groupsgetall)
- [`groups.new`](#groupsnew)
- [`groups.del`](#groupsdel)
- [`groups.update`](#groupsupdate)

---

### `groups.get`:
- **Method**: `GET`
- **Description**: Get group information by `id` or `alias`.
- **Parameters**:
  - `group`: The `id` or `alias` of the group.
  - `token`: **User token**

Request example:\
`GET /api/method/groups.get?group=TestGroup&token=<userToken>`

Response example:
```json
{
  "response": {
    "id": 1,
    "alias": "TestGroup",
    "description": "Description of the TestGroup"
  }
}
```

Errors: `101`, `102`, `103`, `601`

---

### `groups.getAll`:
- **Method**: `GET`
- **Description**: Get a list of all available groups for the token.
- **Parameters**:
  - `token`: **User token**

Request example:\
`GET /api/method/groups.getAll?token=<userToken>`

Response example:
```json
{
  "response": [
    {
      "id": 1,
      "alias": "TestGroup"
    },
    {
      "id": 2,
      "alias": "AnotherGroup"
    }
  ]
}
```

Errors: `101`, `102`, `103`, `601`

---

### `groups.new`:
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

---

### `groups.del`:
- **Method**: `GET`
- **Description**: Delete a group by `id` or `alias`.
- **Parameters**:
  - `group`: The `id` or `alias` of the group.
  - `token`: **Admin token**

Request example:\
`GET /api/method/groups.del?group=TestGroup&token=<adminToken>`

Response example:
```json
{
  "response": {
    "id": 1,
    "alias": "TestGroup"
  }
}
```

Errors: `101`, `102`, `103`, `301`, `401`, `601`

---

### `groups.update`:
- **Method**: `GET`
- **Description**: Update the name or alias of an existing group.
- **Parameters**:
  - `group`: The `id` or `alias` of the group.
  - `name`: The new name of the group.
  - `alias`: The new alias of the group.
  - `token`: **Admin token**

Request example:\
`GET /api/method/groups.update?group=TestGroup&name=NewTestGroup&alias=NewTestAlias&token=<adminToken>`

Response example:
```json
{
  "response": {
    "id": 1,
    "alias": "NewTestAlias"
  }
}
```

Errors: `101`, `102`, `103`, `301`, `302`, `401`

