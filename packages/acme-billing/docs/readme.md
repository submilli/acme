# Billing

Use `@submilli/acme-billing` to list the charges on one customer's account. The
package reads fixed data, so it needs no credential: it stands in for a
real billing API in the Submilli book's examples.

- `listCharges(customerId)` returns the customer's charges, each with the
  customer, an id, and an amount in cents.

A denial means the blueprint does not allow the customer asked for; do
not retry with another id.

```ts
import { listCharges } from "@submilli/acme-billing";

function main(): string {
    const charges = listCharges("cus_northwind");
    return `${charges.length} charges`;
}
```
