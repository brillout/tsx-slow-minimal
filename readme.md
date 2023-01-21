```bash
git clone git@github.com:brillout/tsx-slow-minimal
cd tsx-slow-minimal/
pnpm install
```

Same as single line (copy-paste me):

```shell
git clone git@github.com:brillout/tsx-slow-minimal && cd tsx-slow-minimal/ && pnpm install
```

Run `index.ts` with `ts-node` and measure how long it takes for `console.log(vite)` to show.

```bash
pnpm exec ts-node index.ts
```

Now run `index.ts` with `tsx` and measure how long it takes for `console.log(vite)` to show.

```bash
pnpm exec tsx --no-cache index.ts
```

Observe that `tsx` is much slower than `ts-node`.
