
# Purpose
An example template of files for a comprehensive solution architecture in a documentation-as-code approach.

# Assumption(s)
- Most of the text-based content is in AsciiDoc ( https://github.com/asciidoc/asciidoc ) format
- To create any number of multiple output formats, install and leverage DAPS ( https://github.com/openSUSE/daps )
- The organization is similar to Archimate Enterprise Architecture ( https://pubs.opengroup.org/architecture/archimate3-doc )

# Usage / Process
- either git clone/fork or download a ZIP (and then unzip) of this GitHub repository
- in the top-level directory, review/adjust/modify the following files:
  - [DC-SA](./DC-SA) : to add/enable/disable any of the attributes/sections that you desire)
  - [adoc/SA_vars.adoc](./adoc/SA_vars.adoc) : start adjusting the values of
    - useCase
    - title
    - author information
    - github references
  - [adoc/SA.adoc](./adoc/SA.adoc) : the main document
- every portion of text that cites "FixMe" is a flag to encourage modification
- as you edit the modular text content snippets, create an output format
  - daps --force -d DC-SA <format>
    - where <format> might be "pdf", "html", "html --single" and many others are also available
- you can also add images/media content as needed in those subdirectories

# Feedback
- feel free to provide feedback, ask questions or even submit pull request
