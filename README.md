# ESM_regional_evaluation
Suite of Jupyter Notebooks for calculation of regional and global metrics for evaluation of CMIP6 ESMs

concat_cmip6, standardize_PNW_obs, and standardize_global_obs must be run on preexisting observational and CMIP6
data in order to create the appropriately formatted filed expected by all the other notebooks

cmip6_global_metrics and cmip6_regional_metrics compute all the metrics used in this evaluation over their 
respective regions.  cmip6_regional_metrics can be easily adapted to any lat/lon box over the globe.
Future functionality will add the ability to read shapefiles for region definition.

Once these metrics are computed, cmip6_global_regional_metrics can then be run to compute the Relative Error Scores
and various other things like the effect on the future projections.

cmip6_metrics-splitSample isolates 1901-1950 as the evaluation period and verifies against 1951-2014

cmip6_perfect_model_eval evaluates all models against each "perfect" model and creates ranking distributions for
all models, allowing some evaluation of model similarity
