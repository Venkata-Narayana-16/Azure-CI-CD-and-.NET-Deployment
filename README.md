# .net-calculator-app
Navaigated azure devops portal and created a new project
![image](https://github.com/user-attachments/assets/26f4f9b8-1d2a-415f-bd35-8cb4f3cadc0d)
Opened azure repos and initiated a repository
![image](https://github.com/user-attachments/assets/34e8ddaf-65d7-4a31-a32e-0eb4ae720832)
Then imported the repository to az repos
Then navigated to azure pipelines and created a new pipeline
Used classic editor to create a pipeline
Then selected az repo as repo
Then selected a empty job
Configured windows 2019 as a agent
Added 2 .Net core tasks. One is to build the code and another is to publish the built code
And added another task “publish pipeline artifacts” to publish the artifacts resulted in build process

Then saved the changes and ran the pipeline
Build pieline is successed
Navigated to azure portal and created a appservice with .Net 8 runstalk for production
•
Similarly another app service is created for QA stage
Then again cameback to azure devops portal and created a service connection to authenticate azure portal and azure devops portal
•
Then opened pipelines and created a new release pipeline
•
Selecrted the artifacts generated in build pipeline
•
QA stage is configured to deploy the code into qastage app service
Production stage is configured to deploy the code to webapp19apr24 app service
•
The pipeline is saved and release is created
•
The QA stage is success and the pipeline is waiting for the manual deployment into the production stage
Production stage is also successed
