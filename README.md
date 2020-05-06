# AutomateDeploying

Hasn't the testing and deploying of your webpages always been a recurrent tedious task? Here is a small guide to automating this process so that all you have to worry about is the actual content of your website! Time + Energy + Resources put to the right job. Let's get started from scratch->

Pre-requisites: Jenkins, Docker and a local folder (webfolder in my case) to keep the webpages on your base system.

1. Make a repository with you webpage on GitHub.
2. Make another branch to add some features.
3. Build Job1 on Jenkins to track this branch and to deploy it into a testing environment using Docker.
4. Build Job2 on Jenkins to track master branch and to deploy it into a production environment viewed by the client using Docker.
5. Build Job3 to merge master and the branch before actual build adn trigger it remotely by giving the trigger to someone (QA) who passes the testing version. Since it merges with the master it is deployed into the production environment.

Find the scripts of building the jobs under the respective folders and for a complete tutorial refer my medium article:
https://medium.com/@khushalithakkar/test-deploy-webpages-in-just-seconds-now-put-your-worry-into-committing-new-features-aa83b0d155f5
