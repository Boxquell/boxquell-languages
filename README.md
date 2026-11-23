# boxquell-languages

Official language recipes for [Boxquell](https://github.com/Boxquell/boxquell). Boxquell adds this repository by itself on first use.

```sh
boxquell recipes                      # everything that can be installed
boxquell add mybox node@22 python@3.13
boxquell repo update languages          # fetch the latest recipes
```

## Recipes

| Recipe | Versions (default first) |
|---|---|
| `node` | 24, 26, 22, 20 |
| `python` | 3.15, 3.14, 3.13, 3.12 (managed by uv) |
| `go` | 1.27, 1.26, 1.25 |
| `php` | 8.5, 8.4, 8.3, 8.2 (command line with common extensions) |
| `rust` | stable (rustup) |

Choose a version with `<recipe>@<version>`. Rust needs the C build tools from the [tools](https://github.com/Boxquell/boxquell-tools) repository.

## Contributing

One TOML file per recipe in `recipes/`. The format is described in [docs/recipes.md](https://github.com/Boxquell/boxquell/blob/main/docs/recipes.md); the workflow in this repository checks every file.

## License

Licensed under either of [Apache License 2.0](LICENSE-APACHE) or [MIT license](LICENSE-MIT) at your option.
