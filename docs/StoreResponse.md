# ReccitoSdk::StoreResponse

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  |  |
| **name** | **String** |  |  |
| **code** | **String** |  |  |
| **description** | **String** |  | [optional] |
| **organisation_id** | **String** |  |  |
| **address_line_1** | **String** |  | [optional] |
| **address_line_2** | **String** |  | [optional] |
| **city** | **String** |  | [optional] |
| **state** | **String** |  | [optional] |
| **postal_code** | **String** |  | [optional] |
| **country** | **String** |  |  |
| **full_address** | **String** |  |  |
| **latitude** | **String** |  | [optional] |
| **longitude** | **String** |  | [optional] |
| **phone** | **String** |  | [optional] |
| **email** | **String** |  | [optional] |
| **manager_name** | **String** |  | [optional] |
| **timezone** | **String** |  | [optional] |
| **default_qr_expiry_minutes** | **Integer** |  | [optional] |
| **effective_qr_expiry** | **Integer** |  |  |
| **logo_url** | **String** |  | [optional] |
| **primary_color** | **String** |  | [optional] |
| **effective_logo_url** | **String** |  | [optional] |
| **effective_primary_color** | **String** |  | [optional] |
| **is_active** | **Boolean** |  |  |
| **opening_hours** | **Hash&lt;String, Object&gt;** |  | [optional] |
| **receipts_created_count** | **Integer** |  |  |
| **last_receipt_created** | **Time** |  | [optional] |
| **custom_metadata** | **Hash&lt;String, Object&gt;** |  | [optional] |
| **created_at** | **Time** |  |  |
| **updated_at** | **Time** |  |  |

## Example

```ruby
require 'reccito_sdk'

instance = ReccitoSdk::StoreResponse.new(
  id: null,
  name: null,
  code: null,
  description: null,
  organisation_id: null,
  address_line_1: null,
  address_line_2: null,
  city: null,
  state: null,
  postal_code: null,
  country: null,
  full_address: null,
  latitude: null,
  longitude: null,
  phone: null,
  email: null,
  manager_name: null,
  timezone: null,
  default_qr_expiry_minutes: null,
  effective_qr_expiry: null,
  logo_url: null,
  primary_color: null,
  effective_logo_url: null,
  effective_primary_color: null,
  is_active: null,
  opening_hours: null,
  receipts_created_count: null,
  last_receipt_created: null,
  custom_metadata: null,
  created_at: null,
  updated_at: null
)
```

