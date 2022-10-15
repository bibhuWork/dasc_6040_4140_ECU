Supplementary data package for the paper 'Tracing Semantic Variation in Slang'.

This data package is comprised of two parts:

1) Sample data entries and pre-processing scripts

The sample_entries/ directory contains 3 sample Green's Dictionary of Slang (GDoS; https://greensdictofslang.com/) entries for the slang word "beast" in their raw html forms. The Python files contain pre-processing code used to turn raw data into structured forms used in the paper. See the attached IPython notebook Preprocess.ipynb for detailed instructions and illustrations of how the data is processed.

2) List of words used to in the paper's experiments

The word_lists/ directory contains the list of words used in the paper's experiments where we only consider words with a minimum number of senses (denoted as k) per region. The list is provided in a csv file where each line (excluding the header) contains the word itself and the highest k in which it is sampled. For example, if a word has 5 US senses and 7 UK senses, then k = min(5, 7) = 5 and the word will be considered in all experiment conditions where k <= 5. The file us_uk.csv contains words used for the binary classification (between US and UK regions) experiment in the main results and us_uk_aus.csv contains words used for the 3-way experiment including Australian slang shown in the appendix.