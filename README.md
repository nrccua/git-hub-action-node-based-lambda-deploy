# git-hub-action-node-based-lambda-deploy

Base GitHub action that can be used to deploy any NodeJs based lambda

# How to use:

```
jobs:
  deploy:
    uses: nrccua/git-hub-action-node-based-lambda-deploy/.github/workflows/action.yml@main
    with:
      name: datalab-super-score-scheduler
      product: datalab
      env: dev|stage|prod
      branch: development|staging|main|master
    secrets:
      PAT: ${{ secrets.PAT }}
      AWS_ACCESS_KEY_ID: ${{ secrets.AWS_ACCESS_KEY_ID }}
      AWS_SECRET_KEY_ID: ${{ secrets.AWS_SECRET_KEY_ID }}
      AWS_REGION: ${{ secrets.AWS_REGION }}
      AWS_S3_BUCKET:  ${{ secrets.AWS_S3_BUCKET }}
```
