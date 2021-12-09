# MANSPIDER

**Description:** MANSPDIER will "Crawl SMB shares for juicy information".

## Usage

Build the image locally \
```docker build -t MANSPIDER .```

Run MANSPIDER \
```docker container run MANSPIDER [SHARE/CIDR] -c [STRING_TO_SEARCH_FOR] -e [FILE_EXTENSION] -d [DOMAIN] -u [USERNAME] -p [PASSWORD]```
