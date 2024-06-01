# Run Boman-CLI

This action runs the `boman-cli` tool with specified arguments.

## Inputs

### `action`

**Required** The action to perform. Default `"default-action"`.

### `failbuild`

**Optional** Whether to fail the build on error. Default `"false"`.

### `zap_session_script`

**Optional** Path to the ZAP session script. Default `""`.

### `config`

**Optional** Path to the config file. Default `""`.

### `use-sudo`

**Optional** Whether to run the command with `sudo`. Default `"false"`.

## Outputs

### `result`

The result of the `boman-cli` command.

## Example usage

```yaml
uses: i4mmaddy/boman-ai-action@v1
with:
  action: 'run' # or test-saas, test-yaml
  failbuild: 'high' #optional # or 'high' or 'medium or 'low'
  zap_session_script: 'path/to/your/zap_session_script' #optional
  config: 'path/to/your/config' #optional
  use-sudo: 'true' # or 'false' #optional

