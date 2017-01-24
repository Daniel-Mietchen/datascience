# About
The US [National Library of Medicine (NLM)](https://github.com/Daniel-Mietchen/datascience/blob/master/nih-strategic-plan.md) at the National Institutes of Health (NIH) is [requesting information](https://grants.nih.gov/grants/guide/notice-files/NOT-LM-17-002.html) in relation to the strategic plan it is developing. This builds on a set of broad recommendations for the future of NLM that were compiled in a [2015 report](https://acd.od.nih.gov/reports/Report-NLM-06112015-ACD.pdf).

This file contains the free-text parts of my response to the Request for Information. Along with requesting some metadata, the form asked the following questions (**in bold**) and provided additional comments above each form field (which I have set *in italics* here).


**Please provide input on topics within any or all of the four themes below.**

**1)  Role of NLM in advancing data science, open science, and biomedical informatics**

*Identify what you consider an audacious goal in this area – a challenge that may be daunting but would represent a huge leap forward were it to be achieved.  Include any proposals for the steps and elements needed to reach that goal.*

- There are a number of audacious goals listed in the [report on the strategic vision for the National Library of Medicine](http://acd.od.nih.gov/reports/Report-NLM-06112015-ACD.pdf), which recommends that NLM should
       - "be a leader and innovator in open science efforts worldwide"
       - "lead efforts to support and catalyze open science, data sharing, and research reproducibility, striving to promote the concept that biomedical information and its transparent analysis are public"
       - and, in particular, "lead efforts to promulgate and implement best practices in open source, open science, standards, and data harmonization, forming partnerships across communities, stakeholder organizations, agencies, and countries" as well as "be an active participant in the design and oversight of programs that incentivize and celebrate the open sharing of data and resources."

While I think it would make sense for NIH as a whole to "be a leader and innovator in open science efforts worldwide", I can see why NLM would be well-positioned to take a lead on this within NIH.

A good example on how this might look like in practice is the Human Genome Project: the availability of infrastructure like [GenBank](https://www.ncbi.nlm.nih.gov/genbank/) and its international partners was crucial for implementing the [Bermuda Principles](http://web.ornl.gov/sci/techresources/Human_Genome/research/bermuda.shtml) of sharing data as soon as they arise, rather than after unnecessary delays caused by outdated assessment systems. 

What we need here are similar strides in fields other than human genomics as well (PubMed Central does it to some extent, but only after the above-mentioned delays, plus additional embargo periods). Providing the relevant infrastructure is necessary but not sufficient, with the biggest hurdles being cultural and sociological in nature.

Here, it is crucial to provide room for experimentation with open science, keeping in mind that there are multiple dimensions to it, e.g.:
  - some researchers versus the community at large
  - some steps along the research cycle versus all of them
  - some of the tools or workflows versus all of them within a given research project
  - some research projects versus all of them within a given scope
  - intramural versus extramural
  - immediate switching versus a long-term transition.
  
Importantly, open science should not be seen as solely the task of researchers &mdash; funders, policy makers and other roles within NIH and NLM have very important roles to play here. For instance, by making the funding process itself more open (e.g. as discussed in http://dx.doi.org/10.1371/journal.pbio.1002027 ) or the process of drafting policies (e.g. as described in https://openscience.ub.uni-bielefeld.de/933/what-can-policy-makers-do-to-encourage-open-science ), they would themselves engage in more openness, become more familiar with the actual challenges of doing so, and earn the respect of others &mdash; including researchers &mdash; who have tried more open ways of working themselves, or are pondering to do so.

*The most important thing NLM does in this area, from your perspective.*

The most important thing here is perhaps that NLM has NCBI (working there, I may well be biased), which serves as a major hub of biomedical data and informatics. This environment is also very fertile in terms of breeding generations of data scientists, albeit it is steadily losing some of this appeal as the prominence of data science is rising in other parts of society, and most of the software behind the infrastructure provided by NCBI is not open.

*Research areas that are most critical for NLM to conduct or support.*

- What are the conditions under which open science is more or less efficient than the traditional way of sharing research?
- How can data-related infrastructure be made sustainable?

*Other comments, suggestions, or considerations, keeping in mind that the aim is to build the NLM of the future.*

**2) Role of NLM in advancing biomedical discovery and translational science**

*Identify what you consider an audacious goal in this area – a challenge that may be daunting but would represent a huge leap forward were it to be achieved.  Include input on the barriers to and benefits of achieving the goal.*

*The most important thing NLM does in this area, from your perspective.*

*Research areas that are most critical for NLM to conduct or support.*

*Other comments, suggestions, or considerations, keeping in mind that the aim is to build the NLM of the future.*

**3) Role of NLM in supporting the health of nation: clinical systems, public health systems and services, personal health**

*Identify what you consider an audacious goal in this area – a challenge that may be daunting but would represent a huge leap forward were it to be achieved.  Include input on the barriers to and benefits of achieving the goal.*

*The most important thing NLM does in this area, from your perspective.*

*Research areas that are most critical for NLM to conduct or support.*

*Healthcare systems and public health arenas in which NLM participation is most critical.*

*Other comments, suggestions, or considerations, keeping in mind that the aim is to build the NLM of the future.*

**4) Role of NLM in building collections to support discovery and health in the 21st century**

