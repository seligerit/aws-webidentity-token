# aws-webidentity-token action

This action configures a web identity token issued by github for accessing AWS.

## Inputs

### `aws-role-arn`

**Required** Specify the arn of the AWS role that should be assumed via the token.

### `aws-default-region`

**Optional** Specify a AWS default region.
**Default:** `eu-central-1`

### `aws-token-file`

**Optional** Path to AWS web identity token file
**Default:** `/tmp/awscreds`

## Example usage
```
uses: seligerit/aws-webidentity-token@v1
with:
  aws-role-arn: 'arn:aws:iam::123456789012:role/GitHub-Access'
```
