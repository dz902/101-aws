# CodeDeploy

- **Application** = Configuration of the application to be deployed
  - **ComputePlatform** = _Server (EC2/On-premise)_, _ECS_ or _Lambda_
- **Deployment** = Actual event of deploying the application
- **DeploymentGroup** = Targets for a deployment

# Service Role

- **Service Role** = IAM Role with permission to operate ELB, EC2, etc.
- **AWSCodeDeployServiceRole** = Predefined _policy_ (despite its name) for CodeDeploy
- 
