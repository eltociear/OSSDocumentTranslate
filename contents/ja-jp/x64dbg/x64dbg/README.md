# x64dbg

<img width="100" src="https://github.com/x64dbg/x64dbg/raw/development/src/bug_black.png"/>

[![BountySource](https://www.bountysource.com/badge/team?team_id=18188&style=raised)](https://www.bountysource.com/teams/x64dbg?utm_source=x64dbg&utm_medium=shield&utm_campaign=raised) [![Build status](https://ci.appveyor.com/api/projects/status/h1j489qa1mx67e0h?svg=true)](https://ci.appveyor.com/project/mrexodia/x64dbg) [![Open Source Helpers](https://www.codetriage.com/x64dbg/x64dbg/badges/users.svg)](https://www.codetriage.com/x64dbg/x64dbg) [![Crowdin](https://d322cqt584bo4o.cloudfront.net/x64dbg/localized.svg)](http://translate.x64dbg.com) [![Download x64dbg](https://img.shields.io/sourceforge/dm/x64dbg.svg)](https://sourceforge.net/projects/x64dbg/files/latest/download)

[![Telegram](https://img.shields.io/badge/chat-%20on%20Telegram-blue.svg)](https://telegram.me/x64dbg) [![Discord](https://img.shields.io/badge/chat-on%20Discord-green.svg)](https://invite.gg/x64dbg) [![Slack](https://img.shields.io/badge/chat-on%20Slack-red.svg)](https://x64dbg-slack.herokuapp.com) [![Gitter](https://img.shields.io/badge/chat-on%20Gitter-lightseagreen.svg)](https://gitter.im/x64dbg/x64dbg) [![Freenode](https://img.shields.io/badge/chat-%20on%20freenode-brightgreen.svg)](https://webchat.freenode.net/?channels=x64dbg) [![Matrix](https://img.shields.io/badge/chat-on%20Matrix-yellowgreen.svg)](https://riot.im/app/#/room/#x64dbg:matrix.org) [![XMPP](https://img.shields.io/badge/chat-%20on%20XMPP-orange.svg)](https://inverse.chat/#converse/room?jid=x64dbg@conference.jwchat.org)

Windows用のオープンソースのバイナリデバッガー。マルウェアの分析と、ソースコードがない実行可能ファイルのリバースエンジニアリングを目的としています。利用可能な多くの機能と、独自の機能を追加するための包括的な[プラグインシステム](http://plugins.x64dbg.com)があります。
詳細については、[ブログ](https://x64dbg.com/blog)をご覧ください！

## スクリーンショット

![メインインターフェイス](https://i.imgur.com/V2f5AP9.png)

![グラフ](https://i.imgur.com/gVjzntJ.png) ![メモリマップ](https://i.imgur.com/cLJwTjY.png)

## インストールと使用法

1. [GitHub](https://github.com/x64dbg/x64dbg/releases)、[SourceForge](https://sourceforge.net/projects/x64dbg/files/snapshots)または、[OSDN](https://osdn.net/projects/x64dbg)からスナップショットをダウンロードし、ユーザーが書き込みアクセスできる場所に解凍します。
2. _オプションで_`x96dbg.exe`を使用してシェル拡張を登録し、デスクトップにショートカットを追加します。
3. 32ビットの実行可能ファイルをデバッグする場合は`x32\x32dbg.exe`を実行し、64ビットの実行可能ファイルをデバッグする場合は`x64\x64dbg.exe`を実行できるようになりました。よくわからない場合は、いつでも`x96dbg.exe`を実行して、そこでアーキテクチャを選択できます。

いくつかの簡単な手順で自分で[コンパイル](https://github.com/x64dbg/x64dbg/wiki/Compiling-the-whole-project)x64dbgすることもできます！

## コントリビュート

これはコミュニティの取り組みであり、プルリクエストを受け付けています。詳細については、[コントリビュート](https://github.com/x64dbg/x64dbg/blob/development/CONTRIBUTING.md)ドキュメントを参照してください。ご不明な点がございましたら、いつでも[お問い合わせ](https://x64dbg.com/#contact)または[issue](https://github.com/x64dbg/x64dbg/issues)を開くことができます。[簡単なissue](https://github.com/x64dbg/x64dbg/issues?q=is%3Aissue+is%3Aopen+label%3Aeasy)を参照して開始できます。

## クレジット

- [TitanEngine Community Edition](https://github.com/x64dbg/TitanEngine)によるデバッガコア
- [Zydis](https://zydis.re)によって搭載された逆アセンブル
- [XEDParse](https://github.com/x64dbg/XEDParse)および[asmjit](https://github.com/asmjit)によって搭載されたアセンブル
- [Scylla](https://github.com/NtQuery/Scylla)によって搭載されたインポートの再構築
- [Jansson](http://www.digip.org/jansson)によって搭載されたJSON
- [lz4](https://bitbucket.org/mrexodia/lz4)によって搭載されたデータベース圧縮
- [VisualPharm](http://www.visualpharm.com)によるバグアイコン
- [Fugue](http://p.yusukekamiyamane.com)によるインターフェイスアイコン
- [tr4ceflow](http://tr4ceflow.com)によるWebサイト

## デベロッパー

- [mrexodia](http://mrexodia.github.io)
- Sigma
- [tr4ceflow](http://blog.tr4ceflow.com)
- [Dreg](http://www.fr33project.org)
- [Nukem](https://github.com/Nukem9)
- [Herz3h](https://github.com/Herz3h)
- [torusrxxx](https://github.com/torusrxxx)

## コードへのコントリビュート

GitHubコントリビューターの完全なリストは[ここ](https://github.com/x64dbg/x64dbg/graphs/contributors)にあります。

## スペシャルサンクス

- 初期のGUIを開発したSigma
- すべての[寄付者](https://www.bountysource.com/teams/x64dbg/backers)！
- issueを追加した皆様！
- このリストに追加するのを忘れてしまった人
- [ブログのライター](https://x64dbg.com/blog/2016/07/09/Looking-for-writers.html)！
- [EXEToolsコミュニティ](http://forum.exetools.com)
- [Tuts4Youコミュニティ](http://forum.tuts4you.com)
- [ReSharper](https://www.jetbrains.com/resharper)
- [Coverity](http://www.coverity.com)
- acidflash
- cyberbob
- cypher
- Teddy Rogers
- TEAM DVT
- DMichael
- Artic
- ahmadmansoor
- \_pusher\_
- firelegend
- [kao](http://lifeinhex.com)
- sstrato
- [kobalicek](https://github.com/kobalicek)
- [athre0z](https://github.com/athre0z)
- [ZehMatt](https://github.com/ZehMatt)

多くの人々や他のオープンソースプロジェクトの助けがなければ、今日のx64dbgはありませんでした。ありがとう！

---
[オリジナル](https://github.com/x64dbg/x64dbg/blob/development/README.md)
