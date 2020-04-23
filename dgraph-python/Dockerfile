FROM dgraph/dgraph:v1.2.2 as dgraph
FROM python:3.7.3-slim-stretch
COPY --from=dgraph /usr/local/bin/dgraph /usr/local/bin/dgraph
