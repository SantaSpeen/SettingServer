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

*Sections*:
- [Settings](./API/Settings.md)
- [Groups](./API/Groups.md)
- [Tokens](./API/Tokens.md)
- [Stats](./API/Stats.md)

* [Error Codes](./ErrorCodes.md)
