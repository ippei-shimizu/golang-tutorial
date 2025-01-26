# ベースイメージとしてGoを使用
FROM golang:1.23

# 作業ディレクトリを設定
WORKDIR /app

# 必要なファイルをコンテナにコピー
COPY . .

# 依存関係を取得
RUN go mod tidy

# アプリケーションをビルド
RUN go build -o app .

# コンテナ起動時にアプリを実行
CMD ["./app"]
