# Davis PACS — Imaging Workspace

![Davis PACS Viewer](https://raw.githubusercontent.com/mahdihp1997/mahdihp1997/main/assets/project-pacs-viewer.svg)

A React imaging workspace for reviewing DICOM studies and connecting an imaging operator's daily admission queue with physician review and reporting.

## Workflow

An eligible admission appears in its configured imaging service queue. The operator selects the person and visit, confirms identity, and attaches DICOM files. The physician opens the original study and records a versioned report. Separate visits remain distinct.

## Implemented capabilities

- Study worklists, series navigation and multiple viewports.
- Window/level, zoom/pan, cine, image orientation controls and measurement/ROI tools.
- Draft/final reports, report revisions and addenda, annotation workflows and key image references.
- MPR and intensity slabs for supported conventional CT/MR/PET data; threshold masks and bounded DICOM SEG exchange.
- Patient-space fusion checks and landmark-based rigid registration with residual review.
- Daily monitoring queues with service/device grants, admission context and upload progress.

## Engineering

React, Cornerstone, Java REST APIs, PostgreSQL and DICOM interfaces. The last recorded full local acceptance passed 133 frontend tests across 28 suites. The monitoring adapter also passed 40 native integration checks on isolated synthetic data. Later launcher changes require their own version-matched release evidence.

This is an installation candidate with local verification. Deployment-specific device, identity, display, network and clinical acceptance remain necessary. CPU volume preview and supported input geometry have documented bounds; the project does not claim universal DICOM or registration support.

## Project access

This page is a public project overview. Source access and deployment arrangements are managed separately. Demo material uses synthetic images; no patient data or credentials are included here.

[Developer profile](https://github.com/mahdihp1997)
