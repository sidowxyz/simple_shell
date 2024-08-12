# Simple Shell Project

## Description
This project is a simple UNIX command interpreter written in C that replicates functionalities of the sh shell (sh). It allows for executing commands and scripts in both interactive and non-interactive modes.

## Features
- Handles commands in a similar manner to sh.
- Uses the PATH environment variable to find executable commands.
- Supports the Ctrl+C signal to not exit the shell.
- Handles errors similar to sh.
- Includes a custom getline function.
- Includes basic commands built into the shell:
  - `exit`
  - `env`
  - `setenv`
  - `unsetenv`
  - `cd`

## Installation
To install and compile the shell in your local environment, follow these steps:

```bash
git clone https://github.com/sidowxyz/simple_shell.git
cd simple_shell
gcc -Wall -Werror -Wextra -pedantic *.c -o hsh
```

## Usage
To start the shell in interactive mode, simply run:

```bash
./hsh
```

To use the shell in non-interactive mode, echo your commands into the shell followed by a pipe:

```bash
echo "ls -l" | ./hsh
```

## Examples
Here are some simple examples of using the shell:

**Interactive Mode:**
```
$ ./hsh
$ ls -l
total 10
-rw-r--r-- 1 user user  146 Aug 20 12:00 main.c
drwxr-xr-x 2 user user 4096 Aug 20 12:00 resources
$ exit
$
```

**Non-Interactive Mode:**
```
$ echo "pwd" | ./hsh
/home/user/simple_shell
$
```

## Contributing
Contributions to this project are welcome! Please fork the repository and submit a pull request with your features or fixes.

## Authors
- Sidow Adan - [GitHub](https://github.com/sidowxyz)
- A. Mahadai - [GitHub](https://github.com/AMahadai)

## License
This project is licensed under the MIT License - see the LICENSE.md file for details.

## Acknowledgments
- Holberton School for providing the project requirements.
- The open-source community for continuously inspiring and sharing knowledge.

