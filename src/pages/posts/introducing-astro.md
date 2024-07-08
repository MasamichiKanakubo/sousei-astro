---
title: "技術的なこだわりポイント"
description: "We're excited to announce Astro as a new way to build static websites and deliver lightning-fast performance without sacrificing a modern developer experience."
pubDate: "2024-07-09"
hero: "https://media.dev.to/cdn-cgi/image/width=1000,height=420,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fy7zkrf0t6j58k7gfgd84.jpeg"
tags: ["astro"]
layout: "../../layouts/BlogPostLayout.astro"
---

## こだわりポイント

- [**Astro**](https://astro.build/)という JavaScript のフレームワークを使用して、 Static Site Generator (SSG)を構築し高速なパフォーマンスを提供している
- **Astro**を MDX コンポーネントと組み合わせて、Markdown で開発ができるように開発体験向上の工夫をした
- ヒューマンインターフェースの講義で学んだ認知工学の知識を Tailwind や Sass などの CSS フレームワークを用いて表現している

## パフォーマンス

npm のパッケージをできるだけ CloudFlare の CDN を使うことによってビルドを軽量化させて、高速なパフォーマンスを提供している

## デプロイ

Github と Vercel が連携しているため、main ブランチに push するだけで自動的にデプロイ(CD)されるように設定している

## アーキテクチャ

<img src="/images/astro-architecture.png" alt="アーキテクチャ" >

## 使用技術

- **Astro**: JavaScript フレームワーク
- **TpyeScript**: プログラミング言語
- **JavaScript**: プログラミング言語
- **React JSX**: Reactコンポーネント (XML)
- **MDX**: Markdown と React を組み合わせたフォーマット
- **TailwindCSS**: CSS フレームワーク
- **Sass**: CSSプロセッサ
- **CloudFlare**: CDNキャッシュサーバー
- **Vercel**: サーバーレス環境
