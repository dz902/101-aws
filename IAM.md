# IAM

- **User** = Permanent identity with credentials, can attach policies
- **Group** = Group attached with policies to be acquired by members
- **Role** = Group of policies that can be assumed at run time by a user
  - **Service Role** = Role to be assumed by AWS services

# Defining permissions with policies

- **Statement** = Permission to allow / deny access to resources to a user
- **Policy** = Collection of statements with a name
- **Principal** = User, AWS service, etc.
  - **Service (Principal)** = AWS service represented as URI, e.g. `codedeploy.amazonaws.com`
  - Inline only, cannot be set for policies attached to a user or role
- **Action** = API call
- **Effect** = Allow or deny

# Assume role with STS

- `sts::AssumeRole` = API used to get a temporary token for assuming a role
