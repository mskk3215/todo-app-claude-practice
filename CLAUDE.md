# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## プロジェクト概要

これは Next.js 15.3.5 で作成された Todo アプリの練習プロジェクトです。create-next-app でブートストラップされ、App Router、TypeScript、Tailwind CSS を使用しています。

## 開発コマンド

```bash
# 開発サーバーの起動（Turbopack使用）
npm run dev

# プロダクションビルド
npm run build

# プロダクションサーバーの起動
npm start

# ESLintによるリント
npm run lint
```

## 技術スタック

- **Framework**: Next.js 15.3.5 (App Router)
- **Language**: TypeScript 5
- **Styling**: Tailwind CSS 4 (PostCSS使用)
- **Linting**: ESLint 9 with Next.js config
- **Fonts**: Geist フォントファミリー (next/font/google経由)

## ディレクトリ構造

```
src/
  app/
    layout.tsx     # ルートレイアウト（Geistフォント設定）
    page.tsx       # ホームページコンポーネント
    globals.css    # グローバルスタイル（Tailwind含む）
    favicon.ico    # ファビコン
public/            # 静的アセット（SVGアイコン等）
```

## 重要な設定ファイル

- `next.config.ts`: Next.js設定
- `tsconfig.json`: TypeScript設定
- `eslint.config.mjs`: ESLint設定
- `postcss.config.mjs`: PostCSS設定（Tailwind用）

## フォント設定

プロジェクトではGeistフォントファミリーを使用：
- `--font-geist-sans`: メインフォント
- `--font-geist-mono`: モノスペースフォント

layout.tsx でCSS変数として設定され、Tailwindクラスで参照可能。