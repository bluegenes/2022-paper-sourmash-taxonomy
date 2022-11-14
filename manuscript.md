---
title: 'sourmash taxonomy: LCA summarization of genome-resolved taxonomic profiling'
keywords:
- taxonomic profiling
- FracMinHash
- k-mers
- metagenomics
- taxonomy
lang: en-US
date-meta: '2022-11-14'
author-meta:
- N. Tessa Pierce-Ward
- Luiz Irber
- Taylor Reiter
- C. Titus Brown
header-includes: |-
  <!--
  Manubot generated metadata rendered from header-includes-template.html.
  Suggest improvements at https://github.com/manubot/manubot/blob/main/manubot/process/header-includes-template.html
  -->
  <meta name="dc.format" content="text/html" />
  <meta property="og:type" content="article" />
  <meta name="dc.title" content="sourmash taxonomy: LCA summarization of genome-resolved taxonomic profiling" />
  <meta name="citation_title" content="sourmash taxonomy: LCA summarization of genome-resolved taxonomic profiling" />
  <meta property="og:title" content="sourmash taxonomy: LCA summarization of genome-resolved taxonomic profiling" />
  <meta property="twitter:title" content="sourmash taxonomy: LCA summarization of genome-resolved taxonomic profiling" />
  <meta name="dc.date" content="2022-11-14" />
  <meta name="citation_publication_date" content="2022-11-14" />
  <meta property="article:published_time" content="2022-11-14" />
  <meta name="dc.modified" content="2022-11-14T19:17:16+00:00" />
  <meta property="article:modified_time" content="2022-11-14T19:17:16+00:00" />
  <meta name="dc.language" content="en-US" />
  <meta name="citation_language" content="en-US" />
  <meta name="dc.relation.ispartof" content="Manubot" />
  <meta name="dc.publisher" content="Manubot" />
  <meta name="citation_journal_title" content="Manubot" />
  <meta name="citation_technical_report_institution" content="Manubot" />
  <meta name="citation_author" content="N. Tessa Pierce-Ward" />
  <meta name="citation_author_institution" content="Department of Population Health and Reproduction, UC Davis" />
  <meta name="citation_author_orcid" content="0000-0002-2942-5331" />
  <meta name="twitter:creator" content="@saltyscientist" />
  <meta name="citation_author" content="Luiz Irber" />
  <meta name="citation_author_institution" content="Graduate Group in Computer Science, UC Davis" />
  <meta name="citation_author_institution" content="Department of Population Health and Reproduction, UC Davis" />
  <meta name="citation_author_orcid" content="0000-0003-4371-9659" />
  <meta name="twitter:creator" content="@luizirber" />
  <meta name="citation_author" content="Taylor Reiter" />
  <meta name="citation_author_institution" content="Graduate Group in Food Science, UC Davis" />
  <meta name="citation_author_institution" content="Department of Population Health and Reproduction, UC Davis" />
  <meta name="citation_author_orcid" content="0000-0002-7388-421X" />
  <meta name="twitter:creator" content="@ReiterTaylor" />
  <meta name="citation_author" content="C. Titus Brown" />
  <meta name="citation_author_institution" content="Department of Population Health and Reproduction, UC Davis" />
  <meta name="citation_author_orcid" content="0000-0001-6001-2677" />
  <link rel="canonical" href="https://bluegenes.github.io/2022-paper-sourmash-taxonomy/" />
  <meta property="og:url" content="https://bluegenes.github.io/2022-paper-sourmash-taxonomy/" />
  <meta property="twitter:url" content="https://bluegenes.github.io/2022-paper-sourmash-taxonomy/" />
  <meta name="citation_fulltext_html_url" content="https://bluegenes.github.io/2022-paper-sourmash-taxonomy/" />
  <meta name="citation_pdf_url" content="https://bluegenes.github.io/2022-paper-sourmash-taxonomy/manuscript.pdf" />
  <link rel="alternate" type="application/pdf" href="https://bluegenes.github.io/2022-paper-sourmash-taxonomy/manuscript.pdf" />
  <link rel="alternate" type="text/html" href="https://bluegenes.github.io/2022-paper-sourmash-taxonomy/v/4ded2cacfe63946c35a5751566157687484af1fd/" />
  <meta name="manubot_html_url_versioned" content="https://bluegenes.github.io/2022-paper-sourmash-taxonomy/v/4ded2cacfe63946c35a5751566157687484af1fd/" />
  <meta name="manubot_pdf_url_versioned" content="https://bluegenes.github.io/2022-paper-sourmash-taxonomy/v/4ded2cacfe63946c35a5751566157687484af1fd/manuscript.pdf" />
  <meta property="og:type" content="article" />
  <meta property="twitter:card" content="summary_large_image" />
  <link rel="icon" type="image/png" sizes="192x192" href="https://manubot.org/favicon-192x192.png" />
  <link rel="mask-icon" href="https://manubot.org/safari-pinned-tab.svg" color="#ad1457" />
  <meta name="theme-color" content="#ad1457" />
  <!-- end Manubot generated metadata -->
