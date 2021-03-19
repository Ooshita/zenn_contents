# Python＆AIまわりの新しめのサービス

- [Poetry](https://github.com/python-poetry/poetry)
    - インストール方法

        以下を実行

        ```bash
        curl -sSL [https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py](https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py) | python
        ```

        $HOME/.poetry/binをPATHに追加

        source $HOME/.poetry/envを実行

        [Poetryのwebページ](https://python-poetry.org/)

    - poetryでpythonのプロジェクトを作成

    ```bash
    poetry new poetry-demo
    ```

    ファイルの階層構造の表示

    ```bash
    tree poetry-demo/
    #output
    poetry-demo/
    ├── README.rst
    ├── poetry_demo
    │   └── __init__.py
    ├── pyproject.toml
    └── tests
        ├── __init__.py
        └── test_poetry_demo.py
    ```

    以下の環境を定義するファイルが生成される。

    ```bash
    [tool.poetry]
    name = "poetry-demo"
    version = "0.1.0"
    description = ""
    authors = ["oshita-n <oshita-n@whispon.com>"]

    [tool.poetry.dependencies]
    python = "^3.7"

    [tool.poetry.dev-dependencies]
    pytest = "^5.2"

    [build-system]
    requires = ["poetry-core>=1.0.0"]
    build-backend = "poetry.core.masonry.api"
    ```

    - プロジェクトに定義された依存関係をインストール

    ```bash
    poetry install
    ```

    pip install の代わりにpoetry addを使う

    ```bash
    poetry add pendulum
    ```

    例えばtensorflowをインストールするときは

    ```bash
    poetry add tensorflow
    ```

    そうするとpyploject.tomlが書き換わる

    ```bash
    [tool.poetry]
    name = "poetry-demo"
    version = "0.1.0"
    description = ""
    authors = ["oshita-n <oshita-n@whispon.com>"]

    [tool.poetry.dependencies]
    python = "^3.7"
    pendulum = "^2.1.2"
    tensorflow = "^2.4.1"

    [tool.poetry.dev-dependencies]
    pytest = "^5.2"

    [build-system]
    requires = ["poetry-core>=1.0.0"]
    build-backend = "poetry.core.masonry.api"
    ```

- Pyflow
- MLflow