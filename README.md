# miniShellPokemon

<p align="center">
	https://github.com/user-attachments/assets/a15d1706-bba4-4bac-beb5-78b0af40d7e0
	alt="miniShellPokemon preview" width="900">
</p>

<p align="center">
	A 42-style minishell with a Pokémon twist: a fully interactive shell written in C,
	paired with custom battle-themed data and ASCII art.
</p>

<p align="center">
	<img src="https://img.shields.io/badge/Language-C-blue?style=for-the-badge" alt="Language">
	<img src="https://img.shields.io/badge/Status-42%20project-111827?style=for-the-badge" alt="Status">
	<img src="https://img.shields.io/badge/Theme-Pokémon-ef4444?style=for-the-badge" alt="Theme">
</p>

## Overview

miniShellPokemon is a custom shell built as part of the 42 minishell journey, extended with a Pokémon-flavored layer.
It implements the core shell features expected from a Unix-like interactive shell and adds a playful game-oriented module backed by external Pokémon data.

## Features

- Command parsing with quotes, pipes, redirections, and wildcard expansion.
- Environment variable expansion and shell-like token handling.
- Builtin commands: `echo`, `cd`, `pwd`, `env`, `export`, `unset`, and `exit`.
- Here-doc support and signal handling for interactive use.
- Readline integration with command history.
- Pokémon battle mode with ASCII art, attacks, and external data support.

## Build

### Requirements

- GCC or Clang
- `readline`
- A Unix-like environment

### Compile

```bash
make
```

### Extra targets

```bash
make re      # full rebuild
make clean   # remove object files
make fclean  # remove objects and the binary
make vale    # run with valgrind and the provided suppression file
make poke    # clone the pokemonData repository if it is missing
```

## Run

```bash
./minishell
```

Example commands:

```bash
echo hello world
export USERNAME=gpicchio
pwd
cat file.txt | grep minishell
ls -la > output.txt
```

## Project Structure

- `parsing/` - lexical analysis, quote handling, expansions, redirections, and wildcard logic.
- `exec_commands/` - command execution, pipes, and process orchestration.
- `builtin/` - shell builtin implementations.
- `binary_tree/` - execution tree construction.
- `pipex/` - pipeline helpers reused by the shell.
- `pokemonData/` - data assets for the Pokémon-themed part of the project.

## Notes

- The project uses `libft` and `readline`.
- The `readLine.supp` file is provided to keep Valgrind output clean during interactive runs.
- The `poke` target expects Git to be available so it can fetch the data repository when needed.

---

Made for the 42 minishell project, with a Pokémon-inspired presentation layer.

