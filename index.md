
# Lab Report 4 - Vim and Command Line Efficiency

## Introduction

This lab focused on debugging Java code using Vim and improving workflow efficiency through command line techniques. The main task involved fixing a bug in a method that merges two sorted lists.

## Debugging Process

### Baseline Measurement

Before beginning the debugging, I measured the time it took to complete the tasks without any efficiency techniques.

### Debugging Steps

#### Step 4: Cloning the Repository

Cloned the repository to start the debugging process.

- **Keys Pressed**: `git clone <SSH URL>` `<enter>`
- **Effect**: Cloned my GitHub repository to the ieng6 account.

![Step 4 Screenshot](/path/to/your/screenshot4.png)

#### Step 5: Running the Tests (Before Fix)

Ran the tests to demonstrate the failure and identify the bug.

- **Keys Pressed**: `<up>` `<enter>`
- **Effect**: Tests failed, indicating a bug in the code.

![Step 5 Screenshot](/path/to/your/screenshot5.png)

#### Step 6: Editing with Vim to Fix the Bug

Opened the file in Vim, navigated to the bug, and edited the code.

- **Keys Pressed**: `vim ListExamples.java` `<enter>` `/<buggy_method>` `<enter>` `i`
- **Code Change**: Changed `index1 += 1;` to `index2 += 1;` in the `merge` method's second `while` loop.
- **Effect**: Fixed the logical error.

![Step 6 Screenshot](/path/to/your/screenshot6.png)

#### Step 7: Running the Tests (After Fix)

Reran the tests to ensure the bug was fixed.

- **Keys Pressed**: `<up>` `<up>` `<enter>`
- **Effect**: Tests succeeded, confirming the fix.

![Step 7 Screenshot](/path/to/your/screenshot7.png)

#### Step 8: Committing and Pushing the Changes

Committed the fixed code and pushed the changes to GitHub.

- **Keys Pressed**: `git add ListExamples.java` `<enter>` `git commit -m "Fix merge bug"` `<enter>` `git push` `<enter>`
- **Effect**: Updated the repository with the fixed code.

![Step 8 Screenshot](/path/to/your/screenshot8.png)

#### Step 9: Documenting Time Improvement

After implementing efficiency techniques, I noted an improvement in completion time.

**Improved Time**: _[Insert your improved time here]_

**Efficiency Gains**: _[Describe efficiency gains here]_

![Step 9 Screenshot](/path/to/your/screenshot9.png)

## Command Line Efficiencies Utilized

### Using Bash History

Utilized up/down arrows and Ctrl-R to quickly access previous commands.

### Using Tab for Autocompletion

Leveraged the Tab key's autocomplete feature to speed up command typing.

### Keyboard Shortcuts

Improved efficiency with shortcuts like Ctrl-U, Ctrl-K, Ctrl-A, Ctrl-E, Ctrl-W, and Alt-Left/Right.

### Quick Copy/Paste

Streamlined text selection and manipulation with mouse and keyboard shortcuts.

## Conclusion

This lab enhanced my debugging skills in Vim and command line navigation efficiency. Applying these techniques allowed for a more streamlined development process, highlighting the importance of mastering the tools at our disposal.

