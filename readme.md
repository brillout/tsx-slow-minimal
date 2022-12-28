```bash
git clone git@github.com:brillout/tsx-slow
cd tsx-slow/
pnpm install
```

Same as single line (copy-paste me):

```shell
git clone git@github.com:brillout/tsx-slow && cd tsx-slow/ && pnpm install
```

Run the server with `ts-node` and measure how long it takes for `Server running at http://localhost:3000` to show.

```bash
pnpm exec ts-node server/index.ts
```

Now run the server with `tsx` and measure how long it takes for `Server running at http://localhost:3000` to show.

```bash
pnpm exec tsx --no-cache server/index.ts
```

Observe that `tsx --no-cache` is much slower than `ts-node` (on my machine `tsx` is 4x slower).

Even when using tsx's cache, `tsx` is still more than 2x slower than `ts-node`.
