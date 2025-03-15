# Backdrop CMS 1.27.1 Authenticated Remote Code Execution Exploit

This script exploits a vulnerability in **Backdrop CMS** version 1.27.1 to gain remote code execution by uploading a malicious PHP web shell. The exploit requires authenticated access as an administrator.
Kudos to the original exploit author Ahmet Ümit BAYRAM on ExploitDB (https://www.exploit-db.com/exploits/52021). I modified their script so that the file upload is automized.

## Overview

Backdrop CMS (version 1.27.1) is vulnerable to a remote code execution (RCE) vulnerability where an authenticated administrator can upload a `.tar.gz` file containing a malicious PHP web shell. This exploit allows attackers to execute arbitrary commands on the vulnerable server by interacting with the web shell.

## Prerequisites

- **Backdrop CMS version 1.27.1** is required for this exploit.
- **Administrator credentials** are needed for successful exploitation.
- Python 3.x with the following dependencies:
    - `requests`
    - `BeautifulSoup4`
    - `argparse`
    - `re`
    - `json`
    - `tarfile`
  
You can install the necessary dependencies using pip:

```bash
pip install requests beautifulsoup4
