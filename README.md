# chext

**chext** is a simple Bash script designed to change file extensions.

## Installation

To install the `chext` script on your system, use the following `curl` command.<br>
This command downloads the script from the GitHub repository and installs it to `/usr/bin` with the appropriate permissions.

Run the following command as a superuser (root):

```bash
sudo bash -c 'file="/usr/bin/chext"; curl -L "https://raw.githubusercontent.com/ycomiti/chext/main/chext" --output "${file}"; chown -v root:root "${file}"; chmod -v 755 "${file}"'
```

### Command Details

- `curl -L "https://raw.githubusercontent.com/ycomiti/chext/main/chext" --output "${file}"`: Downloads the `chext` script from the GitHub repository.
- `chown -v root:root "${file}"`: Changes the owner of the script to `root`.
- `chmod -v 755 "${file}"`: Sets the script permissions to be executable by everyone.

## Usage

After installation, you can use the `chext` script to rename files by changing their extensions.<br>
Here’s how to use it:

### Basic Syntax

```bash
chext <file> <ext>
```

- `<file>`: The path to the file you want to rename.
- `<ext>`: The new extension you want to assign to the file.

### Example

Suppose you have a file named `document.txt` and you want to change its extension to `.md`. You would use the following command:

```bash
chext document.txt md
```

After running this command, the file `document.txt` will be renamed to `document.md`.

### Notes

- Ensure that the file you want to rename exists before using the command.<br>
  If the file does not exist, the script will display an error message.
- The new extension should not include a dot (`.`); just provide the extension name (e.g., `md` instead of `.md`).

## License

This project is licensed under the **GNU General Public License v3.0 (GPL-3.0)**.<br>
You may copy, modify, and redistribute this software under the terms of this license.<br>
For more information, please refer to the `LICENSE` file included in this repository.

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request.<br>
For more details, see the `CONTRIBUTING.md` file.

## Support

For support or issues, please open an issue on the [GitHub repository](https://github.com/ycomiti/chext/issues).
