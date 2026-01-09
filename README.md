HashLab
What this is

HashLab is a simple, educational Python tool that shows how common password hashes can be cracked using basic dictionary attacks.

It’s not meant to be fast, advanced, or stealthy.
The point is to understand how hashing works and why weak passwords are a problem.

Why I built it

I wanted something small and readable that helps connect the dots between:

hashing algorithms

stored password hashes

and how attackers test guesses using wordlists

This is meant for learning, not real-world attacks.

How it works (high level)

You choose a hashing algorithm

You provide a wordlist file

Each word is hashed and compared to the target hash

If there’s a match, the original word is printed

That’s it. No magic.

Usage

Run the script:

python hash_cracker.py


You’ll be prompted for:

The hash type (MD5, SHA256, etc.)

A wordlist file path

The hash you want to test

Wordlist requirement (important)

This program does not include a wordlist.

You must provide your own .txt wordlist file (for example, a common password list).
Large wordlists like rockyou.txt are intentionally not included in this repository.

This keeps the project lightweight and avoids redistributing large datasets.

Supported algorithms

MD5

SHA1

SHA224

SHA256

SHA384

SHA512

Requirements

Python 3.x

pyfiglet

Install dependencies:

pip install pyfiglet

Disclaimer

This project is for educational purposes only.
Use it only on data you own or have permission to test.
