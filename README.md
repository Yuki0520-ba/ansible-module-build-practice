# ansible mobule build test

Ansibleの自作モジュール開発を試みる。

## Setup 

初回セットアップ時のみ以下を実行

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirement.txt 
```

開発前に以下を実行

```bash
source .venv/bin/activate
source ansible/hacking/env-setup
```

## Note

- 自作したモジュールはlibraryディレクトリ下に配置
- 自作モジュールをテストするPlaybookはロールとして作成
- 作成したロールをexec-test-modules.ymlから実行