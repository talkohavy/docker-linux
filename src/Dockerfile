FROM node:22.16.0-alpine3.21

WORKDIR "/my-service"

# Step 1: Git configuration
RUN apk add --no-cache git openssh-client
RUN git config --global user.name "Tal Kohavy"
RUN git config --global user.email "tal.kohavy@controlup.com"

# Step 2: corepack
RUN corepack enable

CMD ["echo", "Hello, World!"]
