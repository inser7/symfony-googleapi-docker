# https://docs.docker.com/develop/develop-images/multistage-build/#stop-at-a-specific-build-stage
# https://docs.docker.com/compose/compose-file/#target


# https://docs.docker.com/engine/reference/builder/#understand-how-arg-and-from-interact
ARG NODE_VERSION=13


# "development" stage
FROM node:${NODE_VERSION}-alpine AS googleapis_client_development

WORKDIR /usr/src/client

# prevent the reinstallation of node modules at every changes in the source code
COPY package.json yarn.lock ./
RUN set -eux; \
	yarn install

COPY . ./

VOLUME /usr/src/client/node_modules

CMD ["yarn", "start"]