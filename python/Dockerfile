FROM python:3.10.8

# PYTHONDONTWRITEBYTECODEとPYTHONUNBUFFEREDはオプション
# pycファイル(および__pycache__)の生成を行わないようにする
ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1

# コンテナのワークディレクトリを/codeに指定
WORKDIR /workspace

# ローカルのrequirements.txtをコンテナの/codeフォルダ直下に置く
COPY requirements.txt /workspace/

# コンテナ内でpipをアップグレードした後、pip install -r requirements.txtを実行
RUN pip install --upgrade pip && \
    pip install -r requirements.txt

# ソースコードをコンテナにコピー
COPY . /workspace/