# ReccitoSdk::ReceiptAdjustment

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **scope** | **String** |  | [optional][default to &#39;receipt&#39;] |
| **kind** | **String** |  |  |
| **label** | **String** |  | [optional] |
| **amount** | **String** |  |  |
| **item_name** | **String** |  | [optional] |

## Example

```ruby
require 'reccito_sdk'

instance = ReccitoSdk::ReceiptAdjustment.new(
  scope: null,
  kind: null,
  label: null,
  amount: 12.99,
  item_name: null
)
```

