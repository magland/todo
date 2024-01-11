# todo

- [ ] Dendro: mechanism for saving parameter sets
- [ ] Dendro: in an app, somehow specify what requirements there are for nwb input file
- [ ] Dendro: try kubernetes compute resource - try KIND simulator
---
- [ ] Kachery: revisit docs
- [ ] Kachery: remove fallback bucket stuff
- [ ] Kachery: allow users to create zones (subdirectories of default)
---
- [ ] fi-sci: provide action to upload figurl-tuning-curves to surge.sh
- [ ] Figure out how to dynamically compose figurl views, sharing a context
---
- [ ] Dendro: change landing page
- [ ] Dendro: isomorphic git - handle case where history has changed
- [ ] Dendro: isomorphic git - create own cors server
- [ ] Dendro: projects list - make sortable
- [ ] Dendro: add project without starting with dandiset
- [ ] Dendro: render figurl in notebook in linked analysis
- [ ] Dendro: create example analyses
- [ ] Dendro: Fix CDK stack for attaching large disk to instance
- [ ] Improve spike sorting analysis figurl (show snippets)
- [ ] Archive old repos
- [ ] Clean up github home page
- [ ] [Dendro: Compute receptive fields figurl](https://github.com/flatironinstitute/dendro/issues/114)
- [ ] Dendro: Set up free default resource with limited cpu/ram/disk for basic tasks
- [ ] Audio/video view

---

- [ ] Think about creating sadlytemporary.net on cloudflare

### 2024-01-11

- [x] Dendro: console output PR - merge and publish to pypi

### 2024-01-10

- [x] Dendro: Demo 2D tuning curve notebooks for dandisets 000128 and 000582
- [x] fi-sci: figurl-tuning-curves -- deployed to surge.sh

### 2024-01-09

- [x] Kachery: multiple zones in a bucket
- [x] Dendro: on import, add dandiset tag to project ***
- [x] Dendro: recent projects list - update project names
- [x] Dendro: scroll bar for projects list
- [x] Dendro/neurosift: Associate dendro project with dandi asset - reverse lookup
- [x] Dendro: Show current project name in title bar

### 2024-01-08

- [x] Dendro: Fix CI tests

### 2024-01-05

- [x] Dendro: fix gpu docker issue https://github.com/flatironinstitute/dendro/pull/116
- [x] Dendro: fix console output upload issue (needs to be merged) https://github.com/flatironinstitute/dendro/pull/117
- [x] Dendro frontend: support null parameter values for Optional[int] and Optional[float]

### 2024-01-04

- [x] Dendro: nwb -> spike sorting analysis figurl
- [x] Develop [dendro_apps](https://github.com/magland/dendro_apps) - autodeploy, etc
- [x] Linked analysis: render jupyter notebooks!
- [x] Add allow_float64 to figurl and sortingview to be able to handle very long recordings
- [x] Dendro: linked analysis view

### 2024-01-03

- [x] Figurl: Support json in d query parameter. [Here's an example](https://figurl.org/f?v=https://magland.github.io/fi-sci-dist/apps/figurl-spike-sorting-analysis&d={%22type%22:%22spike_sorting_analysis%22,%22analysisFile%22:%22sha1://84acb43da8a5be84c5d5ff18fc35907a4ab8b0a1?label=test.nh5%22}).
- [x] Export from Neurosift to Dendro

> It is now possible to export nwb files from neurosift into Dendro. See the "Export to Dendro" link in the screenshot.
The user is redirected to the dendro app and can select whether to import into an existing project or create a new project.
This provides a route from dandi to dendro: browse dandi -> export to neurosift -> export to dendro.
It opens possibilities for running non-spike-sorting tasks from neurosift, such as computing autocorrelograms or performing downstream analyses.

<img src="https://github.com/magland/todo/assets/3679296/aa4a587d-21b5-458f-9f59-cded1f1687b8" width="200px" />

