# CodeDeploy

- **Application** = The configuration of the application to be deployed
  - **ComputePlatform** = _Server (EC2/On-premise)_, _ECS_ or _Lambda_
- **Deployment** = The actual event of deploying the application
- **DeploymentGroup** = Targets for a deployment

# Service Role

- CodeDeploy assumes a role to acquire permissions to interact with resources
- **AWSCodeDeployServiceRole** is a predefined _policy_ (despite its name) for CodeDeploy
