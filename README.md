<img src="http://mrwconsulting.s3-website-us-east-1.amazonaws.com/.images/ciflex-platform.png"/>

The CiFlex CICD Platform is an AWS CodePipeline generator, streamlining pipeline creation by simplifying configuration for tasks such as building, unit testing, code style linting, and deploying. Its a fully managed continuous delivery service that automates AWS CodePipeline infrastructure, empowering DevOps teams to efficiently manage and automate their pipeline processes. With CiFlex, DevOps teams can create and publish plugins to introduce new features, enabling application teams to easily enhance their CICD workflows.

## **Pipeline Samples:**

List of plugins implemented by all samples: <br>
<ol>
```
    - pluginName: SAST-Codacy <br>
      pluginAliasName: SAST-Codacy <br>
      isActive: false <br>
      
    - pluginName: SAST-Snyk <br>
      pluginAliasName: SAST-Snyk <br>
      isActive: false

    - pluginName: 4.27-DinD <br>
      pluginAliasName: REGISTRY-DockerHub <br>
      isActive: true <br>

    - pluginName: 4.27-DinD <br>
      pluginAliasName: REGISTRY-GitHub <br>
      isActive: false <br>

    - pluginName: Manual-Approval <br>
      isActive: false <br>

    - pluginName: EKS-Deployment <br>
      pluginAliasName: EKS <br>
      isActive: false <br>
```
</ol>

List of plugins implemented by specific samples: <br>
1. springboot-maven <br>
    - pluginName: 3.9-Maven <br>
      pluginAliasName: OpenJDK <br>
      isActive: true <br>
    - pluginName: 0.18-Trivy:Maven <br>
      pluginAliasName: TRIVY-JiB <br>
      isActive: false <br>
    - pluginName: 0.18-Trivy:Maven <br>
      pluginAliasName: TRIVY-BuildPack <br>
      isActive: true <br>

