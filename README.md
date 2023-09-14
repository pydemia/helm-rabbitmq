# helm-rabbitmq

## Installation

```bash
helm pull oci://registry-1.docker.io/bitnamicharts/rabbitmq \
  --version "12.1.4" \
  --untar

cp rabbitmq/values.yaml ./values-rabbitmq.yaml

helm upgrade --install rabbitmq \
  ./rabbitmq \
  -n rabbitmq \
  --create-namespace \
  -f values-rabbitmq.yaml

```
