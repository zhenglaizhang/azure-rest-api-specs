## Python

These settings apply only when `--python` is specified on the command line.
Please also specify `--python-sdks-folder=<path to the root directory of your azure-sdk-for-python clone>`.


``` yaml $(python)
python: 
    azure-arm: true
    license-header: MICROSOFT_MIT_NO_VERSION
    package-name: azure-mgmt-testcli
    no-namespace-folders: true
    package-version: 1.0.0b1
```

``` yaml $(python-mode) == 'update'
python:
    output-folder: $(python-sdks-folder)/testcli/azure-mgmt-testcli/azure/mgmt/testcli
```
``` yaml $(python-mode) == 'create'
python:
    basic-setup-py: true
    output-folder: $(python-sdks-folder)/testcli/azure-mgmt-testcli
```

``` yaml $(python) && $(track2)
azure-arm: true
license-header: MICROSOFT_MIT_NO_VERSION
package-name: azure-mgmt-testcli
no-namespace-folders: true
package-version: 1.0.0b1
```

``` yaml $(python-mode) == 'update' && $(track2)
output-folder: $(python-sdks-folder)/testcli/azure-mgmt-testcli/azure/mgmt/testcli
```
``` yaml $(python-mode) == 'create' && $(track2)
basic-setup-py: true
output-folder: $(python-sdks-folder)/testcli/azure-mgmt-testcli
```
