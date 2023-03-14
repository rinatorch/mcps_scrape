# Ten years of MCPS demographics 🏫

I coded with Python to extract ten years of demographic data for elementary, middle and high schools within [Montgomery County Public Schools](https://www.montgomeryschoolsmd.org/), the largest public school system in Maryland and one of the largest systems in the United States. With this project, I hope to empower users to analyze and inspect a decade of schools data that had previously been stored in PDFs.

## How MCPS keeps the data

MCPS publishes [annual reports](https://ww2.montgomeryschoolsmd.org/departments/sharedaccountability/glance/index.aspx) in PDFs, with each one measuring about 500 pages long. Over the past 10 years, each annual report included several tables on demographic information broken down by school, including information on student population, race, gender and free and reduced price meal recipients. There is a ton of information packed in each PDF, but this project zeroed in on these specific demographic tables.

The county maintains a [data dictionary](https://www.montgomeryschoolsmd.org/departments/sharedaccountability/glance/definitions.aspx) and [definitions](https://www.montgomeryschoolsmd.org/departments/sharedaccountability/glance/definitions.aspx) here. Fields for EML, emergent multilingual learner, and a gender X option were published only in the final tables of the 2021-2022 report.

## Methodology

I analyzed the data with Python in a Jupyter Notebook. Much of the analysis relied on libraries pdfplumber, pandas and numpy. Tabula was also a major part of the analysis. It was particularly useful to use Tabula when something went wrong with the code that I had built. For example, there was one stubborn column that my code did not always recognize, so Tabula (and a free online PDF page selector) was helpful in manually selecting the missing column.

Throughout this project, I played around with making the code more efficient with for loops. In the interest of time, I used code that was less efficient but consistent. Moving forward, I plan to continue working on ways to make the process more efficient so this extraction could be easily replicated for other school districts across the country.
