# Introduction

This script is for **downloading scientific papers and bibtex** using Google Scholar, Crossref, SciHub, and SciDB.
The tool tries to download papers from different sources such as PDF provided by Scholar, Scholar related links, and Scihub.
It is also able to download the **bibtex** of each paper.

## Installation

Current working directory must be set to auto_paper_download/

Create and activate virtual environment:

### Linux

```bash
python3 -m venv ./venv
source venv/bin/activate
```

### Windows

```bash
python3 -m venv ./venv
venv/Scripts/activate
```

**Make sure the venv is activated!**


Install packages:

```bash
pip install -e.
```

## How to use

First, add your csv files that contains a list of DOIs you wanna download.

Then simply call:

```bash
python3 PyPaperBot
```

### Note

This program does take time as it delays its execution on purpose.
Get a cup of coffee or two meanwhile :)

This script is work in progress.

The output is to be produced under output directory.

## SciHub access

If access to SciHub is blocked in your country, consider using a free VPN service like [ProtonVPN](https://protonvpn.com/) 
Also, you can use proxy option above.

## Example

Using proxy

```
python -m PyPaperBot --query=rheumatoid+arthritis --scholar-pages=1 --scholar-results=7 --dwn-dir=/download --proxy="http://1.1.1.1::8080,https://8.8.8.8::8080"
```
```
python -m PyPaperBot --query=rheumatoid+arthritis --scholar-pages=1 --scholar-results=7 --dwn-dir=/download -single-proxy=http://1.1.1.1::8080
```

