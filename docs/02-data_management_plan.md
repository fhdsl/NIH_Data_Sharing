


# (PART\*) Creating a DMS Plan {-}

# Video Creating Your Plan

Check out the video below. It provides a summary of this section of the course.

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/hjCbLCyetBc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

# Overview of the DMS Plan

The NIH has provided an outline for what components of the Data Sharing and Management Plan are required. We'll introduce these sections and then discuss in more detail some of the important considerations you'll need to include in your specific plan. 

The following are the major sections of the NIH DMS plan:

1. **Data type** - describe what data (amount and type) will be generated over the course of funding and what data will or will not be shared
2. **Tools, software, and code** - describe what tools (and versions) you intend to use to manage and analyze the data (note code is not required to be shared)
3. **Standards** - describe any standards that you might need to use for your data and metadata to make them usable by others or be contributed to a repository
4. **Data preservation, access, timelines** - describe where the data will be made available and when
5. **Access, distribution, reuse considerations** - describe how you have carefully considered any reasons that might limit sharing
6. **Oversight** - describe who will manage compliance of the DMS plan

We will cover specific requirements for each of these sections later. However, before starting to write your plan, it may be helpful to consider the data types and size you plan to generate, the repositories available, and the corresponding budgetary implications prior. 

# Data Management and Storage

To enable a more productive research experience and to ease your future compliance with any data sharing requirements, active data management during the research process can be very helpful.  

<img src="resources/images/02-data_management_plan_files/figure-html//1luFoDzF6aDJEebbL6iWoJ_s8s9nQnaWLL5jghbmWdak_g16b04bd80e5_4_37.png" alt="We are on the third step of the pathway - Data Storage Options." width="80%" style="display: block; margin: auto;" />

## Data Storage Concerns

<div class = "question">

How should you store and interact with data while doing research?
</div>

Your data storage needs will depend greatly on the type of data you will be working with as well as the number of samples you might have. File sizes vary considerably based on the data being stored. A single file can be as small as 1 MB in size (for a PET scan image of the heart) to 60 GB (for an uncompressed fastq of a whole genome sequence). Storing files in a compressed format, especially raw files, can help decrease your storage needs and costs. Below is a table of common types of data and sizes for single files. This list is not comprehensive but instead should be taken as a general guide. You should always get a more specific estimate for your particular project before submitting your grant proposal.

| **Type of data** | **Common size for a _single_ file** |
|------------------|------------------|
| Genomics (WGS, WES) |	15-60 GB |
| Genomics (RNA-seq, scRNA-seq)| 3-25 GB |
| Imaging (microscopy) | 2-8 MB |
| Imaging (human medical) | 1 MB – 2.5 GB |
| Flow cytometry |	1-50 MB |
| Proteomics | 3-5 MB |
| Clinical trials | 2-25 MB |


<img src="resources/images/02-data_management_plan_files/figure-html//1luFoDzF6aDJEebbL6iWoJ_s8s9nQnaWLL5jghbmWdak_g18159f1730a_67_0.png" alt="A cell phone with 64GB of storage can fit 1 WGS file, 2 RNA-seq files, 25 imaging files, and thousands of flow cytometry, clinical trial, microscopy, and proteomics files." width="80%" style="display: block; margin: auto;" />

