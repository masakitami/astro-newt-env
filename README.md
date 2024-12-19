# Spline

<!-- ![screenshot](https://github.com/masakitami/astro-newt-env/blob/main/public/images/image.png) -->

## 🖋 概要
WEBの開発環境です。フロントエンドツールには「vite」を利用しているため、高速に静的サイトを開発することが可能です。
また、フレームワークは[Astro](https://astro.build/)を採用し、ホスティングサービスは[Vercel](https://vercel.com/)を使用しています。

- [テストサイトURL(Vercel)](https://astro-newt-env.vercel.app/)
- [デザインデータ](https://www.figma.com/design/9Q6cyRK2v4icOTtGtJGQa3/Spline_web?node-id=789-1544&t=5GviVwQrAo291kTO-1)


## 👨‍💻 準備
ローカル環境で利用するには以下のツールをマシンにインストールしておく必要があります。
- node.js >= 18.16.0
- git

## 📖 WEBアーキテクチャー
![screenshot](https://github.com/masakitami/astro-newt-env/blob/main/public/images/architecture.jpg)
WordPressではなくJAMstackを導入する。これにより、バックエンドシステムが不要となり、ユーザーフレンドリーでありながら、ページの読み込み速度が非常に速くなるという利点とセキュリティの堅牢さを担保できるため、ユーザーにとって快適な閲覧体験を提供することができます。CMSはHeadlessCMSの[NEWT](https://www.newt.so/)を採用しました。


## 💨 デプロイ方法
[Vercel](https://vercel.com/)とGithubをAPI連携させているためローカル環境からリモート環境にプッシュした時点で本番サイトにデプロイされます。


## 🚀 フォルダ構成

```
/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   └── Card.astro
│   ├── layouts/
│   │   └── Layout.astro
│   └── pages/
│       └── index.astro
└── package.json
```

Astroは、src/pages/ディレクトリ内の.astroまたは.mdファイルを探します。それぞれのページは、ファイル名に基づいてルートとして公開されます。

src/components/ディレクトリに特別な意味はありませんが、AstroやReact、Vue、Svelte、Preactのコンポーネントをここに配置することが一般的です。

画像などの静的アセットは、public/ディレクトリに配置できます。


## 🧞 Command

すべてのコマンドは、プロジェクトのルートディレクトリでターミナルから実行します:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |