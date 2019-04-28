# CloudFormation

- **Template** = Infrastructure described as code (JSON / YAML)
- **Stack** = Resources actually created as described in a template
  - Can be *updated* by a new template, updates are `diff`'d
  - Can be *nested*
- **StackSet** = Multiple stacks working as a whole

# Referring to AWS managed policies

- Use ARN directly as they do not change, e.g. `arn:aws:iam::aws:policy/AlexaForBusinessDeviceSetup`
