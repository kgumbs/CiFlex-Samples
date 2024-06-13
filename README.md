<img src="http://mrwconsulting.s3-website-us-east-1.amazonaws.com/.images/ciflex-platform.png"/>

The CiFlex CICD Platform is an AWS CodePipeline generator, streamlining pipeline creation by simplifying configuration for tasks such as building, unit testing, code style linting, and deploying. Its a fully managed continuous delivery service that automates AWS CodePipeline infrastructure, empowering DevOps teams to efficiently manage and automate their pipeline processes. With CiFlex, DevOps teams can create and publish plugins to introduce new features, enabling application teams to easily enhance their CICD workflows.

## **Pipeline Samples:**

List of plugins implemented by all samples:
<ol>
    - pluginName: SAST-Codacy
      pluginAliasName: SAST-Codacy
      isActive: false
    - pluginName: SAST-Snyk
      pluginAliasName: SAST-Snyk
      isActive: false
    - pluginName: 4.27-DinD
      pluginAliasName: REGISTRY-DockerHub
      isActive: true
    - pluginName: 4.27-DinD
      pluginAliasName: REGISTRY-GitHub
      isActive: false
    - pluginName: Manual-Approval
      isActive: false
    - pluginName: EKS-Deployment
      pluginAliasName: EKS
      isActive: false
</ol>

List of plugins implemented by specific samples:
1. springboot-maven
    - pluginName: 3.9-Maven
      pluginAliasName: OpenJDK
      isActive: true
    - pluginName: 0.18-Trivy:Maven
      pluginAliasName: TRIVY-JiB
      isActive: false
    - pluginName: 0.18-Trivy:Maven
      pluginAliasName: TRIVY-BuildPack
      isActive: true

