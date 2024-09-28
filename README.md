# portable storyを試す

初回のみ実行 (.storybook/preview.tsxがtailwindのビルドに依存しているため)

```shell
pnpm build -F @repo/tailwind
```

テスト用コマンド

```shell
pnpm test -F @repo/ui
```

decoratorやparameterがvitestのテストにも影響するので上書きしておく必要がある

-   https://storybook.js.org/docs/writing-tests/import-stories-in-tests/stories-in-unit-tests

公式のアプローチでは上書きできなかったので別のアプローチでやる
