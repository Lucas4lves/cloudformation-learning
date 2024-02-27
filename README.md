# Learning Cloud Formation

 * A record of my developments on IaC with Cloud Formation


## Updating a Stack:

 * Depends on the attributes changed within a AWS resource:

   * WITH NO INTERRUPTION: does not change physical ID nor its service availability;
   * WITH SOME INTERRUPTION: does not change physical ID and blocks service availability for a while;
   * REPLACEMENT: changes physical ID (recreate resources from ground up);

## Template Options

### Tags: 
    - Enables identifiying resources with up to 100 customized tags
    - Its format has to be captalized: Key: Value
### Permissions:
    - Sets permissions based on Users or ARN's within a Stack;
### Notifications:
    - Specifies a SNS topic to receive notifications on a determined stack; 
### Timeout:
    - Sets how much time to wait before performing a Rollback;
    - It is based on notifications/alarms;
### Rollback on Failure:
    - Part of "Stack Creation Options", sets a default behavior for stack create/update failure scenarios;
    - We're able to delete all new resources, or retain everything created;

## Deploying a Template

 * Manually: through AWS Console CloudFormation resource;

 * Automated: using YAML templates, the AWS CLI tool and a CD tool;