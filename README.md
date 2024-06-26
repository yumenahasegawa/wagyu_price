# Git Lesson

## リモートリポジトリとローカルリポジトリとはそれぞれ何でしょうか？

- リモートリポジトリとは、ネット上に配置して複数人で共有するためのリポジトリ。
- ローカルリポジトリとは、開発者一人ひとりが使用するために自分のPC上に配置するためのリポジトリ。


## プッシュとマージの違いは何でしょうか？

- ローカルの内容をリモートにアップしていく作業であるが、マージは別のブランチの作業内容をブランチに取り込むこと。


## コミットとプッシュの違い

- コミットはステージングしたファイルをローカルリポジストに保存することだが、プッシュはローカルリポジトリにコミットした内容をリモートにアップすること。


## コミットのメッセージはどのように書いてあげるのが最適でしょうか？

- どんな編集を行なったのかを示すメッセージにし、編集内容を正確に表すように書く。また、問題の機能の修正した場合にはfix, 新しく機能などを追加した場合はadd, ファイルを移動した場合にはmoveのようにコミットメッセージの先頭に接頭辞を使うことでコミットメッセージに含める情報を明確にすることができ、これだけでも一目見て、ある程度の変更内容を理解することができる。


## ローカルでマージするフローと、プルリクエストでマージするフローの違いは何でしょうか？


- 本番環境にアップされる前にコードレビューしてからマージすることで事前にバグを発見できるという違い。また、プルリクエストはローカルでadd, commitしたものをリモートにpushしコードレビューを仲介してマージするが、ローカルはadd, commit, mergeをローカルのブランチ同士でした後にリモートにpushするというフローの違いがある。

## コンフリクトを起こしてしまった場合、どう対処すべきですか？

- 先にマージされた変更内容を取り込む、後にマージしようとしている変更内容を取り込む、もしくはどちらの変更内容を取り込む、という3つの対処方法があり、これらはコードを書いた人と相談しながら作業に取り込むべきである。
