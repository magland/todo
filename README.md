# todo

---
- [ ] dendro jobs: option to save local and/or to the cloud

- [ ] dendro: rename project script

- [ ] dendro processor: Extract frame slice -> NWB

- [ ] dandi-nwb-meta: create index file - do not gzip - load from neurosift

- [ ] Neurosift: PSTH button even when units is not in standard place. Pop up with message that they should select a TimeIntervals. Same with TimeAlignedSeries

- [ ] Neurosift: Dendro tab

- [ ] Dendro: figure out how to support projects with very large number of files/jobs

- [ ] Neurosift: Trial Aligned ROI Series: https://github.com/flatironinstitute/neurosift/issues/115

- [ ] Neurosift: dandiset selector: https://github.com/flatironinstitute/neurosift/issues/104

- [ ] Dendro: option to store outputs local to compute resource

- [ ] Dendro: don't refresh the whole file view when a job status changes
- [ ] Dendro: Private projects - do not show on neurosift

- [ ] Dendro compute resource: trigger reload of apps from gui (in case spec.json has changed) - do not crash on fail
- [ ] Dendro - quotas for api requests
- [ ] Dendro: maintain list of system apps
- [ ] Dendro: projects list - make sortable

- [ ] [Generate composite views for dandi-vis](https://github.com/magland/dandi-vis/blob/main/dandisets/000582/000582.md)
- [ ] raster plot nh5 - include binned data array
- [ ] Dendro: users bring their own s3 bucket
- [ ] Dendro: pruning intermediate files
- [ ] Dendro frontent: plugins - create a plugin interface

- [ ] Dendro: compute resource - provide configuration option to determine which jobs require approval
---
- [ ] remfile: improve benchmarks
---
- [ ] Dendro: in an app, somehow specify what requirements there are for nwb input file
---
- [ ] Kachery: revisit docs
- [ ] Kachery: remove fallback bucket stuff
  - Need to think about how to do this. There is ~500GB on wasabi. A lot of this is spikeforest stuff. Maybe should be moved to a spikeforest zone? Then how to redirect existing links?
---
- [ ] Figure out how to dynamically compose figurl views, sharing a context
---
- [ ] Dendro: isomorphic git - handle case where history has changed
- [ ] Dendro: isomorphic git - create own cors server

- [ ] Improve spike sorting analysis figurl (show snippets)
- [ ] Clean up github home page
- [ ] [Dendro: Compute receptive fields figurl](https://github.com/flatironinstitute/dendro/issues/114)
- [ ] Dendro: Set up free default resource with limited cpu/ram/disk for basic tasks
- [ ] Audio/video view

- [ ] Neurosift zoom improvement suggestion from Cody: https://github.com/flatironinstitute/neurosift/issues/120

---

### 2024-02-19

- [x] dendroextractors
- [x] troubleshooting error on writing binary recording

### 2024-02-14

- [x] Dendro: projects scripts

### 2024-02-13

- [x] Dendro: file caching on compute resource
- [x] Dendro: implementing project scripts

### 2024-02-12

- [x] si-dendro-apps: working on si_preprocessing_dev
- [x] dendro: get project file uri
- [x] Figure out cloudflare tunnel


### 2024-02-10

- [x] Neurosift: TimeAlignedSeries

### 2024-02-09

- [x] Neurosift: dandiset page
- [x] Dendro: changes to api supporting SI json files for processed recordings
- [x] Neurosift: show CHANGES file for dandiset

### 2024-04-08

- [x] dandi-vis: ecephys_summary processor

### 2024-02-07

- [x] dendro: spike_sorting_summary (SSS)
- [x] move neurosift source code to fi-sci (this was actually done sometime last week)

### 2024-02-06

- [x] prog rep
- [x] dandi-vis: spike_sorting_summary
- [x] Dendro: file download button
- [x] dendro si-pipelines: stub_test_duration_sec parameter
- [x] dandi-vis links to neurosift
- [x] neurosift - load stuff from dendro project
- [x] figurl-dandi-vis: raster plot: enforce max vert spacing between rows

### 2024-02-01

- [x] nh5 js: implement canceler
- [x] dandi-vis
- [x] dendro app: dandi-vis-1
- [x] fi-sci app: figurl-dandi-vis

### 2024-01-31

- [x] dandiset-vis-generator: 000582
- [x] dandiset-vis-generator: 000784
- [x] NwbSortingExtractor: allow units_path
- [x] NwbSortingExtractor: allow no elec series
- [x] dendro: approve all jobs button
- [x] Create dandiset-vis-generator
- [x] Prepend Project ID on Job ID

### 2024-01-30

- [x] MountainSort5: created Quip
- [x] Collecting blurbs for p. eval

### 2024-01-29

- [x] Create FSBucket
- [x] FSBucket: Deployed on popeye

### Misc

- [x] Dendro: add project without starting with dandiset
- [x] Dendro: create example analyses
- [x] Dendro: Fix CDK stack for attaching large disk to instance
- [x] Archive old repos

### 2024-01-26

- [x] spyndle - initial version of spyglass interface
- [x] spyndle - kubernetes cluster
- [x] dandi-nwb-meta - use h5tojson from rly
- [x] h5tojson - use pydantic models

### 2024-01-22

- [x] dandi-nwb-meta: include namespace (e.g., core)
- [x] [dandi-nwb-meta](https://github.com/magland/dandi-nwb-meta/tree/main)
- [x] Dendro: support folders in gui

### 2024-01-19

- [x] Dendro: change landing page
- [x] Neurosift - fixed display problem for time intervals
- [x] Dendro - folders as inputs and outputs of jobs

### 2024-01-18

- [x] Dendro - pipelining of jobs

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

