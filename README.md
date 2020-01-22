
# ColorTeller App, ECS Fargate, ALB and AppMesh

This is a port of the work in https://github.com/aws/aws-app-mesh-examples/tree/master/examples/apps/colorapp/ecs

It is a reference architecture for using CDK to create the colorapp and its components.

This creates:
  * VPC
  * ECS Cluster
  * Fargate Tasks for the ColorTeller App
  * Service Discovery
  * ALB
  * AppMesh

Source for colorteller containers is from aws-app-mesh-examples.

VPC endpoints can be expensive and we create one in the network stack.

Some modules of AWS CDK are considered experimental and have been used in this example. It may not work with versions older than aws-cdk 1.20.0. It is unlikely that
I will update as time goes by.
