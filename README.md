<img src="http://mrwconsulting.s3-website-us-east-1.amazonaws.com/.images/ciflex-platform.png"/>

The CiFlex CICD Platform is an AWS CodePipeline generator, streamlining pipeline creation by simplifying configuration for tasks such as building, unit testing, code style linting, and deploying. Its a fully managed continuous delivery service that automates AWS CodePipeline infrastructure, empowering DevOps teams to efficiently manage and automate their pipeline processes. With CiFlex, DevOps teams can create and publish plugins to introduce new features, enabling application teams to easily enhance their CICD workflows.

## **Pipeline Samples:**

List of plugins implemented by all samples: <br>
1.  pluginName: SAST-Codacy <br>
    pluginAliasName: SAST-Codacy <br>
    isActive: false <br>

2.  pluginName: SAST-Snyk <br>
    pluginAliasName: SAST-Snyk <br>
    isActive: false

3.  pluginName: 4.27-DinD <br>
    pluginAliasName: REGISTRY-DockerHub <br>
    isActive: true <br>

4.  pluginName: 4.27-DinD <br>
    pluginAliasName: REGISTRY-GitHub <br>
    isActive: false <br>

5.  pluginName: Manual-Approval <br>
    isActive: false <br>

6.  pluginName: EKS-Deployment <br>
    pluginAliasName: EKS <br>
    isActive: false <br>

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

2. springboot-kotlin <br>
    - pluginName: 8.5-Gradle
      pluginAliasName: OpenJDK
      isActive: true

3. springboot-gradle <br>
    - pluginName: 8.5-Gradle
      pluginAliasName: OpenJDK
      isActive: true

4. python-poety <br>
    - pluginName: 3.12-Poetry
      pluginAliasName: Python
      isActive: true

5. python-pip <br>
    - pluginName: 3.12-PiP
      pluginAliasName: Python
      isActive: true

### **Prerequisites**

- [NodeJS Version 20.12.1 or greater](https://nodejs.org/en/)
- [Docker Desktop Version 24.0.2 or greater](https://docs.docker.com/engine/install/)
- [AWS CLI Version 2.11.6 or greater](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)
- **CiFlex Token**: _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_ (30-Day License)

### **Provision Pipeline**
```bash
export AWS_ACCESS_KEY_ID=<AWS_ACCESS_KEY_ID>
export AWS_SECRET_ACCESS_KEY=<AWS_SECRET_ACCESS_KEY>

cd springboot-maven
../bin/access-token.sh 
export CIFLEX_ACCESS_TOKEN=<CIFLEX_ACCESS_TOKEN>
ciflexctl pipeline --deploy
```
