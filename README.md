<img width="1280" height="186" alt="タイトル" src="https://github.com/user-attachments/assets/f213d3ca-3329-41c9-8efc-fc2889dcdf43" />  

# 🌱GitHubとForkを使用したデータ管理入門

## 📘目次
1. 概要  

2. ツールを使用する  
- 2-1.説明
- 2-2.ツールの用意
- 2-3.ツールの使用

3. Git解説
- 3-1.解説
- 3-2.用語集

4. まとめ

---

## 1. 💡概要
この資料は**個人的解釈を多分に含みます！**  
間違いがあれば、ぜひ教えてください。  

> 「Gitに初めて触れる」「とりあえずツールを使ってみたい」  
> 「データ管理ってなに？」「どうやるの？」  

という方向けに、**“理屈よりも使う”** を目標として作成しています。  
GitやGitHub、Forkを使うと、ファイルの変更履歴を残したり、複数人で同じデータを扱ったりするのがとても簡単になります。  

---
## 2.ツールを使用する

### 2-1.🧩説明  
  
簡単にそれぞれのツールの説明をします
<img width="1280" height="383" alt="スライド6" src="https://github.com/user-attachments/assets/652d54a9-e149-4c2f-84b9-6815c4a80ffc" />

直接Gitを操作するよりも簡単に操作できるのが主な利点となります。  
<br/>
### 2-2.⚙️ツールの用意
まず、GitHubの使用にはアカウントが必要となります。  
個人で使う場合には個人のメールアドレスを、組織としてGitHub Copilot等を使用する場合は組織のメールを登録しましょう。  
組織のアカウントの利用は一時的なことが多いので加味して判断してください。  
<br/>
次に[Forkのサイト](https://git-fork.com/)でGUIツールをダウンロードをしましょう。  
<br/>
ダウンロードが終わったらGitHubでリポジトリを作成してみます。
<img width="1280" height="607" alt="リポジトリを作成" src="https://github.com/user-attachments/assets/5145d359-0513-43c5-aa77-e5139a2ff196" />
<img width="1280" height="545" alt="スライド12" src="https://github.com/user-attachments/assets/dd625280-dcd2-404b-a39c-3e702a866766" />

<br/>
<br/>
作成できたら、CodeのHTTPSにあるURLをコピーします。  
Forkを開きCloneからPC上の任意のフォルダにファイルを作成します。
<img width="1405" height="733" alt="スクリーンショット 2025-10-10 040011" src="https://github.com/user-attachments/assets/f353c387-82e9-48a8-a6a6-c501a076e50e" />

---

### 2-3.✍️ツールの使用
さぁようやく用意ができました。早速テキストを追加してみましょう！<br/>
テキストを追加したらForkにも更新されます。<br/>
<img width="802" height="527" alt="スクリーンショット 2025-10-10 041429" src="https://github.com/user-attachments/assets/1dbe21bb-f283-4989-a85c-77c2ca35c329" />
<br/>
<br/>
次に追加したテキストをPCからGitHubに更新してみましょう。  
テキストを選択した状態でStageを押す。
subjectとDescriptionを書く。
commitを押します。
<img width="1919" height="1004" alt="スクリーンショット 2025-10-10 042508" src="https://github.com/user-attachments/assets/0a3582df-f855-4279-9797-b17797e51df7" />

上記が完了したらmainの上で右クリックでメニューを開き、Push and Create Pull Requestを押します。
<img width="1853" height="1079" alt="スクリーンショット 2025-10-10 042607" src="https://github.com/user-attachments/assets/c438d487-95e8-41c1-ad6c-306964d5c60b" />

<br/>
<br/>
GitHubを確認してみると...**追加されてるぜ！**


---

次はブランチを作ってみましょう。  
上部のBranchを押す。  
 **「fix/Edit_Text」** と入力 Create and CheckOutを押します。
<img width="1786" height="1039" alt="image" src="https://github.com/user-attachments/assets/f6dca358-3c66-4388-921d-b8eb0c92ed66" />

Branchesの中で選択しているチェックマークがEdit_Textになっているか確認しましょう。  
確認できたらテキストを開いて中に記述してみましょう。  
テキストを更新し、Forkがこんな風に更新されます。
<img width="938" height="546" alt="スクリーンショット 2025-10-10 051139" src="https://github.com/user-attachments/assets/42cac8f9-00e1-4e53-95a7-6caf8f7800e6" />

先程GitHub側に更新したようにPull Requestまでやって見ましょう。
勝手にブラウザでGitHubが開きます。
<br/>
緑色のボタンを Create → Merge → Confirm の順に押していきます。
<img width="960" height="627" alt="スクリーンショット 2025-10-10 051210" src="https://github.com/user-attachments/assets/f13cdbdf-1df8-4b22-b4f5-82ce1b6d6b46" />
<img width="960" height="629" alt="スクリーンショット 2025-10-10 051228" src="https://github.com/user-attachments/assets/6d2ada07-7db5-403f-b310-ddee2f03f048" />
<img width="960" height="557" alt="スクリーンショット 2025-10-10 051240" src="https://github.com/user-attachments/assets/c0511ebd-1e7f-42e1-b007-04672c4d29f5" />

これでGitHubにブランチのデータを送ることができました！  
<br/>
この変更を自分のPCのmainに更新します。  
Branchesの中で選択しているチェックマークをmainに変更しましょう。  
上部のFetchを押して画面が変わったなーと確認したらPullを押します。  
<img width="938" height="546" alt="スクリーンショット 2025-10-10 051329" src="https://github.com/user-attachments/assets/27afeb6c-cff5-4c0b-a98b-540ef8e799e2" />

これでPCにデータを更新できました！！！
<br/>
<br/>
<br/>
<br/>
...............
<br/>
<br/>
<br/>
<br/>

# いやわかんねぇよ！日本語で話せよ！！！
当時の僕もやってて頭沸騰しそうでした。なんじゃこれです。
<br/>
次は今までやってきたことの解説を僕の解釈で簡単に説明します
<br/>
<br/>

---

## 3.Git解説
### 3-1.🔎解説  
何度も言っていますがあくまで僕の個人的解釈です。  
説明のために省略してる部分や微妙に違うニュアンスになっている部分があります。  
<br/>
まずリポジトリです。  
Git特有の保存場所です。  
主にリモートとローカルに分かれオリジナルとなるリポジトリを複製することをクローンと言います。  
他のリポジトリのデータに影響を与えず自分の作業をする際にはブランチを使用します。  
<img width="1280" height="602" alt="スライド7" src="https://github.com/user-attachments/assets/6afd0006-d26d-4a43-839c-9919c9c80521" />

ブランチのデータをリモートやそこからクローンしている人に受け渡す流れです。  
マージされた物はフェッチでどう更新されたか確認し、プルで自分のデータに反映させます。  
<img width="1280" height="597" alt="スライド8" src="https://github.com/user-attachments/assets/351e903e-baef-4f39-9c4b-98ef6b7b8fe6" />

マージする際には、コンフリクトにも注意しなければなりません。  
同じデータを同時に修正することはできないと思ってください。  
<img width="1280" height="598" alt="スライド9" src="https://github.com/user-attachments/assets/67e8c868-4083-4b74-9223-5710ed6498ed" />

<br/>
<br/>

---

### 3-2.🧾用語集

<br/>

| 用語 | 意味 |
|------|------|
| **リポジトリ (Repository)** | プロジェクトの保存場所。フォルダのようなもの。 |
| **コミット (Commit)** | ファイルの変更を記録する行為。「この時点のスナップショット」。 |
| **プッシュ (Push)** | ローカルで記録した変更をGitHub（オンライン）に送る。 |
| **プル (Pull)** | GitHub上の変更を自分のPCに取り込む。 |
| **ブランチ (Branch)** | メインデータとは別の作業用コピー。安全に試すための枝分かれ。 |
| **マージ (Merge)** | ブランチで行った作業をメインに統合する。 |

---

## 4.まとめ
お疲れさまでした。
実際に運用してみると、さまざまな課題や悩みが出てくると思います。  
<br/>
今回紹介した手法は「バージョン管理」と呼ばれるもので、これに関する詳しいドキュメントや解説は数多く公開されています。  
より高度な運用方法やチームでの活用については、そうした資料を参考にしてみてください。  
<br/>
今回はその第一歩として、初歩的な導入体験をしていただきました。  
それでは、良いデータ管理ライフを！ 🌱  
<br/>
<br/>
icon by [icon8](https://icons8.jp/icons)
