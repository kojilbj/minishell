# minishell

minishellは、C言語で実装されたシンプルなBashシェルの再実装です。プロンプトの構文解析、リダイレクト、シグナルハンドリングなど、基本的なコマンドラインインターフェースを提供します。

## 概要
minishellは、Bashを再実装し、プロンプトの構文解析、リダイレクト、パイプ、シグナルハンドリングなどの基本的なシェル機能に対応しています。
※`&`や`;`などには対応していません。

## インストール
1. リポジトリをクローン：
    ```bash
    git clone git@github.com:kojilbj/minishell.git
    ```
2. `readline`ライブラリをインストール：
    ```bash
    # Debian系システムの場合
    sudo apt-get install libreadline-dev

    # macOSの場合（Homebrewを使用）
    brew install readline
    ```
3. ビルド：
    ```bash
    cd minishell
    make
    ```

## 使用方法
```bash
./minishell
