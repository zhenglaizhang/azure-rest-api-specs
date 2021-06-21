# testdp

> see https://aka.ms/autorest

This is the AutoRest configuration file for testdp.

## Getting Started

To build the SDKs for My API, simply install AutoRest via `npm` (`npm install -g autorest`) and then run:

> `autorest readme.md`

To see additional help and options, run:

> `autorest --help`

For other options on installation see [Installing AutoRest](https://aka.ms/autorest/install) on the AutoRest github page.

---

## Configuration

### Basic Information

These are the global settings for the testdp.

```yaml
openapi-type: data-plane
tag: package-v0.1
```

### Tag: package-v0.1

These settings apply only when `--tag=package-v0.1` is specified on the command line.

```yaml $(tag) == 'package-v0.1'
input-file:
  - Microsoft.TestDp/preview/v0.1/testdp.json
```
