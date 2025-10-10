<img width="1280" height="186" alt="タイトル" src="https://github.com/user-attachments/assets/f213d3ca-3329-41c9-8efc-fc2889dcdf43" />  

# 🌱 GitHubとForkを使用したデータ管理入門

## 📘 目次
1. 概要  
2. ツールを使用する  
3. Git解説  
4. まとめ  

---

## 1. 💡 概要
この資料は **「個人的解釈を多分に含んだ」** ものになります。  
間違いがあれば、ご教授いただければ幸いです。 

> 「Gitに初めて触れる」  
> 「とりあえずツールを使ってみたい」  
> 「データ管理ってなに？」「どうやるの？」  

そんな方に向けて、**“理屈よりもまず使う！”** をテーマにまとめています。  

Git・GitHub・Forkを使えば、  
✅ **ファイルの変更履歴を簡単に残せる！**  
✅ **複数人で同じデータを安全に扱える！**  

便利な管理手法を、実際に使用しながら学びましょう。  

---

## 2. 🧰 ツールを使用する

### 2-1. 🧩 説明  
Gitを直接操作するよりも、**GUIツール（Forkなど）を使うと操作が比較的簡単**です。  

<img width="1280" height="383" alt="スライド6" src="https://github.com/user-attachments/assets/652d54a9-e149-4c2f-84b9-6815c4a80ffc" />

---

### 2-2. ⚙️ ツールの準備  

#### 🧑‍💻 GitHubアカウントを作成  
まずは **GitHubのアカウント** を用意しましょう。  
- 個人で使う → 個人のメールアドレス  
- 組織で使う → 組織用メールアドレス  

> [!CAUTION]
> 💡 組織アカウントは一時的に使う場合も多く消えてしまうこともあるので、利用目的を考えて登録しましょう。

