# About 
This file serves to collect thoughts on how to stimulate the reuse of open data, and on how to quantify such reuse. Reuse is to be understood here as non-primary use, i.e. use in a way that was not the primary purpose of collecting the respective data. [This blog post](http://clintlalonde.net/2014/01/16/building-knowledge-tools-for-the-public-good/) considers some of the conditions that have to be met for reuse to happen, and the importance of generativity in the systems involved. Another blog post [highlighted](http://abject.ca/syndication-and-content/)  
> Open tools, open media, and syndication  

as key factors on how to achieve that. There are others, and the precise mixture probably depends much on context.

# Research questions
* How are research objects being used?
* What kinds of reuses are there?
* What are useful ways to track these kinds of reuses?
* How is reuse distributed over time, space, discipline, application sector, user populations, operating systems?
* How can reuse be encouraged?

# Examples
## JATS
[PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/) (PMC) is a repository for scholarly literature in the biomedical field. Some of its content is available under terms that allow for [Reusing, Revising, Remixing and Redistributing Research](http://blogs.plos.org/blog/2012/10/23/reusing-revising-remixing-and-redistributing-research/), e.g. to extract audio and video materials from these articles and upload them to Wikimedia Commons, as the [Open Access Media Importer](http://commons.wikimedia.org/wiki/User:Open_Access_Media_Importer_Bot) does. 

The bot's activity has revealed a number of [inconsistencies in the XML at PMC](https://en.wikipedia.org/wiki/User:Daniel_Mietchen/Talks/JATS-Con_2014/Inconsistent_XML_as_a_Barrier_to_Reuse_of_Open_Access_Content), since the XML standard in use at PMC ([JATS](http://jats.nlm.nih.gov/)) is by design not very prescriptive and leaves lots of room for interpretation.

This sparked the formation of the [JATS for Reuse](https://github.com/jats4r) (JATS4R) Working Group that now 
elaborates recommendations on how best to tag articles in JATS, so as to facilitate reuse ([overview](http://www.ncbi.nlm.nih.gov/books/NBK279901/)).

### Improving reusability
* adopting [JATS4R recommendations](http://jats4r.github.io/#tag-recs)
      * Background: 
           * [Inconsistent XML as a Barrier to Reuse of Open Access Content](http://www.ncbi.nlm.nih.gov/books/NBK159964/)
           * [Improving the reusability of JATS](http://www.ncbi.nlm.nih.gov/books/NBK279901/)
* providing [high-res images via API](https://github.com/wpoa/JATS-to-Mediawiki/issues/20#issuecomment-47401660)
* making the ingestion XSLT and schematrons public (and under an open license)
    * probably useful for PMC partner repositories (think PMC International but also SciELO or NASA)
    * [useful to publishers](https://twitter.com/invisiblecomma/status/579980606601318400)
    * [useful for Wikimedia](https://github.com/wpoa/JATS-to-Mediawiki)
* [search by license](http://www.ncbi.nlm.nih.gov/pmc/tools/openftlist/) via the [OA webservices API](http://www.ncbi.nlm.nih.gov/pmc/tools/oa-service/)
* more fine-grained search, e.g. for [supplementary video or audio files](http://www.ncbi.nlm.nih.gov/pmc/?term=(%22supplementary+material%22)+AND+(audio+OR+movie+OR+sound+OR+video+OR+animation))
* help standardize the implementation of data citation as per JATS 1.1d2 (cf. [JATS-Con paper](http://www.ncbi.nlm.nih.gov/books/NBK280240/))
* JATS is one of the suggested metadata formats in NISO's [Protocol for Exchanging Serial Content (PESC)](http://www.niso.org/workrooms/pesc/)

## Stats  
* [Page views of medical pages on the English Wikipedia](https://en.wikipedia.org/wiki/Wikipedia:WikiProject_Medicine/Popular_pages)  
* GLAMorous
      * [Open Access Media Importer](http://tools.wmflabs.org/glamtools/glamorous.php?doit=1&category=Uploaded+with+Open+Access+Media+Importer)
      * [NIH](http://tools.wmflabs.org/glamtools/glamorous.php?doit=1&category=National+Institutes+of+Health&use_globalusage=1&ns0=1&depth=20&show_details=1&projects[wikipedia]=1&projects[wikimedia]=1&projects[wikisource]=1&projects[wikibooks]=1&projects[wikiquote]=1&projects[wiktionary]=1&projects[wikinews]=1&projects[wikivoyage]=1&projects[wikispecies]=1&projects[mediawiki]=1&projects[wikidata]=1&projects[wikiversity]=1)
* BaGLAMa
      * [Open Access Media Importer](http://tools.wmflabs.org/glamtools/baglama2/#gid=129&month=201502)  
      * [NIH](http://tools.wmflabs.org/glamtools/baglama2/#gid=201&month=201504&giu=enwiki&server=en.wikipedia.org)
* [Cite-o-Meter](http://tools.wmflabs.org/cite-o-meter/)  
* [Cocytus](http://events.labs.crossref.org/events/types/WikipediaCitation)  
* [Total DOIs cited from the English Wikipedia](https://dx.doi.org/10.6084/m9.figshare.1299540)  

## Wikimedia Commons
* [Category:PD US NIH](https://commons.wikimedia.org/wiki/Category:PD_US_NIH)
      * [Example](https://commons.wikimedia.org/wiki/File:Metastatic_Melanoma_Cells_Nci-vol-9872-300.jpg) from [NCI Visuals](https://visualsonline.cancer.gov/browseaction.cfm?entrydate=newest) 

## OPENi
* [OPENi](http://openi.nlm.nih.gov/faq.php?it=xg) is a searchable collection of images from PubMed Central and other sources

## ImageJ
* [ImageJ](http://imagej.nih.gov/ij/) is a widely used software package for visualizing and analyzing biomedical data.
    * [on Google Scholar](http://scholar.google.co.uk/scholar?hl=en&q=ImageJ&btnG=&as_sdt=1%2C5&as_sdtp=)
    * [on Wikimedia Commons](https://commons.wikimedia.org/wiki/Category:ImageJ)
    * [BoneJ](http://bonej.org/)
          * [BoneJ: free and extensible bone image analysis in ImageJ](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3193171/)
    * [Fiji](https://github.com/fiji/fiji/)
    * [Other ImageJ-based software](http://rsb.info.nih.gov/ij/links.html)

## British Library's Mechanical Curator collection
* [UKSG 2015 Mechanical curator and British Library labs](http://www.slideshare.net/benosteen/uksg-2015-mechanical-curator-and-british-library-labs)
     * contains overview of use and reuse of the collection

## Data Documentation Initiative
* ["A metadata specification for the social and behavioral sciences"](http://www.ddialliance.org/)
* ["an effort to create an international standard in XML for metadata describing social science data"](http://www.ddialliance.org/alliance)

## Te Papa Tongarewa/ Museum of New Zealand
* [Reusing Te Papa’s collections images, by the numbers](http://blog.tepapa.govt.nz/2015/04/10/reusing-te-papas-collections-images-by-the-numbers/)
     * qualitative and quantitative indications of reuse, e.g.
          * [“Uploading to wikimedia and wikipedia article”](http://collections.tepapa.govt.nz/Object/1439306) (no known copyright restrictions)
               * [Download page asking for intended reuse](http://collections.tepapa.govt.nz/Object/1439306/download)
               * [that Wikipedia article](https://en.wikipedia.org/wiki/John_Buchanan_%28botanist%29)
          * [“I knit, and would love to make this into a knitting pattern…”](http://collections.tepapa.govt.nz/Object/711029) (item is NC-ND-licensed)
     * [GitHub repo](https://github.com/te-papa/image-downloads-stats)

# See also
* [Public Domain Status for Publicly Funded Works in the EU](https://meta.wikimedia.org/wiki/EU_policy/Issues_overview#Public_Domain_Status_for_Publicly_Funded_Works)
* [NIH 3D Print Exchange](http://3dprint.nih.gov/)
* reuse biographic info from ORCID to start an NIH Biosketch
* PMC Europe has entity recognition tools and uses them to mine its corpus for identifiers from around 20 databases
* Atul Butte's work
      * e.g. [in his talk at NIH in June 2015](http://videocast.nih.gov/summary.asp?Live=16267&bhcp=1)
* [Drug repositioning](https://en.wikipedia.org/wiki/Drug_repositioning)
      * [dedicated conference](http://www.drugrepositioningconference.com/)
      * NCATS [New Therapeutic Uses program](http://www.ncats.nih.gov/ntu)
* [“Open” disclosure of innovations, incentives and follow-on reuse: Theory on processes of cumulative innovation and a field experiment in computational biology](http://dx.doi.org/10.1016/j.respol.2014.08.001)
* Library usage records as a way to track usage
* ["using text mining to track how the museum's 80-million-specimen collection is used in research papers'](http://dx.doi.org/10.1038/523115a)
* [NIH Data Sharing Repositories](http://www.nlm.nih.gov/NIHbmic/nih_data_sharing_repositories.html) &mdash; "This table lists NIH-supported data repositories that make data accessible for reuse."
* Think about tracking reuse of software libraries
      * [Reuse metrics](https://en.wikipedia.org/wiki/Reuse_metrics)
      * [Code reuse](https://en.wikipedia.org/wiki/Code_reuse)
      * [Code reusability principles](https://en.wikipedia.org/wiki/Reusability)
      * [Why Software Reuse has Failed and How to Make It Work for You](http://www1.cse.wustl.edu/~schmidt/reuse-lessons.html)
      * [Java's top 20: The most used Java libraries on GitHub](http://www.javaworld.com/article/2924315/open-source-tools/javas-top-20-the-most-used-java-libraries-on-github.html)
      * [What's the Most Popular Ruby Library?](http://omniref.com/blog/blog/2014/07/23/whats-the-most-used-ruby-library/)
      * [What are the top 10 most useful and influential Python libraries and frameworks?](http://www.quora.com/What-are-the-top-10-most-useful-and-influential-Python-libraries-and-frameworks)
* [Public Domain Protection: Uses and Reuses of Public Domain Works](http://copy-me.org/2015/08/public-domain-protection-uses-and-reuses-of-public-domain-works/)
* [On the formalization and reuse of scientific research](http://dx.doi.org/10.1098/rsif.2011.0029)
* [Open Data and Data Re-use](http://pro.europeana.eu/get-involved/europeana-tech/europeanatech-insight/issue-3-open-data-and-data-re-use)
* [10 Simple rules for design, provision, and reuse of persistent identifiers for life science data](http://dx.doi.org/10.5281/zenodo.18003)
* [open data as a form of OER](http://education.okfn.org/the-21st-centurys-raw-material-using-open-data-as-open-educational-resources/)
* [Planning for Data Reuse Checklist](http://mozillascience.github.io/checklist/)
* [A century of trends in adult human height](http://dx.doi.org/10.7554/eLife.13410)
      * reuses 1472 datasets
* SciDataCon 2016 session [Data fitness: What are the processes and components to assess and communicate re-usability of data?](http://www.scidatacon.org/2016/sessions/53/)
