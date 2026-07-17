# Bash Basics (freeCodeCamp)

These notes cover the fundamental Bash commands and concepts learned
while working through the freeCodeCamp Relational Databases
Certification.

------------------------------------------------------------------------

## Terminal

The terminal is a command-line interface (CLI) used to interact with the
operating system.

### Opening the Terminal (GitHub Codespaces)

1.  Click the ☰ menu.
2.  Select **Terminal**.
3.  Click **New Terminal**.

------------------------------------------------------------------------

## Common Commands

### `echo`

Display text.

``` bash
echo hello terminal
```

Append text to a file:

``` bash
echo "I made this boilerplate" >> README.md
echo "from the command line" >> README.md
```

### `pwd`

Print the current working directory.

``` bash
pwd
```

### `ls`

List files and folders.

``` bash
ls
```

#### `ls -l`

Long list format showing permissions, owner, size, dates, and file type.

#### `ls -a`

Show hidden files such as `.gitignore`.

#### `ls --help`

Display the help page.

### `cd`

Change directories.

``` bash
cd folder
```

#### `cd ..`

Move up one directory.

#### `cd ../..`

Move up two directories.

Every `..` represents the parent directory.

### `mkdir`

Create directories.

``` bash
mkdir website
mkdir client/src
```

### `touch`

Create empty files.

``` bash
touch index.html
touch index.html styles.css script.js
```

### `cp`

Copy files.

``` bash
cp background.jpg images/
```

#### `cp -r`

Copy an entire directory recursively.

``` bash
cp -r boilerplate toms-website
```

### `mv`

Move or rename files.

``` bash
mv roboto.font roboto.woff
mv logo.png images/
```

### `rm`

Remove a file.

``` bash
rm background.jpg
```

### `rmdir`

Remove an empty directory.

``` bash
rmdir images
```

### `find`

Display or search the directory tree.

``` bash
find
```

#### `find -name`

Search by filename.

``` bash
find -name index.html
```

### `more`

View a file one screen at a time.

``` bash
more README.md
```

### `clear`

Clear the terminal.

### `exit`

Exit the terminal.

------------------------------------------------------------------------

## Key Concepts

-   **Terminal**: Text interface for interacting with the operating
    system.
-   **CLI**: Command Line Interface.
-   **Directory**: Another word for folder.
-   **Parent Directory**: The directory above the current one.
-   **Working Directory**: Your current location.
-   **Path**: Location of a file or folder.
-   **Hidden File**: Begins with a period (`.`), e.g. `.gitignore`.
-   **Source**: Original file in a copy or move.
-   **Destination**: Where the copied or moved file goes.
-   **Recursive**: Includes everything inside a directory.
-   **Append**: Add text to the end of a file.
-   **Output Redirection**: Using `>>` to send output into a file.
-   **HTML**: HyperText Markup Language. Most websites begin with
    `index.html`.

------------------------------------------------------------------------

## Commands Learned

  Command        Description
  -------------- -------------------------------
  `echo`         Display text
  `pwd`          Print working directory
  `ls`           List files
  `ls -l`        Long list format
  `ls -a`        Show hidden files
  `ls --help`    Help page
  `cd`           Change directory
  `cd ..`        Up one directory
  `cd ../..`     Up two directories
  `mkdir`        Create directory
  `touch`        Create file
  `cp`           Copy files
  `cp -r`        Copy directories recursively
  `mv`           Move or rename
  `rm`           Remove file
  `rmdir`        Remove empty directory
  `find`         Search/display directory tree
  `find -name`   Search by filename
  `more`         View file
  `clear`        Clear terminal
  `exit`         Exit terminal
