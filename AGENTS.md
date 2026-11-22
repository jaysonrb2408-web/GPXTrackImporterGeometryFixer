
# AGENTS.md

## Project
GPX Track Importer & Geometry Fixer

## Environment
- QGIS 3.40.11 LTR
- Python bundled with QGIS
- PyQGIS
- Qt / PyQt
- Windows 10/11

## Development Rules

1. Preserve the existing Plugin Builder 3 structure.
2. Work directly within this plugin directory.
3. Do not unnecessarily rename existing plugin files or classes.
4. Maintain compatibility with QGIS 3.40.11 LTR.
5. Use PyQGIS APIs for QGIS layer and geometry operations.
6. Use Qt Designer for the plugin dialog interface.
7. Keep the code modular and maintainable.
8. Do not overwrite or delete existing files without explaining why.
9. Explain changes before implementing major functionality.
10. Test and verify changes where possible.

## Main Plugin Features

- Batch import multiple GPX track files.
- Combine imported features into one QGIS layer.
- User-selectable LineString or Polygon output.
- User-defined output layer name.
- Geometry validation and repair.
- Self-intersection detection.
- Duplicate consecutive vertex detection.
- Starting and ending point checks.
- Preserve GPX elevation information.
- Include elevation attributes.
- Display processing progress and results.

## Development Workflow

- The plugin is installed in the active QGIS plugin directory.
- QGIS Plugin Reloader is used to reload changes.
- Actual GPX samples are used for testing.
- Do not assume that standard system Python has access to PyQGIS.
- Preserve original GPX files during processing.
