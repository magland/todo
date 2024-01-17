# todo

---

- [ ] nh5 - create h5py-like interface for reading - important for inspecting outputs of cebra in dendro
- [ ] Dendro frontent: plugins - create a plugin interface

- [ ] Dendro: maintain list of system apps
- [ ] Dendro: compute resource - provide configuration option to determine which jobs require approval
---
- [ ] remfile: improve benchmarks
---
- [ ] Dendro: in an app, somehow specify what requirements there are for nwb input file
- [ ] Dendro: try kubernetes compute resource - try KIND simulator
---
- [ ] Kachery: revisit docs
- [ ] Kachery: remove fallback bucket stuff
  - Need to think about how to do this. There is ~500GB on wasabi. A lot of this is spikeforest stuff. Maybe should be moved to a spikeforest zone? Then how to redirect existing links?
---
- [ ] fi-sci: provide action to upload figurl-tuning-curves to surge.sh
- [ ] Figure out how to dynamically compose figurl views, sharing a context
---
- [ ] Dendro: change landing page
- [ ] Dendro: isomorphic git - handle case where history has changed
- [ ] Dendro: isomorphic git - create own cors server
- [ ] Dendro: projects list - make sortable
- [ ] Dendro: add project without starting with dandiset
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

### 2024-01-17

- [x] letter for simons neuro collab
- [x] Create cebra dendro app
- [x] Create safepyeval: https://github.com/magland/safepyeval

### 2024-01-16

- [x] simplypyeval: in js
- [x] Denro: Dropdown for options parameters
- [x] Dendro: import/export job parameters from json file

### 2024-01-15

- [x] Backup all github repos, create dev repo, transfer kachery-gateway repo to magland
- [x] Dendro: save parameters -- https://github.com/flatironinstitute/dendro/issues/115
- [x] Dendro: render figurl in notebook in linked analysis (this was actually completed last week)

### 2024-01-13

- [x] remfile/pynwb: [Respond to Ryan](https://github.com/NeurodataWithoutBorders/pynwb/issues/1791#issuecomment-1890384094)
- [x] remfile/pynwb: [created a PR](https://github.com/NeurodataWithoutBorders/pynwb/pull/1823) to update remfile verbiage in the docs.
- [x] remfile/pynwb: Created [pynwb_streaming_benchmark](https://github.com/scratchrealm/pynwb_streaming_benchmark) repo
- [x] Dendro: jobs now require approval

On slack to Luiz: I have implemented and deployed a new 'feature' where you need to manually approve jobs before they will be picked up by the compute resource. Jobs can only be approved by the github owner of the compute resource. It should be evident in the gui how you do the approval (it's just clicking on an "approve" link). We can modify this mechanism in the future, but for now this will allow us to safely open up our aws compute resources to other groups. And it also avoids issues caused by a very large number of jobs accidentally queued by a runaway python script.

### 2024-01-12

- [x] Create nh5 python package, and release to pypi
- [x] Kachery: update log processing job to include all zones
- [x] Dendro: analysis view: render markdown
- [x] Dendro analysis: create app for dendro job
- [x] [Description of Dendro vision](./misc/dendro_vision.md) (posted on CN slack)
- [x] Dendro: create script to submit dendro jobs to project
- [x] Dendro/figurl: created tuning_curves_2d figurl view that reads nh5

### 2024-01-11

- [x] Dendro: console output PR - merge and publish to pypi
- [x] Kachery: allow users to create zones (subdirectories of default)
- [x] Dendro analyses: use poetry to manage dependencies for project analyses
- [x] Dendro: Exploring AWS ec2 options

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

