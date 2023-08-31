FROM quay.io/piracarter1/ubi9:9.2

RUN adduser \
  --no-create-home \
  --system \
  --shell /usr/sbin/nologin \
  python-server && \
  mkdir /server && \
  chown -R 'python-server:python-server' /server

WORKDIR /server

USER python-server

CMD ["python3", "-m", "http.server"]
