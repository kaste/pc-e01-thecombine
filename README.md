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
