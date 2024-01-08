# todo

- [ ] Dendro: render figurl in notebook in linked analysis
- [ ] Dendro: create example analyses
- [ ] Dendro/neurosift: Associate dendro project with dandi asset - reverse lookup
- [ ] Dendro: Fix CDK stack for attaching large disk to instance
- [ ] Improve spike sorting analysis figurl (show snippets)
- [ ] Archive old repos
- [ ] Clean up github home page
- [ ] [Dendro: Compute receptive fields figurl](https://github.com/flatironinstitute/dendro/issues/114)
- [ ] Dendro: Set up free default resource with limited cpu/ram/disk for basic tasks
- [ ] Audio/video view

---

- [ ] Think about creating sadlytemporary.net on cloudflare

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

