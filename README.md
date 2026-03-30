# emojifyi

[![crates.io](https://img.shields.io/crates/v/emojifyi.svg)](https://crates.io/crates/emojifyi)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Emoji metadata, encoding, and Unicode Emoji 16.0 lookup — API client for [emojifyi.com](https://emojifyi.com).

> **Try the interactive tools at [emojifyi.com](https://emojifyi.com)**

## Install

`cargo add emojifyi`

## Quick Start

```rust
use emojifyi::Client;

#[tokio::main]
async fn main() -> Result<(), Box<dyn std::error::Error>> {
    let client = Client::new();
    let result = client.search("grinning-face").await?;
    println!("{} results", result.total);
    Ok(())
}
```

## Also Available

| Platform | Package | Link |
|----------|---------|------|
| **Python** | `pip install emojifyi` | [PyPI](https://pypi.org/project/emojifyi/) |
| **npm** | `npm install emojifyi` | [npm](https://www.npmjs.com/package/emojifyi) |
| **Go** | `go get github.com/fyipedia/emojifyi-go` | [pkg.go.dev](https://pkg.go.dev/github.com/fyipedia/emojifyi-go) |
| **Rust** | `cargo add emojifyi` | [crates.io](https://crates.io/crates/emojifyi) |
| **Ruby** | `gem install emojifyi` | [rubygems](https://rubygems.org/gems/emojifyi) |

## Embed Widget

Embed [EmojiFYI](https://emojifyi.com) widgets on any website with [emojifyi-embed](https://widget.emojifyi.com):

```html
<script src="https://cdn.jsdelivr.net/npm/emojifyi-embed@1/dist/embed.min.js"></script>
<div data-emojifyi="entity" data-slug="grinning-face"></div>
```

Zero dependencies · Shadow DOM · 4 themes (light/dark/sepia/auto) · [Widget docs](https://widget.emojifyi.com)

## Links

- [EmojiFYI](https://emojifyi.com) — Main site
- [API Documentation](https://emojifyi.com/developers/)
- [OpenAPI Spec](https://emojifyi.com/api/openapi.json)
- [Glossary](https://emojifyi.com/glossary/)

## License

MIT
