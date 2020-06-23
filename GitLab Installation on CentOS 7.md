![Installation](https://blog.terraforge.io/02/terraform_gitlab.png)

This project we installed GitLab server using Terraform , on a CentOS 7 only for testing purpose.

First, Terraform needs to initialize with provider AWS.  


![init](https://user-images.githubusercontent.com/63433671/85368690-58e8ef00-b4f1-11ea-96a6-adb26848e723.png)

Using Terraform which creates VPC with following components:  


- 3 private  subnets

- 3 public  subnets

- Public subnets attached to IGW. 

- Private subnets attached to NG. 

- Configure Route tables

- Create Public and private keys

- Install GitLab server


- Add Security groups and open nessasarly ports

- Create Variables and tags

- Create instance


<img width="672" alt="Screen Shot 2020-06-23 at 1 50 39 AM" src="https://user-images.githubusercontent.com/63433671/85370255-08bf5c00-b4f4-11ea-8b5d-eb658fbf77aa.png">
<img width="778" alt="Screen Shot 2020-06-23 at 1 51 53 AM" src="https://user-images.githubusercontent.com/63433671/85370333-22f93a00-b4f4-11ea-9eeb-7e287c40ce08.png">


![](https://user-images.githubusercontent.com/63433671/85369068-04923f00-b4f2-11ea-9799-42e8287d9401.png)

![](https://user-images.githubusercontent.com/63433671/85369086-0a882000-b4f2-11ea-952c-60701aad341f.png)

This is expected Infrastructure Architecture when apply completed with Terraform .

![last pic](https://user-images.githubusercontent.com/63433671/85366530-250bca80-b4ed-11ea-84b1-78fa9d89ff80.png)

remote-exec !!!!!!!!!! explaination needed?

Once installation is succesfully completed you will see the GitLab Logo on your terminal. 



![Screen Shot 2020-06-20 at 12 02 01 PM](https://user-images.githubusercontent.com/63433671/85376353-3361e280-b4fd-11ea-99c2-8249347b8d4e.png)




The last step is Configure GitLab through the Web Interface.
Now that you have configured the GitLab URL you can start with the initial configuration through the GitLab web interface.

The first time you access the web interface you’ll be prompted to set the password for the administrative account.

![](https://lh4.googleusercontent.com/T_ghSl23B95b7RhzjjbEP-UJNOTk4ktopW8UpeqpMsZZ9kqS-A8RsaK7CmSZF5ZNLVqx_E96w8wLC2HOMEldy9GEpI7kgpWePAzcfqeu)

Enter a secure password and click on the Change your password button when you are finished.

You will be redirected to the login page:

![](https://linuxize.com/post/how-to-install-and-configure-gitlab-on-centos-7/gitlab-login-page.jpg?ezimgfmt=ng:webp/ngcb26)

The default administrative account username is root. Later in this tutorial, we will show you how to change the username.

Username: root
Password: [the password you have set]
Enter the login credentials, click the Sign in button and you will be redirected to the GitLab Welcome page.

![](https://linuxize.com/post/how-to-install-and-configure-gitlab-on-centos-7/gitlab-welcome-page.jpg?ezimgfmt=ng:webp/ngcb26)

