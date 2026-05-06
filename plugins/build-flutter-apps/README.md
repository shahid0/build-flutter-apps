# Build Flutter Apps

Local Codex plugin for Flutter and Dart development workflows.

It includes:

- Official Flutter skills from `flutter/skills`.
- Official Dart skills from `dart-lang/skills`.
- MCP configuration for the official Dart/Flutter MCP server using `dart mcp-server`.
- A generated plugin icon at `assets/icon.png`.
- A marketplace entry under `.agents/plugins/marketplace.json`.

Sources:

- https://docs.flutter.dev/ai/mcp-server
- https://docs.flutter.dev/ai/agent-skills
- https://docs.flutter.dev/ai/ai-rules
- https://docs.flutter.dev/ai/best-practices/developer-experience
- https://github.com/flutter/skills
- https://github.com/dart-lang/skills

The MCP server requires a Dart/Flutter SDK that supports `dart mcp-server` on the user's `PATH`.

## Included Skills

Flutter:

- `flutter-add-integration-test`
- `flutter-add-widget-preview`
- `flutter-add-widget-test`
- `flutter-apply-architecture-best-practices`
- `flutter-build-responsive-layout`
- `flutter-fix-layout-issues`
- `flutter-implement-json-serialization`
- `flutter-setup-declarative-routing`
- `flutter-setup-localization`
- `flutter-use-http-package`

Dart:

- `dart-add-unit-test`
- `dart-build-cli-app`
- `dart-collect-coverage`
- `dart-fix-runtime-errors`
- `dart-generate-test-mocks`
- `dart-migrate-to-checks-package`
- `dart-resolve-package-conflicts`
- `dart-run-static-analysis`
- `dart-use-pattern-matching`

## Attribution

The vendored Flutter skills are from https://github.com/flutter/skills at commit `79ac38cc1b41d3d7bd3f5ecace679e1d8fc18918`.

The vendored Dart skills are from https://github.com/dart-lang/skills at commit `3bfffc047dbefb92cb178c0af53f357f802a09d7`.

License copies are included as `FLUTTER_SKILLS_LICENSE` and `DART_SKILLS_LICENSE`.
