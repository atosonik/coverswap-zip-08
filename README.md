# coverswap-zip-08

Zip piece 8 of 9 from https://github.com/atosonik/coverswap.git.

Each `.zip` file is under GitHub's 100 MB limit. Together they stay under 500 MB.

## Restore the project

Download every `coverswap-zip-*` repo listed in `SPLIT.json` and unzip all of the archives into one folder:

```bash
mkdir coverswap && cd coverswap
find /path/to/coverswap-zip-repos -name '*.zip' -exec unzip -n {} \;
python chunker.py merge
```

`unzip -n` keeps the first copy of a path. The zip pieces do not overlap.
