# ReccitoSdk::PaymentInfoResponse

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **method** | **String** |  |  |
| **amount** | **String** |  |  |
| **card_last_four** | **String** |  | [optional] |
| **reference** | **String** |  | [optional] |

## Example

```ruby
require 'reccito_sdk'

instance = ReccitoSdk::PaymentInfoResponse.new(
  method: null,
  amount: 12.99,
  card_last_four: null,
  reference: null
)
```

