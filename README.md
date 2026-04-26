# Programming Assignment 6

## 1. Problem Statement
The goal of this assignment was to modify the source code of two Linux commands from the GNU coreutils package: `ls` and `whoami`.

For the `ls` command, the default behavior needed to be changed so that it displays output in long format automatically, similar to using the `-l` option. This includes showing file permissions, number of links, owner, group, file size, and last modified date.

For the `whoami` command, the output needed to be modified to print the message "You are:" before displaying the current logged-in user's username.

---

## 2. Describe the Solution
To modify the `ls` command, I edited the `ls.c` file and forced the output format to `long_format` after the command-line arguments were processed. This ensures that the command always displays detailed file information without requiring the `-l` option.

To modify the `whoami` command, I edited the `whoami.c` file and replaced the original `puts` statement with a `printf` statement. This allowed me to include a custom message ("You are:") before printing the username.

After making both changes, I rebuilt the coreutils package using the provided build script and tested the updated commands to confirm that the modifications worked correctly.

---

## 3. Pros and Cons of the Solution

### Pros
- The `ls` command now provides detailed file information by default, making it more informative.
- The `whoami` command is clearer and more user-friendly with the added message.
- The solution directly modifies the source code, ensuring consistent behavior every time the commands are run.

### Cons
- Changing default command behavior may confuse users who expect standard Linux outputs.
- The `ls` command now produces more detailed output, which may not always be necessary.
- These changes are specific to this modified version and do not apply to standard system commands.

## Screenshots
https://drive.google.com/file/d/1ugbBL1VF4pwyCNH0W-jsBYcw-LGhe63o/view?usp=sharing
