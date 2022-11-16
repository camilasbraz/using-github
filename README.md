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




Here is a simple flow chart:

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```
