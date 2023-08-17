General Documentation
1. Download application files from Kura's GitHub Repo
2. Create your own GitHub Repo and include the Kura application files previously downnloaded *
3. Login to Jenkins and begin to setup new pipeline. (GitHub Token will be needed. see next step)
4. Create a personal access token from GitHub *
5. Complete the pipeline setup on Jenkins (Token and Repo-link needed) 
6. Run the pipeline on jenkins and if successful, access the Jenkins Console output for documentation
7. Use Scribe resources to setup elastic beanstalk roles and rezip application files to use them to setup environment *
8. initial environment launch failed. Checked Logs on AWS to find the error *
9. Changed the (.py) file name from app.py to application.py on GitHub *
10. Downloaded the application files after the previous change and rezipped the files, then uploaded them to AWS. 
11. Relaunched the enviornment successfully *

2* Make sure the files look the same, meaning when copying and pasting make sure the files that are in folders remain in their respective folders

4* Make sure to save that token in notes in case you need it again. This will be the only time you'll be able to see it

7* To submit application files in AWS you must make sure you redownload the application files from your own repo on GitHub, unzip them all, then rezip them (make sure you  are not including the parent folder)

8* Reading Logs to find the error: [ModuleNotFoundError: No module named 'application'] AWS is trying to find the file named 'application' to run but since we have it named as 'app' it cannot recognize it by that name to run it

<img width="1194" alt="Screen Shot 2023-08-16 at 9 40 13 PM" src="https://github.com/Sameen-k/Deployment1.1/assets/128739962/e64e1c07-af33-4af0-a0c9-a950eb7346e2">




9* Changed the file name from app.py to application.py on GitHub and redownloaded the files

<img width="1186" alt="Screen Shot 2023-08-16 at 9 43 42 PM" src="https://github.com/Sameen-k/Deployment1.1/assets/128739962/222beeec-b7ba-4422-b588-4b6b59b7eae8">




11* Successfully Launched Enviornment!!

<img width="1205" alt="Screen Shot 2023-08-16 at 9 41 19 PM" src="https://github.com/Sameen-k/Deployment1.1/assets/128739962/aa050447-7eed-40dd-a19c-a1b50419edef">

