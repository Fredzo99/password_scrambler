# Password Scrambler

Welcome to Password Scrambler, a small utility written in Python to generate secure and complicated passwords. This tool is designed to enhance the security of your passwords by creating long, non-dictionary-based, and unique passwords for different logins and domains. You only need to remember your easy password and the document used as a generation base.

## Benefits

- **Enhanced Security**: Generates long, non-dictionary-based passwords for increased security.

- **Easy to Remember**: You only need to remember your easy password and the document used as a generation base.

- **Unique Passwords**: Even if you reuse the easy password and base file, different logins at different domains will result in totally new long passwords.

- **No Storage of Complicated Password**: The tool does not save your complicated password anywhere, making it resistant to theft and decryption.

- **Open Source**: Written in Python, the code is open source, allowing everyone to review it before use and make custom changes.

## Installation

To use Password Scrambler, follow these steps:

1. Install Python 3 and PIP on your system.
2. Clone this repository:
   ```bash
   git clone https://github.com/Fredzo99/password_scrambler.git
   ```
3. Navigate to the project directory:
   ```bash
   cd password_scrambler
   ```
4. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## How it Works

```bash
./passcrambler.py --help
```

### Usage

```bash
./passcrambler.py --file FILE --login LOGIN [--special SPECIAL] [--length LENGTH] [--clip] [--scramble-func FUNC]
```

### Optional Arguments

- `--file FILE`: File used to initialize generation.
- `--login LOGIN`: Login for which you want to use the password.
- `--special SPECIAL`: Whitelist of special characters (default='_&#').
- `--length LENGTH`: Length of the password (default=30).
- `--clip`: Copy the generated password into the clipboard instead of displaying.
- `--scramble-func`: Hashing function to use for input data scrambling (default=md5).

### Example

```bash
./passcrambler.py --file MyPhoto.jpg --login hasherezade@hasherezade.net
Password: _password123_
---
txork9Zfa8yXc_lMbb1LCHPZIH7wE1
---
```

### Typical Scenario

1. Need to generate a new password for an email.
2. Prepare an easy password to remember and a document to keep safe without changes.
3. Deploy Password Scrambler with your login and the document.
4. Input the easy password when prompted.
5. Copy the generated password and use it for your email service.
6. Whenever you need to re-login, deploy Scrambler with the same parameters to regenerate the same hash.

## Contributing

Feel free to contribute to Password Scrambler by making edits or commits to enhance functionality or fix bugs. Follow the standard GitHub flow:

1. Fork the repository.
2. Create a new branch for your changes:
   ```bash
   git checkout -b feature/new-feature
   ```
3. Make your changes and commit them:
   ```bash
   git commit -m "Add new feature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/new-feature
   ```
5. Create a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Contact

If you have any questions, feedback, or suggestions, feel free to reach out to Fredzo99.

Thank you for using Password Scrambler!
