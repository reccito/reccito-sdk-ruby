# ReccitoSdk::PaginationInfo

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **page** | **Integer** | Current page number |  |
| **limit** | **Integer** | Items per page |  |
| **total** | **Integer** | Total number of items |  |
| **has_next** | **Boolean** | Whether there is a next page |  |

## Example

```ruby
require 'reccito_sdk'

instance = ReccitoSdk::PaginationInfo.new(
  page: null,
  limit: null,
  total: null,
  has_next: null
)
```

