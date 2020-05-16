# ts-38279-repro

## To Reproduce

```bash
npm ci
npm run build
```

Errors:

```shell
ERROR in ts-38279-repro/src/components/HelloWorld.vue(40,16):
40:16 Function implicitly has return type 'any' because it does not have a return type annotation and is referenced directly or indirectly in one of its return expressions.
    38 |     messages: {
    39 |       type: Array,
  > 40 |       default: () => []
       |                ^
    41 |     }
    42 |   },
    43 | });
```

See [TS #38279](https://github.com/microsoft/TypeScript/issues/38279)
