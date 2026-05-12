# Build Flutter Apps

A Codex plugin for Flutter and Dart development.

This plugin bundles the official Flutter and Dart agent skills and configures the official Dart/Flutter MCP server, so Codex can use project-aware Flutter workflows instead of generic mobile-development guidance.

## What It Includes

- 10 official Flutter agent skills from `flutter/skills`
- 9 official Dart agent skills from `dart-lang/skills`
- Dart/Flutter MCP server configuration using `dart mcp-server`
- Global installation support through Codex Marketplace
- Plugin metadata and icon for Codex

## Repository Structure

```text
.
├── .agents/
│   └── plugins/
│       └── marketplace.json
└── plugins/
    └── build-flutter-apps/
        ├── .codex-plugin/
        │   └── plugin.json
        ├── .mcp.json
        ├── assets/
        │   └── icon.png
        ├── skills/
        │   ├── flutter-*
        │   └── dart-*
        ├── README.md
        ├── SOURCES.md
        ├── FLUTTER_SKILLS_LICENSE
        └── DART_SKILLS_LICENSE
```

## Installation

Install globally with Codex Marketplace:

```bash
npx codex-marketplace add shahid0/build-flutter-apps --plugins --global --yes
```

Restart Codex Desktop or open a new Codex session after installation so the plugin and skills are loaded.

## Requirements

You need Dart or Flutter available on your `PATH`.

Check Dart:

```bash
dart --version
```

Check that the MCP server is available:

```bash
dart mcp-server --help
```

The plugin MCP config uses:

```json
{
  "mcpServers": {
    "dart-flutter": {
      "command": "dart",
      "args": ["mcp-server"]
    }
  }
}
```

## Included Flutter Skills

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

## Included Dart Skills

- `dart-add-unit-test`
- `dart-build-cli-app`
- `dart-collect-coverage`
- `dart-fix-runtime-errors`
- `dart-generate-test-mocks`
- `dart-migrate-to-checks-package`
- `dart-resolve-package-conflicts`
- `dart-run-static-analysis`
- `dart-use-pattern-matching`

## Example Prompts

After installing the plugin, try prompts like:

```text
Build this Flutter feature using the official Flutter and Dart skills.
```

```text
Fix the current Flutter analyzer errors using the Dart/Flutter MCP server where available.
```

```text
Add widget tests for this Flutter screen.
```

```text
Make this Flutter layout responsive for mobile, tablet, and desktop.
```

```text
Set up localization for this Flutter app.
```

## Updating

To reinstall or update from the latest GitHub version:

```bash
npx codex-marketplace add shahid0/build-flutter-apps --plugins --global --yes
```

If your Codex session is already running, restart it after updating.

## Uninstalling

```bash
npx codex-marketplace remove build-flutter-apps --global
```

If the marketplace CLI asks for the fully qualified plugin name, use:

```bash
npx codex-marketplace remove build-flutter-apps@codex-marketplace-global --global
```

## Sources

This plugin vendors official skills from:

- Flutter skills: https://github.com/flutter/skills
- Dart skills: https://github.com/dart-lang/skills

It also follows Flutter’s official AI documentation:

- Dart and Flutter MCP server: https://docs.flutter.dev/ai/mcp-server
- Agent skills for Flutter and Dart: https://docs.flutter.dev/ai/agent-skills
- AI rules for Flutter and Dart: https://docs.flutter.dev/ai/ai-rules
- Developer experience best practices: https://docs.flutter.dev/ai/best-practices/developer-experience

See `plugins/build-flutter-apps/SOURCES.md` for pinned source commits.

## License

The vendored Flutter and Dart skills use BSD-style licenses.

License copies are included:

- `plugins/build-flutter-apps/FLUTTER_SKILLS_LICENSE`
- `plugins/build-flutter-apps/DART_SKILLS_LICENSE`

## Author

Created by Shahid Hussain.

GitHub: https://github.com/shahid0
