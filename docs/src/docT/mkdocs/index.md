###### mkdocks intro
### mkDocs and how to use it
This product wad build using mkdocs. If youre unfamilliar with mkdocs dont't worry. 

MkDocs is used to provide some functonality to this project. It allows users to be able to view this book online or alternativly create a PDF version of it for more comfortable reading while offline. Additionally it allows users to "host" a "local instance" of the documentation platform from their onw computer. This i a facny way of saying youre crating a fake web page in your broweser. 

What this allows developers to do is make sure everyting is displayed and functioning as it is intended to to before making the platform live for the world to see. We dont expect you to be doing any developing but it does offer a neat nieche for wieving the platform offline, as if it was online. 

For anyone interested please follow this sections instructions.

# Mkdocs

Mkdoca allows users to create stunning Github static pages for documentation. We used Mkodcs to implement tihs platform. The following is a quick guide to setting up mkdocs and getting started creating you own unique platform. 

> **Note:** *The following are prerequisites for completing the tutorial. `Python` `pip` `VScode` and a `CLI`. Make sure you have the required software by following this [guide]()*

### Getting started with mkdocks

Altough it might seem complex, creating your own mkdocs project is as simple as following these simple steps. Make sure to chect out the [prerequsites]() to ensure you have everything you require to be able to complete this tutorial. you'll nedd an CLI (command line interface) to follow along. I recommend using linux's terminal as it has been the easiest way for me and it will be the tool of choice for this project. Alternativly for windows user you can enable [WSL]() and have access to the same CLI as found in linux. 

Since we want our pages to be availible online we need to publish it. We can do this without paying a hosting provider a lot of money by simply uploading our site to GitHub pages. GitHub allows pages to be hosted through a GitHub repository for free. This functionality was initially developed to help develpment teams create large and complex documentation sets for products they were working on. Although our project wont be as complex as theirs we can still make use of the same facility to publish our documentation.

#### Step 1: We need to create a GitHub repository which will contain all our files.

> **Note:** *A GitHub profile is required to continue with this ttorial. If you do not have a GitHub profile, you can reister for one [here](https://www.github.com/register) for free*

1. Login to your GitHub account.
[login_github]()

2. Select create new repository.
[new_repo]()

3. Complete the required fields.
GitHub requires some information to be able to effectivly create a repository. You can copy what I do or create your own. the choice is yours. 

- **Repository Name:** This is what your project will be called. i would advice sticking to a descriptive name as it would make it easier for people to find your project. I'll call my project `MkDocs-Tutorial` for simplicity's sake.

> **Note:** *GitHub auomatically checks if your repositiry name is availible, you cannot have more than one repository with the same name, just like you cannot have more than one file which has the same name on your computer in the same namespace.*

[naming_repo]()

- **Readme File:** Its best practice to include a readme file in your project. This file should be populated later to provide a brief discription of what your project is all about. The readme file will be displayed when people view your GitHub repository so providing a little informations goes a long way.

- **Lcense:** As your project will be publicly availible, unless you select a private repository, it is a good idea to include a licensce. Spend some time to read through the licneses availible on GitHub and select the one which fits best. I'd like to point out here that a licence in not nessacerry but simply good practice. Skip this step if you would like. Ill select `{insert licence choise here}`.

4. Select create repository

[create_repository_done]()


#### Step 2: Install mkdocs.

Now that we have a GitHub repository we can get to working on the documentation. First wel need to clone our project repository to our computer.

1. From the GitHub repository click on `code`

[clone_button]()

and select the two squares to copy the address.

[clone_squares]()

2. Open your CLI (command line interface), in my case it the terminal. Linux: press `ctrl` + `T`

[cli_new]()

3. Navigate to the desired folder in which you want to store the project by using the `CD` command. I want to store my project in my documents folder, but you can put it wherever you would like. 

```cd Documents/```

> **Note:** *Make sure your inside the correct folder to avoid confusion later. The path is displayed in the terminal as `~/Documents` or `C:/users/{username}/Documents`*

now clone the GitHub repository by using the `git clone` command. You can paste the previously copied path by pressing `ctrl` + `shift` or `ctrl` + `shift` + `V` depending on your OS. If implemented correctly your comand should look like this:

```git clone https://github.com/EliVolsch/Learn-Centre.git```

4. After your repository has been cloned navigate to the newly created directory. 

```cd Learn-Centre```

5. Once inside the directory we can create and activate a vitual environment, by running the following code:

```python -m venv venv```
```scource venv/bin/activate```

notice your terminal has now changed and displays the following `(venv) (base)`.

[terminal_activate_venv]()

6. Lets open the project in VS Code by running the following commad:

```code .```

> **Note:** *Code is the command to lauch visual studio code from the terminal. The full stop `.` indicates the directory. A full stop is the current or active directory*

[vs_code_new_project]()

Select `trust the authors` from wihin vs code.

7. For simplicity's sake well continue working within the vs code terminal. Open the terminal by selecting `Terminal >> New Terminal` from the top pane. Notice the terminal inside vs code has automatically activated the virtual environment since we can see `(venv) (base)`.

8. Lets install mkdocs by running the following code:

```pip install mkdocs```

9. Once mkdocs has completed its run we can create a new project

```mkdocs new .```

this creates a new folder inside of the directory named `{folder}` and file named `{file}`

10. Lets run this to see what it looks like befor econtinueing.

```mkdocs serve```

inside the terminal a message should appear stating `INFO - [14:44:33] Browser connected: http://127.0.0.1:8000/`. This means that you are now hosting the document site on your local machine and can view it like it would be displayed on the web. Hold `ctrl` and click on the link `http;//127.0.0.1:8000` to open your page in the browser.

Step 3: Sprucing up the platform

When the browser opens you'll see the deafult mkdocs project page. In many cases this will do but we would like something that looks professional and appealing. feel free to play around on the deafult page before continueing with this tutorial.