# Git Lesson

## リモートリポジトリとローカルリポジトリとはそれぞれ何でしょうか？
- リポジトリは、ファイルやディレクトリの状態を記録する場所
- リモートリポジトリは、github等のオンラインに配置する
- リモートリポジトリは、複数人で共有することができる
- ローカルリポジトリは、開発者個人が使用する
- ローカルリポジトリは、自分のPC上に配置する


## プッシュとマージの違いは何でしょうか？
- プッシュは、ローカルリポジトリの内容をリモートリポジトリに反映する
- add→commit→プッシュの順で行う
- マージは既にプッシュされた履歴を、別のブランチに取り込む行為
- マージの方法には2種類存在する
- 1つ目は作業したブランチをプッシュした後、ローカルリポジトリにてマージしたいブランチにて取り込む方法
- 2つ目は作業したブランチをプッシュした後、リモートリポジトリにてマージする
- チームで作業を行う場合は、他の管理者がレビューを行ったり、コンフリクトを避ける必要がある
- チームで行う場合は、リモートにてリーターがマージを行うと致命的なミスを避けられる


## コミットとプッシュの違い
- コミットは、過去の編集状態に遡ることができる
- ゲームでいうセーブポイントのようなもの
- コミットすることで、簡単に過去の編集状態を取り戻すことができる
- コミットはローカルリポジトリにて行う
- プッシュは、コミットしたデータをローカルリポジトリに反映させる


## コミットのメッセージはどのように書いてあげるのが最適でしょうか？
- コードの中身を見返さなくてもいい明解な文章
- 誰が読んでもわかりやすい簡潔な文章
- どんな編集を行ったかわかる文章


## ローカルでマージするフローと、プルリクエストでマージするフローの違いは何でしょうか？
- リモートリポジトリを使用している場合、ローカルでマージすると、マージで反映させたブランチをプッシュする必要がある
- プルリクエストの場合、リモートリポジトリにてマージを行う
- プルリクエストは、他の人にも差分が確認できるためレビューの後、マージすることができる
- プルリクエストは、ミスを防ぎやすい
- プルリクエストは、チームでの開発向き
- プルリクエストを行った場合、ローカルリポジトリのブランチには変更が反映されていない
- ローカルリポジトリにも反映させるには、プルをする必要がある


## コンフリクトを起こしてしまった場合、どう対処すべきですか？
- 先にマージされた変更内容を取り込む
- 後にマージしようとしている変更内容を取り込む
- どちらの変更内容も取り込む
- コンフリクトが起こらないように、ソースコードを書いた人と相談する
- mergeを行う人を決めておく
