# ![LOGO](logo.png) Tasks **flow**ground Connector

## Description

A generated **flow**ground connector for the Tasks API (version v1).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/tasks/v1/swagger.json<br/>
Generated at: 2019-05-07T17:42:04+03:00

## API Description

Manages your tasks and task lists.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Clears all completed tasks from the specified task list. The affected tasks will be marked as 'hidden' and no longer be returned by default when retrieving all tasks for a task list.

*Tags:* `tasks`

#### Input Parameters
* `tasklist` - _required_ - Task list identifier.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Returns all tasks in the specified task list.

*Tags:* `tasks`

#### Input Parameters
* `completedMax` - _optional_ - Upper bound for a task's completion date (as a RFC 3339 timestamp) to filter by. Optional. The default is not to filter by completion date.
* `completedMin` - _optional_ - Lower bound for a task's completion date (as a RFC 3339 timestamp) to filter by. Optional. The default is not to filter by completion date.
* `dueMax` - _optional_ - Upper bound for a task's due date (as a RFC 3339 timestamp) to filter by. Optional. The default is not to filter by due date.
* `dueMin` - _optional_ - Lower bound for a task's due date (as a RFC 3339 timestamp) to filter by. Optional. The default is not to filter by due date.
* `maxResults` - _optional_ - Maximum number of task lists returned on one page. Optional. The default is 20 (max allowed: 100).
* `pageToken` - _optional_ - Token specifying the result page to return. Optional.
* `showCompleted` - _optional_ - Flag indicating whether completed tasks are returned in the result. Optional. The default is True.
* `showDeleted` - _optional_ - Flag indicating whether deleted tasks are returned in the result. Optional. The default is False.
* `showHidden` - _optional_ - Flag indicating whether hidden tasks are returned in the result. Optional. The default is False.
* `tasklist` - _required_ - Task list identifier.
* `updatedMin` - _optional_ - Lower bound for a task's last modification time (as a RFC 3339 timestamp) to filter by. Optional. The default is not to filter by last modification time.

### Creates a new task on the specified task list.

*Tags:* `tasks`

#### Input Parameters
* `parent` - _optional_ - Parent task identifier. If the task is created at the top level, this parameter is omitted. Optional.
* `previous` - _optional_ - Previous sibling task identifier. If the task is created at the first position among its siblings, this parameter is omitted. Optional.
* `tasklist` - _required_ - Task list identifier.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes the specified task from the task list.

*Tags:* `tasks`

#### Input Parameters
* `task` - _required_ - Task identifier.
* `tasklist` - _required_ - Task list identifier.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Returns the specified task.

*Tags:* `tasks`

#### Input Parameters
* `task` - _required_ - Task identifier.
* `tasklist` - _required_ - Task list identifier.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates the specified task. This method supports patch semantics.

*Tags:* `tasks`

#### Input Parameters
* `task` - _required_ - Task identifier.
* `tasklist` - _required_ - Task list identifier.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates the specified task.

*Tags:* `tasks`

#### Input Parameters
* `task` - _required_ - Task identifier.
* `tasklist` - _required_ - Task list identifier.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Moves the specified task to another position in the task list. This can include putting it as a child task under a new parent and/or move it to a different position among its sibling tasks.

*Tags:* `tasks`

#### Input Parameters
* `parent` - _optional_ - New parent task identifier. If the task is moved to the top level, this parameter is omitted. Optional.
* `previous` - _optional_ - New previous sibling task identifier. If the task is moved to the first position among its siblings, this parameter is omitted. Optional.
* `task` - _required_ - Task identifier.
* `tasklist` - _required_ - Task list identifier.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Returns all the authenticated user's task lists.

*Tags:* `tasklists`

#### Input Parameters
* `maxResults` - _optional_ - Maximum number of task lists returned on one page. Optional. The default is 20 (max allowed: 100).
* `pageToken` - _optional_ - Token specifying the result page to return. Optional.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Creates a new task list and adds it to the authenticated user's task lists.

*Tags:* `tasklists`

#### Input Parameters
* `alt` - _optional_ - Data format for the response.
    Possible values: json.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes the authenticated user's specified task list.

*Tags:* `tasklists`

#### Input Parameters
* `tasklist` - _required_ - Task list identifier.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Returns the authenticated user's specified task list.

*Tags:* `tasklists`

#### Input Parameters
* `tasklist` - _required_ - Task list identifier.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates the authenticated user's specified task list. This method supports patch semantics.

*Tags:* `tasklists`

#### Input Parameters
* `tasklist` - _required_ - Task list identifier.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates the authenticated user's specified task list.

*Tags:* `tasklists`

#### Input Parameters
* `tasklist` - _required_ - Task list identifier.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

## License

**flow**ground :- Telekom iPaaS / googleapis-com-tasks-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
