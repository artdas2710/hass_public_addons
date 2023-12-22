FROM linuxserver/wireguard

# Install dependencies
RUN apk add --no-cache jq

# Copy scripts and configuration files
COPY run.sh /run.sh
COPY data/wg-easy/config.yaml /config/wg-easy/config.yaml

# Set permissions
RUN chmod a+x /run.sh

CMD [ "/run.sh" ]
