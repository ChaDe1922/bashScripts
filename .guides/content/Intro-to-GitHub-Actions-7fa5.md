##

Many programmers use GitHub Actions to help them take care of common tasks. They do work in our repositories by making one or more text files that contain actions. The name for these is **workflows**.

![.guides/img/actions_2](.guides/img/actions_2.png)

**Workflows** can take care of common build tasks, such as continuous delivery and integration. This means that when the master branch changes, we can use an action to compress images, test our code, and push the site to our hosting platform. 

We can also have **jobs** that run at certain times or that control what happens when someone interacts with the GitHub repository itself. If someone comments on a pull request, we can get an email, and if someone stars our project, we can run an action.

![.guides/img/workflows](.guides/img/workflows.png)


Actions can run on Linux, macOS, or Windows, as well as on virtual machines or containers. That means we can test our code in different environments. We can even test workflows on more than one platform at the same time.

Every action creates a detailed log that can be used to troubleshoot deploys as they are happening. We will also be able to store **secrets** in the repository on GitHub. This will make it safer and easier for everyone on the team to use.

Actions has a wide community of developers who have already made hundreds of **actions**, examples, and **workflows** so we don't have to start from nothing.

## Checkpoint 🏁