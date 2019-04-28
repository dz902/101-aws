# CodeDeploy

**CodeDeploy** puts binaries to instances. It does not work on its own, must be  as a stage in **CodePipelin**.

- **Application** = Configuration of the application to be deployed
  - **ComputePlatform** = _Server (EC2/On-premise)_, _ECS_ or _Lambda_
- **Deployment** = Actual event of deploying the application
- **DeploymentGroup** = Targets for a deployment

# Service Role

- **AWSCodeDeployServiceRole** = Predefined _policy_ (despite its name) for CodeDeploy
