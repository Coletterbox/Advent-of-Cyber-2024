# Day 1

## Task 1

(Click the "complete" button under where it asks if you've read the terms and conditions.) 

Things I tried:
- inspect element > change placeholder text in disabled textbox above that says "no answer needed" to "yes"
- inspect element > enable disabled textbox > write "yes"
- inspect element > change textbox to checkbox > tick checkbox

What we were supposed to do:
- read the terms and conditions

## Task 2

- "Join our Discord and say hi!" (I'd rather not.)
- "Follow us on LinkedIn!" (I did! :D)
- "Follow us on X!" (I'm not calling it that.)
- "Check out the subreddit!"

I have realised that I've started the write-up too early in the process.

## Task 3-6

(Also onboarding.)

## Task 7 (OPSEC)

Learning Objectives:
- Learn how to investigate malicious link files.
- Learn about OPSEC and OPSEC mistakes.
- Understand how to track and attribute digital identities in cyber investigations.

Notes:
- examine downloaded file in Terminal (use "file" command)
```console
secretlyapontianak:~$ file filename.mp3
```
- the file may be a .lnk (MS Windows shortcut) and not the format suggested by the extension
- use Exiftool on file (install first, if needed)
```console
secretlyapontianak:~$ exiftool filename.mp3
```
- check output for a PowerShell command
  - the following disables usual restrictions:
  ```console
  -ep Bypass -nop 
  ```
  - .DownloadFile() downloads a file
  - iex runs the file
- identify unique parts of the code, e.g. the signature; Google these
- look for:
    - usernames, email addresses that can link to public information
    - identifiable metadata in code, documents or images (e.g. for device names, GPS coordinates, timestamps)
