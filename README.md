# Run Boman-CLI

This action runs the `boman-cli` tool with specified arguments.

## Inputs

### `args`

**Required** The arguments to pass to `boman-cli`. Default `"--help"`.

## Outputs

### `result`

The result of the `boman-cli` command.

## Example usage

```yaml
uses: i4mmaddy/boman-ai-action@v1
with:
  args: '-a run'
