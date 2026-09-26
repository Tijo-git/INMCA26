# Python Installation

## Software Requirements

- A supported version of Windows, macOS, or Linux
- An internet connection
- Administrator access may be required to install Python for all users
- A terminal for checking the installation

Use the current stable Python 3 release offered by [python.org](https://www.python.org/downloads/). This project does not require third-party Python packages.

## Installation Steps

### Windows

1. Open [python.org/downloads](https://www.python.org/downloads/) and download the current stable Python 3 installer for Windows.
2. Run the downloaded installer.
3. On the first installer screen, select **Add python.exe to PATH** if that option is shown. This allows commands such as `python` to work in a terminal.
4. Choose **Install Now** for a standard installation. Approve any Windows permission prompt if required.
5. When installation completes, close and reopen PowerShell or Command Prompt so it picks up the updated PATH.

### macOS

1. Download the macOS installer for the current stable Python 3 release from [python.org/downloads](https://www.python.org/downloads/).
2. Open the downloaded `.pkg` file and follow the installer prompts.
3. Open Terminal after installation.

Some macOS systems include a `python3` command for system tools. Use `python3` to run the separately installed Python 3; do not remove or replace the system-managed Python.

### Linux

Many Linux distributions provide Python 3 through their package manager. Install the `python3` package using the instructions for your distribution, or follow the Python installation guidance from that distribution. Package manager commands differ by distribution.

Avoid replacing or removing the system-managed Python, since system tools may depend on it. Use the `python3` command to run Python 3.

## Verification Steps

1. Open a new terminal window.
2. Run the command for your operating system:

   **Windows PowerShell or Command Prompt:**

   ```text
   py --version
   ```

   If the Python launcher is unavailable, try:

   ```text
   python --version
   ```

   **macOS or Linux:**

   ```text
   python3 --version
   ```

3. Confirm the output reports Python 3, for example `Python 3.x.x`.
4. Optionally, check that the interpreter can execute a short command:

   **Windows:**

   ```text
   py -c "print('Python is ready')"
   ```

   **macOS or Linux:**

   ```text
   python3 -c "print('Python is ready')"
   ```

## Troubleshooting

- **The terminal says the command is not recognized or not found:** Close and reopen the terminal. On Windows, rerun the installer and ensure **Add python.exe to PATH** is selected, or use `py` if the Python launcher is installed. On macOS or Linux, try `python3`.
- **A command opens the Microsoft Store on Windows:** Try `py --version`. If needed, review Windows **Manage app execution aliases** settings and disable conflicting Python aliases.
- **The reported version is Python 2 or an unexpected version:** Use `py -3 --version` on Windows or `python3 --version` on macOS/Linux. Multiple Python versions can coexist.
- **Installation is blocked by permissions:** Choose an install-for-current-user option if available, or ask the computer administrator to install Python.
- **The installer will not download or run:** Confirm the download came from `python.org`, check the network connection, and follow any security guidance from your organization.

## Conclusion

After installing Python 3 and confirming its version in a terminal, the environment is ready to run this project's scripts. No additional packages are required.