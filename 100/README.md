# 100 - Get started: Install the CLI

You can install the CLI with a curl utility script, brew or by downloading the binary from the releases page. Once installed you'll get the faas-cli command and faas alias.

Utility script with curl:
```
$ curl -sSL https://cli.openfaas.com | sudo sh
```

Non-root with curl (requires further actions as advised after downloading):
```
$ curl -sSL https://cli.openfaas.com | sh
```

Via brew:
```
$ brew install faas-cli
```
Note: The brew release may not run the latest minor release but is updated regularly.

Via npm (coming soon):
```
$ npm install --global @openfaas/faas-cli
```
Note: See npm specific installation instructions and usage in the [npm README.md](https://github.com/openfaas/faas-cli/blob/master/npm/README.md)
## Windows
To install the faas-cli on Windows go to [Releases](https://github.com/openfaas/faas-cli/releases) and download the latest faas-cli.exe.

Or in PowerShell:
```
$version = (Invoke-WebRequest "https://api.github.com/repos/openfaas/faas-cli/releases/latest" | ConvertFrom-Json)[0].tag_name
(New-Object System.Net.WebClient).DownloadFile("https://github.com/openfaas/faas-cli/releases/download/$version/faas-cli.exe", "faas-cli.exe")
```

## Build from source
The [contributing guide](https://github.com/openfaas/faas-cli/blob/master/CONTRIBUTING.md) has instructions for building from source and for configuring a Golang development environment.
