### TO RUN USING COMPOSE 

```yml
version: "3.9"

services:
  besu:
    image: ghcr.io/bdigismat/besu:anarchtech
    restart: always
    volumes:
      - ./data:/besu/data
    command: >
      --network=dev
      --rpc-http-enabled
      --rpc-http-api=ETH,NET,WEB3
      --host-allowlist=*
      --rpc-http-cors-origins="*"
      --data-path=/besu/data
    ports:
      - "30303:30303"
      - "30303:30303/udp"
    environment:
      - VIRTUAL_HOST=rpc.anarchtech.dantalion.org
      - VIRTUAL_PORT=8545
    networks:
        - proxy
networks:
    proxy:
        external: true
```