*Identify what you consider an audacious goal in this area – a challenge that may be daunting but would represent a huge leap forward were it to be achieved.  Include input on the barriers to and benefits of achieving the goal.*

- Make all metadata of all NLM collections publicly available in a way that is friendly to both humans and machines.
- Digitize the collections to the extent feasible, allowing for community feedback on prioritization.
- Make the digital collections publicly available to the extent possible (e.g. taking into account privacy or copyright restrictions).
- Be clear about reuse rights &mdash; express them in ways that both humans and machines can easily parse.
- Invite crowd contributions in annotating the digital collections and improving their metadata.

*The most important thing NLM does in this area, from your perspective.*
- Building and maintaining collections relevant to medicine.

What is missing is a closer integration of the collection materials into research workflows.

*Research areas that are most critical for NLM to conduct or support.*
- So far, the role of NLM in terms of collections has mainly been focused on preserving the materials, and everyone who wanted to extract information from the materials would basically have to do it on their own, from scratch. It would be very useful if NLM could proactively (think [PubTator](https://www.ncbi.nlm.nih.gov/CBBresearch/Lu/Demo/PubTator/) here) extract data from materials in its collections and make it available in usable formats and in places where people or machines might actually find it.
- This is especially important for materials that encapsulate unique data that cannot be easily replicated.

*New data types or data collections anticipated over the next 10 years.*
- As the diversity of research workflows and outputs keeps increasing, new opportunities open up to mine, reproduce, remix and otherwise reuse them to extract data, information or knowledge. NLM should facilitate such reproducibility and reuse and assist with their standardization, e.g. by keeping records and workflows of what has been mined before (think [PubRunner](http://pubrunner.org/)).
- Traditionally, scholarly communication has focused much on the results of the research process. With the ongoing shift to open science, the importance of the research process itself will grow, and this should be reflected in the collections. For example, software repositories, data management plans or open lab notebooks might be collected, along with annotations and other contributions from both the original authors and others.

*Other comments, suggestions, or considerations, keeping in mind that the aim is to build the NLM of the future.*
- A copy of my response is available via [https://github.com/Daniel-Mietchen/datascience/blob/master/nih-strategic-plan.md](https://github.com/Daniel-Mietchen/datascience/blob/master/nih-strategic-plan.md), which is public and can be updated. I am also keeping a public collection of thoughts on what individual stakeholders in the research process can do to advance open science, which can be found at [https://openscience.ub.uni-bielefeld.de/tag/stakeholders](https://openscience.ub.uni-bielefeld.de/tag/stakeholders).

# See also
- My [response](https://github.com/Daniel-Mietchen/datascience/blob/master/nih-strategic-plan.md) to a similar Request for Information regarding the Strategic Plan of NIH as a whole.
