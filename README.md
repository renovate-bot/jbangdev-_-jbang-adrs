# jbang-adrs
ADRs for jbang and jbangorg related projects


## Managing ADRs

[ADR-J](https://github.com/adoble/adr-j) is a command-line tool to manage ADRs in a project. It can be used to create new ADRs, generate a table of contents, and more. ADR-J supports JBang and is available as JBang alias `adr@adoble`. To use ADR-J, follow these steps.

### Display ADR-J version

```bash
jbang run adr@adoble version
```

### Update ADR TOC

```bash
jbang run adr@adoble generate toc
```

or

```bash
./gradlew generateAdrToc
```

## Updating the ADR template

File `madr.adoc` is the template file that is used to create new ADRs. The template can be refreshed by running command:

```bash
wget https://raw.githubusercontent.com/adoble/adr-j/refs/heads/main/doc/example_templates/madr.adoc
```

## Default editor for ADRs

Set the `EDITOR` environment variable to your preferred editor. For example, to use Visual Studio Code, run the following command:

```bash
export EDITOR=code
```

## Creating a new ADR

To create a new ADR, run the following command:

```bash
jbang run adr@adoble new Document Title
``` 

For example, the ADR for `Application Versioning` was created by running command:

```bash
jbang run adr@adoble new Application Versioning
```
