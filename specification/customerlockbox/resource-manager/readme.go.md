## Go

These settings apply only when `--go` is specified on the command line.

```yaml $(go)
go:
  license-header: MICROSOFT_MIT_NO_VERSION
  clear-output-folder: true
```

### Tag: package-2018-02-28-preview and go

These settings apply only when `--tag=package-2018-02-28-preview --go` is specified on the command line.
Please also specify `--go-sdks-folder=<path to the root directory of your azure-sdk-for-go clone>`.

```yaml $(tag) == 'package-2018-02-28-preview' && $(go)
namespace: customerlockbox
output-folder: $(go-sdk-folder)/services/preview/$(namespace)/mgmt/2018-02-28-preview/$(namespace)
```