As you can see some of these data types require large data files. These files may quickly add up to require more storage or computing capacity than your laptop (which typically have 250 GB-1 TB of storage)! If you want to learn more about data file sizes check out the [data file size details section](https://hutchdatascience.org/NIH_Data_Sharing/data-file-size-details.html) of the appendix and this class on [Computing for Cancer Informatics](https://jhudatascience.org/Computing_for_Cancer_Informatics/index.html) from the [Informatics Technology for Cancer Research (ITCR)](https://itcr.cancer.gov/) [Training Network (ITN)](https://www.itcrtraining.org/) for options on how to manage large data files.

## Data Repositories


<div class = "question">
Where will I share my data? What repositories exist that might work for my data type?
</div>

Some programs or Funding Opportunity Announcements (FOA) will specify where the data should be shared. If this applies, you should plan to use the repositories mentioned in the FOA. 

Other programs or FOAs will not specify where the data should be shared, however the NIH provides an [interactive table of NIH-supported data repositories](https://sharing.nih.gov/data-management-and-sharing-policy/sharing-scientific-data/repositories-for-sharing-scientific-data) to help you identify repositories that might be appropriate for your data. 

<img src="resources/images/02-data_management_plan_files/figure-html//1luFoDzF6aDJEebbL6iWoJ_s8s9nQnaWLL5jghbmWdak_g18159f1730a_67_39.png" alt="The interactive table provided by NIH can help you find an appropriate repository." width="80%" style="display: block; margin: auto;" />

If you don't find a repository there, additional repositories can also be found at the following links:

- [Open NIH-supported domain-specific repositories](https://www.nlm.nih.gov/NIHbmic/domain_specific_repositories.html)
- [Other NIH-supported domain-specific resources](https://www.nlm.nih.gov/NIHbmic/other_data_resources.html)
- [Nature data sharing resources](https://www.nature.com/sdata/policies/repositories)
- [Registry of research data repositories](https://www.re3data.org/)

Researchers should aim to find repository with the following characteristics according to the NIH:



- **Established**: If the repository is established (well-known or has been around for a significant period of time), it is likely to improve the FAIRness [@wilkinson_citation_2016] of the data. 
- **Specific**: Repositories that are discipline or data-type specific should be prioritized to promote reuse.
- **Unique Persistent Identifiers**: Assigns datasets a citable, unique persistent identifier, such as a digital object identifier (DOI) or accession number, to support data discovery, reporting, and research assessment. The identifier points to a persistent landing page that remains accessible even if the dataset is de-accessioned or no longer available.
- **Long-Term Sustainability**: Has a plan for long-term management of data, including maintaining integrity, authenticity, and availability of datasets; building on a stable technical infrastructure and funding plans; and having contingency plans to ensure data are available and maintained during and after unforeseen events.
- **Metadata**: Ensures datasets are accompanied by metadata to enable discovery, reuse, and citation of datasets, using schema that are appropriate to, and ideally widely used across, the community/communities the repository serves. Domain-specific repositories would generally have more detailed metadata than generalist repositories.
- **Curation and Quality Assurance**: Provides, or has a mechanism for others to provide, expert curation and quality assurance to improve the accuracy and integrity of datasets and metadata.
- **Free and Easy Access**: Provides broad, equitable, and maximally open access to datasets and their metadata free of charge in a timely manner after submission, consistent with legal and ethical limits required to maintain privacy and confidentiality, Tribal sovereignty, and protection of other sensitive data.
- **Broad and Measured Reuse**: Makes datasets and their metadata available with broadest possible terms of reuse; and provides the ability to measure attribution, citation, and reuse of data (i.e., through assignment of adequate metadata and unique identifiers).
- **Clear Use Guidance**: Provides accompanying documentation describing terms of dataset access and use (e.g., particular licenses, need for approval by a data use committee).
- **Security and Integrity**: Has documented measures in place to meet generally accepted criteria for preventing unauthorized access to, modification of, or release of data, with levels of security that are appropriate to the sensitivity of data.
- **Confidentiality**: Has documented capabilities for ensuring that administrative, technical, and physical safeguards are employed to comply with applicable confidentiality, risk management, and continuous monitoring requirements for sensitive data (should your data require such safeguards).
- **Common Format**: Allows datasets and metadata downloaded, accessed, or exported from the repository to be in widely used, preferably non-proprietary, formats consistent with those used in the community/communities the repository serves.
- **Provenance**: Has mechanisms in place to record the origin, chain of custody, and any modifications to submitted datasets and metadata.
- **Retention Policy**: Provides documentation on policies for data retention within the repository.



## Considerations for Human Data

When working with human participant data, including de-identified human data, here are some additional characteristics to look for:

- **Fidelity to Consent**: Uses documented procedures to restrict dataset access and use to those that are consistent with participant consent and changes in consent.
- **Restricted Use Compliant**: Uses documented procedures to communicate and enforce data use restrictions, such as preventing reidentification or redistribution to unauthorized users.
- **Privacy**: Implements and provides documentation of measures (for example, tiered access, credentialing of data users, security safeguards against potential breaches) to protect human subjects data from inappropriate access.
- **Plan for Breach**: Has security measures that include a response plan for detected data breaches.
- **Download Control**: Controls and audits access to and download of datasets (if download is permitted).
- **Violations**: Has procedures for addressing violations of terms-of-use by users and data mismanagement by the repository.
- **Request Review**: Makes use of an established and transparent process for reviewing data access requests.


<div class = "dictionary">
**Data FAIRness**

Data that is **Findable**, **Accessible**, **Interoperable**, and **Reusable**. For more information about data FAIRness, check out this [manuscript](https://www.nature.com/articles/sdata201618) by @wilkinson_citation_2016.

In brief, it is described by the [NIH](https://datascience.nih.gov/sites/default/files/NIH_Strategic_Plan_for_Data_Science_Final_508.pdf) as follows:

- To be Findable, data must have unique identifiers, effectively
labeling it within searchable resources.
- To be Accessible, data must be easily retrievable via open systems
and effective and secure authentication and authorization
procedures.
-  To be Interoperable, data should “use and speak the same
language” via use of standardized vocabularies.
- To be Reusable, data must be adequately described to a new user,
have clear information about data-usage licenses, and have a
traceable “owner’s manual,” or provenance.

</div>


## No Existing Repository?
<div class = "question">
What if I can't find an appropriate repository? 
</div>

- **Supplemental material** - If the data are small (less than 2 GB), it may be included as supplemental material for an article. See [here](https://www.ncbi.nlm.nih.gov/pmc/about/guidelines/#suppm) for more information. 

- **Institutional repositories** - Check to see if your institute has a repository where you could publicly share the data
- **[Generalist repositories](https://www.nlm.nih.gov/NIHbmic/generalist_repositories.html)**- Host your data somewhere that hosts different types of data publicly, such as:

    - [Dataverse](https://dataverse.org/)
    - [Dryad](https://datadryad.org/)
    - [Figshare](https://figshare.com/)
    - [IEEE Dataport](https://ieee-dataport.org/)
    - [Mendeley Data](https://data.mendeley.com/)
    - [Open Science Framework](https://osf.io/)
    - [Synapse](https://www.synapse.org/)
    - [Vivli](https://vivli.org/)
    - [Zenodo](https://zenodo.org/)
    
Note that the NIH encourages that an existing data sharing repository be used whenever one is available instead of one of these options.

<img src="resources/images/02-data_management_plan_files/figure-html//1luFoDzF6aDJEebbL6iWoJ_s8s9nQnaWLL5jghbmWdak_g18159f1730a_44_28.png" alt="NIH prefers you to use the explicitly mentioned repository, followed by a known, FAIR repository, followed by a public generalist repository for data storage." width="80%" style="display: block; margin: auto;" />

## Summary

The following links can help you find a data repository for your data: 

- [Interactive table of NIH-supported data repositories](https://sharing.nih.gov/data-management-and-sharing-policy/sharing-scientific-data/repositories-for-sharing-scientific-data) *Start here!*
- [Open NIH-supported domain-specific repositories](https://www.nlm.nih.gov/NIHbmic/domain_specific_repositories.html)
- [Other NIH-supported domain-specific resources](https://www.nlm.nih.gov/NIHbmic/other_data_resources.html)
- [Nature data sharing resources](https://www.nature.com/sdata/policies/repositories)
- [Registry of research data repositories](https://www.re3data.org/)

If you don't find an appropriate repository for your data type:

- Consider adding your data as a supplementary file to a manuscript if it is small
- Consider an institutional repository
- Check out the [generalist repositories](https://www.nlm.nih.gov/NIHbmic/generalist_repositories.html)
