FROM node:22-bullseye

ENV TZ Asia/Tokyo

# install Lib
RUN apt-get update -qq && \
    apt-get clean && \
    curl -o- -L https://yarnpkg.com/install.sh | sh && \
    yarn global add create-next-app

# set PATH
ENV PATH $HOME/.yarn/bin:$HOME/.config/yarn/global/node_modules/.bin:$PATH

WORKDIR /app

CMD ["/bin/bash"]
