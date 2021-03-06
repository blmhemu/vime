# @vime/core

Vime is a customizable, extensible, accessible and framework agnostic media player. The `@vime/core` 
package contains the web components for the player, plugins, providers and UI elements that makeup 
the building blocks of Vime.

## Example

```html
<vime-player autoplay muted>
  <vime-video poster="/media/poster.png" cross-origin>
    <source data-src="/media/video.mp4" type="video/mp4" />
    <track
      default
      kind="subtitles"
      src="/media/subs/en.vtt"
      srclang="en"
      label="English"
    />
    <track
      kind="subtitles"
      src="/media/subs/es.vtt"
      srclang="es"
      label="Spanish"
    />
  </vime-video>

  <vime-ui>
    <vime-click-to-play />
    <vime-captions />
    <vime-poster />
    <vime-spinner />
    <vime-default-settings />
    <vime-controls pin="bottomLeft" active-duration="2750" full-width>
      <vime-playback-control tooltip-direction="right" />
      <vime-volume-control />
      <vime-time-progress />
      <vime-control-spacer />
      <vime-caption-control />
      <vime-pip-control keys="p" />
      <vime-settings-control />
      <vime-fullscreen-control keys="f" tooltip-direction="left" />
    </vime-controls>
  </vime-ui>

  <vime-plugins>
    <vime-chromecast />
  </vime-plugins>
</vime-player>
```

## Related

- [GitHub](https://github.com/vime-js/vime)
- [Discord](https://discord.gg/feZ6cAE)
- [Documentation](https://vimejs.com)
