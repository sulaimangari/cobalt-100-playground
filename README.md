## Running arm machine SSH through github arm runner
- Profide your secret key with **AUTHORIZED_KEY** (convert your public key to base64 before pasting)
- Check 'run tunnel' job for served port
- It will be displayed like this:

    ```console
    2025-05-20T11:29:58.208254Z  INFO bore_cli::client: connected to server remote_port=41974
    2025-05-20T11:29:58.208277Z  INFO bore_cli::client: listening at bore.pub:41974
    ```

- Now you can run SSH

    ```bash
    ssh -p 41974 runner@bore.pub
    ```
