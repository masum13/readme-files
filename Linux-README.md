# Linux Command Guide

## Installation of Packages
Install a package using `apt`:
```bash
sudo apt install <package-name>
```

## Working with Directories and Paths
Print the current directory path:
```bash
pwd
```

Navigate using relative and absolute paths:

- `Relative path`: Navigate from the current directory.
- `Absolute path`: Starts from the root directory (/).

Change directories:
```bash
cd <path to directory>
cd ../       # Move one directory back
cd ../../    # Move two directories back
```

## Listing Files and Directories
List current folder contents:

```bash
ls
ls -al       # View details including hidden files
```
## Managing Files and Directories
Create directories:

```bash
mkdir <dir-name>
mkdir -p <dir-name>/<sub-folder>    # Create nested directories
```

## Remove files/folders (use with caution):
```bash
rm -rf <folder-name>    # Recursive and forceful deletion
```

## Viewing File Contents

#### View entire file content:
```bash
cat <file-name>
```
#### View the first or last lines of a file:
```bash
head -n 10 <file-name>    # View first 10 lines
tail -n 10 <file-name>    # View last 10 lines
```

## Editing Files
#### Edit files using vi:

```bash
vi <file-name>    # Edit file, press "i" to start editing, "esc" then ":wq" to exit
```

## Create an empty file:

```bash
touch <file-name>
```

## Print to terminal:
```bash
echo "Desired string"
```

## Redirecting Output

#### Redirect output to a file:
```bash
echo "Desired string" > <file-name> # Replace file content
echo "New data" >> <file-name> # Append to file
```

#### Add multiple lines to a file:
```bash
cat <<EOF > <file-name>
Line1
Line2
EOF
```

## Monitoring Processes
Check running processes:
```bash
ps -ef # View all processes
```

## Downloading Files
Download files:
```bash
wget <URL> # Using wget
curl -o "download-file-name" <URL> # Using curl
```

## Searching within Files
Search in files:

```bash
grep -r <search-keyword> <search-location> # Recursive search
grep "search-term" <file-name> # Search in a specific file
```