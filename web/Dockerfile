
FROM nginx:1.14-alpine

COPY site.conf /etc/nginx/conf.d/site.template

ARG WORKDIR

ENV DOLLAR $
ENV WORKDIR=${WORKDIR}

CMD /bin/sh -c "envsubst < /etc/nginx/conf.d/site.template > /etc/nginx/conf.d/default.conf && nginx -g 'daemon off;'"
