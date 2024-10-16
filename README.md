# About the project
Creation of an interactive website where learners can exchange their experiences and knowledge. The objective is to promote collaborative
learning by enabling users to share their ideas, ask questions, and explore computer science challenges together.
 ## Built with
- **Front-End:** Angular, Bootstrap, TypeScript.
- **Backend:** Spring Boot
- **DataBases:** Mysql.
- ## Demo
[![Watch the video](https://github.com/EYABA12/code-warriors/blob/master/screenshot.PNG)](https://vimeo.com/manage/videos/943214153/privacy)
## Devops
**Implementation of a CI pipeline with Jenkins to automate deployment.**
**Integration of tests in CI with SonarQube to analyze code quality.**
**Configuration and management of a Kubernetes cluster using Kubernetes and 
 Helm Charts.**
 **Configuration of remote state in Azure to avoid conflicts, ensuring that all users 
 always have the latest version of infrastructure configurations.**
 **Implementation of a GitOps approach for continuous delivery with ArgoCD**
 **Backup Management: Setting up database backups with scheduled automation using cron jobs.**
 
 **Test1**: Data recovery test using the backup.
          - The current database is stored in "moncomptebackup."
          ![Project Architecture](TEST2/1.png) <!-- Replace with the link to your architecture image -->

          - Simulate a failure by deleting the cluster.
          - After rebuilding the cluster, we notice that the data is missing.
          - Run the script to restore the data from the backup stored in "moncomptebackup."
          - The data is successfully restored in the cluster.
         
         

         

