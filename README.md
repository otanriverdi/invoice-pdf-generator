
# PDF Generator

The goal with this.

1. Create a PDF invoice given some data about a customer's recent transactions

### Creating a PDF invoice

Given data like the following, generates a PDF invoice.

```go
data := []struct {
  UnitName       string
  PricePerUnit   int
  UnitsPurchased int
}{
  {
    UnitName:       "2x6 Lumber - 8'",
    PricePerUnit:   375, // in cents
    UnitsPurchased: 220,
  }, {
    UnitName:       "Drywall Sheet",
    PricePerUnit:   822, // in cents
    UnitsPurchased: 50,
  }, {
    UnitName:       "Paint",
    PricePerUnit:   1455, // in cents
    UnitsPurchased: 3,
  },
}
```
