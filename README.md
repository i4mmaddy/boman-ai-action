# Run Boman-CLI

This action runs the `boman-cli` tool with specified arguments.



## Example usages



```yaml
- name: boman-ai-action
  uses: i4mmaddy/boman-ai-action@v7
            
```

### Advance Options


```yaml
uses: i4mmaddy/boman-ai-action@v7
with:
  action: 'run' #optional default is run. other values are test-saas, test-yaml
  failbuild: 'all' #optional values are 'high' or 'medium or 'low'
  zap_session_script: 'path/to/your/zap_session_script' #optional 
  config: 'path/to/your/config' #optional Pass path to the custom boman.yaml file
  use-sudo: 'true' #optinal Pass 'false' if sudo is not required



## Inputs

### `action`

**Optional** The action to perform. Default `"run"`.

### `failbuild`

**Optional** Whether to fail the build on error. Default `"false"`.

### `zap_session_script`

**Optional** Path to the ZAP session script. Default `"session_management.js"`.

### `config`

**Optional** Path to the config file. Default `"boman.yaml"`.

### `use-sudo`

**Optional** Whether to run the command with `sudo`. Default `"true"`.

## Outputs

### `result`

The result of the `boman-cli` command.

