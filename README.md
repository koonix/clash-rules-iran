# Clash Rules for Iran

Single-file classical
[Clash](https://github.com/topics/clash)
and [Mihomo](https://github.com/MetaCubeX/mihomo/tree/Meta)
rules for routing Iranian domains and IPs.

Automatically updated every day.

## Note about formats

Clash rules are available in `text` and `yaml` formats.

The `text` format is preferred as it's smaller and faster to process.

The `text` format is supported in:

- Mihomo (formerly Clash.Meta) 1.14.4+
- Clash Premium 1.15.0+

## Usage

### Yaml format

```yaml
rule-providers:
  iran:
    type: http
    format: yaml
    behavior: classical
    url: https://github.com/koonix/clash-rules-iran/releases/latest/download/rules.yaml
    path: ./ruleset/iran.yaml
    interval: 86400

rules:
  - RULE-SET,iran,DIRECT
```

### Text format

```yaml
rule-providers:
  iran:
    type: http
    format: text
    behavior: classical
    url: https://github.com/koonix/clash-rules-iran/releases/latest/download/rules.txt
    path: ./ruleset/iran.txt
    interval: 86400

rules:
  - RULE-SET,iran,DIRECT
```
