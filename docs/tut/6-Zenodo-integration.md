---
layout: default
title: 6. Issue a doi with Zenodo
nav_order: 6
parent: Tutorials
has_children: false
---


<!-- https://guides.lib.berkeley.edu/citeyourcode -->



# Creating a doi
{: .fs-9 }

How to create a doi using Zenodo for your GitHub project
{: .fs-6 .fw-300 }

---

Zenodo is free to use tool for creating a digital object identifier (doi) for your shared resources. A doi is essential for enabling other researchers to cite and reuse your material, and for you to receive proper attribution. Your doi entry will include your [ORCID ID](https://info.orcid.org/benefits-for-researchers/), so it can be tracked against all your other research outputs.

There are two ways to create a doi for a GitHub repository using Zenodo:
1. Manual upload of your repository materials (simple)[##1-manual-upload-of-your-repository-materials-simple]
2. Automated DOI generation and versioning with Zenodo-GitHub integration (more advanced!)[#automated-doi-generation-and-versioning-with-zenodo-github-integration-more-advanced]

## 1. Manual upload of your repository materials (simple)


### First time creating a doi for a GitLab repository

1. In [zenodo](https://zenodo.org), log in or create an account. Go to "[new upload](https://zenodo.org/deposit/new)" and add details about your material. Click the "reserve" button to get the doi which will be issued by zenodo.
2. Copy this doi into your README for your project on GitLab, or other documentation. Include this in a section entitled "How to cite this material".
3. Make a “[release](https://stackoverflow.com/questions/29520905/how-to-create-releases-in-gitlab)” of the repository. Add a note to mark this as the initial release.
4. Download the repository from GitLab (download icon on the repository home page) as a .zip or other compressed file type.
5. Upload the compressed file collection to zenodo.
6. Finalise the zenodo entry with all contributors including their ORDIC IDs. Include a link to the GitLab repository.
7. Set an embargo period for the material if it is not yet publicly available on GitLab.

### Updating the material

If you make substantial changes to your material, you may want to update the doi record. Changes may include adding new contributors, or new code.

Zenodo allows you to issue a new "version" of your record. All versions will resolve to a single doi, therefore anyone who follows your old doi will see that a new version is available. Read [more about this from zenodo](https://blog.zenodo.org/2017/05/30/doi-versioning-launched/).

To create a new version of your record:

1. Make a “[release](https://stackoverflow.com/questions/29520905/how-to-create-releases-in-gitlab)” of your GitLab repository. Add a note to describe the changes that have been made.
2. Download the repository from GitLab (download icon on the repository home page) as a .zip or other compressed file type.
3. Go to your zenodo entry for the first release. Click the "new version" button and upload the new material. Make any other changes to the record as necessary.

## 2. Automated DOI generation and versioning with Zenodo-GitHub integration (more advanced!)

Follow this [guide from Code Refinary](https://coderefinery.github.io/github-without-command-line/doi/) for the more advanced automated integration method.

!Note! When the API builds your contibutor list for Zenodo, it looks first for contibutors to your GitHub repository and the list will be re-written with every new release of your code (that is, when a new versio of your DOI is triggered).

Make sure all your contributors (and their ORCIDs) are included by adding a [.zenodo.json](https://developers.zenodo.org/#add-metadata-to-your-github-repository-release) (another example here)](https://github.com/openresearchcalendar/openresearchcalendar.github.io/blob/master/.zenodo.json) file to your repository, including all your contributor metadata.

Contibutor metadata can also be parsed form a [CITATION.cff file](https://citation-file-format.github.io/#/supported-by-zenodo-). 
