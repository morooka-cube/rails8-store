# Make sure RUBY_VERSION matches the Ruby version in .ruby-version
ARG RUBY_VERSION=3.3.4
FROM ghcr.io/rails/devcontainer/images/ruby:$RUBY_VERSION

# ruby3.4.1をインストール(ruby3.4用のdevcontainerイメージが用意されていないため、rbenvでインストール)
RUN sudo git -C $(rbenv root)/plugins/ruby-build pull && \
    rbenv install 3.4.1 && \
    rbenv global 3.4.1
