# LinkedIn Banner Assets

Professional LinkedIn banner designs in light and dark themes.

## Specifications

- **Dimensions**: 1584×396 px (exact LinkedIn recommended cover size)
- **Safe text area**: Text positioned within left 1180×300 px to avoid mobile avatar overlap/cropping
- **Color profile**: sRGB
- **Fonts**: System-safe font stack (no external dependencies)

## Files

- `banner-light.svg` - Light theme banner
- `banner-dark.svg` - Dark theme banner

## Content

**Line 1**: Halil Aybar — Full‑Stack Developer  
**Line 2**: JavaScript · React · Node · Express · MongoDB · JWT

## Generating PNGs

### Automated (GitHub Actions)

The workflow automatically generates PNG exports when:
1. **Manual trigger**: Go to Actions → "Export LinkedIn banners" → "Run workflow"
2. **Automatic**: Any push to `assets/linkedin-banners/**` files

To download the generated PNGs:
1. Go to the [Actions tab](../../actions)
2. Click on the latest "Export LinkedIn banners" workflow run
3. Download the `linkedin-banners` artifact — it contains both PNGs

### Manual export (local)

If you have Inkscape installed locally:

```bash
# Light theme
inkscape -w 1584 -h 396 -o banner-light.png banner-light.svg

# Dark theme  
inkscape -w 1584 -h 396 -o banner-dark.png banner-dark.svg
```

## Upload tips for LinkedIn

- **Format**: Use PNG (recommended), under 8 MB
- **Color profile**: sRGB, baseline (not progressive)
- **Transparency**: Avoid transparency for best compatibility
- **Text placement**: Keep important text on the left; avatars can cover the bottom-left on mobile

These banner designs include appropriate padding for safety and professional appearance.