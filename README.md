# Pelican To Hugo Migration Script

This script helps you move your Pelican content to Hugo. For more context, read [this blog post](//avi.im/blag/2020/moving-to-hugo/).

## Usage

Just pass the path to content directory. E.g.:

```bash
python3 script.py src/content
```

This will overwrite the existing files and makes them Hugo compatible.

## Caveats

This script makes some assumptions about existing Pelican files:

1. Each file starts with `Title:` and ends its metadata section with `Summary: <some content>`
2. Processes only these metadata fields:
	- Title
	- Slug
	- FacebookImage
	- Date
	- Modified
	- Category
	- Tags

## License

Released under MIT License. Check [License](LICENSE) file for more details.