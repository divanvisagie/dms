# dms - Dark Mode Switcher

`dms` is a command-line tool for switching between dark and light modes on macOS and Linux. It allows you to toggle your system's theme with a simple command.  It also has a mechanism to reload tmux after switching to refresh the theme.

## Installation

**Using Cargo:**

```bash
cargo install dms
```

## Usage

```bash
dms [OPTIONS]
```

### Options

*   `-c, --check`: Only prints the current dark mode status (true or false).
*   `-f, --force-dark <true | false>`: Forces dark mode on or off.
    *   `true`: Enables dark mode.
    *   `false`: Enables light mode.
*   `-h, --help`:  Displays the help message.
*   `-V, --version`:  Displays the version of `dms`.

### Examples

1.  **Check the current dark mode status:**

    ```bash
    dms --check
    ```

    Output:

    ```
    true
    ```

2.  **Force dark mode on:**

    ```bash
    dms --force-dark true
    ```

3.  **Force light mode on:**

    ```bash
    dms --force-dark false
    ```

4.  **Toggle to opposite theme**
    ```bash
    dms
    ```

## Building from Source

1.  Clone the repository:

    ```bash
    git clone https://github.com/your-username/dms.git
    cd dms
    ```

2.  Build the project:

    ```bash
    cargo build --release
    ```

    The executable will be located in `target/release/dms`.

## Contributing

(A section on how users can contribute)

## License

GPL-2.0
