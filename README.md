# Preset public examples

This list contains a series of examples that are loaded into Preset workspaces.

## Adding new examples

To add a new example:

1. Create a dashboard or chart in Preset using one of the datasets from the examples database.
2. Export the dashboard or chart.
3. Unzip the file into a directory.
4. Copy all the files from `charts/` and `dashboards/` to this repo.
5. Copy any files from `datasets/` that don't exist in this repo.
6. Do not copy `metadata.yaml` or `databases/examples.yaml`.
7. For every new dataset file added, export the table data to CSV, compress with `gzip`, and put the file in the `data/` directory.
8. Edit the dataset file, and add an attribute `data` that points to the URL of the data (see [this example](https://github.com/preset-io/public-examples/blob/64e0328b53e3798152fafa4268f22b15ca8e240d/datasets/examples/FCC_2018_Survey.yaml#L1487)).
