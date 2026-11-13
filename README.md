# Tinyjs Build
Just an action to build tinyjs apps

## Usage
### Inputs

```yml
- uses: DreamLateXD/tinyjs-build-action@v1
  with:
    # Name of the artifact to upload.
    # Optional. Default is 'tinyjs-app'
    name:

    # Run `tinyjs publish` instead of `tinyjs build`
    # Optional. Default is 'true'
    publish:

    # Upload built files or not
    # Optional. Default is 'false'
    upload-artifact:
```

### Outputs

| Name | Description | Example |
| ---- | ----------- | ------- |
| `artifact-id` | GitHub ID of an Artifact, can be used by the REST API, only exists when `inputs.upload-artifact` is `true` | `1234` |
