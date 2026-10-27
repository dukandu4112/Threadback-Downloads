# Start using Threadback on Windows

## Download and open

1. Open the public Threadback-Downloads repository's **Releases** page. No GitHub account is required for a public download.
2. Download **Threadback-1.0.1-Windows.zip** under **Assets**. The automatic **Source code** downloads are for developers.
3. Right-click the ZIP and choose **Extract All**. Open the extracted **Threadback** folder.
4. Open **Threadback.exe**. Keep the `app` and `runtime` folders next to it. Java is included; a separate Java installation is unnecessary.

The build was tested on a Windows x64 GitHub Actions runner. Windows ARM, macOS, and every individual Windows device have not been verified.

## Your first return point

1. Give your thread a name, such as **Fix the search result order**.
2. Write your last thought: **The older response replaces the newer one**.
3. Write a next tiny action: **Read the callback that updates the result list**.
4. Optionally add a project, blocker, and breadcrumb. A breadcrumb can be a filename or URL; Threadback stores it as text.
5. Choose **Park this thought**.
6. Open the saved thread, read Return Mode, and choose **I'm back — resume**.
7. Close and reopen Threadback. Your saved thread should still be present.

Use **I need a gentle start** when you want a smaller starting step. Edit your capture when your context changes. Earlier captures remain in history, and reusing one creates a new capture.

## Back up and recover

Choose **Backup** in the header and select a new filename. Existing backup files are not overwritten. Keep a copy on another drive if you want protection against device failure.

**Restore backup** replaces the current workspace after confirmation. Threadback first saves a recovery snapshot under `recovery-backups` next to the live database. It validates the selected source and leaves the source backup unchanged.

Your default data location is `%USERPROFILE%\.threadback\threads.db`. Data and backups are unencrypted. Removing the extracted application folder does not remove this separate data folder.

## If it does not open

- Extract the complete ZIP before launching; do not run the executable from inside the ZIP.
- Keep the original folder structure. Moving only the executable leaves its runtime behind.
- Close an existing Threadback window before opening the same workspace again.
- Record any exact error text and the Windows version when reporting a problem. Do not attach your database or private notes to a public issue.
- If Windows displays a security warning, check the download source and checksum. Do not disable Windows security protections to run the app. The release does not claim a verified publisher signature.

## Check the download

Download **SHA256SUMS.txt** from the same release. In PowerShell, run:

```powershell
Get-FileHash .\Threadback-1.0.1-Windows.zip -Algorithm SHA256
```

Compare the result with the ZIP's entry in SHA256SUMS.txt. A matching checksum detects an incomplete or altered download; it is not a publisher signature.

F1 opens Help. See [README.md](README.md) for keyboard shortcuts and [VALIDATION.md](VALIDATION.md) for the test scope.

