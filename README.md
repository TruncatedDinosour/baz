# Baz

> A lightweight plugin manager for GNU bash

# Credits

- @DannyBen -- For creating an awesome tool for completion: https://github.com/DannyBen/completely

# Dependencies

- GNU coreutils
- GNU bash
- Git cli
- Linux
- Rlwrap (optional, but it's nice for special keys)
- Bash-completion (optional, but it's nice for well.. Completion)

# Plugin indexing

You can leave a link to it in the [PLUGINS.md](/PLUGINS.md) file :)

# Setup

0. Clone the repo

```bash
$ git clone https://github.com/TruncatedDinosour/baz-example-plugin
```

1. Install the script anywhere, or even run it standalone

- Running standalone means just running it
- Installing could be done in for example `/usr/local/bin`:

```bash
$ su -c 'install -Dm755 baz /usr/local/bin'
```

2. Setup

```bash
$ baz setup
```

Or

```bash
$ ./baz setup
```

3. Add this to your `~/.bashrc`:

```bash
export BAZ_LOADER_ENABLED=true
[ -f "$HOME/.local/share/baz/loader.sh" ] && source "$HOME/.local/share/baz/loader.sh"
```

This is the main loader for plugins

# Installing completion

```bash
$ ./scripts/comp.sh
```

# Help page

```bash
$ ./baz help
```

# Upgrading

Just upgrade your package or pull the repo
and run:

```bash
$ ./baz upgrade
```

And if you also have completion, rerun the completion
script:

```bash
$ ./scripts/comp.sh
```

# Other docs

- [Doc folder](/doc)

# Examples

- [Examples folder](/examples)
- [My example plugin repo](https://github.com/TruncatedDinosour/baz-example-plugin)
