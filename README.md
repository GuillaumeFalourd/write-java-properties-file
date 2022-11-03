# Write Java Properties File

<!-- markdownlint-disable MD013 -->
[![Action test on Ubuntu](https://github.com/GuillaumeFalourd/write-java-properties-file/actions/workflows/ubuntu_action_test.yml/badge.svg)](https://github.com/GuillaumeFalourd/write-java-properties-file/actions/workflows/ubuntu_action_test.yml) [![Action test on MacOS](https://github.com/GuillaumeFalourd/write-java-properties-file/actions/workflows/macos_action_test.yml/badge.svg)](https://github.com/GuillaumeFalourd/write-java-properties-file/actions/workflows/macos_action_test.yml) [![Action test on Windows](https://github.com/GuillaumeFalourd/write-java-properties-file/actions/workflows/windows_action_test.yml/badge.svg)](https://github.com/GuillaumeFalourd/write-java-properties-file/actions/workflows/windows_action_test.yml)
<!-- markdownlint-enable MD013 -->

☞ GitHub Action to write keys=values to a java `.properties` file ☕️ :octocat:

## 📚 Usage

### Simple value

```yaml
- name: Write simple value to application.properties file
  uses: GuillaumeFalourd/write-java-properties-file@v1
  with:
    file_path: ./src/main/resources/application.properties
    property: property.key
    value: value
```

### Multiline values

```yaml
- name: Write multiple values to application.properties file
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

## 🕵️ Troubleshooting

- If the action is adding the first `key=value` at the same line as the last `key=value` present on the file, **add a new empty line to the file** before using the action.

- The action currently **doesn't support** updating a key-value (PR are welcome!).

## 🤝 Contributing

☞ If you're interested in contributing to this repository, please follow the [guidelines](https://github.com/GuillaumeFalourd/write-java-properties-file/blob/main/CONTRIBUTING.md)

## 🏅 Licensed

☞ This repository uses the [Apache License 2.0](https://github.com/GuillaumeFalourd/write-java-properties-file/blob/main/LICENSE)

<!-- ### Contribuidores

<a href="https://github.com/GuillaumeFalourd/write-java-properties-file/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=GuillaumeFalourd/write-java-properties-file" />
</a>

(Criado com [contributors-img](https://contrib.rocks)) -->
