# ARG VARIANT="18"
# FROM mcr.microsoft.com/vscode/devcontainers/typescript-node:0-${VARIANT}
FROM mcr.microsoft.com/devcontainers/typescript-node
RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip" \
  && unzip awscliv2.zip \
  && ./aws/install \
  && rm -rf ./aws awscliv2.zip \
  && npm install -g typescript \
  && npm install -g aws-cdk \
  && npm install -g npm-check-updates