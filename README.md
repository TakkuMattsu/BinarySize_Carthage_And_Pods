# 概要

CarthageとPodsでバイナリのサイズが結構違うので調査する

[iOS - CarthageとCocoaPodsでバイナリのサイズが変わってる！？と思ったら変わってなかった](http://qiita.com/NorsteinBekkler/items/36b8f410b0c6c20e2b79)で利用したプロジェクトです

## 環境

- Xcode8.3.3
- Carthage0.23.0
- CocoaPods1.2.1
- Swift3.1
- Realm2.8.3

## ビルド結果

| Pods(デバッグ) | Carthage(デバッグ) |
|:----:|:--------:|
| 41.1MB | 81.3MB |

| Pods(ipa直接インストール) | Carthage(ipa直接インストール) |
|:----:|:--------:|
| 23.8MB | 23.9MB |


- Carthageは `carthage update` を実行
- Podsは `pod update` を実行

# 結論:アーカイブすればサイズは同じになる！
