# MCPS PDF Scrape

In this project, I coded with Python to extract ten years of demographic data for public elementary, middle and high schools in Montgomery County, Maryland. Montgomery County Public Schools is the largest public school system in Maryland. It's also one of the largest systems in the United States.

## How MCPS keeps the data

MCPS publishes annual reports in PDFs. Each of the PDFs are around 500 pages long. Over the past ten years, each annual report included several tables on demographic information broken down by school, including information on student population, race, gender and free and reduced price lunch. There is a ton of information packed in each PDF, but this project zeroed in on these demographics tables.

## Methodology

I analyzed the data with Python in a Jupyter Notebook. Much of the analysis relied on libraries pdfplumber, pandas and numpy. Tabula was also a major part of the analysis. It was particularly useful to use Tabula when something went wrong with the code that I had built. There was one stubborn column that did not always appear in the dataframe, so Tabula (and a free online PDF page extractor) was helpful as a tool to manually include the missing column.

Throughout this analysis, I played around with making the code more efficient with for loops. In the extraneous notebooks in this repository, there are a lot of attempts to do that. Many were only intermittently successful. In the interest of time, I used code that was less efficient but consistent. Moving forward, I plan to continue working on ways to make the process more efficient so that this analysis could easily be replicates for other school districts, and maybe for even more years of MCPS data.
