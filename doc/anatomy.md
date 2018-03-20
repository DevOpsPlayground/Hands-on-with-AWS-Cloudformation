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
    - (Optional) AWSTemplateFormatVersion: '2010-09-09' - date is the the cloudformation version that the template conforms to.
- `Description` - Text string that describes the template and _must_ if present come after `AWSTemplateFormatVersion`
- `Metadata` - (Optional) provides additional information about the template. Can use to provide more meaning labels to Console.
- `Parameters` - (Optional) Specifies values that you can pass in to your template at runtime (when you create or update a stack). You can refer to parameters in the Resources and Outputs sections of the template.
- `Mappings` - (Optional) A mapping of keys and associated values that you can use to specify conditional parameter values, similar to a lookup table. You can match a key to a corresponding value by using the `Fn::FindInMap` intrinsic function in the Resources and Outputs section.
- `Conditions` - (Optional) Defines conditions that control whether certain resources are created or whether certain resource properties are assigned a value during stack creation or update. 
- `Transforms` - (Optional) For serverless applications (Lambda-based applications), specifies the version of the AWS Serverless Application Model (AWS SAM) to use. 
- `Resources` - (Required) Specifies the stack resources and their properties, such as an EC2 instance or an S3 bucket. You can refer to resources in the `Resources` and `Outputs` sections of the template.
- `Output` - Describes the values that are returned whenever you view your stack's properties.



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
- __HEADERS__ - Description of what your stack does, contains, etc.
- __PARAMETERES__ - Provision time values that add structured flexibility and customisation
- __MAPPINGS__ - Pre-defined conditional case statements
- __CONDITIONALS__ - Conditional values set via evaluations of passed References
- __RESOURCES__ - AWS resource definitions
- __OUTPUTS__ - Resulting attributes of stack resource creation


## Further Reading




## References
1. AWS Docs - [Template Anatomy](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/template-anatomy.html)
1. [Convert JSON to YAML online](https://www.json2yaml.com/)
1. AWS Console (us-east-1) [CloudFormation Designer](https://console.aws.amazon.com/cloudformation/designer/home?region=us-east-1)
