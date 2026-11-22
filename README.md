# AllanStruthersPublicCourses

Public publication destination for reviewed student-facing course materials.

## Publishing source

This repository receives copies from [`PrivateCourses`](https://github.com/AllanStruthersMTU/PrivateCourses). Only material deliberately placed under that repository's `ToBePublished/` directory should be copied here.

This repository should not be used as the source of truth for source edits. Make material changes in `PrivateCourses`, review them there, and publish them through the copying script.

## Copying script location

The planned one-way copying script is maintained in the private source repository at:

- `.github/scripts/publish_courses.py`

The script and its configuration are not stored in this public repository. This prevents public edits from changing the publishing process independently of the private source repository.

## How to edit the copying process

To change the copying process, edit `.github/scripts/publish_courses.py` in [`PrivateCourses`](https://github.com/AllanStruthersMTU/PrivateCourses). Use pull requests or a branch to review changes.

Workflow triggers and permissions are planned in:

- `.github/workflows/publish-courses.yml`

Changes to this public repository that do not originate in `PrivateCourses` should be treated as out-of-band changes and reviewed before the next publication.

## Safety requirements

- Never copy private directories or secrets.
- Keep the destination and branch allowlisted.
- Preview changes before publishing to this repository.
- Do not enable automatic deletion until all existing paths have been reviewed.
- Remember that removing a file here from the public repository does not remove it from public Git history.

## Active Fall 2026 repository

The existing [`2026-Fall-Classes`](https://github.com/AllanStruthersMTU/2026-Fall-Classes) repository remains independent and unchanged until an explicit migration is approved.
