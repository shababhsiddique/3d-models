# Workspace rules

This workspace holds many 3D models designed with ScanRuler. Follow these rules for every model.

## Design tool

- Design every model with ScanRuler's reverse-engineering feature (the `reverse` plugin: `reverse_*` tools), feature by feature, saved as a `.scanruler` project in the model's folder.
- Read the relevant ScanRuler guides (`model`, `scan-to-cad`) with `guide_read` before a model's first step.

## Requirements per model

- Each model has its own requirements in `REQUIREMENTS.md` inside its folder: purpose, dimensions, fit and clearances, material, printer and print settings, and any constraints the user gives.
- Requirements belong to one model only. Never carry requirements, dimensions or design choices from one model into another unless the user says to.
- Before working on a model, read that model's `REQUIREMENTS.md`. When the user gives or changes a requirement, update that file.
- `REQUIREMENTS.md` is a working file, so the documentation rule below does not apply to it.

## One folder per model

- Each model lives in its own folder at the workspace root, named in PascalCase (e.g. `ScannerPhoneMount/`, `UnderShelfPoopDrawer/`).
- Everything for that model goes inside its folder: the `.scanruler` project, STEP, STLs, and any reference files.
- Never put model files at the workspace root or in another model's folder.

## No documentation until the user says the model is done

- While designing or revising a model, produce only the working files: the `.scanruler` project and the exports needed to check or print it (STEP, STL).
- Do NOT create README files, guides, how-tos, PDFs, rendered images, or other write-ups until the user explicitly says the model is done.
- Revisions follow the same rule. When a finished model is reopened for changes, do not create or update its docs, images or PDFs until the user says the revision is done.
- Render views in ScanRuler to check work yourself, but do not save them as files in the model folder.
