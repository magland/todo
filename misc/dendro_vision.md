posted on CN slack 1/12/24

I think it's useful to consider two types of analyses: (a) free-form exploration in notebooks and one-off scripts and (b) pipelines that use well-defined dendro apps. (And there are also hybrid scripts that submit dendro jobs via the dendro.client api.)

There are obvious advantages to (a) when the particular processing apps have not been established/implemented and when people are trying things out or creating demos.

But then there are advantages to (b) once the apps have been established -- use of cloud resources, parallelization, reproducibility, ability to use different environments for different processing steps, and many more.

There are many existing approaches to doing (a), so I think I'd like to focus on (b) for dendro, but also have it play nicely with (a).

Today I have been working on this... and so I have two scripts that demonstrate (a) and (b).

See https://dendro.vercel.app/project/a7852166?tab=project-linked-analysis

You'll see main.ipynb (you've seen it yesterday) which is approach (a)

Now there's a new file test.py -- that programatically submits a job to dendro to achieve the same processing result. -- that's (b)

Now click on the files tab, and you will see the generated file tuning_curves_2d.nh5

I haven't implemented yet, but you'd click on that to get the visualization.

You can see that with (b), we're on a position to process all the nwb files in the dandiset and benefit from cloud parallelization, etc. (edited) 

Here's the associated dendro app: https://github.com/magland/dendro_analyses/tree/main/apps/dendro1

...

Another comment about this. With (b) you have the full provenance of every file - exactly which steps were used in the pipeline to generate that file, but you don't necessarily have the script that generated the pipeline. With (a) you have (if you do the work to preserve it) the script/notebook that generated the entire analysis, but for a given output file, you don't have its provenance without sifting through the script. It's two different approaches to reproducibility, but both are important.

...

I've imported 12 sessions into the project and updated the test.py script to submit jobs for all of them... and now you can click to view the tuning curves for the outputs
