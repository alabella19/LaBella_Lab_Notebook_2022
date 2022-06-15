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

Working on verifying novoparasiticus results from Miya's work. Downloading the genome and annotation to start. I got a slightly higher S-value than Miya did but it's still not very high. I could investigate why this is?

Now analyzing the "normal" yeast Reverse Jump Bayes Traits analysis to see the rates of trait gain and loss in this group


##June 14 2022

__Goals__
- Finish Bayes Traits analysis round 1 - launch second set of analyses if ACCRE permits
- Finish Eco Ontolgy and start looking up analyses that I can do for enrichment
- Do I have time to do some analyses for the talk??

## June 15 2022

__Summary__

Today has been rough! I've done the following things
- Downloaded the ontology from the web protege 
- Used the desktop protege to identify errors in the ontology - aka I resolved multple conflicts where an object was a subclass of disjointed classes
- I have now been trying to get the ontology into a visualization analysis platform HOWEVER I think I can just extract the names for each annotation and then do some sort of fishers exact test to see if anything is enriched in our groups... but we'll see
- I was able to get the ontology into cytoscape using the following things:
1. Save the ontology in OBO format
2. Use python script to convert OBO into SIF format
3. Replace the dumb IRI with our actual annotations

Now I'm working on getting the annotations working

Ok so in order to use UFO I have to change the syntax from
is_a: Human_animal_type
to
is_a: Human_animal_type ! Human_animal_type
