# Bash-Scripts

## git_manager

Can manage all git repos and composer found with the find command. It's extremely minimal but does the job. maxdepth is about mandatory not to change stuff in vendors or other gits you wouldn't want to manage.

### Installation

```
~$ git clone git@github.com:pierrelocus/Bash-Scripts.git
~$ sudo cp Bash-Scripts/git_manager /usr/bin

# Use for git
~$ git_manager stash                    # Will stash all gits within 3 folder depth
~$ git_manager pull                     # Will pull all gits within 3 folder depth
~$ git_manager checkout -b new_branch   # Will switch branch all gits within 3 folder depth
~$ git_manager stash pop                # ... :)

# Use for composer
~$ git_manager composer install             # Run composer install in all subdirectories that contain a .git folder
~$ git_manager composer require new_package # ... :)
```
