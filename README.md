# DonorAtlas Software Engineering: Round 2

Understanding **how** our current users use our software is one of the best tools we have to improve it, and to choose what we should build next.

Today, you are the DonorAtlas Head of Logs, and you are tasked with building some new tools to help us understand usage patterns from our existing platform log files.

Our logs are stored as CSV files, one for each day, which contain the following columns:

- timestamp
- user_id
- action: "search", "donor_view", "export", "login", "logout"
- search_query: the query the user searched for, if the action was a search
- donor_id: the donor ID the user viewed, if the action was a donor view
- export_n_ids: the number of donors the user exported, if the action was an export