# Legendary AWS DevOps Project 🚀

This project showcases a complete end-to-end CI/CD pipeline using AWS Developer Tools to deploy a Java web application on an EC2 instance. The pipeline is designed to automate every phase of software delivery — from coding to deployment — using tools like CodeArtifact, CodeBuild, CodeDeploy, and CodePipeline.

## 📁 Project Structure

This project was completed over 5 days, each covering a critical component of the DevOps lifecycle:

### ✅ Part 1 - Set Up EC2 & VS Code Integration
- Launched an EC2 instance to serve as a development environment.
- Configured key pairs for SSH access.
- Connected EC2 with Visual Studio Code using the Remote - SSH extension.
- Created a Java web app using Maven and `index.jsp`.

### ✅ Part 2 - Connect GitHub with AWS
- Initialized a local Git repository.
- Pushed source code to GitHub with secure authentication using a personal access token.
- Learned Git concepts like `add`, `commit`, and `push`.

### ✅ Part 3 - Configure CodeArtifact
- Created a CodeArtifact domain and repository to manage dependencies securely.
- Attached IAM policies to EC2 for CodeArtifact access.
- Configured `settings.xml` for Maven to pull dependencies from CodeArtifact.

### ✅ Part 4 - Automate Build with CodeBuild
- Created a CodeBuild project to compile and package the web app.
- Set up `buildspec.yml` to define build steps.
- Stored build artifacts in an S3 bucket.
- Enabled CloudWatch logging for monitoring build jobs.

### ✅ Part 5 - Deploy with CodeDeploy
- Used CloudFormation to provision a production EC2 environment.
- Wrote deployment scripts (`install_dependencies.sh`, `start_server.sh`, `stop_server.sh`).
- Created an `appspec.yml` to orchestrate deployment events.
- Configured a CodeDeploy application and deployment group.
- Verified successful deployment from CodeDeploy Console.

---

## ⚙️ Tools & Services Used

- **AWS EC2**
- **AWS CodeArtifact**
- **AWS CodeBuild**
- **AWS CodeDeploy**
- **AWS CodePipeline**
- **Amazon S3**
- **GitHub**
- **VS Code**
- **CloudWatch Logs**
- **CloudFormation**
- **Maven + Java (Amazon Corretto 8)**

---

## 📦 Artifacts & Config Files

- `index.jsp` – Web app homepage
- `buildspec.yml` – CI build instructions
- `appspec.yml` – Deployment lifecycle configuration
- `settings.xml` – Maven repository configuration
- Deployment scripts – Shell scripts to manage servers

---

## ✅ Final Output

Live deployment of the Java web application hosted on an EC2 instance with full CI/CD automation.

---

## 🙌 Author

**Rushabh Satarkar**  
[LinkedIn Profile](https://linkedin.com/in/rushabh-satarkar-2244ab190) 
