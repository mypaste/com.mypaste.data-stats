# 数据统计

MyPaste extension `com.mypaste.data-stats` (version `1.0.4`).

按内容类型、来源与时间统计当前数据；页面只读取宿主聚合后的计数，不读取条目正文。

This repository is an independent copy extracted from the former `mypaste-code-extensions` monorepo at commit `825232c29681e0acf4b3a3100996281bec6b667e`. It contains only this extension's tracked source files. The published `.mypaste-plugin` archives and marketplace index live in [`mypaste-extensions-catalog`](https://github.com/mypaste/mypaste-extensions-catalog).

The manifest speaks MyPaste plugin protocol v3. Installation, capability mediation, and content-digest verification are performed by the MyPaste desktop host.

## Files

- `mypaste.plugin.json`: package identity, the `stats.read` capability, and the
  settings-window menu entry (`menus[0]`).
- `panel.html`: the menu page. It is a surface document with no runtime
  process; every number it shows comes from the host's `stats.read` aggregate,
  which only carries counts and form/source labels — never entry text, titles,
  or paths.

## License

MIT. See [LICENSE](LICENSE).
