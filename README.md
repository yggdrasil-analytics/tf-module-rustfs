# tf-module-rustfs

Terraform module that deploys RustFS, an S3-compatible object store for local development and testing.

This is not used on AWS. Production AWS deployments use native S3.

This is a reusable module. Another Terraform project calls it and supplies the inputs.

## Usage

```hcl
module "rustfs" {
  source = "git::https://github.com/yggdrasil-analytics/tf-module-rustfs.git"
}
```

Pin the source with `?ref=<tag>` so callers get a fixed version rather than whatever is on `main`.
