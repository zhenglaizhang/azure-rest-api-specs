## AzureResourceSchema

These settings apply only when `--azureresourceschema` is specified on the command line.

### AzureResourceSchema multi-api

``` yaml $(azureresourceschema) && $(multiapi)
batch:
  - tag: schema-tianenapimanagement-2020-09-22
  
```

Please also specify `--azureresourceschema-folder=<path to the root directory of your azure-resource-manager-schemas clone>`.

### Tag: schema-tianenapimanagement-2020-09-22 and azureresourceschema

``` yaml $(tag) == 'schema-tianenapimanagement-2020-09-22' && $(azureresourceschema)
output-folder: $(azureresourceschema-folder)/schemas

# all the input files in this apiVersion
input-file:
  - Microsoft.TianenApiManagement/preview/2020-09-22/tianenapimanagement.json
```