#### 📦 Forkをダウンロード  
次に [Fork公式サイト](https://git-fork.com/) から **GUIツールをダウンロード** します。  

ダウンロード後、GitHub上でリポジトリを作成！  
<img width="1280" height="597" alt="リポジトリ作成" src="https://github.com/user-attachments/assets/e5077c41-6d43-485d-8727-3119c008607f" />
<img width="1280" height="555" alt="ignoreとライセンスの解説" src="https://github.com/user-attachments/assets/76cd6fef-d809-4dc2-90e7-57adc46c910a" />


作成できたら、**「Code」→「HTTPS」→「URLをコピー」**。  
Forkを開き、「Clone」からPC上の任意フォルダへファイルを作成します。  

<img width="1405" height="479" alt="スクリーンショット 2025-10-10 040011" src="https://github.com/user-attachments/assets/5cb0572d-fd86-4cf8-b793-ec980eb5ed52" />

---

### 2-3. ✍️ 実際に使ってみる  

さあ、準備完了！  
まずは **テキストを追加** してみましょう。  
<img width="1196" height="406" alt="スクリーンショット 2025-10-10 120104" src="https://github.com/user-attachments/assets/1b13ccbc-d99f-4b45-9d76-88eec0abc17d" />

追加すると、Forkにもすぐ反映されます👇  


---

#### 💾 変更をGitHubへアップロードする  
次にGitHubへ変更を更新します。以下の順に操作しましょう。

1. 変更したファイルを選択し **Stage** をクリック  
2. **Subject（タイトル）** と **Description（説明）** を記入  
3. **Commit** ボタンを押す  

<img width="1919" height="1004" alt="スクリーンショット 2025-10-10 042508" src="https://github.com/user-attachments/assets/0a3582df-f855-4279-9797-b17797e51df7" />

次に、`main` の上で右クリック → **「Push and Create Pull Request」** を選択  
<img width="1853" height="1079" alt="スクリーンショット 2025-10-10 042607" src="https://github.com/user-attachments/assets/c438d487-95e8-41c1-ad6c-306964d5c60b" />

すると…  
💥 **GitHub上で反映されてる！やったぜ！**  

---

### 🌿 ブランチを作って作業してみよう  

1. 上部メニューの「Branch」を押す  
2. 名前を **`fix/Edit_Text`** にして「Create and CheckOut」  

<img width="1786" height="1039" alt="image" src="https://github.com/user-attachments/assets/f6dca358-3c66-4388-921d-b8eb0c92ed66" />

ブランチが `Edit_Text` になっているか確認したら、テキストを編集します。  

編集が終わると、Forkが次のように更新されます👇  
<img width="938" height="546" alt="スクリーンショット 2025-10-10 051139" src="https://github.com/user-attachments/assets/42cac8f9-00e1-4e53-95a7-6caf8f7800e6" />

先程やったように **Pull Request** までやって見ましょう。  
すると **ブラウザ上で勝手にGitHubが開く** はずです。  

次に、以下の**3つのステップ**で進めましょう👇  

1️⃣ **Create**  
2️⃣ **Merge**  
3️⃣ **Confirm**  

それぞれの段階で **緑のボタン** を押していけばOKです！
<img width="1280" height="720" alt="cmc" src="https://github.com/user-attachments/assets/cbd43171-882a-4245-92b5-a9b0b4c08587" />

これで **ブランチの変更がGitHubに反映** されました 🎉  

最後に、`main` に戻って **Fetch → Pull** でローカルを更新します。  
<img width="938" height="546" alt="スクリーンショット 2025-10-10 051329" src="https://github.com/user-attachments/assets/27afeb6c-cff5-4c0b-a98b-540ef8e799e2" />

✅ これで **ローカルも最新状態に！**  
<img width="944" height="668" alt="スクリーンショット 2025-10-10 044045" src="https://github.com/user-attachments/assets/b3fe01fc-25b1-4982-b488-6efc2bb1fc55" />

---

# 😫 いやわかんねぇよ！日本語で話せよ！！！

……そう思ったあなた、大丈夫です。  
**当時の僕も頭が沸騰してました。なんじゃこれ状態。**  

ここからは、今までやってきたことを**ざっくり解説**します！  

---

## 3. 🔍 Gitの解説（ざっくり版）

> ※あくまで個人的な理解に基づく解説です。

### 🗂️ リポジトリとは  
Git特有の「保存場所」。  
**リモート（GitHub上）** と **ローカル（自分のPC）** に分かれています。  
他人に影響を与えず作業するには「ブランチ」を使います。  

<img width="1280" height="591" alt="リポジトリ" src="https://github.com/user-attachments/assets/44ae0948-77be-4311-a765-3501a71bc7eb" />

### 🔄 データの流れ  
決定し通知
- **Commit（コミット）**：更新したい自分の作業内容を決定（変更履歴を記録）  
- **Pull Request（プルリクエスト）**：更新したい内容を管理者に通知  
- **Merge（マージ）**：承認された変更をメインのデータに統合する

<br/>

確認し更新
- **Fetch（フェッチ）**：GitHubの更新を確認  
- **Pull（プル）**：その更新を自分のPCへ反映  

<img width="1280" height="552" alt="データの流れ" src="https://github.com/user-attachments/assets/068ebe2d-8692-4694-a4cd-419182091134" />

### 💥コンフリクト
> [!CAUTION]
> ⚠️ 同じファイルを同時に編集すると「コンフリクト（衝突）」が起きます。  
> つまり、**“同時に同じ場所は書き換えられない”** と考えてよいです。

<img width="1280" height="553" alt="コンフリクト" src="https://github.com/user-attachments/assets/193349ce-020f-4510-b305-7f91d77f710f" />


---

### 3-2. 📖 用語まとめ

| 用語 | 意味 |
|------|------|
| **リポジトリ (Repository)** | プロジェクトの保存場所。フォルダのようなもの。 |
| **コミット (Commit)** | ファイルの変更を記録する。「この時点のスナップショット」。 |
| **プッシュ (Push)** | ローカルの変更をGitHubへ送信。 |
| **プル (Pull)** | GitHubの更新をローカルへ取得。 |
| **ブランチ (Branch)** | メインとは別の作業用コピー。安全に試す枝分かれ。 |
| **マージ (Merge)** | ブランチの変更をメインに統合。 |

---

## 4. 🧭 まとめ

お疲れさまでした！ 🎉  

実際に運用してみると、  
「思ってたより複雑…」「なんでエラー出るの？」  
など、さまざまな悩みが出てくると思います。  

今回紹介したのは **“バージョン管理” の第一歩**。  
より高度な運用やチームでの活用方法については、  
公式ドキュメントや他の資料もぜひ参考にしてみてください。  

> 🌱 一歩ずつ慣れていけば大丈夫。  
> あなたのデータ管理ライフが、もっと快適になりますように！

---

icon by [icon8](https://icons8.jp/icons)
