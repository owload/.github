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
- **Open your files in the app.** Photos and videos play in place, and file formats such as text, spreadsheets, HEIC and AVI are handled by extensions.

## Repositories

| Repository | What it is |
| --- | --- |
| [owload-frontend](https://github.com/owload/owload-frontend) | The web and desktop client: where the encryption happens |
| [editor-sdk](https://github.com/owload/editor-sdk) | The contract that file-format extensions are written against |
| [text-editor](https://github.com/owload/text-editor) | Extension: a plain-text (`.txt`) editor |
| [xlsx-editor](https://github.com/owload/xlsx-editor) | Extension: a spreadsheet (`.xlsx`) editor for React |
| [heic-viewer](https://github.com/owload/heic-viewer) | Extension: a view-only HEIC/HEIF photo viewer |
| [avi-viewer](https://github.com/owload/avi-viewer) | Extension: a view-only AVI viewer (re-wraps H.264 AVI into MP4 in the browser) |

## Contact

[info@owload.com](mailto:info@owload.com)
