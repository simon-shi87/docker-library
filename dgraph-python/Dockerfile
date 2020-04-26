FROM dgraph/dgraph:v20.03.1 as dgraph
FROM python:3.7.3-slim-stretch
COPY --from=dgraph /usr/local/bin/dgraph /usr/local/bin/dgraph
