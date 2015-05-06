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

## Stats  
* [Page views of medical pages on the English Wikipedia](https://en.wikipedia.org/wiki/Wikipedia:WikiProject_Medicine/Popular_pages)  
* [GLAMorous](http://tools.wmflabs.org/glamtools/glamorous.php?doit=1&category=Uploaded+with+Open+Access+Media+Importer)  
* [BaGLAMa](http://tools.wmflabs.org/glamtools/baglama2/#gid=129&month=201502)  
* [Cite-o-Meter](http://tools.wmflabs.org/cite-o-meter/)  
* [Cocytus](http://events.labs.crossref.org/events/types/WikipediaCitation)  
* [Total DOIs cited from the English Wikipedia](https://dx.doi.org/10.6084/m9.figshare.1299540)  

## Wikimedia Commons
* [Category:PD US NIH](https://commons.wikimedia.org/wiki/Category:PD_US_NIH)
      * [Example](https://commons.wikimedia.org/wiki/File:Metastatic_Melanoma_Cells_Nci-vol-9872-300.jpg) from [NCI Visuals](https://visualsonline.cancer.gov/browseaction.cfm?entrydate=newest) 

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
