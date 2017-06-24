# 概要

CarthageとPodsでバイナリのサイズが結構違うので調査する

## 環境

- Xcode8.3.3
- Carthage0.23.0
- CocoaPods1.2.1
- Swift3.1
- Realm2.8.3

## ビルド結果

| Pods | Carthage |
|:----:|:--------:|
| 41.1MB | 81.3MB |

- Carthageは `carthage update` を実行
- Podsは `pod update` を実行

