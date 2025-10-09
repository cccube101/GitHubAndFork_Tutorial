<img width="1280" height="186" alt="タイトル" src="https://github.com/user-attachments/assets/f213d3ca-3329-41c9-8efc-fc2889dcdf43" />  

# GitHubとForkを使用したデータ管理入門

## 目次
1. 概要  

2. ツールを使用する  
- 2-1.説明
- 2-2.ツールの用意
- 2-3.ツールの使用

---

## 1. 概要
この資料は**個人的解釈を多分に含みます！**  
間違いがあれば、ぜひ教えてください。  

> 「Gitに初めて触れる」「とりあえずツールを使ってみたい」  
> 「データ管理ってなに？」「どうやるの？」  

という方向けに、**“理屈よりも使う”** を目標として作成しています。  
GitやGitHub、Forkを使うと、ファイルの変更履歴を残したり、複数人で同じデータを扱ったりするのがとても簡単になります。  

---
## 2.ツールを使用する

### 2-1.説明  
  
簡単にそれぞれのツールの説明をします
<img width="1280" height="383" alt="スライド6" src="https://github.com/user-attachments/assets/652d54a9-e149-4c2f-84b9-6815c4a80ffc" />
直接Gitを操作するよりも簡単に操作できるのが主な利点となります。  
<br/>
### 2-2.ツールの用意
  
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
<br/>
<br/>
### 2-3.ツールの使用


---
## 3.解説


| 用語 | 意味 |
|------|------|
| **リポジトリ (Repository)** | プロジェクトの保存場所。フォルダのようなもの。 |
| **コミット (Commit)** | ファイルの変更を記録する行為。「この時点のスナップショット」。 |
| **プッシュ (Push)** | ローカルで記録した変更をGitHub（オンライン）に送る。 |
| **プル (Pull)** | GitHub上の変更を自分のPCに取り込む。 |
| **ブランチ (Branch)** | メインデータとは別の作業用コピー。安全に試すための枝分かれ。 |
| **マージ (Merge)** | ブランチで行った作業をメインに統合する。 |

icon by [icon8](https://icons8.jp/icons)
