# docker-node

## Basic usage

### gitbook

Run the following command in the GitBook repoistory:

```bash
docker run --name=gitbook --rm -v $(pwd):/gitbook -p 4000:4000 tommylau/gitbook
```

then you can visit the GitBook preview at the following address: ```http://localhost:4000/```

If you want to see the quit, press ```CTRL + C``` to terminate the program.

### hexo

Run the following command in the Hexo repoistory:

```bash
docker run --name=hexo --rm -v $(pwd):/hexo -p 4000:4000 tommylau/hexo
```

then you can visit the Hexo preview at the following address: `http://localhost:4000/`

If you want to see the quit, press `CTRL + C` to terminate the program.

## Advanced usage

Copy `hexo` and `gitbook` from `bin` to your system's run path, for example: `/usr/local/bin/` and remember to give them to execute right:

```bash
chmod +x /usr/local/bin/hexo
chmod +x /usr/local/bin/gitbook
```

Then you can call `hexo` or `gitbook` just like it's a native program, you can't even feel the containers ever existed.

```bash
$ cd /path/to/hexo
$ hexo generate
$ hexo deploy
```

```bash
$ cd /path/to/gitbook
$ gitbook pdf
$ gitbook epub
```

