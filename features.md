# Meridian Compositor features

## 2026-11-03

- Added the Meridian-Precision theme for compositor-drawn titlebars. Close, minimize, maximize and restore use Meridian glyphs and green hover states, with controls on the left by default. Existing configurations can select the new theme explicitly. App-drawn buttons continue to follow their own toolkits.
- Added a configurable floating window corner radius, defaulting to 12 logical pixels. The clip covers the app content and its frame. Tiled, maximized, fullscreen and shaded windows bypass clipping, and popups retain their existing geometry. Clipped windows lose shadows outside their frame and the clip uses logical-pixel steps. Set `windowCornerRadius` to 0 to disable clipping. The build pins wlroots 0.20.1 and applies a scene patch.
