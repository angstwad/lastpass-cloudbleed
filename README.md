# lastpass-cloudbleed
Compares the publicly available CloudFlare domains list to your LastPass vault, listing potentially compromised domains in your vault.

## Install

```
pip install lastpass-cloudbleed
```

## Usage

```
usage: lastpass-cloudbleed [-h] [-u URL_TO_LIST] [-o OUTPUT_FILE]
                           [-f {group,id,name,password,url,username} [{group,id,name,password,url,username} ...]]

optional arguments:
  -h, --help            show this help message and exit
  -u URL_TO_LIST, --url-to-list URL_TO_LIST
                        URL to list of affected CloudFlare domains. Default is
                        https://raw.githubusercontent.com/pirate/sites-using-
                        cloudflare/master/sorted_unique_cf.txt.
  -o OUTPUT_FILE, --output-file OUTPUT_FILE
                        File to output affected domains to as CSV
  -f {group,id,name,password,url,username} [{group,id,name,password,url,username} ...],
  --fields {group,id,name,password,url,username} [{group,id,name,password,url,username} ...]
                        Fields to use in output, defaults: 'id', 'group',
                        'name', 'url', 'username'
```

