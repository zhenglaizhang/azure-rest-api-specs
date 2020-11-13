## Ruby

These settings apply only when `--ruby` is specified on the command line.

```yaml
package-name: azure_mgmt_testservice1
package-version: 2020-11-13
azure-arm: true
```

### Tag: package-2020-11-13 and ruby

These settings apply only when `--tag=package-2020-11-13 --ruby` is specified on the command line.
Please also specify `--ruby-sdks-folder=<path to the root directory of your azure-sdk-for-ruby clone>`.

```yaml $(tag) == 'package-2020-11-13' && $(ruby)
namespace: Microsoft.TestService1
output-folder: $(ruby-sdks-folder)/testservice1
```
