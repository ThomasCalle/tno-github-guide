#  Instructor Demo: Command Line

* Terminal commands are useful ways to navigate between folders, also called directories, quickly and easily. The commands are entered into the terminal or bash.

* Open your terminal and do the following:

  * We use `ls` to list the contents of the current directory. In the home directory, we see a list of directories including the `Desktop` directory. 

  ```bash
  ls
  ```

  * We use `cd` to change directories. We can change into the `Desktop` directory with the following command: 

  ```bash
  cd Desktop
  ```

  * To move back up to our previous directory, we use `cd ..`. 

  ```bash
  cd ..
  ```

  * We check our working directory with `pwd`. When we print the working directory, it shows us the path.

  ```bash
  pwd
  ```

  * To create a new folder inside the `Desktop` directory, we navigate into the `Desktop` directory using `cd`.

  ```
  cd Desktop
  ```

  * We use the `mkdir` command to create a new directory named `demo-folder`.
 
  ```bash
  mkdir demo-folder
  ```

  * To add a file to our new directory, we first use `cd` to navigate into `demo-folder`.

  ```bash
  cd demo-folder
  ```

  * We use `touch` to create a new file named `index.html`.

  ```bash
  touch index.html
  ```

  *  We use `ls` to check that our new file has been successfully added to the directory.

  ```bash
  ls
  ```

---
This guide ensures efficient collaboration in 2024 using GitHub and VSCode on both Windows and macOS.

A special thank you to all the mentors and volunteers who made this TNO Community possible and accessible to all participants.

© 2024 Thomas Calle. Confidential and Proprietary. All Rights Reserved.