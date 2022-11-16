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




Here is a simple flow chart:

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```
