# AVOBMAT - Analysis and Visualization of Bibliographic Metadata and Text 

[AVOBMAT website](https://avobmat.hu/)

[Registration](https://avobmat-gwdg.web.app/register)

# Description
The [AVOBMAT](https://avobmat.hu/) (Analysis and Visualization of Bibliographic Metadata and Texts) multilingual research tool enables researchers, without programming skills, to critically analyse bibliographic data and texts at scale. This exploratory tool offers a range of dynamic text and data mining tasks and provides interactive parameter tuning and control from the preprocessing to the analytical stages. The implemented analytical and visualization tools provide close and distant reading of texts and bibliographic data. It helps users realize the epistemological challenges, limitations and strengths of computational text analysis and visual representation of digital texts and datasets. 

**The unique features of the [AVOBMAT](https://avobmat.hu/) toolkit are:**
- it combines bibliographic data and textual analysis, enabling users to ask complex research questions, in one integrated, interactive and user-friendly web application; 
- the use of transformer language models on a scalable, cloud-based infrastructure that allows researchers to preprocess and analyse texts and metadata at scale; 
- it analyses and enriches texts and metadata in 16 languages; 
- users can make their private databases public. 

The workflow of [AVOBMAT](https://avobmat.hu/) was published in the peer-reviewed [Journal of Open Humanities Data](https://openhumanitiesdata.metajnl.com/articles/10.5334/johd.175) and the [Social Sciences and Humanities Open Marketplace](https://marketplace.sshopencloud.eu/workflow/RzvCOP).

# AVOBMAT features

- **Multilingual Text Enrichment:** [AVOBMAT](https://avobmat.hu/) can preprocess, analyse, and (semantically) enrich a large number of texts and metadata in several languages without coding skills.

- **Interactive Text Analysis:** The analytical and visualization tools provide interactive close and distant reading of texts and bibliographic data.

- **Validated, Transparent and Customizable Workflow:** [AVOBMAT](https://avobmat.hu/) has a transparent, peer-reviewed workflow with customizable parameter settings for all tools.

- **User-friendly NLP tools:** [AVOBMAT](https://avobmat.hu/) combines bibliographic data and natural language processing research methods (e.g. transformer models) in an integrated, interactive and user-friendly web application.

- **Critical Analysis and Visualizations:** [AVOBMAT](https://avobmat.hu/) fosters critical analysis, for instance, by identifying data gaps and missing metadata values.

- **Comparative and Diachronic Analysis:** [AVOBMAT](https://avobmat.hu/) offers multilingual comparative analysis with time-based components.

# Contents
This github repository contains the following:

1. Sample upload databases, files and the supported metadata fields (179)

2. Enriched and corrected [DraCor](https://dracor.org/) drama metadata. 
- We added the following new fields to the original CSVs of the DraCor repository: Author gender, Author birth, Author death, Characters (with their gender), Co-authors,			Author age (time of writing), Posthumous publication. 
		 
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
- EP3 XML (metadata)
- EP3 XML (metadata with external links to text files)

**Important Remarks:**

1. AVOBMAT currently supports 178 metadata fields including the ones used by the [Zotero](https://www.zotero.org/) reference manager. 
2. Use only the metadata fields that you need and feel free to delete unnecessary ones..
3. The mandatory CSV fields are: Key and one of the date fields (Date, Publication Year, Reference year, Normalised year).
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

# Citation
We kindly request that you acknowledge AVOBMAT by citing the following paper in any publications resulting from its use:

Péter, R.; Szántó, Zs; Biacsi, Z.; Berend, G.; Bilicki, V. (2024). “Multilingual Analysis and Visualization of Bibliographic Metadata and Texts with the AVOBMAT Research Tool” *Journal of Open Humanities Data* 10: 1-10.
