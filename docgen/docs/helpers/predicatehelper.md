# PredicateHelper

A helper contract for executing boolean functions on arbitrary target call results

## Functions

### or

```text
function or(
  address[] targets,
  bytes[] data
) external returns (bool)
```

Calls every target with corresponding data

#### Parameters:

| Name | Type | Description |
| :--- | :--- | :--- |
| `targets` | address\[\] |  |
| `data` | bytes\[\] |  |

#### Return Values:

| Name | Type | Description |
| :--- | :--- | :--- |
| `Result` | address\[\] | True if call to any target returned True. Otherwise, false |

### and

```text
function and(
  address[] targets,
  bytes[] data
) external returns (bool)
```

Calls every target with corresponding data

#### Parameters:

| Name | Type | Description |
| :--- | :--- | :--- |
| `targets` | address\[\] |  |
| `data` | bytes\[\] |  |

#### Return Values:

| Name | Type | Description |
| :--- | :--- | :--- |
| `Result` | address\[\] | True if calls to all targets returned True. Otherwise, false |

### eq

```text
function eq(
  uint256 value,
  address target,
  bytes data
) external returns (bool)
```

Calls target with specified data and tests if it's equal to the value

#### Parameters:

| Name | Type | Description |
| :--- | :--- | :--- |
| `value` | uint256 | Value to test |
| `target` | address |  |
| `data` | bytes |  |

#### Return Values:

| Name | Type | Description |
| :--- | :--- | :--- |
| `Result` | uint256 | True if call to target returns the same value as `value`. Otherwise, false |

### lt

```text
function lt(
  uint256 value,
  address target,
  bytes data
) external returns (bool)
```

Calls target with specified data and tests if it's lower than value

#### Parameters:

| Name | Type | Description |
| :--- | :--- | :--- |
| `value` | uint256 | Value to test |
| `target` | address |  |
| `data` | bytes |  |

#### Return Values:

| Name | Type | Description |
| :--- | :--- | :--- |
| `Result` | uint256 | True if call to target returns value which is lower than `value`. Otherwise, false |

### gt

```text
function gt(
  uint256 value,
  address target,
  bytes data
) external returns (bool)
```

Calls target with specified data and tests if it's bigger than value

#### Parameters:

| Name | Type | Description |
| :--- | :--- | :--- |
| `value` | uint256 | Value to test |
| `target` | address |  |
| `data` | bytes |  |

#### Return Values:

| Name | Type | Description |
| :--- | :--- | :--- |
| `Result` | uint256 | True if call to target returns value which is bigger than `value`. Otherwise, false |

### timestampBelow

```text
function timestampBelow(
  uint256 time
) external returns (bool)
```

Checks passed time against block timestamp

#### Parameters:

| Name | Type | Description |
| :--- | :--- | :--- |
| `time` | uint256 |  |

#### Return Values:

| Name | Type | Description |
| :--- | :--- | :--- |
| `Result` | uint256 | True if current block timestamp is lower than `time`. Otherwise, false |

