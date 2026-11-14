## Welcome to my repository

**IT analyst** building data pipelines and analytics, from raw data to a live, published tool. Sydney, Australia · Master of Analytics, UNSW.

[Portfolio](https://kohstack.tech) · [LinkedIn](https://www.linkedin.com/in/sylvester-koh/) · [Email](mailto:sylvester@kohstack.au)

<table>
  <tr>
    <th width="50%" align="left">Flight delays at Ho Chi Minh City airport (SGN)</th>
    <th width="50%" align="left">Payment fraud in 590,540 transactions</th>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>0.864 ROC-AUC</h3>
      Predicts which arrivals land 15+ minutes late, tested against real arrival times on 1,321 later flights held out from training. The earlier model's 0.796 was scored against forecast delays, because 0 of 243 late flights had a recorded arrival time. I found and fixed that label bias.
      <br>
      <b><a href="https://kohstack.tech/sgn/">Live SGN tool</a></b> · <a href="https://github.com/sKoih-pond/sgn-flight-warehouse">sgn-flight-warehouse</a>
    </td>
    <td width="50%" valign="top">
      <h3>0.913 ROC-AUC</h3>
      Documented features only, tested forward in time, matching a black box given 339 more anonymised columns. A cost-based block rule costs 73% less than a 0.5 cut-off and recovers 80% of the $967k at risk.
      <br>
      <b><a href="https://lookerstudio.google.com/reporting/d0032be5-ae94-487d-8046-d5649f64453c">Live fraud dashboard</a></b> · <a href="https://github.com/sKoih-pond/user-analytics-risk/blob/main/docs/results.md">Results</a> · <a href="https://github.com/sKoih-pond/user-analytics-risk">user-analytics-risk</a>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      FlightRadar24 public data<br>
      → Azure Functions (Python)<br>
      → Azure SQL star schema<br>
      → calibrated XGBoost<br>
      → public web tool
      <br><br>
      Grafana monitoring surfaced a silent 6-week outage the status emails couldn't report. The ingest slice also ran on AWS and Azure via OpenTofu, with the same 177 rows on both.
    </td>
    <td width="50%" valign="top">
      <img src="https://raw.githubusercontent.com/sKoih-pond/user-analytics-risk/6879d00644c3d627218c043d57051781e5006086/docs/charts/model_comparison.png" width="100%" alt="Bar chart of fraud-model PR-AUC on a time-split test: explainable model 0.540, black box with 339 extra columns 0.538, deep MLP 0.316, autoencoder 0.057.">
    </td>
  </tr>
  <tr>
    <th width="50%" align="left">Stack</th>
    <th width="50%" align="left">Activity</th>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <b>Modelling:</b> SQL, T-SQL, dbt, star schema<br>
      <b>Warehouses:</b> Azure SQL, DuckDB, BigQuery<br>
      <b>Python:</b> pandas, scikit-learn, XGBoost, MLflow<br>
      <b>Cloud:</b> Azure Functions, OpenTofu (AWS and Azure)<br>
      <b>BI and alerts:</b> Looker Studio, Grafana, Prometheus
    </td>
    <td width="50%" valign="top">
      Most of my contributions are in private repos, so the graph below shows the activity but not the code. The projects above are public.
      <details>
        <summary>Two more public projects</summary>
        <br>
        <a href="https://github.com/sKoih-pond/support-ops-analytics">support-ops-analytics</a>: SLA reporting in SQL and dbt on 12,000 synthetic ServiceNow cases. SLA attainment falls from 93% with no reassignments to 74% with four.<br><br>
        <a href="https://github.com/sKoih-pond/unsw-nb15-ids-evaluation">unsw-nb15-ids-evaluation</a>: my UNSW Master of Analytics capstone, testing four ML intrusion-detection models by attack type. Fuzzers, built to mimic normal traffic, are detected 25 to 30 points lower.
      </details>
    </td>
  </tr>
</table>

