This is the code to replicate the results from the study Unraveling the Role of Viral Interference in Disrupting Biennial RSV Epidemics in Northern Stockholm.


- The code in Figures 1–6 can be used to reproduce the figures in the manuscript.

- Model calibration_baseline_model.zip: to estimate model parameters for the baseline model without viral interference parameters. ODE model can be found in "RSV_transmission_model.R". Run "	fit_hosp_data.R" in the local machine to get the output (model1.rds), or running "batch1.sh" in HPC.

- Model calibration_viral_interference_model.zip: to estimate model parameters for the viral interference model with assuming viral interference effects differ across 3 phases. ODE model can be found in "RSV_transmission_model_interferen_climate.R". Run "fit_hosp_data.R" in the local machine to get the output (model3.rds), or running "batch1.sh" in HPC.

- LHS_SIR.zip: latin-hypercube sampling and sampling-importance-resampling. The latin-hypercube sampling code can be found in LHS_sampling.R. High performance computers are required to generate 100,000 model predictions. Run batch(1-50).sh in the cluster. Output for viral interference parameters can be found in sampled_xi1.rds, sampled_xi2.rds, sampled_xi3.rds, and sampled_eta.rds. 

