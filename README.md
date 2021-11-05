# Salesforce Starter Pack - Main tools for Developers in the SFDC platform, including useful VSC and Chrome extensions.

<p align="center">
    <img height="auto" width="auto" src="img/img0.png" />
</p>


## Table of Contents  
- [Basic configuration](#basic-configuration)  
    - [Node.js](#node-js)
    - [Java SE Development Kit](#java-se-development-kit)
    - [Visual Studio Code](#visual-studio-code)
    - [GIT](#git)
    - [Salesforce CLI](#salesforce-cli)
    - [Uncrustify](#uncrustify)
- [VSC configuration](#visual-studio-code-configuration)  

## Basic configuration

### Node.js
Node.js is a server-side platform built on Google Chrome's JavaScript Engine (V8 Engine) for easily building fast and scalable network applications. Most of tools are executed using this runtime (in our case Visual Studio Code and Salesforce CLI);

Node uses a package manager call NPM (Node Package Manager).

- Link => https://nodejs.org/es/

### Java SE Development Kit (JDK) 11.0 version (or Java 8.0)
The Java Development Kit (JDK) is one of three core technology packages used in Java programming, along with the JVM (Java Virtual Machine) and the JRE (Java Runtime Environment). It's important to differentiate between these three technologies, as well as understanding how they're connected:

The JVM is the Java platform component that executes programs.
The JRE is the on-disk part of Java that creates the JVM.
The JDK allows developers to create Java programs that can be executed and run by the JVM and JRE.
Developers new to Java often confuse the Java Development Kit and the Java Runtime Environment. The distinction is that the JDK is a package of tools for developing Java-based software, whereas the JRE is a package of tools for running Java code.

The JRE can be used as a standalone component to simply run Java programs, but it's also part of the JDK. The JDK requires a JRE because running Java programs is part of developing them.

- Link => https://www.oracle.com/es/java/technologies/javase/jdk11-archive-downloads.html

### Visual Studio Code (VSC)
Visual Studio Code combines the simplicity of a source code editor with powerful developer tooling, like IntelliSense code completion and debugging.

First and foremost, it is an editor that gets out of your way. The delightfully frictionless edit-build-debug cycle means less time fiddling with your environment, and more time executing on your ideas.

Visual Studio Code supports macOS, Linux, and Windows - so you can hit the ground running, no matter the platform.

Customize every feature to your liking and install any number of third-party extensions. While most scenarios work "out of the box" with no configuration, VS Code also grows with you, and we encourage you to optimize your experience to suit your unique needs. VS Code is an open-source project so you can also contribute to the growing and vibrant community on GitHub :octocat:

- Link => https://code.visualstudio.com/
### Git
Git is the most commonly used version control system. Git tracks the changes you make to files, so you have a record of what has been done, and you can revert to specific versions should you ever need to. Git also makes collaboration easier, allowing changes by multiple people to all be merged into one source. 

So regardless of whether you write code that only you will see, or work as part of a team, Git will be useful for you.

Git is software that runs locally. Your files and their history are stored on your computer. You can also use online hosts (such as GitHub :octocat: or Bitbucket) to store a copy of the files and their revision history. Having a centrally located place where you can upload your changes and download changes from others, enable you to collaborate more easily with other developers. Git can automatically merge the changes, so two people can even work on different parts of the same file and later merge those changes without losing each other’s work!

- Link => https://git-scm.com/
### Salesforce CLI
The Salesforce CLI is a powerful command line interface that simplifies development and build automation when working with your Salesforce org. Use it to:

- Aggregate all the tools you need to develop with and perform commands against your Salesforce org
- Synchronize source to and from scratch orgs
- Create and manage orgs
- Import and export data
- Create and execute tests
- Create and install packages

After you install Salesforce CLI, run "sfdx commands" in a terminal or command shell to view the list of available commands.

- Link => https://developer.salesforce.com/tools/sfdxcli 

### Uncrustify
A source code beautifier for C, C++, C#, ObjectiveC, D, Java, Pawn and VALA

Features:
- Highly configurable - 753 configurable options as of version 0.73.0
- add/remove spaces
- add/remove newlines
- add/remove blanklines
- indent code
- align code
- modify code

To install Uncrustify you need to use Chocolatey, a Package Manager for Windows.

- Link => https://chocolatey.org/install#install-step1

And then execute this command line:

```Powershell
choco install uncrustify
```

After finishing the installation copy this [file](./resources/uncrustify.cfg) to the following directory.

```bash
C:\\Users\USER_NAME
```

## Visual Studio Code Configuration

To access Visual Studio Code configuration file you can edit the .json file directly or use the UI (this is the easiest one). Go to:

```bash
File > Preferences > Settings
```

Keep the default values, except for the following points:
| Extension | Configuration | Value |
| Text editor | Render Whitespace | X |
| Diff tool | Ignore Trim Whitespace | |
| Breadcrumbs | Enabled | X |
| Git | autofetch | |
| Git | Enable Smart Commit | X |
| Git | Fetch On Pull | |
| Git | Rebase When Sync | |
| Git | Show Push Success Notification | X |
| npm | Npm: Enable Scrip[t Explorer| X |
| npm | Npm: Script Explorer Action | run |