# 第6回 解答

## 演習

<!-- [tool call] の行は、表示された行をそのまま貼り付けてください。終わらなかった STEP は、空欄のままでかまいません。 -->

- STEP 1 のツールの名前：glossary_search_glossary
- STEP 2 の [tool call]：glossary_search_glossary({'query': '3レベル'})
- STEP 3 の [tool call]： fetch_fetch({'url': 'https://modelcontextprotocol.io/'})
- STEP 4 の [tool call]：aws_aws___search_documentation({'topics': ['general'], 'search_phrase': 'Amazon S3 Versioning overview what is it'})
- 気づき・疑問：そもそも、複数のツールの中からどのようにして使うツールを選んでいるのかが分かりませんでした。

## 宿題

<!-- 基礎・実装・発展のどれか1つに取り組めば完了です。 -->

- 取り組んだレベル：基礎 
- やったこと：サーバー側の app/mcp_server.py に server.tool()(tools.get_lecture_summary)の1行を追加した。
- 結果：エージェント側を変更していないにもかかわらず、正確に動作した。
- 気づき・疑問：サーバー側に1行足すだけで、エージェント側の設定を何も変えずに新しいツールが使えるようになるのが不思議で便利だと感じた。
