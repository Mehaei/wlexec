# wlexec

## Quick start

### download script
```bash
git clone https://github.com/Mehaei/wlexec.git
cd wlexec
```

### install(Used as a system tool)

#### Linux
```bash
# Add executable permissions
chmod u+x wlexec
# Add to system env variables
sudo mv wlexec /bin/
```

#### Mac
```bash
# Open the Settings env variables file
vi ~/.bash_profile
# Add to system env variables
alias wlexec="bash {project_dir}/wlexec/wlexec"
# Enables the environment variables file to take effect
source ~/.bash_profile
```

### Use

#### help
```bash
wlexec OR wlexec --help OR wlexec -H
```

#### version
```bash
wlexec --version OR wlexec -V
```

#### Execute the command
```bash
wlexec "shell command" attempts
```

##### sample
```bash
wlexec "echo 1"
```
##### output
======================================== Program starts ========================================
Command: "echo 1"
echo 1 command execute OK!
exec result:
 1
======================================== Program end ===========================================

#### Execute a limited number of commands
```bash
wlexec "echosa" 2
```

##### output
======================================== Program starts ========================================

Command: "echosa"

"echosa" 1th execution failure, error message:

/Users/msw/Desktop/wlexec/wlexec: line 101: echosa: command not found

"echosa" 2th execution failure, error message:

/Users/msw/Desktop/wlexec/wlexec: line 101: echosa: command not found

Terminate the process. 2 attempts have been made

======================================== Program end ===========================================


>> Execute commands in quotes

>> Thank you for pointing out any mistakes




