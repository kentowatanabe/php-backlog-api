# Backlog API

## 概要

- BacklogにAPIを使用して課題を追加
- 添付ファイルの送信のサンプル

## 説明

Bakclogで課題にファイルを添付する場合、先に添付するファイルを送信し、添付ファイルに発行されたIDを取得する。
その後、レスポンスで受け取ったIDを課題と紐付けることで、課題にファイルを添付することができる。
送信されたファイルは添付された後に削除される。添付されなかった場合は1時間後に削除される仕様。	

## 使用法

- アカウント
    - スペースID（$spaceId）
    - API KEY（$apiKey）
- 課題
    - プロジェクトID（$params['projectId']）
    - 種別ID（$params['issueTypeId']）

上記を適宜変更。