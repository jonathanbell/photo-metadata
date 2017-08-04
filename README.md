# photo-metadata

A PHP script that can update and read date metadata information from an image file.

## Usage

```
php photo-metadata [--read | --read-date | --write-date] [http://example.com/path/to/image.[jpg|JPG|png] | /local/path/to/image.[jpg|JPG|png] [yearmmdd]]
```

### Examples

Get information about an image file on the Internet:

```
php photo-metadata --read http://example.com/path/to/image.[jpg|JPG|png]
```

Get information about an image on the local hard disk:

```
php photo-metadata --read /path/to/image.[jpg|JPG|png]
```

Get the date an image was shot from a file on the Internet:

```
php photo-metadata --read-date http://example.com/path/to/image.[jpg|JPG|png]
```

Get the date an image was shot from a file on the local hard disk:

```
php photo-metadata --read-date /path/to/image.[jpg|JPG|png]
```

Write (or overwrite) IPTC date to a local image file:

```
# NOTE: Pass the date param in the form: 20170101 (yearmmdd)
# Currently, this parameter is not validated.
php photo-metadata --write-date /path/to/image.[jpg|JPG|png] 20170101
```
