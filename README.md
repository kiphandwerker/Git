# Git commands I use regularly

## Global Options

<ul>
<li> <strong>gl:</strong> Displays the contents of the global config file in the terminal
<li> <strong>gle:</strong> Opens the global config file in the default / editor of choice
</ul>

# Logs
<ul>
<li> <strong>ls: </strong> Creates a much better looking git log with passable parameter (default 10)

```git
git ls 5
```
Outputs the log for the last 5 commits

<li> <strong>lsn: </strong> Creates a much better looking git log with stats with passable parameter (default 5)

```git
git lsn 8
```
Outputs the log with stats for the last 8 commits
</ul>


# Commits
<ul>
<li> <strong>ac:</strong> Adds files and commits with message

```git
git ac . "Adding all"
```
The is the equivilant to:

```git
git add . && git commit -m "Adding all"
```

<li> <strong>ict:</strong> Adds all files and commits with "Initial commit" message
</ul>

# Inits
<ul>
<li> <strong>gi:</strong> New commit that changes branch from master to main and creates .gitignore and README.md
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