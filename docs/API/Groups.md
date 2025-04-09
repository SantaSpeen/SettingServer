# Section: `Groups`

## Contents:
- [`groups.get`](#groupsget)
- [`groups.getAll`](#groupsgetall)
- [`groups.new`](#groupsnew)
- [`groups.del`](#groupsdel)
- [`groups.update`](#groupsupdate)


### `groups.get`:
### `groups.getAll`:

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

### `groups.del`:
### `groups.update`: