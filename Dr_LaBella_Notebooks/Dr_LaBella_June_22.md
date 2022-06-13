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


## June 8 2022

__Goals__ 

Analyze the RJ MCMC analysis 

__Methods__

__Results__

The MCMC runs were not finished for the anlayses I wanted to conduct. So I worked on figures for the manuscript including Figures 2c and 2d. I also used most of my time to work on finishing the ontology we started. I got all the classes finished!! Now we just have to add the different instances.

## June 9 2022

_Today was a day of catching up on UNC-Charlotte activities_


## June 10 2022

__Goals__

Analyse RJ MCMC Analysis

__Results__

First - apparently for a single trait the RJ MCMC cannot do a restricted analysis. It never runs a single iteration in about 2 days. So I assume I will have to use the Unrestricted to see if there is evidence of one of the rates not being zero?

##June 13 2022

__Goals__

Wrap up MCMC analysis and move on to KEGG anlaysis for the evolutionary patterns of generalist and specialist species

__Results__

L_Arabinose didn't run correctly and needs to be re-run. Should be done tomorrow. 

Working on verifying novoparasiticus results from Miya's work. Downloading the genome and annotation to start. 
