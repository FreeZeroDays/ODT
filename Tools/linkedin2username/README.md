# Linkedin2username

**Description:** Linkedin2username is my go-to OSINT tool when performing both external and internal penetration tests.

## Usage

Build the image locally \
```docker build -t linkedin2username .```

Run linkedin2username and store the data locally \
```docker container run -v /$HOME/output/:/linkedin2username/li2u-output linkedin2username -u [USERNAME] -p [PASSWORD] -c [COMPANY]```
