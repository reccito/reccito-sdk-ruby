# ReccitoSdk::ReceiptInsights

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **return_window_days** | **Integer** |  | [optional] |
| **return_deadline** | **Time** |  | [optional] |
| **refund_eligible** | **Boolean** |  | [optional] |
| **warranty_items** | [**Array&lt;WarrantyInfo&gt;**](WarrantyInfo.md) |  | [optional] |

## Example

```ruby
require 'reccito_sdk'

instance = ReccitoSdk::ReceiptInsights.new(
  return_window_days: null,
  return_deadline: null,
  refund_eligible: null,
  warranty_items: null
)
```

