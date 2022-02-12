# github-action-node-based-lambda-deploy

Base GitHub action that can be used to deploy any NodeJs based lambda

# Example:

<!-- start usage -->

```yaml
steps:
  - name: Run Zip and Deploy
    uses: nrccua/github-action-node-based-lambda-deploy@main
    with:
      name: datalab-super-score-scheduler
      product: datalab
      env: dev
      AWS_IAM_ROLE: ${{ inputs.roleName }}
      AWS_REGION: ${{ inputs.awsRegion }}
      AWS_S3_BUCKET: ${{ inputs.targetBucket }}
```

<!-- end usage -->
