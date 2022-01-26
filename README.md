user テーブル
email (string型,NOT NUL,ユニーク制約)
encrypted_password(string型,NOT MULL)
name(string型,NOT NULL)
profile(text型,NOT NULL)
occupation(text型,NOT NULL)
position(text型,NOT NULL)


prototypesテーブル
title(string型,NOT NULL)
catch_copy(text型,NOT NULL)
concept(text型,NOT NULL)
user(references型,NOT NULL,外部キー)
※imageはActiveStorageで実装するため含まない


commentテーブル
content(text型、NOT NULL)
prototype(references型,NOT NULL,外部キー)
user(reference型,NOT NULl,外部キー)


