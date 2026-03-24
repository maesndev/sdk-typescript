# TransactionResponseDtoType

## Example Usage

```typescript
import { TransactionResponseDtoType } from "maesn/models";

let value: TransactionResponseDtoType = "RECEIVE-OVERPAYMENT";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"RECEIVE" | "RECEIVE-OVERPAYMENT" | "RECEIVE-PREPAYMENT" | "SPEND" | "SPEND-OVERPAYMENT" | "SPEND-PREPAYMENT" | "RECEIVE-TRANSFER" | "SPEND-TRANSFER" | Unrecognized<string>
```