# ReccitoSdk::ReceiptListResponse

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **receipts** | [**Array&lt;ReceiptSummary&gt;**](ReceiptSummary.md) |  |  |
| **total** | **Integer** |  |  |
| **page** | **Integer** |  |  |
| **limit** | **Integer** |  |  |
| **has_next** | **Boolean** |  |  |
| **has_prev** | **Boolean** |  |  |

## Example

```ruby
require 'reccito_sdk'

instance = ReccitoSdk::ReceiptListResponse.new(
  receipts: null,
  total: null,
  page: null,
  limit: null,
  has_next: null,
  has_prev: null
)
```

