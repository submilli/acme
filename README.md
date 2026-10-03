# Acme example packages

The example packages the [Submilli](https://github.com/submilli/submilli-runtime)
book uses. Acme is the fictional company whose support agent the book
follows.

| Package | What it is |
| --- | --- |
| `@acme/billing` | A charge lookup over fixed data, standing in for a billing API. No credential needed. |

Install one into your local store:

```sh
submilli install submilli/acme @acme/billing
```

Build and test from a checkout:

```sh
submilli build test
submilli build publish-local
```
