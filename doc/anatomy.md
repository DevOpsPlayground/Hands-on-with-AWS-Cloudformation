# Cloud Formation Template Anatomy

[Home](../README.md) |
[AWS Console](https://console.aws.amazon.com) |
Anatomy |
[lab-001](lab-001.md) |
[lab-002](lab-002.md) |
[lab-003](lab-003.md) |
[lab-004](lab-004.md) |
[lab-005](lab-005.md) |
[lab-006](lab-006.md)

## Template Sections

- `AWSTemplateFormatVersion`
    - AWSTemplateFormatVersion: '2010-09-09' - date is the the cloudformation version that the template conforms to.
- `Description` - Text string that describes the template and _must_
- `Metadata` -
- `Parameters` -
- `Mappings` -
- `Conditions` -
- `Transforms` -
- `Resources` -
- `Output` -




#### YAML-formatted template fragment.
```
---
AWSTemplateFormatVersion: "version date"

Description:
  # String

Metadata:
  # template metadata

Parameters:
  # set of parameters

Mappings:
  # set of mappings

Conditions:
  # set of conditions

Transform:
  # set of transforms

Resources:
  # set of resources (REQUIRED)

Outputs:
  # set of outputs
```


#### JSON-formatted template fragment
```
{
  "AWSTemplateFormatVersion" : "version date",

  "Description" : "JSON string",

  "Metadata" : {
    template metadata
  },

  "Parameters" : {
    set of parameters
  },

  "Mappings" : {
    set of mappings
  },

  "Conditions" : {
    set of conditions
  },

  "Transform" : {
    set of transforms
  },

  "Resources" : {
    set of resources
  },

  "Outputs" : {
    set of outputs
  }
}
```

## Notes
- When writing templates use YMAL its easier to read and work with.

## Further Reading




## References
1. AWS Docs - [Template Anatomy](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/template-anatomy.html)
1. [Convert JSON to YAML online](https://www.json2yaml.com/)
1. AWS Console (us-east-1) [CloudFormation Designer](https://console.aws.amazon.com/cloudformation/designer/home?region=us-east-1)
