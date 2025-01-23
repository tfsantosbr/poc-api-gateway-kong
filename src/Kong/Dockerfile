# Use a versão mais recente e estável do Kong
FROM kong:3.9.0

# Defina as versões das dependências
ENV OIDC_PLUGIN_VERSION=1.1.0
ENV JWT_PLUGIN_VERSION=1.1.0

# Mude para o usuário root para instalar as dependências
USER root

# Atualize os repositórios e instale as dependências necessárias
RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    git \
    unzip \
    luarocks \
    && rm -rf /var/lib/apt/lists/*

# Instale o plugin kong-oidc
RUN luarocks install kong-oidc ${OIDC_PLUGIN_VERSION}

# Clone e instale o plugin kong-plugin-jwt-keycloak
RUN git clone --branch v${JWT_PLUGIN_VERSION} https://github.com/gbbirkisson/kong-plugin-jwt-keycloak.git && \
    cd kong-plugin-jwt-keycloak && \
    luarocks make && \
    cd .. && \
    rm -rf kong-plugin-jwt-keycloak

# Retorne ao usuário 'kong'
USER kong
