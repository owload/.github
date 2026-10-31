# Owload

**Cloud file storage with security you can verify.** [owload.com](https://owload.com)

Owload keeps your files in an encrypted drive. Everything is encrypted on your device before it is sent: the contents, the names and the
folder structure. The server stores only ciphertext and never receives your password or your keys, so a breach of the server or of the storage
reveals only ciphertext.

## What makes it different

- **Encrypted on your device.** AES-256 with keys derived from your password, which never leaves the browser or the desktop app.
- **A client you can inspect.** The code that does the encrypting is open, so you can check what it does instead of taking our word for it.
- **Your storage, or ours.** Keep a drive on Owload's storage, on your own S3-compatible bucket, or on several at once, each holding a copy.
- **Share without giving up the keys.** Invite people to a drive as readers, writers or admins, or publish a read-only link.
- **Open your files in the app.** Photos and videos play in place, and file formats such as text, spreadsheets and HEIC are handled by extensions.

## Three ways to use Owload

| | Where your encrypted files are | Who runs the service | Cost |
| --- | --- | --- | --- |
| **Web version** | Owload's storage, 3 GB | Owload | Free |
| **Web version with your own S3** | **Your S3 bucket**, as much as it holds | Owload | Free |
| **Self-hosted** | **Your S3 bucket** | **You**, from the Docker images | Free (your own server) |

The self-hosted version is the same Owload: the client, the API, the database and your sign-in (Keycloak) run on your server, from the images on
Docker Hub. Nothing of yours is on Owload's servers. Paid plans with more space on Owload's storage are coming soon.

## AI Guard

An AI agent keeps watch over the server and its logs and checks that nothing suspicious is going on. Before every release the code is also
reviewed by AI, attacked by AI the way a real attacker would, and reviewed by engineers. Nothing ships on the AI's word alone.

## Repositories

| Repository | What it is |
| --- | --- |
| [owload-frontend](https://github.com/owload/owload-frontend) | The web client: where the encryption happens |
| [owload-backend](https://github.com/owload/owload-backend) | The API: accounts, drives, access, and the encrypted data. It never receives a password or a key |
| [owload-keycloakify](https://github.com/owload/owload-keycloakify) | The sign-in and registration pages (a Keycloak theme) |
| [owload-docs](https://github.com/owload/owload-docs) | The architecture, the decisions behind it and the operating notes |
| [editor-sdk](https://github.com/owload/editor-sdk) | The contract that file-format extensions are written against |
| [text-editor](https://github.com/owload/text-editor) | Extension: a plain-text (`.txt`) editor |
| [xlsx-editor](https://github.com/owload/xlsx-editor) | Extension: a spreadsheet (`.xlsx`) editor for React |
| [heic-viewer](https://github.com/owload/heic-viewer) | Extension: a view-only HEIC/HEIF photo viewer |

## Contact

[info@owload.com](mailto:info@owload.com)
