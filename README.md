# AVOBMAT - Analysis and Visualization of Bibliographic Metadata and Text 

[AVOBMAT website](https://avobmat.hu/)

[Registration](https://avobmat-gwdg.web.app/register)

# What is AVOBMAT?
[AVOBMAT](https://avobmat.hu/) stands for “Analysis and Visualization of Bibliographic Metadata and Text.”

[AVOBMAT](https://avobmat.hu/) is a multilingual text mining service created in close collaboration with researchers for research and teaching. It empowers scholars, educators, and students to explore large collections of textual and bibliographic data—without programming skills or costly hardware—on a user-friendly, web-based platform.

Built on an extensible, scalable, and modular cloud-based infrastructure, AVOBMAT ensures a transparent and reproducible research process supported by a wide range of analytical and visualization tools. Designed for environment-conscious use, it enables researchers to reveal hidden connections, enrich texts and metadata, and collaborate by sharing private databases. With support for 25 languages and customizable features, AVOBMAT makes advanced text analysis accessible so researchers can focus on critical interpretation and discovery.

The implemented analytical and visualization tools provide both close and distant reading of texts and bibliographic data. AVOBMAT also helps users realize the epistemological challenges, limitations, and strengths of computational text analysis and visual representation of digital texts and datasets.

The workflow of [AVOBMAT](https://avobmat.hu/) was published in the peer-reviewed [Journal of Open Humanities Data](https://openhumanitiesdata.metajnl.com/articles/10.5334/johd.175) and the [Social Sciences and Humanities Open Marketplace](https://marketplace.sshopencloud.eu/workflow/RzvCOP).

# Why use [AVOBMAT](https://avobmat.hu/)?
- Uncover new insights by revealing connections, themes, trends, and patterns that might otherwise remain hidden.- the use of transformer language models on a scalable, cloud-based infrastructure that allows researchers to preprocess and analyse texts and metadata at scale; 
- Test hypotheses and discover new evidence with advanced analytical methods.
- Upload and explore large digital collections from your own research or your library with customizable preprocessing, analysis, and visualization tools.
- Combine bibliographic data and text analysis to ask complex research questions using natural language processing techniques.
- Critically interpret texts, metadata, and visualizations, recognizing the strengths and limitations of computational methods.
- Detect biases and errors (e.g. selection, metadata, classification) in large databases to make more informed research decisions.
- Teach digital humanities by demonstrating both the possibilities and challenges of computational text analysis and visualization.
- Collaborate and share your findings or make your databases public to support collective knowledge-building.

# AVOBMAT features

- **Multilingual Text Enrichment:** Preprocess, analyze, and semantically enrich large numbers of texts and metadata in 25 languages without coding skills.

- **Interactive analysis:** Explore texts and bibliographic data with tools that support both close and distant reading.

- **Transparent and reproducible workflows:** Built on a peer-reviewed, extensible, scalable, and modular cloud-based infrastructure, with customizable settings for every tool.

- **Environment-conscious use**: Infrastructure designed with sustainability in mind.

- **User-friendly NLP tools:** Integrates bibliographic data with cutting-edge natural language processing methods in a single, interactive platform.

- **Critical Analysis and Visualizations:** Identify data gaps, missing metadata, or inconsistencies to strengthen your research.

- **Comparative and diachronic analysis:** Conduct multilingual, time-based comparisons across different corpora.

- **Collaboration tools**: Share private databases and results to foster cooperation between researchers.

# Contents
This github repository contains the following:

1. Sample upload databases, files and the supported metadata fields (179)

2. Enriched and corrected [DraCor](https://dracor.org/) drama metadata. 
- We added the following new fields to the original CSVs of the DraCor repository: Author forename, Author gender, Author birth, Author death, Characters (with their gender), Co-authors, Author age (time of writing), Posthumous publication
		 
3. Enriched and corrected [ELTeC](https://github.com/COST-ELTeC) novel metadata.
- We added the following new fields to the original CSVs of the ELTeC repository: Author age (time of writing) and Posthumous publication.

The Notes field contains all the corrections and modifications that Róbert Péter and Zoltán Kocsis made in the DraCor and ELTeC original metadata.

# Supported File Formats

You can upload your databases in various formats or submit upload requests with your preferred configuration settings in AVOBMAT. Sample databases and files are available in this repository. 

**The supported formats are as follows:**

- CSV (metadata only), including Zotero CSV 
- CSV and text files
- CSV with external links to text files
- CSV with embedded texts
- TEI XMLs with CSV (metadata)
- Zotero RDF (metadata and text files)


# Steps for Preparing and Uploading Textual Data

You don’t need programming knowledge to upload your own databases. Just follow these steps carefully.

1. Fill in your spreadsheet (Excel or LibreOffice)
    - Start with one of the fillable templates provided in the sample_upload_databases folder of this GitHub repository (for example, avobmat_fillable_and_instructions_xlsx.xlsx).
    - These templates already contain all supported metadata fields such as Author, Title and Date, so you don’t have to create the spreadsheet from scratch.
    - AVOBMAT supports over 200 metadata fields (including Zotero fields), but you only need to use the ones relevant to your project. Extra columns can be left blank or deleted.
    - If the required metadata field is not available in the spreadsheet, use one of the existing fields. You will be able to rename it after uploading your database.
    - The mandatory columns in the spreadsheet are the following:
        1. Key → a unique identifier for each item (e.g. a book)
        2. Date → a date associated with the item (e.g. Publication Year, Reference Year, First Edition Year, Print Edition Year, Premier Year, etc.).

2. Handle fields with multiple values
    - Some fields allow more than one value (for example: Author, Co-authors, Characters, Manual Tags, files).
    - In the template file avobmat_fillable_and_instructions_xlsx.xlsx, fields that allow multiple values are marked with a green check mark ✅.
    - Separate multiple values with a semicolon ( ; ). Example: Smith,John;Doe,Jane

3. Add files or texts
    - To include files for analysis, put their file names in the files column.
    - Supported file formats: You can attach any file type supported by Apache Tika. These include:
        1. Microsoft Office: .doc, .docx, .xls, .xlsx, .ppt, .pptx
        2. OpenDocument: .odt, .ods, .odp
        3. Web formats: .html, .xhtml
        4. Plain text: .txt
        5. PDF: .pdf
        6. TEI XML format: .xml
        7. Rich Text Format: .rtf
    - You may also include URLs in the files column. AVOBMAT will download and preprocess them automatically.
    - If you prefer to provide text directly, paste it into the text column.
    - It is also possible to run analyses on metadata only (CSV without any text).

4. Save your spreadsheet as CSV (UTF-8)
    - When your database is ready, export it from Excel or LibreOffice as a CSV (UTF-8) file.
    - In Excel:
        1. Open your filled worksheet.
        2. If you want to save all metadata, clear filters. If you only want to save a filtered subset, apply filters first.
        3. Go to File > Save As, choose a location, and select CSV (UTF-8) format.
        4. Click Save.
    - In LibreOffice: use File > Save As and select Text CSV (.csv), making sure UTF-8 is chosen as the encoding.
    - AVOBMAT accepts CSVs with comma (,), semicolon (;), or tab delimiters.
    - Always save in UTF-8 encoding so that all special characters display correctly. Using other encodings may cause certain characters (such as accents or special symbols) to look wrong.
    - If you are unsure whether your CSV is UTF-8, you can check and convert it using this simple guide.

5. Export (textual) data from Zotero (OPTIONAL)
    - To use your Zotero collections, right-click on a collection and select “Export Collection…”.
    - Export in CSV or RDF (metadata and texts) format. You can then adapt the exported file to AVOBMAT.


6. Bundle your files for upload
    - If you are analyzing only metadata: just upload your CSV file.
    - If you are analyzing texts as well: either
        - include them directly in the text column of the CSV, or
        - place the CSV and text files together in one folder.
    - If you have separate text files, compress the CSV and text files into a single ZIP file before uploading.


7. If you are not a privileged user with full upload rights, please provide a link to the shared folder (e.g., Google Drive, Dropbox, or OneDrive) where we can access your zipped file. Please make sure the folder is shared so that anyone with the link can view and download the file; otherwise we will receive a ‘You need access’ message and will not be able to process your data.


# License
[Terms of Use](https://docs.google.com/document/d/17XWovDNecfE-GNvso7LRIQ_UcDc5FxDW0-i5eBq7X7Q/edit?tab=t.0)

# Acknowledgement
We kindly request that you acknowledge AVOBMAT by citing the following papers in any publications resulting from its use and mentioning the support of the Hungarian Research Network Cloud (https://science-cloud.hu/).

Péter, R.; Szántó, Zs; Biacsi, Z.; Berend, G.; Bilicki, V. (2024). “Multilingual Analysis and Visualization of Bibliographic Metadata and Texts with the AVOBMAT Research Tool”, Journal of
Open Humanities Data vol. 10. pp. 1-10. DOI: 10.5334/johd.175.
Héder, M. et al. (2022) “The Past, Present and Future of the ELKH Cloud”, Információs Társadalom, vol. 22, no. 2. p. 128, DOI: 10.22503/inftars.xxii.2022.2.8.
