# Repository Instructions

- Name local build artifacts with the short Git commit hash immediately after the plugin name: `CoreProtect-<short-hash>-<version>.jar`.
- Use the shaded, non-`original-` JAR from `target/` as the build artifact.
- Always build with `-Dproject.branch=development`; otherwise Maven leaves the required `branch` metadata empty and the plugin will refuse to start.
