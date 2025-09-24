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


**Important Remarks:**

1. AVOBMAT currently supports 178 metadata fields including the ones used by the [Zotero](https://www.zotero.org/) reference manager. 
2. Use only the metadata fields that you need and feel free to delete unnecessary ones..
3. The mandatory CSV fields are 'Key' and 'Date'. The value of the 'Date' field can correspond to one of the following date fields: Publication Year, Reference Year, Normalized Year, First Edition, Print Edition, Premier Year, etc.
4. To export Zotero collections in CSV and RDF formats, right-click on the collection and choose “Export Collection…”.
5. If you want to upload and preprocess files, include their file names in the “files” field of the CSV.
6. The CSV file and the text files of various sorts must be compressed into a single ZIP file.
7. AVOBMAT can download files directly from the internet and preprocess them. To enable this, include the file URLs in the “files” field of the CSV.
8. Texts for analysis can also be provided in the “text” field of the CSV.
9. For fields with multiple values (Author, Co-authors, Characters, Manual Tags, Automatic Tags, or files), separate the values using a semicolon (;).
10. Supported CSV delimiters are comma (,), semicolon (;), and tab.
11. This GitHub repository contains fillable templates in CSV, Excel, and OpenDocument formats. Be sure to export Excel and OpenDocument files as CSV before uploading.
12. CSV files must use UTF-8 encoding. Using other encodings may cause certain characters to display incorrectly. Refer to this simple [guide](https://drive.google.com/drive/folders/1SBmLK9Qur2xCvLeBfUTYMXU6NX9KoBsO) to check your CSV’s encoding and convert it to UTF-8 if needed.


**File formats supported by the Apache Tika software can be used as attachments.** 

**They include the following formats:**

- Microsoft Office: .doc, .docx, .xls, .xlsx, .ppt, .pptx
- OpenDocument: .odt, .ods, .odp
- Html, xhtml
- TXT
- PDF
- RTF


# License
[Terms of Use](https://docs.google.com/document/d/17XWovDNecfE-GNvso7LRIQ_UcDc5FxDW0-i5eBq7X7Q/edit?tab=t.0)

# Acknowledgement
We kindly request that you acknowledge AVOBMAT by citing the following papers in any publications resulting from its use and mentioning the support of the Hungarian Research Network Cloud (https://science-cloud.hu/).

Péter, R.; Szántó, Zs; Biacsi, Z.; Berend, G.; Bilicki, V. (2024). “Multilingual Analysis and Visualization of Bibliographic Metadata and Texts with the AVOBMAT Research Tool”, Journal of
Open Humanities Data vol. 10. pp. 1-10. DOI: 10.5334/johd.175.
Héder, M. et al. (2022) “The Past, Present and Future of the ELKH Cloud”, Információs Társadalom, vol. 22, no. 2. p. 128, DOI: 10.22503/inftars.xxii.2022.2.8.
