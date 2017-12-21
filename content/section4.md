# Section 4 - そのほかの使用例

## コードブロックのシンタックスハイライト

```json
[
  {
    "title": "apples",
    "count": [12000, 20000],
    "description": {"text": "...", "sensitive": false}
  },
  {
    "title": "oranges",
    "count": [17500, null],
    "description": {"text": "...", "sensitive": false}
  }
]
```

## PlantUML による作図

```uml
@startuml
アリス -> ボブ: Authentication Request
ボブ --> アリス: Authentication Response

アリス -> ボブ: Another authentication Request
アリス <-- ボブ: another authentication Response
@enduml
```

## 追加

本システムの内容の詳細は、以下の通りである。
