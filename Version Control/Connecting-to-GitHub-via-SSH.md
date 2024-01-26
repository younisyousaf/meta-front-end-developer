# Connecting to GitHub via SSH

If you plan to use GitHub from your local device, the recommended way to authenticate is using Secure Shell, or SSH for short. This requires the creation of keys: a public and a private key. The advantage of using SSH is that you don't need to enter your credentials when interacting with the remote repository. The keys are generated and stored on your local machine, and then the public key is copied to the GitHub server. After you finish setting up, every operation will be authenticated using the keys.

## Generate SSH Keys

The process is the same for both Windows and Mac. On Windows, you can use the Git Bash terminal, and on Mac, the standard terminal will work.

1. Open the terminal

2. Enter the following:
   ```bash
   ssh-keygen -t ed25519 -C "your@email.com"
   ```
## Replace the email with your own and press enter.

1. It will prompt to enter a password. Hit enter to skip setting a password.

2. Once confirmed, the keys will be generated.

Both keys will be stored in the .ssh folder.

## To add the key to GitHub:

1. Find the name of the key file using the below command: 
    ```bash
    ls ~/.ssh/
    ```
2. Copy the file using the below command, replacing <YOUR KEY> with the name of the key file on your device.

    - For Mac:
        ```bash
        pbcopy < ~/.ssh/<YOUR KEY>.pub
        ```
    - For Windows:
        ```bash
        cat ~/.ssh/<YOUR KEY>.pub | clip
        ```
## Adding Your Keys to GitHub

### Step 1: Log on to GitHub

### Step 2: Click on the profile icon in the top right of the screen and select Settings.

![Click on Settings](images/github_settings.png)

### Step 3: On the Settings screen, on the left-hand side under the Access section, click SSH and GPG Keys.

![Click on SSH and GPG Keys](images/github_ssh_gpg_keys.png)

### Step 4: Click the New SSH key button in Green on the right-hand side of the screen.

![Click on New SSH key button](images/github_new_ssh_key.png)

### Step 5: Enter a title and paste in your public key that you copied previously.

![Enter title and paste public key](images/github_enter_ssh_key.png)

### Step 6: Click the Add SSH key button.

You are now ready to access GitHub via SSH.

## Accessing Repositories

When accessing a repository and using SSH authentication, make sure to always use the SSH address of the repository.

**Always use the SSH address of the repository.**
