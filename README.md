# Go-json
## 仕様
sample.logファイルに複数のJSONがある。このログをGoの構造体に変換してPostgreSQLにINSERTする。
- PostgreSQLはDockerコンテナで作ること
- forループしてINSERTすること
- トランザクションを実装すること
- usersテーブルのカラムはid(primary key), age(integer), name(varchar(500)), role(char(15))にすること
- ```go run main.go sample.log```のようにファイルを引数で渡せること
- 複数の引数を渡すとエラー終了すること
- table plusでdbの中身確認
