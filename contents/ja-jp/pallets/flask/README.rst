Flask
=====

Flaskは、軽量の`WSGI`_Webアプリケーションフレームワークです。複雑なアプリケーションに
スケールアップする機能を備えており、すばやく簡単に開始できるように設計されています。
これは、`Werkzeug`_と`Jinja`_の単純なラッパーとして始まり、最も人気のある
Python Webアプリケーションフレームワークの1つになりました。

Flaskは提案を提供しますが、依存関係やプロジェクトレイアウトを強制しません。
使用したいツールとライブラリを選択するのは開発者次第です。
新しい機能を簡単に追加できるようにする、コミュニティによって提供される多くの拡張機能があります。

.. _WSGI: https://wsgi.readthedocs.io/
.. _Werkzeug: https://werkzeug.palletsprojects.com/
.. _Jinja: https://jinja.palletsprojects.com/


インストール
----------

`pip`_を使用してインストールおよび更新します：

.. code-block:: text

    $ pip install -U Flask

.. _pip: https://pip.pypa.io/en/stable/quickstart/


簡単な例
----------------

.. code-block:: python

    # これをapp.pyとして保存します
    from flask import Flask

    app = Flask(__name__)

    @app.route("/")
    def hello():
        return "Hello, World!"

.. code-block:: text

    $ flask run
      * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)


コントリビュート
------------

開発環境のセットアップとFlaskへの貢献方法に関するガイダンスについては、
`コントリビュートガイドライン`_を参照してください。

.. _コントリビュートガイドライン： https://github.com/pallets/flask/blob/master/CONTRIBUTING.rst


寄付
------

Pallets組織は、Flaskとそれが使用するライブラリを開発およびサポートしています。
寄稿者とユーザーのコミュニティを成長させ、メンテナがプロジェクトにより
多くの時間を割けるようにするために、`今日寄付してください` 。

.. _今日寄付してください： https://palletsprojects.com/donate


リンク
-----

-   ドキュメント： https://flask.palletsprojects.com/
-   変更点： https://flask.palletsprojects.com/changes/
-   PyPI Releases: https://pypi.org/project/Flask/
-   ソースコード： https://github.com/pallets/flask/
-   課題追跡： https://github.com/pallets/flask/issues/
-   Webサイト： https://palletsprojects.com/p/flask/
-   Twitter: https://twitter.com/PalletsTeam
-   チャット： https://discord.gg/pallets

---
[オリジナル](https://github.com/pallets/flask/blob/main/README.rst)
