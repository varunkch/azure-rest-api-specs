# OperationsManagement
    
> see https://aka.ms/autorest

This is the AutoRest configuration file for OperationsManagement



---
## Getting Started 
To build the SDK for OperationsManagement, simply [Install AutoRest](https://aka.ms/autorest/install) and in this folder, run:

> `autorest`

To see additional help and options, run:

> `autorest --help`
---

## Configuration



### Basic Information 
These are the global settings for the OperationsManagement API.

``` yaml
title: OperationsManagementClient
description: Operations Management Client
openapi-type: arm
tag: package-2015-11-preview
```


### Tag: package-2015-11-preview

These settings apply only when `--tag=package-2015-11-preview` is specified on the command line.

``` yaml $(tag) == 'package-2015-11-preview'
input-file:
- Microsoft.OperationsManagement/preview/2015-11-01-preview/OperationsManagement.json
```


---
# Code Generation


## C#

These settings apply only when `--csharp` is specified on the command line.
Please also specify `--csharp-sdks-folder=<path to "SDKs" directory of your azure-sdk-for-net clone>`.

```yaml $(csharp)
csharp:
  # last generated using AutoRest.1.0.0-Nightly20170126 
  azure-arm: true
  namespace: Microsoft.Azure.Management.OperationsManagement
  payload-flattening-threshold: 1
  license-header: MICROSOFT_MIT_NO_VERSION
  output-folder: $(csharp-sdks-folder)/OperationsManagement/Management.OperationsManagement/Generated
  clear-output-folder: true
```


## Go

These settings apply only when `--go` is specified on the command line.

``` yaml $(go)
go:
  license-header: MICROSOFT_APACHE_NO_VERSION
  namespace: operationsmanagement
  clear-output-folder: true
```

### Tag: package-2015-11-preview and go

These settings apply only when `--tag=package-2015-11-preview --go` is specified on the command line.
Please also specify `--go-sdk-folder=<path to the root directory of your azure-sdk-for-go clone>`.

``` yaml $(tag) == 'package-2015-11-preview' && $(go)
output-folder: $(go-sdk-folder)/services/operationsmanagement/mgmt/2015-11-01-preview/operationsmanagement
```
