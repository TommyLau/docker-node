# docker-node

## gitbook

### How to use it:

Run the following command in the GitBook repoistory:

```
docker run --rm -v $(pwd):/gitbook -p 4000:4000 tommylau/gitbook
```

then you can visit the GitBook preview at the following address: ```http://localhost:4000/```

If you want to see the quit, press ```CTRL + C``` to terminate the program.

