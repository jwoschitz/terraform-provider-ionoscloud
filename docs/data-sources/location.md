---
layout: "ionoscloud"
page_title: "IonosCloud: location"
sidebar_current: "docs-datasource-location"
description: |-
  Get information on a IonosCloud Locations
---

# ionoscloud\_location

The locations data source can be used to search for and return an existing location which can then be used elsewhere in the configuration.

## Example Usage

```hcl
data "ionoscloud_location" "loc1" {
  name    = "karlsruhe"
  feature = "SSD"
}
```

## Argument Reference

 * `name` - (Required) Name or part of the location name to search for.
 * `feature` - (Optional) A desired feature that the location must be able to provide.

## Attributes Reference

 * `id` - UUID of the location
