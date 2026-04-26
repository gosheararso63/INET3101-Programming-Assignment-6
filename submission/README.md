# Programming Assignment 6

## Problem Statement
This assignment required modifying the ls and whoami commands.

The ls command was modified so that it displays long format output by default instead of requiring the -l option.

The whoami command was modified to print "You are:" before displaying the username.

## Describe the Solution
For ls.c, I updated the code to force the format to long_format after processing command-line arguments.

For whoami.c, I replaced the puts function with printf to include a custom message before the username.

After making the changes, I rebuilt the program and tested both commands to verify the updated behavior.

## Pros and Cons

### Pros
Provides more detailed file information by default.
Improves clarity of whoami output.

### Cons
Changes default Linux behavior, which may confuse users.
Long format output may be unnecessary in some cases.
