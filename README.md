![publisher][publisher]
![version][version]

---

# Analysis Options for Dart/Flutter

**_The set of rules that encourage good coding practices for applications, packages, and plugins._**

---

## Features

Analyzer and Linting Rules

---

## Getting started

To add the package, `analysis_options`, to an project:

1. Depend on it

   - Add `analysis_options` under `dev_dependencies` in the `pubspec.yaml` file.

2. Install it

   - From the terminal: Run `flutter pub get`.

3. Import it

   - Add a corresponding `include` statement in the YAML code.

---

## Usage

To use the analysis options, add the following dev dependency in your `pubspec.yaml` file:

```yaml
dev_dependencies:
  analysis_options: any
```

Add the following line in your `analysis_options.yaml` file:

```yaml
include: package:analysis_options/analysis_options.yaml
```

---

## Additional information

- `Analyzer`: Customize static analysis.
- `Linter`: Configure linter rules.

### Enabling stricter type checks

```yaml
analyzer:
  language:
    strict-casts: true
```

### Enabling individual rules

```yaml
linter:
  rules:
    - avoid_print
```

### Disabling individual rules

```yaml
linter:
  rules:
    public_member_api_docs: false
```

### Excluding files

```yaml
analyzer:
  exclude:
    - lib/generated_plugin_registrant.dart
```

### Ignoring rules

```yaml
analyzer:
  errors:
    todo: ignore
```

### Changing the severity of rules

```yaml
analyzer:
  errors:
    dead_code: info
```

---

[publisher]: https://img.shields.io/pub/publisher/analysis_options
[version]: https://img.shields.io/pub/v/analysis_options
