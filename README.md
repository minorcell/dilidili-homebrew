# DILIDILI Homebrew Tap

[DILIDILI](https://github.com/minorcell/dilidili) 的 Homebrew Tap —— 哔哩哔哩视频下载器。

## 安装

这个 tap 的仓库名是 `dilidili-homebrew`，不是 Homebrew 默认的 `homebrew-*` 形式，因此需要显式指定仓库地址：

```bash
brew tap minorcell/dilidili-homebrew https://github.com/minorcell/dilidili-homebrew
```

```bash
brew install --cask dilidili
```

## 更新

```bash
brew upgrade --cask dilidili
```

## 签名说明

DILIDILI 尚未使用 Apple 开发者证书签名与公证。通过 Homebrew 安装的副本通常可以直接打开；如果 macOS 提示“无法验证开发者”，请执行：

```bash
xattr -dr com.apple.quarantine "/Applications/DILIDILI.app"
```

或前往“系统设置 → 隐私与安全性”选择“仍要打开”。

## 维护

Cask 文件位于 `Casks/dilidili.rb`，由 [dilidili](https://github.com/minorcell/dilidili) 的 Release 工作流自动更新版本号与 SHA256。
