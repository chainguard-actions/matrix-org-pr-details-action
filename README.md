# pr-details-action
A Github Action for finding details about a PR relating to the workflow run

## Example for running from a `workflow_run` reacting to a `pull_request` workflow.

```yaml
steps:
  - id: details
    uses: matrix-org/pr-details-action@v1
    with:
      owner: ${{ github.event.workflow_run.head_repository.owner.login }}
      branch: ${{ github.event.workflow_run.head_branch }}
```

## Privacy

This Action contacts Chainguard's licensing server to verify authorization. Connection metadata (IP address, GitHub repository identifier, timestamp, and any metadata encoded in the auth token) is transmitted to Chainguard, Inc. even if authorization is denied in accordance with our [Privacy Notice](https://www.chainguard.dev/legal/privacy-notice)
