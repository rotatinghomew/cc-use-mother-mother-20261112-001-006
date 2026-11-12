测试：python3 -m unittest discover -s tests/reorder_sagas -p 'test_*.py'
构建：python3 -m compileall -q b2b_reorder_network tests/reorder_sagas
验收：python3 -m b2b_reorder_network.dispatch.cli fixtures/demo.json --database /tmp/b2b_reorder_network-acceptance.sqlite3
所有输入均为本地合成数据，运行不需要网络。
