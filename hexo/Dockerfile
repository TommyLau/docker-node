FROM node:slim

MAINTAINER Tommy Lau <tommy@gen-new.com>

# Install Git, needed to publish to GitHub
RUN apt-get update && apt-get install -y git --no-install-recommends && rm -r /var/lib/apt/lists/*

# Install Hexo
RUN npm install hexo@2.8.3 -g

# Prepare work directory
RUN mkdir /hexo
WORKDIR /hexo

EXPOSE 4000

CMD ["hexo", "server", "-i", "0.0.0.0"]
