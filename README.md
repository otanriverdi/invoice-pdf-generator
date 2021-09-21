
# PDF Generator

There are two goals with this.

1. Create a PDF invoice given some data about a fake customer's recent transactions
2. Generate a course completion certificate and add your name to it!

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
