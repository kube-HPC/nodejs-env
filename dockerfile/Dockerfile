
ARG DOCKER_REGISTRY=""
FROM ${DOCKER_REGISTRY}hkube/base-node:v1.1.1
LABEL maintainer="yehiyam@gmail.com"

ADD package.json package-lock.json /hkube/algorithm-runner/
WORKDIR /hkube/algorithm-runner
RUN npm ci
COPY . /hkube/algorithm-runner
CMD ["npm", "start"]