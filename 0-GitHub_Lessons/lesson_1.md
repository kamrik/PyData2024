
# **Session 1: Creating a GitHub Profile and Applying for the Educational Version**

## **1. Introduction to GitHub**

GitHub is a platform that developers and researchers use to collaborate on projects, manage version control, and showcase their work. It’s a powerful tool to learn for any software development or data science career.

## **2. Creating Your GitHub Profile**

Let’s start by creating your GitHub profile:

1. **Go to the GitHub website**:
   - Open your web browser and go to [GitHub.com](https://github.com).

2. **Sign up for an account**:
   - Click on the "Sign up" button.
   - Enter your email address, create a password, and choose a username. Make sure to select a professional username, as this will be part of your GitHub profile URL.
   - Follow the prompts to complete the sign-up process.

3. **Set up your profile**:
   - Once your account is created, click on your profile picture in the top right corner and select "Your profile."
   - Add a profile picture and a short bio about yourself. Include any skills or areas of interest.
   - Consider adding links to your other professional profiles or personal website.

## **3. Applying for the GitHub Student Developer Pack**

GitHub offers a special pack of benefits for students, including free access to premium tools and services. Here’s how you can apply:

1. **Visit the GitHub Education page**:
   - Go to [GitHub Education](https://education.github.com).

2. **Apply for the Student Developer Pack**:
   - Sign in to your GitHub account if you’re not already signed in.

   - Click on "GitHub Student Developer Pack" in the student section of the page."
   - Follow the instructions to verify your student status. You will need to provide proof of enrollment, such as a student ID or a school email address.
   - Submit your application and wait for approval. Once approved, you will have access to a range of free tools and resources.

---

# **Session 2: Cloning a Repository and Understanding Git Concepts**

## **1. Introduction to Git and Repositories**

Now that you have your GitHub account set up, let’s learn about Git and repositories:

- **Git** is a version control system that helps you manage changes to your code and collaborate with others.
- A **repository** (or "repo") is a storage space for your project files and their history. You can have a repo on GitHub (remote) and on your computer (local). 

>Note: In other words, a `repository` is like other folders/directoris in your computer but with the ability to track changes. In orther to activate this feature for a folder, navigate to the folder and type `git init` in the terminal. By doing this you can see that a hidden folder `.git` is created in the folder. This folder is where git stores all the information about the changes made to the files in the folder.

## **2. Understanding Key Git Concepts**

Before we start working with the repository, let’s understand some key concepts:

- **Remote Repository**: This is the version of your project hosted on GitHub, which can be accessed by anyone you share it with.
- **Local Repository**: This is the version of the project that is on your computer. It’s your own private copy where you make changes.
- **Working Directory**: This is the folder on your computer where the local repository is stored. It’s where you edit files and make changes to your project.
## **3. Cloning a Repository**

Cloning a repository means making a copy of a remote repository to your local machine. Let’s clone the course repository to your computer:

1. **Find the repository URL**:
   - Go to the course repository page on GitHub.
   - Click on the green “Code” button and copy the URL provided.

2. **Open your terminal or Git Bash**:
   - Windows users can use [Git Bash](https://git-scm.com/downloads). Mac and Linux users can use the terminal.

3. **Clone the repository**:
   - Type the following command in your terminal:
     ```bash
     git clone <repository-url>
     ```
   - Replace `<repository-url>` with the URL you copied. For example:
     ```bash
     git clone https://github.com/username/course-repo.git
     ```
   - Press Enter. This will create a local copy of the repository on your computer.

The process explained above is depicted in the image below:

<p align="center">
      <img src="./assets/clone.png" alt="Cloning a repository" width="250" hight="250"/>
</p>

Notes: 
   - `master` branch is sometimes called the `main` branch. This is the default branch in a repository.
   - The green rectangle represents a save-point in the repository. You are going to create many of these save points in the repository when you want to save your chnages in the repository.


## **4. Change the Local Repo**

Let’s practice what we’ve learned:

1. **Navigate to the cloned repository**:
   - In your terminal, use the `cd` command to navigate to the directory where you cloned the repository.
   - Example:
     ```bash
     cd course-repo
     ```

2. **Make a small change to a file**:
   - Adding, removing, or upadating any files in the repository is considered a modified state. 
   - Open any file in the repository with a text editor.
   - Make a simple change, such as adding a comment or a line of text.

3. **Commit your changes**:
   <br>
   These changes are saved in your <i>working directory</i>, however git does not know if you want to save them in the <i>local repository</i>. To save the changes in the local repository, you need to commit the changes.

   - To stage create a save-point in the local repo also known as commit changes, type:
   ```bash
     git add .
     git commit -m "Your message here"
   ```
   
   Replace `"Your message here"` with a brief description of your changes.

The image below shows the process of modifying the repo in working directory and commiting changes to the local repository: