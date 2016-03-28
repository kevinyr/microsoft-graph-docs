# contactFolder resource type

A folder that contains contacts.

### JSON representation

Here is a JSON representation of the resource

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts"
  ],
  "@odata.type": "microsoft.graph.contactfolder"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string"
}

```
### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|displayName|String|The folder's display name.|
|id|String|Unique identifier of the contact folder. Read-only.|
|parentFolderId|String|The ID of the folder's parent folder.|

### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|childFolders|[ContactFolder](contactfolder.md) collection|The collection of child folders in the folder. Navigation property. Read-only. Nullable.|
|contacts|[Contact](contact.md) collection|The contacts in the folder. Navigation property. Read-only. Nullable.|

### Methods

| Method       | Return Type  |Description|
|:---------------|:--------|:----------|
|[Get contactFolder](../api/contactfolder_get.md) | [contactFolder](contactfolder.md) |Get a contact folder by using the contact folder ID.|
|[Update](../api/contactfolder_update.md) | [contactFolder](contactfolder.md) |Update contactFolder object. |
|[Delete](../api/contactfolder_delete.md) | None |Delete contactFolder object. |
|[List childFolders](../api/contactfolder_list_childfolders.md) |[ContactFolder](contactfolder.md) collection| Get a collection of child folders under the specified contact folder.|
|[Create child contactFolder](../api/contactfolder_post_childfolders.md) |[ContactFolder](contactfolder.md)| Create a new contactFolder as a child of a specified folder.|
|[List contacts in folder](../api/contactfolder_list_contacts.md) |[Contact](contact.md) collection| Get all the contacts in the signed-in user's mailbox (`.../me/contacts`), or from the specified contact folder.|
|[Create contact in folder](../api/contactfolder_post_contacts.md) |[Contact](contact.md)| Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->