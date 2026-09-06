# ReccitoSdk::ApiResponse

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **data** | **Hash&lt;String, Object&gt;** | Response payload data | [optional] |
| **error** | [**ErrorDetail**](ErrorDetail.md) | Error information | [optional] |
| **pagination** | [**PaginationInfo**](PaginationInfo.md) | Pagination information for list responses | [optional] |

## Example

```ruby
require 'reccito_sdk'

instance = ReccitoSdk::ApiResponse.new(
  data: null,
  error: null,
  pagination: null
)
```

