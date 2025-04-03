FROM openjdk:17-alpine

WORKDIR /app

COPY ./* /app/

ENV PORT=80
ENV JAVA_OPTS="-Xms512m -Xmx1G"

CMD ["sh", "-c", "./bin/application_name -Dconfig.file=./conf/application.conf -Dhttp.port=$PORT -Dfile.encoding=UTF8 > application.log 2>&1"]