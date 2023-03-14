# Montgomery County Public Schools PDF Scrape

In this project, I coded with Python to extract ten years of demographic data for public elementary, middle and high schools in within Montgomery County Public Schools, the largest public school system in Maryland and one of the largest systems in the United States. With this project, I hope to empower users to analyze and inspect a decade of schools data that had previously been stored in PDFs.

## How MCPS keeps the data

MCPS publishes annual reports in PDFs. Each of the PDFs are around 500 pages long. Over the past ten years, each annual report included several tables on demographic information broken down by school, including information on student population, race, gender and free and reduced price lunch. There is a ton of information packed in each PDF, but this project zeroed in on these demographics tables.

## Methodology

I analyzed the data with Python in a Jupyter Notebook. Much of the analysis relied on libraries pdfplumber, pandas and numpy. Tabula was also a major part of the analysis. It was particularly useful to use Tabula when something went wrong with the code that I had built. There was one stubborn column that did not always appear in the dataframe, so Tabula (and a free online PDF page selector) was helpful in manually including the missing column.

Throughout this analysis, I played around with making the code more efficient with for loops. In the interest of time, I used code that was less efficient but consistent. Moving forward, I plan to continue working on ways to make the process more efficient so that this analysis could easily be replicated for other school districts, and maybe for even more years of MCPS data.
