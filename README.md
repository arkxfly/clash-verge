<h1 align="center">
  <img src="./src/assets/image/logo.png" alt="Clash" width="128" />
  <br>
  Clash Verge
  <br>
</h1>

<h3 align="center">
A <a href="https://github.com/Dreamacro/clash">Clash</a> GUI based on <a href="https://github.com/tauri-apps/tauri">tauri</a>.
</h3>

## Features

- Full `clash` config supported, Partial `clash premium` config supported.
- Profiles management and enhancement (by yaml and Javascript). [Doc](https://github.com/Antiwall/clash-verge/wiki/%E4%BD%BF%E7%94%A8%E6%8C%87%E5%8D%97)
- Simple UI and supports custom theme color.
- Built-in support [Clash.Meta](https://github.com/MetaCubeX/Clash.Meta) core.
- System proxy setting and guard.

## Install

Download from [release](https://github.com/Antiwall/clash-verge/releases). Supports Windows x64, Linux x86_64 and macOS 11+

- [Windows x64](https://github.com/Antiwall/clash-verge/releases/download/v1.3.8/Clash.Verge_1.3.8_x64_en-US.msi)
- [macOS intel](https://github.com/Antiwall/clash-verge/releases/download/v1.3.8/Clash.Verge_1.3.8_x64.dmg)
- [macOS arm](https://github.com/Antiwall/clash-verge/releases/download/v1.3.8/Clash.Verge_1.3.8_aarch64.dmg)
- [Linux AppImage](https://github.com/Antiwall/clash-verge/releases/download/v1.3.8/clash-verge_1.3.8_amd64.AppImage)
- [Linux deb](https://github.com/Antiwall/clash-verge/releases/download/v1.3.8/clash-verge_1.3.8_amd64.deb)
- [Fedora Linux](https://github.com/Antiwall/clash-verge/issues/352)

Or you can build it yourself. Supports Windows, Linux and macOS 10.15+

Notes: If you could not start the app on Windows, please check that you have [Webview2](https://developer.microsoft.com/en-us/microsoft-edge/webview2/#download-section) installed.

### FAQ

#### 1. **macOS** "Clash Verge" is damaged and can't be opened

open the terminal and run `sudo xattr -r -d com.apple.quarantine /Applications/Clash\ Verge.app`

## Development

You should install Rust and Nodejs, see [here](https://tauri.app/v1/guides/getting-started/prerequisites) for more details. Then install Nodejs packages.

```shell
pnpm install
```

Then download the clash binary... Or you can download it from [clash premium release](https://github.com/Dreamacro/clash/releases/tag/premium) and rename it according to [tauri config](https://tauri.studio/docs/api/config/#tauri.bundle.externalBin).

```shell
# force update to latest version
# npm run check --force

npm run check
```

Then run

```shell
npm dev

# run it in another way if app instance exists
npm dev:diff
```

Or you can build it

```shell
npm build
```

## Todos

> This keng is a little big...

## Screenshots

<div align="center">
  <img src="./docs/demo1.png" alt="demo1" width="32%" />
  <img src="./docs/demo2.png" alt="demo2" width="32%" />
  <img src="./docs/demo3.png" alt="demo3" width="32%" />
  <img src="./docs/demo4.png" alt="demo4" width="32%" />
  <img src="./docs/demo5.png" alt="demo5" width="32%" />
  <img src="./docs/demo6.png" alt="demo6" width="32%" />
</div>

### Custom Theme

<div align="center">
  <img src="./docs/color1.png" alt="demo1" width="16%" />
  <img src="./docs/color2.png" alt="demo2" width="16%" />
  <img src="./docs/color3.png" alt="demo3" width="16%" />
  <img src="./docs/color4.png" alt="demo4" width="16%" />
  <img src="./docs/color5.png" alt="demo5" width="16%" />
  <img src="./docs/color6.png" alt="demo6" width="16%" />
</div>

## Disclaimer

This is a learning project for Rust practice.

## Contributions

Issue and PR welcome!

## Acknowledgement

Clash Verge was based on or inspired by these projects and so on:

- [tauri-apps/tauri](https://github.com/tauri-apps/tauri): Build smaller, faster, and more secure desktop applications with a web frontend.
- [Dreamacro/clash](https://github.com/Dreamacro/clash): A rule-based tunnel in Go.
- [MetaCubeX/Clash.Meta](https://github.com/MetaCubeX/Clash.Meta): A rule-based tunnel in Go.
- [Fndroid/clash_for_windows_pkg](https://github.com/Fndroid/clash_for_windows_pkg): A Windows/macOS GUI based on Clash.
- [vitejs/vite](https://github.com/vitejs/vite): Next generation frontend tooling. It's fast!

## License

GPL-3.0 License. See [License here](./LICENSE) for details.
