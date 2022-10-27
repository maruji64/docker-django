FROM nginx:1.23.2

# ローカルのdefault.confをコンテナにコピー
COPY ./default.conf /etc/nginx/conf.d/default.conf
COPY ./uwsgi_params /etc/nginx/uwsgi_params