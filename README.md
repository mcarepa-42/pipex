# Pipex

`pipex` is a 42 project that recreates the behavior of shell pipes and redirections in C.

The program receives an input file, two commands, and an output file. It connects the commands with a pipe so that the output of the first command becomes the input of the second command.

Equivalent shell behavior:

```bash
< infile cmd1 | cmd2 > outfile
```

## How to download

Clone the repository:

```bash
git clone https://github.com/mcarepa-42/pipex.git
cd pipex
```

Or download it from GitHub by clicking **Code** > **Download ZIP**, then extract the ZIP and open a terminal inside the project folder.

## Requirements

You need:

- `make`
- a C compiler such as `cc`, `gcc`, or `clang`
- a Unix-like system such as Linux or macOS

## How to build

```bash
make
```

This creates the executable:

```text
./pipex
```

To build the bonus version, if needed:

```bash
make bonus
```

## How to run

Basic syntax:

```bash
./pipex infile "cmd1" "cmd2" outfile
```

Example:

```bash
echo "hello world" > infile
./pipex infile "grep hello" "wc -w" outfile
cat outfile
```

This behaves like:

```bash
< infile grep hello | wc -w > outfile
```

Another example:

```bash
./pipex infile "cat" "wc -l" outfile
```

## Useful commands

```bash
make clean    # Remove object files
make fclean   # Remove object files and the pipex executable
make re       # Rebuild everything
```

## Notes

The project focuses on file descriptors, `fork`, `pipe`, `dup2`, `execve`, process management, and error handling.
