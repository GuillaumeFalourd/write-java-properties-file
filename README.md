# Write Java Properties File

<!-- markdownlint-disable MD013 -->
[![Security Pipeline](https://github.com/GuillaumeFalourd/write-java-properties-file/actions/workflows/security-pipeline.yml/badge.svg)](https://github.com/GuillaumeFalourd/write-java-properties-file/actions/workflows/security-pipeline.yml) [![Super Linter](https://github.com/GuillaumeFalourd/write-java-properties-file/actions/workflows/super-linter.yml/badge.svg)](https://github.com/GuillaumeFalourd/write-java-properties-file/actions/workflows/super-linter.yml) [![Gitleaks](https://github.com/GuillaumeFalourd/write-java-properties-file/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/GuillaumeFalourd/write-java-properties-file/actions/workflows/gitleaks.yml)
<!-- markdownlint-enale MD013 -->

☞ GitHub Action to write keys=values to a java `.properties` file ☕️ :octocat:

## 📚 Usage

### Simple value

```
- name: Write values to application.properties file
  uses: GuillaumeFalourd/write-java-properties-file@v1
  with:
    file_path: ./src/main/resources/application.properties
    property: property.key
    value: value
```

### Multiline values

```
- name: Write values to application.properties file
  uses: GuillaumeFalourd/write-java-properties-file@v1
  with:
    file_path: ./src/main/resources/application.properties
    property: |
       first.property.key
       second.property.key
    value: |
       first value
       second value
```

## ▶️ Action Inputs

Field | Mandatory | Observation
------------ | ------------  | -------------
**file_path** | YES | Path to the `.properties` file.
**property** | YES | Property / Properties keys to write.
**value** | YES | Value(s) of the given property / properties, in the same order.

## 🤝 Contributing

☞ If you're interested in contributing to this repository, please follow the [guidelines](https://github.com/GuillaumeFalourd/write-java-properties-file/blob/main/CONTRIBUTING.md)

## 🏅 Licensed

☞ This repository uses the [Apache License 2.0](https://github.com/GuillaumeFalourd/write-java-properties-file/blob/main/LICENSE)

<!-- ### Contribuidores

<a href="https://github.com/GuillaumeFalourd/write-java-properties-file/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=GuillaumeFalourd/write-java-properties-file" />
</a>

(Criado com [contributors-img](https://contrib.rocks)) -->
