##

The **workflow** is the engine that drives GitHub actions. In our repositories, we build actions by putting together a set of **workflow files**.

Let's look at how they are made and build one using one of the existing templates. 

To make a **workflow**, we make a series of **YAML files**, which are like `.txt` files. These files live inside the `.github/workflows`.

Each of these **workflows** can have several jobs that do different things, and each workflow begins when a specific event happens.

Let's work with an existing template to create our first workflow.



- ### Pull our `bashScripts` project from the last assignment down into this assignment space using the `git pull` command.

```bash

```

Let's add some actions. First, we'll navigate to the Actions tab and see that there are no workflows or that the workflow is untitled. We can either build a workflow ourselves or use one of the templates.  We'll use this simple workflow action template for our exploration.

We'll click Set Up This Workflow to create a file. Right now it's named blank.yml. Let's rename it `actionPractice`.  It creates a .github folder and a workflows subdirectory, then places this action in those folders. It has generated some text for us automatically and given the workflow a name.

The `push` event triggers this process, so whenever someone pushes to this repository, it executes jobs.

The first job it will do is named build. We want it to run on an Ubuntu system with the latest version. Then, we describe a sequence of stages. This operation uses checkout@v1 and echoes something using a terminal.

We'll give each command a name, and this command will accomplish two tasks: echo Hello World and run a script in several lines.

The indentation between the lines is important. When we see a dash like this, it means we're making a list of sorts. All of these things are included in the list.

Let's start the commit. Committing the new file will cause a push on our repository, triggering the action. It may take a little for the Actions tab to load, but once it does, we can see that the Hello Action is waiting for us. After some time, it should appear under All Workflows.

We can click on the activity to view what's happening in real time. It will  cycle through each of the jobs and execute them. If we open them up, we can see that the one-line script is hello world and the multi-line script is the other content we added. Then, the workflow finishes the job.

We can see how the action is running.  If we want to change the action, we can click View Workflow File and edit it like any other GitHub file. We can edit these activities using Edit This File.

Thanks to all of GitHub's existing resources, it's easy to create basic GitHub actions using existing templates.

## Checkpoint 