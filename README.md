# A sample to run `rsync` with debian-based image

## Usage

Build.

```zsh
docker build -t rsync src/
```

Copy all the contents of `volume_from` to `volume_to`.

```zsh
docker run --rm -it -v volume_from:/from -v volume_to:/to rsync rsync -arv /from/ /to
```

`/` in the end of `/from/` is required.
