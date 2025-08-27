# 第1回ケモインフォマティクス×ハッカソン合宿 in 横浜 🧪💻

## 🎯 プロジェクト概要

このリポジトリは、[第1回ケモインフォマティクス×ハッカソン合宿 in 横浜](https://zenn.dev/poclab_techblog/articles/32394ed5a4fd68?redirected=1)での **毒性の二値分類** 課題に挑戦したプロジェクトです。

前日にテーマが公開され、初日の午後に集まって合宿を開始し、2日目のお昼までにモデルと資料を完成させる短期集中型のハッカソンになります。

## 📊 課題の内容

- **タスク**: 化学化合物の毒性二値分類（毒性あり/なし）
- **データ**: 分子構造データ（SMILES記法）
- **目標**: 高精度な毒性予測モデルの構築
- **期間**: 1.5日間での短期集中開発

## 🏗️ プロジェクト構造

```text
chemoinformatics-hackathon-2025/
├── data/                            # データセット
│   ├── train.csv                    # 訓練データ
│   ├── test_public.csv              # 公開テストデータ
│   └── test_private.csv             # プライベートテストデータ
├── note/                            # 実験ノート・資料
│   ├── test_notebook.ipynb          # Jupyter実験ノート
│   └── ハッカソンのチュートリアル.pdf   # ハッカソン説明資料
├── requirements.txt                 # 必要なライブラリ
└── LICENSE                          # ライセンス
```

## 🔬 ケモインフォマティクス手法

### 分子記述子・特徴量エンジニアリング

- **ECFP (Extended Connectivity Fingerprints)**: 分子の局所構造特徴
- **分子記述子**: RDKitを用いた物理化学的特性の計算
- **構造アラート**: 既知の毒性パターンに基づく化学専門知識の活用
など色々なものがあるが、選択して良いものを探す。

### 機械学習アプローチ

- ランダムフォレスト、XGBoost等のアンサンブル手法
- ハイパーパラメータ最適化
- クロスバリデーションによる性能評価
などの一連の流れで汎化性が高いモデルの作成に挑戦する。

## ⏰ ハッカソンスケジュール

### 開催形式

- **前日**: テーマの公開・事前準備・チーム編成
- **1日目午後**: 集合・チームで課題開始
- **1日目夕方**: 合宿形式での開発継続
- **2日目午前**: 開発・モデル調整
- **2日目昼**: 最終発表・資料提出

### 成果物

- 毒性予測モデル
- 手法説明資料
- 実験結果・分析レポート

## 🚀 使い方

### 環境構築

```bash
# リポジトリのクローン
git clone https://github.com/gotoh-poclab/chemoinformatics-hackathon-2025.git
cd chemoinformatics-hackathon-2025

# 依存パッケージのインストール
pip install -r requirements.txt
```

もしくは、note/test_notebook.ipynb はgoogle colabolatoryでも実行することができます。

### データの確認

```bash
# データセットの確認
ls data/
# train.csv, test_public.csv, test_private.csv

# Jupyter Notebookでの実験
jupyter notebook note/test_notebook.ipynb
```

## 📚 使用技術・ライブラリ

- **Python 3.x**
- **RDKit**: 化学情報学ライブラリ
- **scikit-learn**: 機械学習
- **XGBoost**: 勾配ブースティング
- **Pandas/NumPy**: データ処理
- **Matplotlib/Seaborn**: 可視化

## 🎉 イベント情報

### 第1回ケモインフォマティクス×ハッカソン合宿 in 横浜

**開催概要**:

- 📅 **開催時期**: 2025年8月（2日間の短期集中合宿）
- 📍 **会場**: 横浜
- 🎯 **テーマ**: ケモインフォマティクス×機械学習による毒性予測
- 💡 **目的**: 化学とデータサイエンスの融合・実践的な課題解決
- ⚡ **特徴**: 前日テーマ公開→1.5日での集中開発

**詳細情報**:

- [技術ブログ記事](https://zenn.dev/poclab_techblog/articles/32394ed5a4fd68?redirected=1)
- [参加者募集ページ](https://connpass.com/event/350848/)

## 👥 イベント参加について

このハッカソンは既に開催済みです。ケモインフォマティクスに興味がある方は、次年度のイベントにぜひご参加ください！

**このハッカソンの特徴**:

- 🔰 **初心者歓迎**: 基礎から学べる環境
- 🤝 **チーム開発**: 協力して課題解決
- 🏆 **実践経験**: リアルな化学データでの挑戦
- 🌟 **ネットワーキング**: 同じ興味を持つ仲間との出会い
- ⚡ **短期集中**: 1.5日での集中的な学習・開発

**関連リンク**:

- [参加者募集ページ（終了）](https://connpass.com/event/350848/)
- [技術ブログ記事](https://zenn.dev/poclab_techblog/articles/32394ed5a4fd68?redirected=1)

## 📄 ライセンス

このプロジェクトはMITライセンスの下で公開されています。詳細は[LICENSE](LICENSE)をご覧ください。

---

Let's explore the fascinating world of chemoinformatics together! 🧬✨
