# CloudFormation

- **Template** = Infrastructure described as code (JSON / YAML)
- **Stack** = Resources actually created as described in a template
  - Can be *updated* by a new template, updates are `diff`'d
  - Can be *nested*
- **StackSet** = Multiple stacks working as a whole

## Syntax

### Join with Ref

```
!Join
  - '-'
  - - !Ref AWS::Region
    - p-data-dash-code-deploy
```

## CodeDeploy

### TagFilters & TagSet ###

- **TagFilters** = a list of TagFilter, select instances that match any tag
- **TagSet** = see below, must match all tags to proceed

```
Ec2TagSet:
  Ec2TagSetList:
    - Ec2TagGroup:
      - Key: project
        Value: data-dash
        Type: KEY_AND_VALUE
    - Ec2TagGroup:
      - Key: environment
        Value: production
        Type: KEY_AND_VALUE
```

## Other

### Referring to AWS managed policies

- Use ARN directly as they do not change, e.g. `arn:aws:iam::aws:policy/AlexaForBusinessDeviceSetup`

### Don't forget double colon (::)

- `AWS::IAM:Role` is missing a colon

### Lambda macros

- Lambda macros can be used to make templates more dynamic but may make managing templates harder
