# ‼ Common install issues

## MacOS

### Couldn't link to library libzstd.1.dylib

In order to fix this issue, you can (currently) execute the following `hacky` command:

```sh
brew install zstd
sudo ln -s /opt/homebrew/Cellar/zstd/1.5.5/lib/libzstd.1.5.5.dylib /usr/local/lib/libzstd.1.dylib
```

{% hint style="info" %}
Please replace `1.5.5` with the zstd version you have installed (although this one is required since it's the latest and the one used to build Snowball)
{% endhint %}
