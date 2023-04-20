# git-Troubleshooting-onJenkins
ERROR: Couldn't find any revision to build. Verify the repository and branch configuration for this job.

```sh
For this same error. You need to confirm the repository URL and confirm the branch. If you are using github, the master is now changed to main branch.
```

Failed to connect to repository : Error performing git command: git ls-remote -h https://github.com/chrislucky5/hello-world.git HEAD
```sh
In my case this issue happened because of there is no git installed on my Linux server.

sudo yum install git -y
git --version
After installing git I just make sure that my Global Tool Configuration default pointed to git Jenkins > Manage Jenkins > Global Tool Configuration > Git

Name : git
Path to Git executable : git
just posting this may help you in case of similar issue you had
```
