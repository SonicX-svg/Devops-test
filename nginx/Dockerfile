FROM nginx:1.26-alpine

# Устанавливаем curl для healthcheck (один пакет, без лишнего мусора)
RUN apk add --no-cache curl

# Копируем конфиг nginx
COPY nginx.conf /etc/nginx/conf.d/default.conf

# Проверяем, что ничего лишнего не установлено
RUN nginx -t

# Запускаем nginx
CMD ["nginx", "-g", "daemon off;"]
