# Slate Goodnight

## Run

```bash
git clone https://github.com/harryuan65/slate.git
cd slate
bundle lock --add-platform x86_64-linux # for M1 Macs
docker build . -t slatedocs/slate
docker run --rm --name slate -p 4567:4567 -v $(pwd)/source:/srv/slate/source slatedocs/slate serve
```