bibliography:
- content/manual-references.json
manubot-output-bibliography: output/references.json
manubot-output-citekeys: output/citations.tsv
manubot-requests-cache-path: ci/cache/requests-cache
manubot-clear-requests-cache: false
...






<small><em>
This manuscript
([permalink](https://bluegenes.github.io/2022-paper-sourmash-taxonomy/v/4ded2cacfe63946c35a5751566157687484af1fd/))
was automatically generated
from [bluegenes/2022-paper-sourmash-taxonomy@4ded2ca](https://github.com/bluegenes/2022-paper-sourmash-taxonomy/tree/4ded2cacfe63946c35a5751566157687484af1fd)
on November 14, 2022.
</em></small>



## Authors



+ **N. Tessa Pierce-Ward**
  <br>
    ![ORCID icon](images/orcid.svg){.inline_icon width=16 height=16}
    [0000-0002-2942-5331](https://orcid.org/0000-0002-2942-5331)
    · ![GitHub icon](images/github.svg){.inline_icon width=16 height=16}
    [bluegenes](https://github.com/bluegenes)
    · ![Twitter icon](images/twitter.svg){.inline_icon width=16 height=16}
    [saltyscientist](https://twitter.com/saltyscientist)
    <br>
  <small>
     Department of Population Health and Reproduction, UC Davis
     · Funded by Grant 1711984 from the NSF; Grant GBMF4551 from the Gordon and Betty Moore Foundation; Grant 2018911 from the NSF
  </small>

+ **Luiz Irber**
  <br>
    ![ORCID icon](images/orcid.svg){.inline_icon width=16 height=16}
    [0000-0003-4371-9659](https://orcid.org/0000-0003-4371-9659)
    · ![GitHub icon](images/github.svg){.inline_icon width=16 height=16}
    [luizirber](https://github.com/luizirber)
    · ![Twitter icon](images/twitter.svg){.inline_icon width=16 height=16}
    [luizirber](https://twitter.com/luizirber)
    <br>
  <small>
     Graduate Group in Computer Science, UC Davis; Department of Population Health and Reproduction, UC Davis
     · Funded by Grant GBMF4551 from the Gordon and Betty Moore Foundation; Grant R01HG007513 from the NIH NHGRI
  </small>

+ **Taylor Reiter**
  <br>
    ![ORCID icon](images/orcid.svg){.inline_icon width=16 height=16}
    [0000-0002-7388-421X](https://orcid.org/0000-0002-7388-421X)
    · ![GitHub icon](images/github.svg){.inline_icon width=16 height=16}
    [taylorreiter](https://github.com/taylorreiter)
    · ![Twitter icon](images/twitter.svg){.inline_icon width=16 height=16}
    [ReiterTaylor](https://twitter.com/ReiterTaylor)
    <br>
  <small>
     Graduate Group in Food Science, UC Davis; Department of Population Health and Reproduction, UC Davis
     · Funded by Grant GBMF4551 from the Gordon and Betty Moore Foundation; Grant R03OD030596 from the NIH Common Fund
  </small>

+ **C. Titus Brown**
  <br>
    ![ORCID icon](images/orcid.svg){.inline_icon width=16 height=16}
    [0000-0001-6001-2677](https://orcid.org/0000-0001-6001-2677)
    · ![GitHub icon](images/github.svg){.inline_icon width=16 height=16}
    [ctb](https://github.com/ctb)
    <br>
  <small>
     Department of Population Health and Reproduction, UC Davis
     · Funded by Grant GBMF4551 from the Gordon and Betty Moore Foundation; Grant R01HG007513 from the NIH NHGRI; Grant 2018911 from the NSF; Grant R03OD030596 from the NIH Common Fund
  </small>


::: {#correspondence}
✉ — Correspondence possible via [GitHub Issues](https://github.com/bluegenes/2022-paper-sourmash-taxonomy/issues)

:::


## Abstract {.page_break_before}




## Background {.page_break_before}
    
Taxonomic profiling intro...

Sourmash gather is a method to use combinatorial observations of k-mers to find the minimum set of reference genomes that contain all k-mers of the query dataset. Sourmash gather results are non-overlapping: each k-mer is assigned to one and only one genome match. Gather results are to specific genomes, but many biological applications work at the species-level, rather than strain level. This is especially important as these strain matches may not be the best/ideal results. In many cases, the specific strain in your dataset may not be available in the database, meaning the results end up matching to a few suboptimal reference genomes. Sourmash taxonomy is a sourmash module designed to ingest sourmash gather results, integrate taxonomic information, and optionally aggregate the results using a lowest-common-ancestor approach. 


<!--
from blog post:

As the exact strains from novel sequencing projects are often not present in reference databases, gather results commonly include matches to multiple strains of the same species, if there are multiple strains present in the reference database. These matches represent the portions of our novel query strain(s) that share genomic content with strains in the reference database.

he main innovation of the gather–>tax method is that LCA aggregation occurs at the genome level, or really at the “groups of k-mers” level, rather than at the individual k-mer level.

Single k-mers, either for true biological reasons or as a result of reference inaccuracies, can sometimes match to quite different organisms and derail the individual k-mer LCA approach (nicely laid out in this twitter thread):
In our experience, aggregating k-mer matches to the set of best genome matches with gather prior to LCA means contamination and other reference issues are far less likely to impact LCA annotations. As an added benefit, this approach allows us to do taxonomic assignment with multiple taxonomies (e.g. GTDB if available, NCBI for the remaining), so long as the gather was run against the appropriate databases.
-->

## Implementation

Sourmash taxonomy conducts LCA-style taxonomic summarization of the genomic profiling results from sourmash gather.
It was introduced in sourmash v4.2.

### LCA-Style Lineage summarization

Sourmash gather uses a minimum set cover approach to identify the smallest set of reference genomes that contain all query information (k-mers) [@sourmash_gather].
These matches are non-overlapping; that is, the sum of the query fraction assigned to each genome will be at most 100% (entire query matched to reference genomes).

Sourmash taxonomy LCA methods apply the taxonomic information from these reference genomes to their assigned query fraction and sum matches that correspond to the same taxonomic rank. For example, if the `sourmash gather` results for a metagenome include matches to 10 different strains of a given species, `sourmash tax` LCA can sum the fraction uniquely matched to each strain to obtain the total fraction uniquely matched to this species.

Because this approach relies upon non-overlapping reference assignments, separate `sourmash gather` results for the same query cannot be combined. However, `sourmash gather` can be run with any number of desired reference databases at once to produce a single set of non-overlapping assignments.

Two `sourmash tax` commands use this LCA-Style summarization: `metagenome` and `genome`.

<!--
tax commands rely upon the fact that gather provides both the total fraction of the query matched to each database matched, as well as a non-overlapping f_unique_to_query, which is the fraction of the query uniquely matched to each reference genome. The f_unique_to_query for any reference match will always be between (0% of query matched) and 1 (100% of query matched), and for a query matched to multiple references, the f_unique_to_query will sum to at most 1 (100% of query matched). We use this property to aggregate gather matches at the desired taxonomic rank. For example, if the gather results for a metagenome include results for 30 different strains of a given species, we can sum the fraction uniquely matched to each strain to obtain the fraction uniquely matched to this species. Alternatively, taxonomic summarization can take into account abundance weighting; see classifying signatures for more information.

-->

#### sourmash tax metagenome

“sourmash tax metagenome” is designed to conduct LCA aggregation for metagenomes to build a taxonomic profile.
`tax metagenome` ingests sourmash gather results from one or more metagenome queries and summarize the results for each metagenome at each taxonomic rank.
`tax metagenome` provides several output file options, including some that are designed to facilitate input into downstream analysis tools.

**csv_summary** This output file reports a lineage summarization for each query at each taxonomic rank.

**krona** When used with `-F krona --rank RANK`, `sourmash tax metagenome` optionally produces a tab-separated list of results at a specific rank, which can be directly used to generate a `krona` plot (cite krona; add krona figure to results). This format is minimal, containing fraction of the query matched to the reported rank and lineage, with columns for each taxonomic rank down to the rank used for summarization.

**lineage_summary** The lineage summary format is a way to compare taxonomy results over multiple metagenome queries. It can be generated with `-F lineage_summary --rank RANK`, and will consist of one row per summarized lineage, with columns for the fraction matched in each metagenome sample.

**kreport** The kreport output reports kraken-style kreport output, which may be useful for comparison with other taxonomic profiling methods. While this format typically records the percent of number of reads assigned to taxa, `sourmash taxonomy` creates comparable output by reporting the percent of k-mers matched to each taxon and the estimated number of base pairs that these k-mers represent. To best represent the percent of all reads, we use k-mer abundance information in this output. To generate this properly, query FracMinHash sketches should be generated with abundance information (`-p abund`), which will yield gather results with abundance weighting information.

#### sourmash tax genome

`sourmash tax genome` is designed to aggregate sourmash gather results run on genome assemblies.
Rather than summarizing at each taxonomic rank, sourmash `tax genome` summarizes gather results starting from the lowest rank (species) and will classify the genome as soon as a user-modifiable criterion is reached. There are two classification strategies: classify the query once a match threshold is reached (e.g. 10% containment or 95% cANI), or classify the query once a rank is reached, regardless of percent match. The first strategy is recommended for more robust classification; the second strategy is required for downstream tools requiring all inputs at the same rank.

**csv_summary** This outputs a csv with taxonomic classification for each query genome. This output currently consists of six columns, query_name,rank,fraction,lineage,query_md5,query_filename, where fraction is the fraction of the query matched to the reported rank and lineage. The status column provides additional information on the classification:

**krona** When used with `-F krona --rank RANK`, `sourmash tax genome` optionally produces a tab-separated list of results at a specific rank, which can be directly used to generate a `krona` plot (cite krona; add krona figure to results). This format is minimal, containing fraction of the query matched to the reported rank and lineage, with columns for each taxonomic rank down to the rank used for summarization.

### Utility commands

#### sourmash tax annotate

tax annotate annotates gather results with taxonomic information, without doing any LCA summarization.

#### sourmash tax prepare
tax prepare is a method for converting a csv of taxonomic lineage information into an sqlite database to enable faster loading and lineage assignment. It can also be used to combine lineage information for more that one database (e.g. GTDB, NCBI).

#### sourmash tax summarize

Summarize the lineage information in a human-reaedable summary

#### sourmash tax crosscheck


#### sourmash tax grep

select genomes entries by lineage; most useful for selecting subsets of results or reference genomes for sourmash analyses.

## Results

### Tax Metagenome

#### Reads

#### Contigs


### Tax Genome



## Discussion



- Database recommendations
<!--
As with all reference-based analysis, results can be affected by the completeness of the reference database. However, summarizing taxonomic results from gather minimizes issues associated with increasing size and redundancy of reference databases.
For supported databases (e.g. GTDB, NCBI), we provide taxonomy csv files, but they can also be generated for user-generated databases. 

-->

- gather thresholding discussion/recommendations

- Limitations
  - K-mer size -- > specificity/ sensitivity
  - K21 will give you species assignments, but you might not want to use them...
- Improvements:
  - Tax db inside of zip database?
  - Additional plotting?
  - CAMI output (need taxid)
  - genbank vs gtdb taxonomy translation?


[@dk_fracminhash]: doi:10.1101/2022.01.11.475870

[@sourmash_gather]: doi:10.1101/2022.01.11.475838

[@meganlr]: doi:10.1186/s13062-018-0208-7

[@mmseqs_tax]: doi:10.1093/bioinformatics/btab184

[@mash]: doi:10.1186/s13059-016-0997-x

[@mash_screen]: doi:10.1186/s13059-019-1841-x

[@kaiju]: doi:10.1038/ncomms11257

[@catbat]: doi:10.1186/s13059-019-1817-x

[@portik_tax]: doi:10.1101/2022.01.31.478527

[@breit_classif]: doi:10.1093/bib/bbx120

[@koslicki_containment]: doi:10.1016/j.amc.2019.02.018

[@metapalette]: doi:10.1128/mSystems.00020-16

[@dashing]: doi:10.1186/s13059-019-1875-0

[@blast]: pubmed:2231712

[@diamond]: doi:10.1038/nmeth.3176

[@ganon]: doi:10.1093/bioinformatics/btaa458

[@metalign]: doi:10.1186/s13059-020-02159-0

[@genomic_std]: doi:10.1073/pnas.0906412106

[@fastaai]: doi:10.21203/rs.3.rs-1459378/v1

[@blanca]: doi:10.1089/cmb.2021.0431

[@kraken2]: doi:10.1186/s13059-019-1891-0

[@sourmash_joss]: doi:10.21105/joss.00027

[@sourmash_f1000]: doi:10.12688/f1000research.19675.1

[@cmash]: doi:10.1101/184150

[@bussi]: doi:10.1371/journal.pone.0258693

[@fan_AAF]: doi:10.1186/s12864-015-1647-5

[@kaamer]: doi:10.1038/s41598-022-12843-9

[@orpheum]: doi:10.1101/2021.07.09.450799

[@kaa_metapan]: doi:10.1101/2022.06.27.497795

[@ezaai]: doi:10.1007/s12275-021-1154-0

[@palmer_ani]: doi:10.1099/ijsem.0.004124

[@miga]: doi:10.1093/nar/gky467

[@snekmer]: url:https://github.com/PNNL-CompBio/Snekmer


## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
