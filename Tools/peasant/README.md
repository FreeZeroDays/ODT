# peasant

**Description:** peasant is another one my go-to LinkedIn-focused tools when performing both external and internal penetration tests.

## Usage

Build the image locally \
```docker build -t peasant .```

Run peasant \
```docker container run peasant harvest -C [CREDS] -cns [COMPANY] -of [OUTPUTFILE.CSV]`
