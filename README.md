# README: HathiTrust US Federal Document Suggester Analysis

This repository is a pilot project to find records that may be US Federal Documents, but not marked as such in the 008 MARC fields. This analysis uses two data sources, Zephir Database and the HathiTrust US Federal Document database. Analysis will be limited to a the included dataset without access to the Zephir environment. The 

## How to Use

### Option A. Read-only
This repository includes notebooks, datasets, and reports accurate to the time they were committed into the repository. They can be read and used as-is. Github will display juypyter notebook files online.

#### Main Analysis
HathiTrust US Federal Document Suggester Analysis (usfd_suggestion_analysis.ipynb)

#### Prototpye Reports
Are included in the `/reports` directory

### Option B. Running
This requires a python and jupyter notebook environment. Also, without Zephir credentials, you will have to skip to step 3 or later with the dataset included in the repository.

#### Step 1. Gather external data.
Run the following notebooks.
 * Create Zephir Dataset (create_zephir_dataset.ipynb)
 * Create HT US Federal Documents (create_htusfd_dataset.ipynb)
 
#### Step 2. Calulate the overlap between the datasets.
Run the following notebooks.
 * Create Overlap Dataset (create_overlap_dataset.ipynb)

#### Step 3. Run analysis to identify candidate suggestions.
Run the following notebooks.
 * HathiTrust US Federal Document Suggester Analysis (usfd_suggestion_analysis.ipynb)
 
#### Step 4. Create prototype reports
Run the following notebooks.
 * Build Reports (build_reports.ipynb)