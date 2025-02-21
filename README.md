> Виконувала самостійно Слобожан Софія РПЗ-23А

  ### Лабораторна_ робота №3
Тема: “Знайомство з базовими командами CLI-режиму в Linux”

Мета роботи: 
Знайомство з базовими командами CLI-режиму в Linux.
Знайомство з базовими текстовими командами в термінальному режимі роботи в різних ОС.

---

### Glossary of Terms

1. **Command Interpreter** - A program that executes commands entered by the user and interacts with the operating system.

2. **Shell** - An interface that allows the user to interact with the operating system through the command line. It can be text-based (e.g., Bash) or graphical.

3. **Command** - An instruction that the user enters in the shell to perform a specific action, such as copying files or viewing the contents of a directory.

---

### Answers to Questions

1. **What basic information does the prompt provide?**  
   The prompt provides information indicating that the system is ready to accept commands. It may include the username, hostname, current directory, and other parameters that help the user navigate the environment.

2. **What are parameters and arguments needed for a command?**  
   Parameters and arguments allow the user to specify how the command should be executed. Parameters can modify the behavior of the command, while arguments indicate the objects the command should operate on (e.g., files or directories).

3. **What is the purpose of the `ls` command, and what parameters and arguments can it have? Provide 3 examples.**  
   The `ls` command is used to view the contents of a directory.  
   - Example 1: `ls` - displays a list of files and folders in the current directory.  
   - Example 2: `ls -l` - displays a detailed list of files with information about permissions, owner, size, and modification date.  
   - Example 3: `ls /home/user` - displays the contents of the `/home/user` directory.

4. **How can command history be used, and what advantages does it provide?**  
   Command history allows users to view and reuse previously entered commands, saving time and reducing the likelihood of errors. Users can navigate through command history using the up and down arrow keys.

5. **What is the purpose of the `echo` command?**  
   The `echo` command is used to output text or variable values to the screen. It is useful for checking variable values or displaying messages.

6. **Describe the concept of a variable in the Bash shell. What types of variables does it support?**  
   A variable in the Bash shell is a named storage location for data. Bash supports several types of variables, including:
   - Environment variables - accessible to all processes.
   - Local variables - accessible only within the current shell or function.

7. **What are the purposes of the `env`, `export`, and `unset` commands?**  
   - `env` - displays a list of environment variables.
   - `export` - makes a local variable available to child processes.
   - `unset` - removes a variable or function.

8. **What commands do you know for obtaining help on commands in the terminal?**  
   - `man <command>` - opens the manual for the specified command.
   - `--help` - often an available parameter for obtaining brief help about a command (e.g., `ls --help`).
     Хід роботи:
Опрацюйте всі приклади команд, що представлені у лабораторній роботі курсу NDG Linux Essentials - Lab 5: Command Line Skills та Lab 6: Getting Help. Створіть таблицю для опису цих команд 

  ![image](https://github.com/user-attachments/assets/9b86734e-1c1c-46bb-92ce-84f4f46acfcb)
  
  ### Control Questions

1. **What types of commands exist in the Bash shell?**  
   In the Bash shell, there are several types of commands:
   - **Built-in commands**: Commands that are implemented directly in the shell, such as `cd`, `echo`, and `export`.
   - **External commands**: Commands that are implemented in separate executable files, such as `ls`, `grep`, and `cp`.
   - **Scripts**: Files that contain a sequence of commands that can be executed in the shell.

2. **What are environment variables? What types are there? How can they be viewed in the terminal?**  
   Environment variables are variables that store information about the execution environment of a program. They can be system variables (e.g., `PATH`, `HOME`) or user-defined variables. To view environment variables in the terminal, you can use the `printenv` or `env` command.

3. **Describe the `$PS1` variable. How can its content be viewed in the terminal?**  
   The `$PS1` variable defines the format of the command prompt in the Bash shell. It can contain various characters that represent information such as the username, hostname, and current directory. To view its content, you can enter the command:
   ```bash
   echo $PS1
   ```

4. **How can the value of the `$PS1` variable be changed? What happens to the command prompt in Bash? How can this variable's value be changed permanently?**  
   To change the value of the `$PS1` variable, you can enter a command like:
   ```bash
   export PS1="[\u@\h \W]\$ "
   ```
   This will change the format of the command prompt. To change this variable's value permanently, you need to add this command to a configuration file, such as `~/.bashrc` or `~/.bash_profile`. The changes will take effect the next time you start a terminal session.

5. **What are quotes used for in the Bash shell?**  
   Quotes in the Bash shell are used to control the processing of text. There are three types of quotes:
   - **Single quotes (' ')**: The text inside is treated literally, with no variable expansion.
   - **Double quotes (" ")**: The text inside is processed, and variables are expanded, but special characters like `\` are processed.
   - **No quotes**: The text is processed, variables are expanded, and special characters are processed.

6. **What are control statements used for, and what types do you know?**  
   Control statements are used to manage the flow of execution in scripts or commands. Types of control statements include:
   - **Conditional statements (if, case)**: Allow commands to be executed based on conditions.
   - **Loops (for, while, until)**: Allow commands to be repeated.
   - **Control commands (break, continue)**: Used to manage the execution of loops.

7. **What is the difference if the command prompt ends with a `$` or a `#`?**  
   A `$` symbol indicates that you are logged in as a regular user, while a `#` symbol indicates that you are logged in as the superuser (root). This is important for security, as the superuser has more privileges and can execute commands that may change the system.

8. **What is the purpose of the `whereis` and `locate` commands? What is the difference between them?**  
   - The `whereis` command is used to locate the binary, source, and manual page files for a command. It provides information about where the command is installed on the system.
   - The `locate` command is used to find files by name in a database that is updated periodically. It is faster than searching the filesystem directly but may not always reflect the most current state of the filesystem.
   - The main difference is that `whereis` focuses on specific commands and their associated files, while `locate` searches for files based on their names across the entire filesystem.
   ### Conclusions  
In summary, this work provided valuable insights into the Bash shell in a Linux environment, covering essential skills such as creating and manipulating variables, defining aliases, and implementing functions. We learned the significance of quoting mechanisms and control statements for managing command execution. Additionally, we explored how to customize the command prompt and utilize help commands for better command understanding. Overall, these skills are fundamental for effectively navigating and utilizing the Linux command line, enhancing productivity and system management.
