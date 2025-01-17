# UncheckedAddress

## Functions

### uncheckedFunctionCall

```text
function uncheckedFunctionCall(
  address target,
  bytes data,
  string errorMessage
) internal returns (bytes)
```

#### Parameters:

| Name | Type | Description |
| :--- | :--- | :--- |
| `target` | address |  |
| `data` | bytes |  |
| `errorMessage` | string |  |

### uncheckedFunctionCallWithValue

```text
function uncheckedFunctionCallWithValue(
  address target,
  bytes data,
  uint256 value,
  string errorMessage
) internal returns (bytes)
```

#### Parameters:

| Name | Type | Description |
| :--- | :--- | :--- |
| `target` | address |  |
| `data` | bytes |  |
| `value` | uint256 |  |
| `errorMessage` | string |  |

### uncheckedFunctionStaticCall

```text
function uncheckedFunctionStaticCall(
  address target,
  bytes data,
  string errorMessage
) internal returns (bytes)
```

#### Parameters:

| Name | Type | Description |
| :--- | :--- | :--- |
| `target` | address |  |
| `data` | bytes |  |
| `errorMessage` | string |  |

