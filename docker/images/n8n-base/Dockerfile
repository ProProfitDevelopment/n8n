# Используем готовый образ n8n с Node и зависимостями
FROM n8nio/n8n:latest

# Устанавливаем нужные OS-пакеты (без фиксированных версий)
RUN echo "http://dl-cdn.alpinelinux.org/alpine/edge/main" >> /etc/apk/repositories && \
    apk update && \
    apk upgrade && \
    apk add --no-cache \
        git \
        openssh \
        openssl \
        graphicsmagick \
        tini \
        tzdata \
        ca-certificates \
        libc6-compat \
        jq
