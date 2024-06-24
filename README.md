# minishell
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
~: ./minishell
#標準入力
minishell: cat
Hello World
Hello World
^C
#出力のリダイレクト
minishell: cat > test.txt
Hello World
#入力のリダイレクト
minishell: < test.txt cat
Hello World
#パイプ
minishell: cat test.txt | wc
       1       2      12
#パイプと出力のリダイレクト
minishell: cat test.txt | wc > wc.txt
minishell: cat wc.txt 
       1       2      12
```
