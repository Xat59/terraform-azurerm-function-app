# v5.1.0 - 2022-02-11

Added
  * AZ-615: Add an option to enable or disable default tags

# v5.0.0 - 2022-01-13

Breaking
  * AZ-515: Option to use Azure CAF naming provider to name resources
  * AZ-515: Require Terraform 0.13+

# v4.2.0 - 2021-11-18

Changed
  * AZ-572: Revamp examples and improve CI
  * AZ-592: Bump minimum AzureRM provider version to `v2.57`

Added
  * AZ-588: VNet integration option
  * AZ-592: Support for the `site_config.ip_restrictions.headers` property
  * AZ-595: SCM parameters now uses dedicated variables, like in `app-service-web` module

Fixed
  * AZ-589: Avoid plan drift when specifying Diagnostic Settings categories

# v4.1.0 - 2021-09-07

Breaking
  * AZ-565: Add `client_name` to default storage account name

Fixed
  * AZ-530: Fix unused `https_only` variable

Changed
  * AZ-532: Revamp README with latest `terraform-docs` tool

# v4.0.1 - 2021-07-21

Fixed
  * AZ-534: Fix `is-local-zip` for default value of `application_zip_package_path` at `null`

# v4.0.0 - 2021-07-16

Added
  * AZ-488: Merge `function-app-with-plan`  `function-app-single` modules with the second as submodule.
  * AZ-486: Allow deploying ZIP packages

Changed
  * AZ-489: Reuse existing variable for `function_app_os_type`
  * AZ-160: Unify diagnostics settings on all Claranet modules
  * AZ-488: Refactor variables

Fixed
  * AZ-489: Fix submodule default value for `function_app_version`
  * AZ-489: Force user to define `storage_account_name` if `storage_account_primary_access_key` is set
  * AZ-489: Set setting `WEBSITES_ENABLE_APP_SERVICE_STORAGE` to false when using custom Docker image (Azure issue)
