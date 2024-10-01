##Marking Criteria
->Are there unit tests for the API?
Yes, see tests/app_test.py.
->Are there unit tests for the model?
Yes, see tests/model_test.py.
->Are there unit tests for the logging?
Yes, see tests/log_test.py.
->Can all of the unit tests be run with a single script and do all of the unit tests pass?
Yes, run python run_tests.py.
->Is there a mechanism to monitor performance?
Yes, see src/monitor.py which contains a function to compute the Wasserstein distance metric.
->Was there an attempt to isolate the read/write unit tests from production models and logs?
Yes, see src/log.py.
->Does the API work as expected? For example, can you get predictions for a specific country as well as for all countries combined?
Yes
->Does the data ingestion exists as a function or script to facilitate automation?
Yes, see src/ingest.py.
->Were multiple models compared?
Yes, an ARIMA and SARIMA model were compared. Model comparisons are in nb/results.ipynb.
->Did the EDA investigation use visualizations?
Yes, see nb/analysis.ipynb which includes time-series, seasonal-trend decomposition, auto-correlation and partial auto-correlation plots.
->Is everything containerized within a working Docker image?
Yes, see Dockerfile.
->Did they use a visualization to compare their model to the baseline model?
Yes, see nb/results.ipynb where the ARIMA and SARIMA model results are compared to the actual revenue.
