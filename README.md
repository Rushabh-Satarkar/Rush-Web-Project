# DevOps Project: CI/CD Pipeline with AWS Developer Tools 🚀

This repository documents a 6-day, end-to-end DevOps journey where I built and automated the deployment of a Java web application using native AWS services like CodeBuild, CodeDeploy, CodePipeline, CodeArtifact, and EC2.

---

## 📅 Project Breakdown

### ✅ Part 1: Setup Cloud Dev Environment (EC2 + VS Code)
- Launched EC2 instance (Amazon Linux 2)
- Connected EC2 to VS Code via Remote SSH
- Installed Java, Maven, Git
- Created a basic Java web application using Maven archetypes
- Edited `index.jsp` as our entry point

### ✅ Part 2: Source Code Management with GitHub
- Initialized Git in EC2
- Created remote GitHub repository
- Configured Git username & email
- Used GitHub token to push code securely

### ✅ Part 3: Secure Dependencies with AWS CodeArtifact
- Created CodeArtifact domain & repository
- Configured `settings.xml` to pull dependencies via Maven
- Attached IAM role with permissions to generate authorization token

### ✅ Part 4: Build Automation with AWS CodeBuild
- Created a `buildspec.yml` to compile and package the `.war` file
- Connected CodeBuild with GitHub via CodeConnection
- Stored artifacts in S3 bucket
- Enabled CloudWatch for build monitoring

### ✅ Part 5: Deployment Automation with AWS CodeDeploy
- Created deployment scripts (`install_dependencies.sh`, `start_server.sh`, etc.)
- Defined deployment lifecycle in `appspec.yml`
- Set up CodeDeploy application & deployment group
- Verified application deployed to EC2 successfully

### ✅ part 6: Full CI/CD with AWS CodePipeline
- Created CodePipeline with Source → Build → Deploy stages
- Enabled webhook triggers for auto-builds on every `git push`
- Validated changes reflected immediately on the live app

---

## 🛠️ Tools & Services Used

- **Cloud**: AWS EC2, S3, CodePipeline
- **Build & Deploy**: CodeBuild, CodeDeploy
- **Artifact Repository**: CodeArtifact
- **Source Control**: Git, GitHub
- **Monitoring**: Amazon CloudWatch
- **Languages**: Java (Amazon Corretto 8), JSP
- **IDE**: Visual Studio Code

---

## 🌐 Final Result

An automatically deployed Java web app on EC2 with changes from GitHub instantly pushed live via a fully configured CI/CD pipeline.

---

## 👨‍💻 Author

**Rushabh Satarkar**  
DevOps Enthusiast | Cloud Learner | Automation Explorer  
[LinkedIn Profile](https://linkedin.com/in/rushabh-satarkar-2244ab190)
