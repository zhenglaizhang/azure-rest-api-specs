## Go

These settings apply only when `--go` is specified on the command line.

```yaml $(go)
go:
  license-header: MICROSOFT_MIT_NO_VERSION
  namespace: test0002
  clear-output-folder: true
```

### Go multi-api

``` yaml $(go) && $(multiapi)
batch:
  - tag: package-1990-01-01[[-ReleaseState]]
```

### Tag: package-1990-01-01[[-ReleaseState]] and go

These settings apply only when `--tag=package-1990-01-01[[-ReleaseState]] --go` is specified on the command line.
Please also specify `--go-sdk-folder=<path to the root directory of your azure-sdk-for-go clone>`.

```yaml $(tag) == 'package-1990-01-01[[-ReleaseState]]' && $(go)
output-folder: $(go-sdk-folder)/services[[/ReleaseState]]/$(namespace)/mgmt/1990-01-01/$(namespace)
```
