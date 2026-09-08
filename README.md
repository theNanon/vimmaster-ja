# VIM Master 非公式日本語版

Vimができるようになりたい！と思って触り始めたら、気づけば日本語化してGitHub Pagesで公開するところまで来ていました。

こちらは [VIM Master](https://github.com/renzorlive/vimmaster) v3.0.0 をベースにした、**非公式の日本語ローカライズ版**です。

**遊ぶ:** https://thenanon.github.io/vimmaster-ja/

## 何を日本語化したの？

- メインUI
- 通常レッスンの説明
- チートモード
- 練習モード / スピードチャレンジ
- プロフィール・実績画面
- 実績カードや共有まわり

Vimのコマンド名やモード名、動作判定に使われる一部の課題テキストは、ゲームの動作を壊さないように英語のまま残しています。

## なぜ作ったの？

VIM Masterを触ってみて「これ日本語で遊べたらもっと入りやすそう」と思ったのがきっかけです。

最初は画面の数か所だけ直すつもりだったのですが
レッスン、練習モード、プロフィール……と触っているうちに、だんだん止まらなくなりました。

まだ改善できるところはあると思いますが、ひとまず日本語で一通り遊べるところまで来たので公開しています。

## オリジナルプロジェクト

VIM Master  
https://github.com/renzorlive/vimmaster

このリポジトリは元プロジェクトの公式配布物ではありません。  
元プロジェクトの著作権表示およびライセンス表記を保持しています。

MIT License

---

# VIM Master

Learn Vim by playing.

[![Tests](https://github.com/renzorlive/vimmaster/actions/workflows/test.yml/badge.svg)](https://github.com/renzorlive/vimmaster/actions)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-v3.0.0-blue.svg)](https://github.com/renzorlive/vimmaster/releases/tag/v3.0.0)

<p align="center">
  <img src="images/vm.gif" alt="VIM Master Screenshot" width="100%">
</p>

## Features

- 🎮 Learn Vim through interactive lessons
- 🏆 XP & Combo progression
- 📚 JSON-driven lesson system
- ✅ Contract, Golden & Regression tests
- 🌍 Community-ready architecture
- 💾 Offline support

## Quick Start

```bash
git clone https://github.com/renzorlive/vimmaster.git
cd vimmaster
npm install
npm run check
npm start
```

## Project Structure

```
content/     # JSON lessons and schema definitions
docs/        # Community guides, architecture, and principles
js/          # Game engine, progress system, and UI components
tests/       # Contract, Golden, and Regression test suites
```

## Development

```bash
npm run check          # Run all test suites
npm run test           # Run unit tests
npm run build:content  # Compile JSON lessons into generated-content.js
```

## Architecture

- **Content Provider:** Single source of truth for the game engine, feeding dynamically compiled JSON content.
- **Contract Suite:** Validates lesson schemas and schema rules to prevent bad data.
- **Golden Suite:** E2E validation ensuring the engine respects lesson solutions without breaking.
- **Regression Suite:** Protects against previously resolved bugs re-emerging.

## Contributing

Want to add a new lesson or Vim command? You don't need to touch the engine code!  
Read our guide: [Contributing a Lesson](docs/community/contributing-a-lesson.md)

## Roadmap

- ✅ V2 Architecture Freeze
- ✅ Community Alpha
- 🚧 V3 UX Polish
- 🔜 Public Beta

## License

MIT License
