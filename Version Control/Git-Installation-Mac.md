# Installing Git on Mac

Git works on all operating system platforms such as Windows, Mac, and Linux. On Mac or Linux, in some cases, it is installed by default. The majority of users will use Git via the command line as its syntax is very easy to understand and follow. Git also works well in development environments and integrates into IDEs and other GUI offerings.

Macs tend to have Git installed by default, so before diving into the installation, we can run a `git version` command to check if Git is already installed. If the command returns a Git version, then Git is already installed. If it returns "command not found", Git needs to be installed.

## Install with Xcode

Install the latest version of Xcode for your Mac by downloading it from the Apple Store or going to the official website - [https://developer.apple.com/xcode/](https://developer.apple.com/xcode/)

## Install Git from Homebrew

Homebrew is a popular package manager for Macs. It’s easy to use and makes it simple to install new packages such as Git. Follow these steps:

1. Go to the Homebrew website at [https://brew.sh/](https://brew.sh/) and follow the install instructions for Mac.
   
2. Once Homebrew is installed, open a terminal window and then type the command:

    ```bash
    brew install git
    ```

3. Once installed, run the `git version` command to verify the installation is complete.

You should see something similar to the following output:

```bash
$ git version
git version 2.34.1
```