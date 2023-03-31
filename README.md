# asdf-skopeo

Plugin to manage [Skopeo](https://github.com/containers/skopeo), a command line utility that performs various operations on container images and image repositories.

For details on `asdf` plugin development, see the `asdf` documentation on how to [create a plugin](https://asdf-vm.com/plugins/create.html).

## How to install

### Build dependencies

To download and build `skopeo`, the plugin depends on `curl` and `golang` (1.12 or above). Please also ensure the `GOPATH` environment variable is defined.

The plugin follows the Skopeo instructions on [building from source](https://github.com/containers/skopeo/blob/main/install.md#building-from-source).

#### Ubuntu

If running Ubuntu (18.10 or above), install additional dependencies:

```shell
> sudo apt install libgpgme-dev libassuan-dev libbtrfs-dev libdevmapper-dev pkg-config
```

#### macOS

If running macOS, install additional dependencies:

```shell
> brew install gpgme
```

### Adding the plugin

Add `asdf-skopeo` plugin by pointing to this repository:

```shell
> asdf plugin add skopeo https://github.com/kheino/asdf-skopeo
```

### Installing the tool

Now install the `skopeo` tool provided by the plugin:

```shell
> asdf install skopeo latest
```
