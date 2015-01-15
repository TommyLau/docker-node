FROM node

MAINTAINER Tommy Lau <tommy@gen-new.com>

# Install GitBook
RUN npm install hexo@2.8.3 -g

# Prepare work directory
RUN mkdir /hexo
WORKDIR /hexo

EXPOSE 4000

CMD ["hexo", "server"]
