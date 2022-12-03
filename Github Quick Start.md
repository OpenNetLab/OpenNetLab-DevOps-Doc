# Github Quick Start
## 1.Code Download  
> git clone  

Add the link obtained from the corresponding project to copy the project locally.
## 2.Default Agreement  
If the command provided in the documentation does not explicitly specify a directory, it means that the command is executed in the directory of the downloaded folder.  
## 3.User Settings  
The download of the public code in Github does not require authentication (the private repo requires), but the upload of code requires authentication, which requires some local configuration.    
> git config --global user.name YourUserName  
> git config --global user.email YourEmail 
 
Generate your own key  
>ssh-keygen -t rsa -C YourEmail  

Keep pressing enter and the key will be saved in the default directory.    
View Key    
> cd ~/.ssh/  
> vim id_rsa.pub  

Copy the key to the corresponding project on Github to complete the authentication.  
![](https://github.com/wangyf2001/Azure-picture/blob/main/Github1.jpg)


## 4.Code Upload
### Code Modification
Generally the cloned code will go to the master branch by default, we need to create a separate branch and make changes to the code on our own branch.  
> git branch your-Alias/filename  
> git checkout your-Alias/filename  
### Code Submission
After making changes on the cloned document, you can start the code commit process.  
Add the changes to the staging area  
> git add yourfilename  

Adding cache contents to the local repository.  
> git commit -m ‘Your File Note’  

Submitting code to the cloud repository.  
> git push --set-upstream origin your-Alias/filename  

# Some good learning documents of Github
[Github配置及使用](http://t.zoukankan.com/jiaxblog-p-9574441.html"github配置及使用")   
[Github文档](https://docs.github.com/cn"Github中文文档")  
[Github docs](https://docs.github.com/en"Github英文文档")

