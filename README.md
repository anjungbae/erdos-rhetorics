# erdos-rhetorics

Rhetorics for Attitudinal Convergence

For Erdős Institute Data Science Boot Camp, May-Summer-2024.

Members: Adam Perhala, Jungbae An


1. Project overview
We identify rhetorical strategies that can induce attitudinal convergence in discussions. We will track attitudinal changes in longitudinal discussions and infer the factors driving the convergence of attitudes among discussion participants:
(1) Classification: We classify the expressed attention to each policy topic paid by each Senate member at a given time, using a Latent Dirichlet Allocation (Blei et al. 2003).
(2) Convergence: We examine similarity/modularity of participants' attitudes.
(3) Network Inference (using, e.g., NetInf or its variants): Finally, we will infer the cause of converging attitudes from participant, speech, and issue characteristics.

3. Stakeholders
  - Academic community
  - Policy makers and government agencies
  - Advocacy groups and political activists

3. Key Performance Indicators
  - Classification (wrt the number of K topics)
    - Semantic coherence (Mimno et al., 2011)
    - Exclusivity (Bischof and Airoldi 2012)
    - Perplexity (Wallach et al., 2009)
    - Residual dispersion (Taddy 2012)
  - Convergence
    - Similarity scores (e.g., arccos)
    - Modularity
    - Stability, with or without interventions
  - Network inference
    - Balance (wrt causal inference)
    - Estimation: DCRSEs (Aronow et al. 2013)
    - Inference: predictive power, sensitivity

4. Description of the dataset
  - Dataset: The standing committee transcripts of the US Senate in the 105-114th Congresses 
    - We use the dataset with covariates provided by Park (2021; (https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/GSMBFX)
    - Raw source: https://www.congress.gov/senate-hearing-transcripts
  - Contains: 1,026,677 speeches, held by 12,405 Senators, affiliated in the 22 Senate committees, in the 105-114th Congresses.
  - Variables include: Congress #; Committee code; Hearing title; Senator name (THOMAS name); Senator govtrack id; speech text; other covariates
