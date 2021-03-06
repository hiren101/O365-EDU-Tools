# educationSubmission: release

Action makes the grade and feedback associated with this submission available back to the student.  This will change the status of the submission from "submitted" to "released" and indicates that grading is done.  This action can only be done by the teacher.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) |  EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite   |
|Delegated (personal Microsoft account) |  Not supported.  |
|Application | Not supported. | 

## HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/<id>/assignments/<id>/submissions/<id>/release

```
## Request headers
| Header       | Value |
|:---------------|:--------|
| Authorization  | Bearer {token}. Required.  |

## Request body

## Response
If successful, this method returns `204, No Content` response code. It does not return anything in the response body.

## Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "educationsubmission_release"
}-->

##### Response
```http
POST https://graph.microsoft.com/beta/education/classes/<id>/assignments/<id>/submissions/<id>/release
```
If successful, this method returns `204, No Content` response code. It does not return anything in the response body.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmission: release",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->