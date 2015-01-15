# docker-node

## gitbook

### How to use it:

Run the following command in the GitBook repoistory:

```bash
docker run --name=gitbook --rm -v $(pwd):/gitbook -p 4000:4000 tommylau/gitbook
```

then you can visit the GitBook preview at the following address: ```http://localhost:4000/```

If you want to see the quit, press ```CTRL + C``` to terminate the program.

## hexo

### How to use it:

Run the following command in the Hexo repoistory:

```bash
docker run --name=hexo --rm -v $(pwd):/gitbook -p 4000:4000 tommylau/hexo
```

then you can visit the Hexo preview at the following address: ```http://localhost:4000/```

If you want to see the quit, press ```CTRL + C``` to terminate the program.
