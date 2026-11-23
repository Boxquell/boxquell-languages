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
| `ruby` | 4.0, 3.4, 3.3 (built from source) |
| `java` | 25, 21, 17 (Eclipse Temurin JDK, with Maven and Gradle) |
| `kotlin` | 2.4, 2.3, 2.2 (installs `java`) |
| `lua` | 5.5, 5.4 (built from source) |
| `dotnet` | 10.0, 11.0 (.NET SDK) |
| `deno` | latest release |
| `bun` | latest release |
| `elixir` | 1.20, 1.19, 1.18 (with Erlang/OTP 28) |
| `zig` | 0.17, 0.16, 0.15 |
| `pnpm` | latest release (installs `node`) |
| `yarn` | latest stable, through Corepack (installs `node`) |
| `cmake` | latest release |
| `just` | latest release |

Choose a version with `<recipe>@<version>`. Rust, Ruby and Lua need the C build tools from the [tools](https://github.com/Boxquell/boxquell-tools) repository.

## Contributing

One TOML file per recipe in `recipes/`. The format is described in [docs/recipes.md](https://github.com/Boxquell/boxquell/blob/main/docs/recipes.md); the workflow in this repository checks every file.

A recipe may carry `icon = "<file>.svg"` right after its `description`; the file lives in `icons/` and is a single-colour SVG under 8 KB. Icons in `icons/` come from [Simple Icons](https://simpleicons.org) (CC0). The logos remain trademarks of their owners.

## License

Licensed under either of [Apache License 2.0](LICENSE-APACHE) or [MIT license](LICENSE-MIT) at your option.
