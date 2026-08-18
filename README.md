# MOE Flutter Templates

Starter dependencies and conventions for creating Flutter applications on top
of the MOE Flutter ecosystem.

This repository is a template/reference project, not a required dependency for
every MOE Flutter package. Copy the starter structure or select only the
packages required by the application.

## Validation

```bash
flutter pub get
flutter analyze
flutter test
```

The template consumes standalone Git repositories. It must not rely on sibling
paths when used outside the local package workspace.
