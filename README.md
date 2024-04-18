# lotr-commit - Middle-Earth Generated Git Commit Messages

Use the `lotr-commit` command to generate commit messages, modify them, and commit!

![lotr-commit screenshot](https://raw.githubusercontent.com/tnorthcutt/lotr-commit/c1e5a1c11ddf65d8c4d3aa024eb17b2b218790cb/lotr-commit.png)

Forked from https://github.com/marissamarym/commitm

## Features

- Generates commit messages using the `llm` CLI based on staged changes
- Allows modifying messages to be more general, specific, longer, shorter etc
- Commits generated messages (with the prefix 🧙) or custom messages

## Getting Started

### Prerequisites

Install and configure the [llm](https://llm.datasette.io/en/stable/#quick-start) CLI tool. `llm` needs an API key (like the OpenAI API key) to make LLM calls.

### Installation

Clone this repository to your desired location:

```bash
git clone https://github.com/tnorthcutt/lotr-commit.git
```

To make the script easily accessible from anywhere, add the following alias to your .zshrc file:

```bash
echo 'alias lotr-commit="$HOME/path/to/lotr-commit/src/lotr-commit.zsh"' >> ~/.zshrc
```

Replace `$HOME/path/to/lotr-commit` with the actual path to where you cloned or placed `lotr-commit`.

Apply the changes to your `.zshrc` by running:

```bash
source ~/.zshrc
```

## Usage

To generate a commit message:

```bash
lotr-commit
```

To generate a commit message and commit it immediately:

```bash
lotr-commit -e
```

To generate a commit message with a custom prefix (✨) (default is 🧙):

```bash
lotr-commit -p ✨
```

To generate a commit message without a custom prefix (default is 🧙):

```bash
lotr-commit --no-prefix
```

To generate a commit message and commit immediately without showing output:

```bash
lotr-commit -e -q
```

## Caveats

- `lotr-commit` limits the prompt to 4096 tokens.

## Contributing

Any contributions you make are greatly appreciated.

## License

Distributed under the MIT License. See LICENSE for more information.
