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

## General

* [Google search](https://scholar.google.ch/scholar?q=%22we+used+*+data%22+OR+%22we+used+*+dataset%22+OR+%22we+used+*+database%22+OR+%28data+AND+%28reused+OR+reuse%29%29+OR+%22data+*+used%22+OR+%22dataset+*+used%22+OR+%22database+*+used%22&btnG=&hl=en&as_sdt=0%2C5)
* [Data reuse stories](https://www.slideshare.net/VarshaKhodiyar/gaining-credit-for-sharing-research-data/37)
  - all examples given are from Scientific Data
* [The (Re)usable Data Project](http://reusabledata.org/)

## Klosneuviruses

* [From the abstract](https://doi.org/10.1126/science.aal4657):

> Examining the genomes within a sample from a wastewater treatment plant in Austria, Schulz et al. assembled a previously undiscovered giant virus genome, which they used to mine genetic databases for related viruses.

> Here we report the discovery of a group of giant viruses (Klosneuviruses) in metagenomic data.

* [background](http://www.sciencemag.org/news/2017/04/giant-viruses-found-austrian-sewage-fuel-debate-over-potential-fourth-domain-life)

## Diffuse intrinsic pontine glioma

* From the abstract of [Integrated Molecular Meta-Analysis of 1,000 Pediatric High-Grade and Diffuse Intrinsic Pontine Glioma](https://doi.org/10.1016/j.ccell.2017.08.017) (emphasis added):
  - > We collated data from 157 unpublished cases of pediatric high-grade glioma and diffuse intrinsic pontine glioma and **20 publicly available datasets** in an integrated analysis of >1,000 cases. We identified co-segregating mutations in histone-mutant subgroups including loss of FBXW7 in H3.3G34R/V, TOP3A rearrangements in H3.3K27M, and BCOR mutations in H3.1K27M. Histone wild-type subgroups are refined by the presence of key oncogenic events or methylation profiles more closely resembling lower-grade tumors. Genomic aberrations increase with age, highlighting the infant population as biologically and clinically distinct. Uncommon pathway dysregulation is seen in small subsets of tumors, further defining the molecular diversity of the disease, opening up avenues for biological study and providing a basis for functionally defined future treatment stratification.

## H1N1 viral sequences

* From the abstract of [Novel antigenic shift in HA sequences of H1N1 viruses detected by big data analysis](https://doi.org/10.1016/J.MEEGID.2017.03.028) (emphasis added):
  - > The influenza virus H1N1 has been prevalent all over the world for nearly a century. Many studies on its evolutionary history, substitution rate and antigenicity-associated sites have been done with small datasets. To have a complete view, we analysed **3171 full-length HA sequences from human H1N1 viruses sampled from 1918 to 2016**, and discovered a new clade has formed with sequences isolated in Iran. 

## Visualization of wind speeds in an area

* https://twitter.com/blueraster/status/1168933523924889603
  - intended for monitoring fires but can be used for [monitoring hurricanes as well](https://fires.globalforestwatch.org/map/?utm_content=buffer5d41c&utm_medium=social&utm_source=twitter.com&utm_campaign=buffer#activeLayers=windDirection&activeBasemap=dark-gray&activeImagery=&planetCategory=PLANET-MONTHLY&planetPeriod=Jan%200000&x=-78.986206&y=27.139501&z=7)

## JATS
[PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/) (PMC) is a repository for scholarly literature in the biomedical field. Some of its content is available under terms that allow for [Reusing, Revising, Remixing and Redistributing Research](http://blogs.plos.org/blog/2012/10/23/reusing-revising-remixing-and-redistributing-research/), e.g. to extract audio and video materials from these articles and upload them to Wikimedia Commons, as the [Open Access Media Importer](http://commons.wikimedia.org/wiki/User:Open_Access_Media_Importer_Bot) does. 

The bot's activity has revealed a number of [inconsistencies in the XML at PMC](https://en.wikipedia.org/wiki/User:Daniel_Mietchen/Talks/JATS-Con_2014/Inconsistent_XML_as_a_Barrier_to_Reuse_of_Open_Access_Content), since the XML standard in use at PMC ([JATS](http://jats.nlm.nih.gov/)) is by design not very prescriptive and leaves lots of room for interpretation.

This sparked the formation of the [JATS for Reuse](https://github.com/jats4r) (JATS4R) Working Group that now 
elaborates recommendations on how best to tag articles in JATS, so as to facilitate reuse ([overview](http://www.ncbi.nlm.nih.gov/books/NBK279901/)).

### Improving reusability
* adopting [JATS4R recommendations](http://jats4r.github.io/#tag-recs)
  - Background: 
    - [Inconsistent XML as a Barrier to Reuse of Open Access Content](http://www.ncbi.nlm.nih.gov/books/NBK159964/)
    - [Improving the reusability of JATS](http://www.ncbi.nlm.nih.gov/books/NBK279901/)
* providing [high-res images via API](https://github.com/wpoa/JATS-to-Mediawiki/issues/20#issuecomment-47401660)
* making the ingestion XSLT and schematrons public (and under an open license)
  - probably useful for PMC partner repositories (think PMC International but also SciELO or NASA)
  - [useful to publishers](https://twitter.com/invisiblecomma/status/579980606601318400)
  - [useful for Wikimedia](https://github.com/wpoa/JATS-to-Mediawiki)
* [search by license](http://www.ncbi.nlm.nih.gov/pmc/tools/openftlist/) via the [OA webservices API](http://www.ncbi.nlm.nih.gov/pmc/tools/oa-service/)
* more fine-grained search, e.g. for [supplementary video or audio files](http://www.ncbi.nlm.nih.gov/pmc/?term=(%22supplementary+material%22)+AND+(audio+OR+movie+OR+sound+OR+video+OR+animation))
* help standardize the implementation of data citation as per JATS 1.1d2 (cf. [JATS-Con paper](http://www.ncbi.nlm.nih.gov/books/NBK280240/))
* JATS is one of the suggested metadata formats in NISO's [Protocol for Exchanging Serial Content (PESC)](http://www.niso.org/workrooms/pesc/)

## Stats  
* [Page views of medical pages on the English Wikipedia](https://en.wikipedia.org/wiki/Wikipedia:WikiProject_Medicine/Popular_pages)  
* GLAMorous
  - [Open Access Media Importer](http://tools.wmflabs.org/glamtools/glamorous.php?doit=1&category=Uploaded+with+Open+Access+Media+Importer)
    - [NIH](http://tools.wmflabs.org/glamtools/glamorous.php?doit=1&category=National+Institutes+of+Health&use_globalusage=1&ns0=1&depth=20&show_details=1&projects[wikipedia]=1&projects[wikimedia]=1&projects[wikisource]=1&projects[wikibooks]=1&projects[wikiquote]=1&projects[wiktionary]=1&projects[wikinews]=1&projects[wikivoyage]=1&projects[wikispecies]=1&projects[mediawiki]=1&projects[wikidata]=1&projects[wikiversity]=1)
* BaGLAMa
  - [Open Access Media Importer](http://tools.wmflabs.org/glamtools/baglama2/#gid=129&month=201502)  
    - [NIH](http://tools.wmflabs.org/glamtools/baglama2/#gid=201&month=201504&giu=enwiki&server=en.wikipedia.org)
* [Cite-o-Meter](http://tools.wmflabs.org/cite-o-meter/)  
* [Cocytus](http://events.labs.crossref.org/events/types/WikipediaCitation)  
* [Total DOIs cited from the English Wikipedia](https://dx.doi.org/10.6084/m9.figshare.1299540)  

## Wikimedia Commons
* [Category:PD US NIH](https://commons.wikimedia.org/wiki/Category:PD_US_NIH)
  - [Example](https://commons.wikimedia.org/wiki/File:Metastatic_Melanoma_Cells_Nci-vol-9872-300.jpg) from [NCI Visuals](https://visualsonline.cancer.gov/browseaction.cfm?entrydate=newest) 

## OPENi
* [OPENi](http://openi.nlm.nih.gov/faq.php?it=xg) is a searchable collection of images from PubMed Central and other sources

## ImageJ
* [ImageJ](http://imagej.nih.gov/ij/) is a widely used software package for visualizing and analyzing biomedical data.
  - [on Google Scholar](http://scholar.google.co.uk/scholar?hl=en&q=ImageJ&btnG=&as_sdt=1%2C5&as_sdtp=)
  - [on Wikimedia Commons](https://commons.wikimedia.org/wiki/Category:ImageJ)
  - [BoneJ](http://bonej.org/)
    - [BoneJ: free and extensible bone image analysis in ImageJ](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3193171/)
  - [Fiji](https://github.com/fiji/fiji/)
  - [Other ImageJ-based software](http://rsb.info.nih.gov/ij/links.html)

## British Library's Mechanical Curator collection
* [UKSG 2015 Mechanical curator and British Library labs](http://www.slideshare.net/benosteen/uksg-2015-mechanical-curator-and-british-library-labs)
  - contains overview of use and reuse of the collection

## Data Documentation Initiative
* ["A metadata specification for the social and behavioral sciences"](http://www.ddialliance.org/)
* ["an effort to create an international standard in XML for metadata describing social science data"](http://www.ddialliance.org/alliance)

## Te Papa Tongarewa/ Museum of New Zealand
* [Reusing Te Papa’s collections images, by the numbers](http://blog.tepapa.govt.nz/2015/04/10/reusing-te-papas-collections-images-by-the-numbers/)
  - qualitative and quantitative indications of reuse, e.g.
    - [“Uploading to wikimedia and wikipedia article”](http://collections.tepapa.govt.nz/Object/1439306) (no known copyright restrictions)
      - [Download page asking for intended reuse](http://collections.tepapa.govt.nz/Object/1439306/download)
      - [that Wikipedia article](https://en.wikipedia.org/wiki/John_Buchanan_%28botanist%29)
    - [“I knit, and would love to make this into a knitting pattern…”](http://collections.tepapa.govt.nz/Object/711029) (item is NC-ND-licensed)
    - [GitHub repo](https://github.com/te-papa/image-downloads-stats)

# Repurposed media files
* [Wikimedia Commons as a media source](https://commons.wikimedia.org/wiki/Category:Commons_as_a_media_source)
* Fig. 5 of [Three-dimensional Magnetic Resonance Imaging of fossils across taxa](https://doi.org/10.5194/bg-5-25-2008) (CC BY) is reused in final figure of [NMR Studies of Fossilized Wood](http://dx.doi.org/10.1016/bs.arnmr.2016.07.002) (paywalled)
* [File:Ernst-Abbe-Denkmal Jena Fürstengraben - 20140802 125709.jpg](https://commons.wikimedia.org/wiki/File:Ernst-Abbe-Denkmal_Jena_F%C3%BCrstengraben_-_20140802_125709.jpg) (CC0) reused in [Cell imaging: Beyond the limits](http://dx.doi.org/10.1038/526S50a) (paywalled)
* [Deletion discussion of a video due to deletions of images that had been used in the video](https://commons.wikimedia.org/wiki/Commons:Deletion_requests/File:Wikipedia_Edit_2014.webm)

# See also
* [Pop Culture Pulsar: Origin Story of Joy Division’s Unknown Pleasures Album Cover](https://blogs.scientificamerican.com/sa-visual/pop-culture-pulsar-origin-story-of-joy-division-s-unknown-pleasures-album-cover-video/)
* [If We Share Data, Will Anyone Use Them? Data Sharing and Reuse in the Long Tail of Science and Technology]( http://dx.doi.org/10.1371/journal.pone.0067332)
* [Public Domain Status for Publicly Funded Works in the EU](https://meta.wikimedia.org/wiki/EU_policy/Issues_overview#Public_Domain_Status_for_Publicly_Funded_Works)
* [NIH 3D Print Exchange](http://3dprint.nih.gov/)
* reuse biographic info from ORCID to start an NIH Biosketch
* PMC Europe has entity recognition tools and uses them to mine its corpus for identifiers from around 20 databases
* Atul Butte's work
  - e.g. [in his talk at NIH in June 2015](http://videocast.nih.gov/summary.asp?Live=16267&bhcp=1)
* [Drug repositioning](https://en.wikipedia.org/wiki/Drug_repositioning)
  - [dedicated conference](http://www.drugrepositioningconference.com/)
  - NCATS [New Therapeutic Uses program](http://www.ncats.nih.gov/ntu)
* [“Open” disclosure of innovations, incentives and follow-on reuse: Theory on processes of cumulative innovation and a field experiment in computational biology](http://dx.doi.org/10.1016/j.respol.2014.08.001)
* Library usage records as a way to track usage
* ["using text mining to track how the museum's 80-million-specimen collection is used in research papers'](http://dx.doi.org/10.1038/523115a)
* [NIH Data Sharing Repositories](http://www.nlm.nih.gov/NIHbmic/nih_data_sharing_repositories.html) &mdash; "This table lists NIH-supported data repositories that make data accessible for reuse."
* Think about tracking reuse of software libraries
  - [Reuse metrics](https://en.wikipedia.org/wiki/Reuse_metrics)
  - [Code reuse](https://en.wikipedia.org/wiki/Code_reuse)
  - [Code reusability principles](https://en.wikipedia.org/wiki/Reusability)
  - [Why Software Reuse has Failed and How to Make It Work for You](http://www1.cse.wustl.edu/~schmidt/reuse-lessons.html)
  - [Java's top 20: The most used Java libraries on GitHub](http://www.javaworld.com/article/2924315/open-source-tools/javas-top-20-the-most-used-java-libraries-on-github.html)
  - [What's the Most Popular Ruby Library?](http://omniref.com/blog/blog/2014/07/23/whats-the-most-used-ruby-library/)
  - [What are the top 10 most useful and influential Python libraries and frameworks?](http://www.quora.com/What-are-the-top-10-most-useful-and-influential-Python-libraries-and-frameworks)
* [Public Domain Protection: Uses and Reuses of Public Domain Works](http://copy-me.org/2015/08/public-domain-protection-uses-and-reuses-of-public-domain-works/)
* [On the formalization and reuse of scientific research](http://dx.doi.org/10.1098/rsif.2011.0029)
* [Open Data and Data Re-use](http://pro.europeana.eu/get-involved/europeana-tech/europeanatech-insight/issue-3-open-data-and-data-re-use)
* [10 Simple rules for design, provision, and reuse of persistent identifiers for life science data](http://dx.doi.org/10.5281/zenodo.18003)
* [open data as a form of OER](http://education.okfn.org/the-21st-centurys-raw-material-using-open-data-as-open-educational-resources/)
* [Planning for Data Reuse Checklist](http://mozillascience.github.io/checklist/)
* [A century of trends in adult human height](http://dx.doi.org/10.7554/eLife.13410)
  - reuses 1472 datasets
* SciDataCon 2016 session [Data fitness: What are the processes and components to assess and communicate re-usability of data?](http://www.scidatacon.org/2016/sessions/53/)
* Robotics in general
* [Whole genome resequencing of a laboratory-adapted Drosophila melanogaster population sample](http://dx.doi.org/10.1101/081554 )
* [407 publications used GBIF data in 2015](https://twitter.com/vsmithuk/status/788867195258429440) (as per the [GBIF Science Review 2016](http://www.gbif.org/resource/82873))
* [http://plos.io/allofplos](http://plos.io/allofplos) (3.9GB zip)
* [Raw diffraction data preservation and reuse: overview, update on practicalities and metadata requirements](https://doi.org/10.1107/S2052252516018315)
* [Measurement of the Earth's rotation: 720 BC to AD 2015](https://doi.org/10.1098/rspa.2016.0404)
  - reuses astronomical data recorded on Babylonian clay tables
* [1970s and ‘Patient 0’ HIV-1 genomes illuminate early HIV/AIDS history in North America](https://doi.org/10.1038/nature19827)
  - reused blood samples to sequence patient genomes to analyze the spread of HIV
* [Reilly Center's annual Top 10 List of Ethical Dilemmas and Policy Issues in Science and Technology](http://reilly.nd.edu/top10/)
  - [reused in Spanish class at Massachusetts high school](https://www.youtube.com/watch?v=cMdxxRoha0M)
* [The Sharing Experimental Animal Resources, Coordinating Holdings (SEARCH) Framework: Encouraging Reduction, Replacement, and Refinement in Animal Research](http://dx.doi.org/10.1371/journal.pbio.2000719)
* [reCAPTCHA](https://en.wikipedia.org/wiki/ReCAPTCHA)
* [Why Are Scientific Data Rarely Reused?](https://works.bepress.com/borgman/272/)
* [Australian National Data Service: Data Impact Book](http://doi.org/10.4225/14/588ed360036eb)
* [UK DataService: Case Studies](https://impact.ukdataservice.ac.uk/case-studies)
* [Drug repurposing/drug repositioning](https://en.wikipedia.org/wiki/Drug_repositioning)
* [2016 dataset usage stats at Dryad](https://blog.datadryad.org/2017/03/14/and-now-the-numbers/)
* ["This is what #OpenScience is all about. A team in France used our data to build The Virtual Mouse Brain. Great work!"](https://twitter.com/Allen_Institute/status/851921617940774914)
* EU action [Promoting sharing and reuse of IT solutions](https://ec.europa.eu/isa2/actions/promoting-sharing-and-reuse-interoperability-solutions_en)
  - [Sharing and Reuse Awards](https://ec.europa.eu/isa2/awards_en) &mdash; for shared IT solutions in public administration
* [How is Open Data being re-used in Europe?](https://www.europeandataportal.eu/en/highlights/how-open-data-being-re-used-europe)
* [Communicating Use and Reuse in the Digital Collection Interface](https://medium.com/berkman-klein-center/communicating-use-and-reuse-in-the-digital-collection-interface-434d970c4d38) &mdash; on reuse policies at various GLAM institutions
* [University of Oklahoma Astrophysicists Discover Extragalactic Planets for First Time](http://www.ou.edu/web/news_events/articles/news_2018/ou-discover-planets.html) &mdash; based on open data from NASA's Chandra X-ray Observatory
* [Crowdsourcing 600 Years of Human History](https://directorsblog.nih.gov/2018/03/13/crowdsourcing-600-years-of-human-history/) &mdash; uses family-level genealogy data to analyze population-level history
* [Reusing photos from INaturalist to study goat molt](https://www.inaturalist.org/blog/16807-mountain-goat-molts-inat-photos-and-climate-change)
* [Global Infections by the Numbers](https://www.scientificamerican.com/article/global-infections-by-the-numbers/) &mdash; journalistic infographic reusing data from various sources
* [Data use Ontology](https://www.ga4gh.org/news/now-open-for-comment-ga4gh-data-use-ontology/)
* [Reanalyzing environmental lidar data for archaeology: Mesoamerican applications and implications](https://doi.org/10.1016/j.jasrep.2016.07.029)
