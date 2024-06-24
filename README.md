# Minishell

Minishellは、C言語で実装されたシンプルで軽量なBashシェルの再実装です。プロンプトの構文解析、リダイレクト、シグナルハンドリングなど、基本的なコマンドラインインターフェースを提供します。

## 概要
Minishellは、Bashを再実装し、プロンプトの構文解析、リダイレクト、シグナルハンドリングなどの基本的なシェル機能を提供します。多くの一般的なBash機能をサポートしていますが、`&`や`;`などの高度な機能はサポートしていません。

## インストール
Minishellをインストールするには、以下の手順に従ってください：

1. リポジトリをクローンします：
    ```bash
    git clone git@github.com:kojilbj/minishell.git
    ```
2. `readline`ライブラリをインストールします：
    ```bash
    # Debian系システムの場合
    sudo apt-get install libreadline-dev

    # macOSの場合（Homebrewを使用）
    brew install readline
    ```
3. プロジェクトをビルドします：
    ```bash
    cd minishell
    make
    ```

## 使用方法
プロジェクトをビルドした後、以下のコマンドでMinishellを起動できます：

```bash
./minishell
