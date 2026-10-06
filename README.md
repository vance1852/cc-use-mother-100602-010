# 农产品质量抽检与召回闭环

这是面向数字农业运营场景的 Python 后端基础服务，提供可追溯的业务状态、权限边界和 SQLite 持久化能力。

## 测试

```bash
PYTHONPATH=src python3 -m unittest discover -s tests -v
```

## 构建检查

```bash
python3 -m compileall -q src tests
```

## 离线验收

```bash
PYTHONPATH=src python3 -m science_strategy_foundation.acceptance
```

## HTTP 服务

```bash
PYTHONPATH=src python3 -m science_strategy_foundation.api --database agriculture.sqlite3 --host 127.0.0.1 --port 8080
```
