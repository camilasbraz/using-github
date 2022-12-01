# using-github

## Windows

### First steps
<a href = 'https://www.pluralsight.com/guides/using-git-and-github-on-windows'> Based on this website </a>

1. Download and intall git: <a href = "https://git-scm.com/download/win"> Available here

2. Create a new folder, right click on it and choose 'Git bash here'

3. Configure your user name and email
```
git config --global user.name username
git config --global user.email email
```
4. Initialize git with
```
git init
```

5. Testing commits
```
touch test.txt
git add .
git commit -m "First commit"
```

6. Link the ssh key to your email
```
ssh-keygen -t rsa -C email
```
Press enter or choose in which folder you wish to save the ssh key and set (or not) a passphrase

7. Go to your github settings and then to SSH and GPG Keys. Click on New SSH Key, give it a title and pass the key you just created on the above step. It can
be found using the `notepad ~/.ssh/id_rsa.pub` command on bash.

8. Go back to git Bash and type 
```
ssh -T git@github.com
```
<img width="453" alt="image" src="https://user-images.githubusercontent.com/45129483/202311626-b5394268-c97c-4b6b-a7de-6ec6e2535dd2.png">
Choose yes then type your password. If everything works out fine, the message "You've successfully authenticated, but GitHub does not provide shell access.
" will appear
9. To clone a repository in your local machine, click on Code --> SSH and copy the link

<img width="649" alt="image" src="https://user-images.githubusercontent.com/45129483/203391936-f8070854-80a0-4af4-9bd1-2da4d10fa6a5.png">

10. Then, git bash on tha folder you want to clone the repository to and type
```
git remote add origin git@github.com:user/repo_name.git
```
change user and repo_name!

### Basic commands
1. Update the folder in your computer
```
git push
```
2. Commit and pull
```
git add . 
git commit -m 'comment'
git pull origin branch_name
```
3. Change branch
```
git checkout <existing_branch>
git checkout -b <new_branch> (if branch does not exist)
```
<!---
<> teste4213
<> +---[RSA 3072]----+
<> |+.. .  o... +E   |
<> |o+o. .. .  + o   |
<> |BB+...      o    |
<> |X===.            |
<> |oXo.+ . S        |
<> |+.*o+o o .       |
<> |.+.oo.+ .        |
<> | .   + .         |
<> |    .            |
<> +----[SHA256]-----+

-->

### SmartGit

<a href = "https://www.syntevo.com/smartgit/"> Download </a>
