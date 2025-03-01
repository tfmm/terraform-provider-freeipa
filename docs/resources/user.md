---
page_title: "freeipa_user Resource - freeipa"
description: |-
FreeIPA User resource
---

# freeipa_user (Resource)



## Example Usage

```terraform
resource "freeipa_user" "user-1" {
  first_name        = "Roman"
  last_name         = "Roman"
  name              = "roman"
  telephone_numbers = ["+380982555429", "2-10-11"]
  email_address     = ["roman@example.com"]
}
```




<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `first_name` (String) First name
- `last_name` (String) Last name
- `name` (String) UID or login

### Optional

- `account_disabled` (Boolean) Account disabled
- `car_license` (List of String) Car Licenses
- `city` (String) City
- `display_name` (String) Display name
- `email_address` (List of String) Email address
- `employee_number` (String) Employee Number
- `employee_type` (String) Employee Type
- `full_name` (String) Full name
- `gecos` (String) GECOS
- `gid_number` (Number) Group ID Number
- `home_directory` (String) Home Directory
- `initials` (String) Initials
- `job_title` (String) Job Title
- `krb_password_expiration` (String) User password expiration [RFC3339](https://datatracker.ietf.org/doc/html/rfc3339#section-5.8) format (see [RFC3339 time string](https://tools.ietf.org/html/rfc3339#section-5.8) e.g., `YYYY-MM-DDTHH:MM:SSZ`)
- `krb_principal_expiration` (String) Kerberos principal expiration [RFC3339](https://datatracker.ietf.org/doc/html/rfc3339#section-5.8) format (see [RFC3339 time string](https://tools.ietf.org/html/rfc3339#section-5.8) e.g., `YYYY-MM-DDTHH:MM:SSZ`)
- `krb_principal_name` (List of String) Principal alias
- `login_shell` (String) Login Shell
- `manager` (String) Manager
- `mobile_numbers` (List of String) Mobile Number
- `organisation_unit` (String) Org. Unit
- `postal_code` (String) Postal code
- `preferred_language` (String) Preferred Language
- `province` (String) Province/State/Country
- `random_password` (Boolean) Generate a random user password
- `ssh_public_key` (List of String) List of SSH public keys
- `street_address` (String) Street address
- `telephone_numbers` (List of String) Telephone Number
- `uid_number` (Number) User ID Number (system will assign one if not provided)
- `userclass` (List of String) User category (semantics placed on this attribute are for local interpretation)
- `userpassword` (String, Sensitive) Prompt to set the user password
- `external_idp_username` (String) External IDP Username (for use when users will authenticate via external IDP)
- `external_idp_config` (String) External IDP Configuration name (for use when users will authenticate via external IDP)

### Read-Only

- `id` (String) ID of the resource
