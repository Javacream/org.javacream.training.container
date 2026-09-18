FROM alpine

ENV USER=alpine_user
ENV UID=12345
ENV GID=23456

RUN addgroup "$USER"
RUN adduser \
    --disabled-password \
    --gecos "" \
    --home "$(pwd)" \
    --ingroup "$USER" \
    --no-create-home \
    --uid "$UID" \
    "$USER"
USER "$USER"