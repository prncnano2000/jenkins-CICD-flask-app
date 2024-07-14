|| [Prerequisites](#prerequisites) ||
[Deployment](#deployment) ||
[Authors](#authors) ||


# jenkins-CICD-flask-app

This `Jenkins CI-CD pipeline with Docker` allows you to automate the process of building, testing and deploying your `Flask application` in a more efficient way. This helps you save time, reduce errors, and ensure consistent delivery of your application.


## Technologies

- **Jenkins**

- **Docker**

- **Git et GitHub**


## Features


- `Checkout`: Retrieving the source code from the Git repository.

- `Build Docker Image`: Building the Docker image for the Flask application.

- `Test`: Execution of unit or integration tests (to be completed according to your needs).

- `Push to DockerHub`: Pushing the Docker image to DockerHub.

- `Deploy`: Deployment of the application to the staging or production environment (customize according to your needs)



## Prerequisites


- A running Jenkins server.
  
- Docker installed on your Jenkins server.
  
- A GitHub account to store your Flask application code.

  
## Installation


\
In your command prompt download the repo with the commands:
```bash
  git clone https://github.com/AnselmeG300/jenkins-CICD-flask-app.git

  cd jenkins-CICD-flask-app
  
  code . 
```

    
## Deployment


A. **Create a `Git repository` for your Flask application**🥇

 - Create a `new Git repository` on GitHub or another code hosting provider.

 - Clone the repository to your development machine.

 - Add your code files to the Git repository and make commits.



NB: Add `DockerHub Credits` (Add your DockerHub credentials in Jenkins Credits.)


B. **Configure Jenkins**🥈

- Access the Jenkins web interface.

- Create a new project (job) by selecting `New project`.

- Give your project a name, for example `Flask-App`.

- Select `Git` as `version control system`.

- Enter the Git `repository URL' of your Flask application.

- Set Git credentials if necessary.


C. **Create a build pipeline**🥉

- Select the `Pipeline` tab.

- Click on `New pipeline`.

- Choose `Pipeline Scripted`.

- Paste the `Jenkinsfile` script from this git repository into the script editor.


D. **Save and run the pipeline**:

- Save the Jenkins pipeline.

- Start the pipeline `manually` or configure a trigger to run `automatically` every time you push code to the Git repository.

D-1. `Manually deployed`:
- Access the Jenkins web interface.
  
- Select your Flask project.
  
- Click the “Build Now” button to launch the pipeline manually.

D-2. `Automatic deployment`:
- Configure a webhook in your code hosting provider (GitHub, GitLab, etc.) to send a notification to Jenkins whenever you push code to the repository.
  
- Jenkins will automatically trigger the pipeline when it receives a webhook notification.

**```Conclusion```**

You now have `a working CI-CD pipeline` for a `Flask` ​​application using `Jenkins and Docker`. This pipeline will build your Docker image, run tests, push the image to DockerHub and deploy the application to the staging or production environment.


Documentation Jenkins: https://www.jenkins.io/doc/


## Authors

- [@AnselmeG300](https://github.com/AnselmeG300/terraform-cloud.git)


## License

[MIT](https://choosealicense.com/licenses/mit/)


## Badges

Add badges from somewhere like: [shields.io](https://shields.io/)

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
