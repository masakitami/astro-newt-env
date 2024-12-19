# SplineWEB構成

![screenshot](https://github.com/masakitami/astro-newt-env/blob/main/public/images/image.png)

## 🖋 概要
WEBの開発環境です。フロントエンドツールには「vite」を利用しているため、高速に静的サイトを開発することが可能です。
また、フレームワークは[Astro](https://astro.build/)を採用し、ホスティングサービスは[Vercel](https://vercel.com/)を使用しています。

- [vercelサーバーのURL](https://astro-newt-env.vercel.app/)
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


```
npm create astro@latest -- --template basics
```

[![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/withastro/astro/tree/latest/examples/basics)
[![Open with CodeSandbox](https://assets.codesandbox.io/github/button-edit-lime.svg)](https://codesandbox.io/p/sandbox/github/withastro/astro/tree/latest/examples/basics)
[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/withastro/astro?devcontainer_path=.devcontainer/basics/devcontainer.json)

> 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!

![just-the-basics](https://github.com/withastro/astro/assets/2244813/a0a5533c-a856-4198-8470-2d67b1d7c554)

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

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

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

Any static assets, like images, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).
# astro-orelop-cli
