# Git commands I use regularly

## Global Options

<ul>
<li> <strong>gl:</strong> Displays the contents of the global config file in the terminal

```git
git gl
```

This is equivilant to:

```git
git config --global -l
```

<li> <strong>gle:</strong> Opens the global config file in the default / editor of choice


```git
git gle
```

This is equivilant to:

```git
git config --global --edit
```
</ul>

# Logs
The log has been refurbished to be much more pleasant to look at. The structure is as follows:

$\color{yellow}{\textsf{hash}}$
$\color{red}{\textsf{[}}$
$\color{green}{\textsf{Author date ..}}$
$\color{teal}{\textsf{Author name}}$
$\color{red}{\textsf{]}}$
Commit message


<ul>
<li> <strong>ls: </strong> Log with the last 5 commits

```git
git ls 5
```

This is equivilant to :

```git
git log -5 HEAD
```

<li> <strong>ls: </strong> Log with the last 5 commits and the stats

```git
git lsn 5
```

This is equivilant to :

```git
git log -5 HEAD --stat
```
</ul>

# Commits
<ul>
<li> <strong>ac:</strong> Adds files and commits with message

```git
git ac . "Adding all"
----or----
git ac file1/ file2/ "Updates to file 1 and file2"
```
This is the equivilant to:

```git
git add . && git commit -m "Adding all"
----or----
git add file1/ file2/ && git commit -m "Updates to file 1 and file2"
```



<li> <strong>ict:</strong> Adds all files and commits with "Initial commit" message

```git
git ict
```
This is the equivilant to:

```git
git add . && git commit -m "Initial commit"
```

</ul>

# Inits
<ul>
<li> <strong>gi:</strong> Creates a new git repo that changes branch from master to main and creates .gitignore and README.md


```git 
git gi
```

This is the equivilant to:

```git
git init
git branch -m master main
touch .gitignore
touch README.md
```
</ul>

# Status
<ul>
<li> <strong>s:</strong> Displays status log
</ul>

# Push and branches
<ul>
<li> <strong>gmain:</strong> Switches to main branch
<li> <strong>eow:</strong> Go to main branch, merge with wip, and pushes
</ul>