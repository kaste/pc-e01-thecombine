the-combine combines the two Package Control channels (v3 and v4) into
one big channel, and uploads it as an release asset.  (With proper ETag/Last-Modified headers.)

You can point Package Control settings to that channel.

```
https://github.com/kaste/pc-e01-thecombine/releases/download/channel-latest/channel.json
```

```
    "channels": [
        // default channel for packages
        // Repo: https://github.com/packagecontrol/channel
        // default channel for packages
        // Repo: https://github.com/wbond/package_control_channel
        // Combined:
        "https://github.com/kaste/pc-e01-thecombine/releases/download/channel-latest/channel.json"
    ],
```

See public PR https://github.com/wbond/package_control/pull/1698


```bash
$ uv run scripts/generate_channel.py && sha256sum channel.json
fdb31ca8eafde0df47aeb059fbdb20095b03b0f1ba1ee74f8988eed34d6ac6d1 *channel.json
```
