# Helm Labby

A helm chart for deploying labby the rat, our opsdroid bot.

## Config

If you're in the Informatics Lab you'll need to symlink out `config.yaml` file from our [private config](https://github.com/met-office-lab/private-config).

```shell
ln -s /path/to/private-config/helm-labby/config.yaml config.yaml
```

Otherwise you'll need to get your own.

## Usage

```shell
helm install labby --name labby --namespace labby -f config.yaml
```

```shell
helm upgrade labby labby -f config.yaml
```

```shell
helm delete labby --purge
```
