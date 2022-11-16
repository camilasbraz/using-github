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

9.
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

Here is a simple flow chart:

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```
-->
