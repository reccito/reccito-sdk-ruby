# ReccitoSdk::ErrorDetail

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **code** | **String** | Error code identifier |  |
| **message** | **String** | Human-readable error message |  |
| **details** | **Hash&lt;String, Object&gt;** | Additional error details | [optional] |

## Example

```ruby
require 'reccito_sdk'

instance = ReccitoSdk::ErrorDetail.new(
  code: null,
  message: null,
  details: null
)
```

