# ReccitoSdk::StoreCreate

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  |  |
| **code** | **String** |  |  |
| **description** | **String** |  | [optional] |
| **address_line_1** | **String** |  | [optional] |
| **address_line_2** | **String** |  | [optional] |
| **city** | **String** |  | [optional] |
| **state** | **String** |  | [optional] |
| **postal_code** | **String** |  | [optional] |
| **country** | **String** |  | [optional][default to &#39;US&#39;] |
| **latitude** | **String** |  | [optional] |
| **longitude** | **String** |  | [optional] |
| **phone** | **String** |  | [optional] |
| **email** | **String** |  | [optional] |
| **manager_name** | **String** |  | [optional] |
| **timezone** | **String** |  | [optional] |
| **default_qr_expiry_minutes** | **Integer** |  | [optional] |
| **logo_url** | **String** |  | [optional] |
| **primary_color** | **String** |  | [optional] |
| **opening_hours** | **Hash&lt;String, Object&gt;** |  | [optional] |
| **custom_metadata** | **Hash&lt;String, Object&gt;** |  | [optional] |

## Example

```ruby
require 'reccito_sdk'

instance = ReccitoSdk::StoreCreate.new(
  name: null,
  code: null,
  description: null,
  address_line_1: null,
  address_line_2: null,
  city: null,
  state: null,
  postal_code: null,
  country: null,
  latitude: null,
  longitude: null,
  phone: null,
  email: null,
  manager_name: null,
  timezone: null,
  default_qr_expiry_minutes: null,
  logo_url: null,
  primary_color: null,
  opening_hours: null,
  custom_metadata: null
)
```

