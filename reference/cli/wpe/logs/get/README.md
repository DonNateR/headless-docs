# wpe  logs get

## Description
Get the application logs for the WP Engine Headless CLI.

## Usage

```bash
$ wpe logs get [OPTIONS]
```

## Extended Description

The `wpe logs get` command will print the current account logs that the WP Engine Headless CLI is using to deploy applications.

## Options

| Name, shorthand     | Description  |
|:--------------------|:-------------|
| `--help, -h`        | Help for get |

## Examples

Let's assume the environment ID is `bmna3gedlzerwcb4vc04gssl` and the app name is `myapp`. Running the following command will print the logs for the environment:

```bash
$ wpe logs get -e bmna3gedlzerwcb4vc04gssl -a myapp
```

The above command will print something similar to the following:

```text
TIMESTAMP               SEVERITY        MESSAGE
2021-01-01T00:00:46Z    Info
2021-01-01T00:00:46Z    Info            > myapp@1.0.0 start /app/repo
2021-01-01T00:00:46Z    Info            > next start -p 8080
2021-01-01T00:00:46Z    Info
2021-01-01T00:00:47Z    Info            ready - started server on http://localhost:8080
```

## Parent Command
| Command                                         | Description               |
|:------------------------------------------------|:--------------------------|
| [wpe  logs](/reference/cli/wpe/logs) | The base command for logs |
