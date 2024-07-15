## Docker
以下に、各Dockerコマンドが具体的に何を行い、どのような結果が得られるかを詳細に説明します。

### Docker イメージ関連コマンド

- **docker build**:
  - **用途**: Dockerfileをもとにイメージを作成します。
  - **実行例**:
    ```sh
    docker build -t myapp:latest .
    ```
  - **結果**: カレントディレクトリ（`.`）にあるDockerfileを基に、`myapp:latest`という名前のDockerイメージが作成されます。

- **docker pull**:
  - **用途**: Docker Hubや他のレジストリからイメージをダウンロードします。
  - **実行例**:
    ```sh
    docker pull ubuntu:latest
    ```
  - **結果**: Ubuntuの最新バージョンのDockerイメージがローカルにダウンロードされます。

- **docker images**:
  - **用途**: ローカルに存在するイメージの一覧を表示します。
  - **実行例**:
    ```sh
    docker images
    ```
  - **結果**: ローカルに保存されているすべてのDockerイメージの一覧が表示されます。

- **docker rmi**:
  - **用途**: 指定したイメージをローカルから削除します。
  - **実行例**:
    ```sh
    docker rmi myapp:latest
    ```
  - **結果**: `myapp:latest`という名前のDockerイメージがローカルから削除されます。

### Docker コンテナ関連コマンド

- **docker run**:
  - **用途**: 新しいコンテナを作成して実行します。
  - **実行例**:
    ```sh
    docker run -d --name mycontainer myapp:latest
    ```
  - **結果**: `myapp:latest`イメージから`mycontainer`という名前のコンテナが作成され、バックグラウンドで実行されます。

- **docker ps**:
  - **用途**: 実行中のコンテナの一覧を表示します。
  - **実行例**:
    ```sh
    docker ps
    ```
  - **結果**: 現在実行中のすべてのコンテナの一覧が表示されます。

- **docker ps -a**:
  - **用途**: 停止中のコンテナも含めた全てのコンテナの一覧を表示します。
  - **実行例**:
    ```sh
    docker ps -a
    ```
  - **結果**: 停止中のコンテナも含めたすべてのコンテナの一覧が表示されます。

- **docker stop**:
  - **用途**: 実行中のコンテナを停止します。
  - **実行例**:
    ```sh
    docker stop mycontainer
    ```
  - **結果**: `mycontainer`という名前の実行中のコンテナが停止されます。

- **docker start**:
  - **用途**: 停止中のコンテナを再起動します。
  - **実行例**:
    ```sh
    docker start mycontainer
    ```
  - **結果**: `mycontainer`という名前の停止中のコンテナが再起動されます。

- **docker restart**:
  - **用途**: コンテナを再起動します。
  - **実行例**:
    ```sh
    docker restart mycontainer
    ```
  - **結果**: `mycontainer`という名前のコンテナが再起動されます（停止して再度起動）。

- **docker rm**:
  - **用途**: コンテナを削除します。
  - **実行例**:
    ```sh
    docker rm mycontainer
    ```
  - **結果**: `mycontainer`という名前のコンテナがローカルから削除されます。

- **docker logs**:
  - **用途**: コンテナのログを表示します。
  - **実行例**:
    ```sh
    docker logs mycontainer
    ```
  - **結果**: `mycontainer`の標準出力と標準エラー出力のログが表示されます。

- **docker exec**:
  - **用途**: 実行中のコンテナ内でコマンドを実行します。
  - **実行例**:
    ```sh
    docker exec -it mycontainer /bin/bash
    ```
  - **結果**: `mycontainer`というコンテナ内でインタラクティブなシェル（`/bin/bash`）が起動されます。

### Docker ネットワーク関連コマンド

- **docker network ls**:
  - **用途**: Dockerネットワークの一覧を表示します。
  - **実行例**:
    ```sh
    docker network ls
    ```
  - **結果**: すべてのDockerネットワークの一覧が表示されます。

- **docker network create**:
  - **用途**: 新しいネットワークを作成します。
  - **実行例**:
    ```sh
    docker network create mynetwork
    ```
  - **結果**: `mynetwork`という名前の新しいDockerネットワークが作成されます。

- **docker network connect**:
  - **用途**: コンテナをネットワークに接続します。
  - **実行例**:
    ```sh
    docker network connect mynetwork mycontainer
    ```
  - **結果**: `mycontainer`というコンテナが`mynetwork`ネットワークに接続されます。

- **docker network disconnect**:
  - **用途**: コンテナをネットワークから切断します。
  - **実行例**:
    ```sh
    docker network disconnect mynetwork mycontainer
    ```
  - **結果**: `mycontainer`というコンテナが`mynetwork`ネットワークから切断されます。

- **docker network rm**:
  - **用途**: ネットワークを削除します。
  - **実行例**:
    ```sh
    docker network rm mynetwork
    ```
  - **結果**: `mynetwork`というDockerネットワークが削除されます。

### Docker ボリューム関連コマンド

- **docker volume ls**:
  - **用途**: Dockerボリュームの一覧を表示します。
  - **実行例**:
    ```sh
    docker volume ls
    ```
  - **結果**: すべてのDockerボリュームの一覧が表示されます。

- **docker volume create**:
  - **用途**: 新しいボリュームを作成します。
  - **実行例**:
    ```sh
    docker volume create myvolume
    ```
  - **結果**: `myvolume`という名前の新しいDockerボリュームが作成されます。

- **docker volume rm**:
  - **用途**: ボリュームを削除します。
  - **実行例**:
    ```sh
    docker volume rm myvolume
    ```
  - **結果**: `myvolume`というDockerボリュームが削除されます。

- **docker volume inspect**:
  - **用途**: ボリュームの詳細情報を表示します。
  - **実行例**:
    ```sh
    docker volume inspect myvolume
    ```
  - **結果**: `myvolume`というDockerボリュームの詳細情報が表示されます。

以上が各Dockerコマンドの具体的な動作と結果です。これらのコマンドを理解し、適切に使用することで、Dockerの操作が効率的に行えるようになります。