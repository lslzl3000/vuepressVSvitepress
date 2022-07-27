## How to Test

Try to build docs(about 1000 .md) by vuepess and vitepress

```bash
# first try vuepress
npm run build:vupress
# then try vitepress
npm run build:vitepress
```

1. You will see how much longer the `Vuepress` will take, in my Macbook Pro 2022 with M2, 13~14min vs 60~70s
2. `Vuepress` also use much much more memory then `Vitepress`
It has to build with `NODE_OPTIONS=--max_old_space_size=20480`, otherwise node process will exit by JavaScript heap out of memory 
