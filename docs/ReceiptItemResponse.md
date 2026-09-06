# ReccitoSdk::ReceiptItemResponse

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  |  |
| **quantity** | **Integer** |  |  |
| **unit_price** | **String** |  |  |
| **total_price** | **String** |  |  |
| **description** | **String** |  | [optional] |
| **sku** | **String** |  | [optional] |
| **category** | **String** |  | [optional] |

## Example

```ruby
require 'reccito_sdk'

instance = ReccitoSdk::ReceiptItemResponse.new(
  name: null,
  quantity: null,
  unit_price: 12.99,
  total_price: 12.99,
  description: null,
  sku: null,
  category: null
)
```

