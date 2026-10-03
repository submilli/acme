# Acme example packages

The example packages the [Submilli](https://github.com/submilli/submilli-runtime)
book uses. Acme is the fictional company whose support agent the book
follows. The packages are scoped `@submilli/` because a package's scope
must be the GitHub owner it is installed from; the `acme-` prefix keeps
them apart from the curated ones.

| Package | What it is |
| --- | --- |
| `@submilli/acme-billing` | A charge lookup over fixed data, standing in for a billing API. No credential needed. |

Install one into your local store:

```sh
submilli install submilli/acme @submilli/acme-billing
```

Build and test from a checkout:

```sh
submilli build test
submilli build publish-local
```
