# parachute-science

Colonial science, also referred to as ’helicopter science’ or ’parachute science, is the practice whereby researchers from highly developed nations conduct research in nations with a lower economic status, without properly acknowledging local infrastructure and expertise (Odeny & Bosurgi, 2022). This creates a form of neo-colonialism in which global north nations dominate research and fail to form meaningful collaborations with researchers from other backgrounds. In an increasing globalised world, it is important that research becomes more inclusive and equitable, and this, unfortunately, is not reality (Akudinobi & Kilmarx, 2022). While the practice is becoming more recognised in fields such as infectious disease research and general medical research (Yozwiak et al., 2016), there remains a lack of publications bringing attention to the problem in fields such as Paleoecology, where input from local researchers and communities is vital to enrich the cultural understanding and context of a given research question about the environment. Here I outline the python based methods I used to turn publication data into a visualisation like this:


![Screen Shot 2023-04-13 at 1 50 48 PM](https://github.com/BurhanAnis/parachute-science/assets/115022379/9a31060f-cb83-4cec-905b-309d068bc20a)


Note the density of publications in the European and American countries, as compared to the countries they perform their research in.

The data used was obtained by exporting a large .csv file from the abstract and citation database Scopus (Scopus, Elsevier, n.d.). A search string, crafted by a researcher in this field at the Uni- versity of Exeter, was used to select a subset of the entire database containing journals and article titles that are relevant to Paleoecology (see QR code on final visualisation). The data ex- ported was approximately 10,000 x 55, containing information such as Journal name, article title, article abstract, author, author institutional affiliation lists, and other meta-data such as funding. You can see anexample of this in the "scopus 1999-1963" file. For the purposes of this visualisation, additional information needed to be extracted from this data set. Specifically, this information was:
• The country which the first author (proxy for lead author) is affiliated to,
• The country in which the given study took place.

This data was extracted using the "country_scraper" notebook. Note that any code used to set up the final data frame using these functions is not included as these will depend on the specific data set.

The preparation of the scraped data for the connection diagram is done using the code in "connection_diagram_setup".
