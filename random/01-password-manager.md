# Your own password manager

Here are the steps to make custom password manager. It might be useful in some cases.

1. Generate password randomly

    ```sh
    openssl rand -base64 13
    ```

1. Store it securely

    Copy the generated password, and paste it in a simple text file, after that, encrypt that file. I use [gpg](https://www.gnupg.org/download/index.en.html) for that.

    ```sh
    gpg -c passwords.txt
    ```

1. Use a very strong passphrase. Delete the original file

    ```sh
    rm passwords.txt
    ```

1. Get the password by decrypting the file

    ```sh
    gpg passwords.txt.gpg
    ```

    Enter the passphrase, and you have access to your passwords :smile:
