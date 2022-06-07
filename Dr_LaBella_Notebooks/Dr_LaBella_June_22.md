## June 6 2022

__Goals__ 

Analyse the Reverse Jump MCMC analysis conducted in BayesTraits on the correlated evolution of growth traits and generalist/specialists.

__Methods__ 

- Analyze trace files in TRACER to ensure convergence - use both the likelihood AND the ESS to determine if the analysis has run long enough
- Create custom R script to determine the frequency of various models - this was created in an R-markdown file called trace_to_model_counts.Rmd 
- Tested to see if any rates are zero - from reading the paper it seems like it should be well above 80% zero score

__Results__ 

I'm still trying to figure out which comes first, gain of growth or gain of generalist in specific carbon sources


__Additional Things__

Started this lab notebook!! 


## June 7 2022

__Goals__ 

Finalize anlaysis of RJ MCMC analysis using new comparison to see if growth comes first or generalism comes first

__Methods__

- Updated trace_to_model_counts.Rmd
- Worked on making figures to show distribution of growth traits in generalists 

__Results__ 

I think I've identified which auxiliary sugars are added after a species becomes a generalist. I could test to see if that growth is correlated with another core growth?
