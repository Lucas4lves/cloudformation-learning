# Parameters

## Theory 

 - It is how users are able to provide input to CF Templates;
 - Adds up reusability to templates across an organization;
 - Type-check parameters may improve stack creating/updating security;

## Settings

### Type
    - String;
    - Number;
    - CommaDelimitedList;
    - List<Number>
    - AWS Specific (regarding data of your own account or resources);
    - List<AWS-Specific>:

## Description

## Constraint Description

## Min/MaxLength
## Min/MaxValue
## Default
## Allowed Patterns (regex)
## Allowed Values (arr)
## NoEcho (bool)


## Referencing 

 - Fn::Ref function is used to reference parameters almost anywhere;
 - Exceptions: AWSTemplateFormatVersion, Description, Transform, Mappings;
 - Shorthand: !Ref (YAML)
<br>

# Systems Manager Parameter Store (SSM)

 - Globally available CloudFormation Template Parameters;

## Use Cases:

 - Fetch latest AMI IDs
