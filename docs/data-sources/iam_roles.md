---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "st-aws_iam_roles Data Source - st-aws"
subcategory: ""
description: |-
  Use this data source to retrieve list of IAM roles with attached tags.
---

# st-aws_iam_roles (Data Source)

Use this data source to retrieve list of IAM roles with attached tags.

## Example Usage

```terraform
data "st-aws_iam_roles" "aws_iam_roles" {
  tags = {
    "key" = "value"
  }
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Optional

- `tags` (Map of String) Filter by map of tags assigned to the IAM role.

### Read-Only

- `roles` (Attributes List) List of IAM roles. (see [below for nested schema](#nestedatt--roles))

<a id="nestedatt--roles"></a>
### Nested Schema for `roles`

Read-Only:

- `arn` (String) The Amazon Resource Name (ARN) that identifies the role.
- `assume_role_policy_document` (String) The policy that grants an entity permission to assume the role.
- `create_date` (String) The date and time, in ISO 8601 date-time string format, when the role was created.
- `description` (String) A description of the role that you provide.
- `max_session_duration` (Number) The maximum session duration (in seconds) for the specified role.
- `path` (String) The path to the role.
- `role_id` (String) The stable and unique string identifying the role.
- `role_name` (String) The friendly name identifying the role.
- `tags` (Map of String) A list of tags that are associated with the role.


