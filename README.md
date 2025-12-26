Bitcoin Mnemonic Recovery Tool

Overview :-
This tool helps recover up to 3 lost words from a BIP39 mnemonic seed phrase, supporting both 12-word and 24-word phrases. It is designed to assist users who may have lost a few words from their seed phrase and need to recover access to their Bitcoin wallets.

Warning: This tool is intended for educational purposes only. Use it wisely and securely. Never share your seed phrase or private key with anyone. Always ensure you are using it in a trusted environment.

Features :-
Recovery of up to 3 lost words from BIP39 12-word and 24-word seed phrases.

Compatible with Bitcoin and other cryptocurrencies that use BIP39.

Works by systematically guessing missing words and testing valid combinations to recover the full seed phrase.

Designed for local use with no need for internet access, ensuring maximum privacy.

Installation

To use this tool, follow these steps:

1. Clone this repository
git clone https://github.com/yourusername/bitcoin-mnemonic-recovery-tool.git
cd bitcoin-mnemonic-recovery-tool

2. Install dependencies

If you're using Python, ensure that Python 3.7+ is installed. Then, run:

pip install -r requirements.txt

Usage -
1. Prepare Your Seed Phrase

You will need the 12-word or 24-word seed phrase with missing words. The tool will attempt to recover those missing words.

2. Input Format

Use ? to indicate missing words in your seed phrase. The tool will recover those missing words. For example:

Example of a 12-word seed phrase with missing words:

abandon ability absent ? abyss actor actress acute adult amazing


In the above example, the ? represents a missing word.

3. Run the Recovery Tool

Execute the script to start the recovery process:

python recover_mnemonic.py


You will be prompted to input your seed phrase with the missing words represented as ? (Question mark symbol).

Example input:

Enter your seed phrase with missing words (use ? for missing words):
abandon ability absent ? abyss actor actress acute adult amazing

4. Recovery Process

The tool will systematically guess the missing words using a pre-defined BIP39 wordlist. Depending on how many words are missing, the recovery process may take a few moments.

Once the missing words are found, the tool will show the recovered seed phrases.

5. Use the Recovered Seed Phrase

After the missing words are recovered, you will be able to use the full seed phrase to recover your Bitcoin wallet on any compatible wallet software (e.g., Electrum, Bitcoin Core).

Example
$ python recover_mnemonic.py
Enter seed phrase with missing words (use ? for missing words):
abandon ability absent ? abyss actor actress acute adult amazing
Starting recovery...
Recovery process complete. Possible recovered seed phrases:

1. abandon ability absent board abyss actor actress acute adult amazing
2. abandon ability absent bread abyss actor actress acute adult amazing
3. abandon ability absent bronze abyss actor actress acute adult amazing
...

Important Notes

Security: Never share your seed phrase with anyone. Only enter it in trusted, secure environments.

Privacy: The recovery process happens locally and no information is transmitted to external servers.

Word List: This tool uses the official BIP39 word list. Ensure that the missing words are from this list.

Partial Recovery: If only one or two words are missing, the tool can attempt all valid combinations of words in those positions to recover the full seed phrase.

Contributing

If you'd like to contribute to this project, feel free to fork the repository and submit a pull request. Any improvements, bug fixes, or new features are always welcome!

Support the Project

**If you find this tool useful and would like to support its development, feel free to send a donation to the following Bitcoin address:

bc1qljc2hgctk9xhwgk8t2t6f7nlccdvxg78xzt57k

Thank you for your support! 💖**

License

This project is licensed under the MIT License - see the LICENSE
 file for details.

Disclaimer

Use this tool at your own risk. While this tool is designed to recover lost words from a mnemonic seed phrase, there is always a possibility of errors. Always test the recovered seed phrase with caution and ensure you are using it in a safe and trusted wallet.
