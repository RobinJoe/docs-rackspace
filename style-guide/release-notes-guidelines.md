# Release notes guidelines

This topic provides guidelines for writing release notes (RN) for Rackspace Cloud services APIs.

A template for the API RN is available in the [docs-common repo](https://github.com/rackerlabs/docs-common/blob/master/templates/release-note-latest-template.rst).

For an example that illustrates most of these guidelines, see the [Cloud Block Storage Release Notes](https://developer.rackspace.com/docs/cloud-block-storage/v1/developer-guide/#release-notes).

- [Structure](#structure)
- [Formatting](#formatting)
- [Wording](#wording)
- [Editing existing release notes](#editing-existing-release-notes)

## Structure
For each release-specific RN file that you create, observe the following guidelines:

- Use one of the following formats for the title of the RN file:

  - If the release has a version number, use that in the title. For example:

    **v2.20.0, June 25, 2016**

  - If the release does not have a version number, use the API contract version and date.	For example:

    **API | contract version | updates, January 07, 2016**

  - If you are documenting a named or initial release, indicate the initial release in the title. For example:

    **API |contract version| release, January 07, 2016**

    You can precede release with a type, such as EA or UA. For example:

    **API |contract version| EA release, January 07, 2016**

- Use the following main sections in the release notes:

  - What's new
  - Resolved issues
  - Known issues
  - Documentation changes

  **Note:** Anything previously labeled as "enhancements" can be included either in "What's new" or "Resolved issues" as appropriate.

- Include the "What's new," "Resolved issues," and "Known issues" sections in every RN file, even if you have no content for one of those sections. If one of these sections has no content for a release, use the |no changes| variable for the body text. This variable inserts the boilerplate text "None for this release." For example:

  **Known issues**

  `|no changes|`  

- Include the "Documentation changes" section only if you have significant content changes, such as adding an extended example, a tutorial, or new content. If you have no significant content changes for a release, omit that section entirely.

- Order your RN files from latest to earliest, so that the latest is always "on top.". For example, the release notes for version 1.1 should precede the release notes for version 1.0 in the hierarchy.  

## Formatting
- Use sentence-style capitalization for all headings, including the title of the file (see the examples in the preceding section). The only exception to this rule is the high-level title of the release notes section, which is **Release Notes**.

- If a section has several items&mdash;for example, there are several resolved issues to document&mdash;provide the descriptions in a bullet list. You do not need to precede the bullet list with an introductory sentence, unless one is necessary for clarity.

- If you have only one item to document in a section, do not show it as a bullet item. Show it as regular text.

- Use the punctuation guidelines for lists at [Writing list items](https://github.com/rackerlabs/docs-rackspace/blob/master/style-guide/a-l-style-guidelines.md#lists-writing).

- As needed, use the [text formatting guidelines](https://github.com/rackerlabs/docs-rackspace/blob/master/style-guide/m-z-style-guidelines.md#text-formatting).

## Wording
You do not need to include an introductory paragraph for each file. The one that exists for the "Release Notes" section as a whole is sufficient. You can begin each file with the "What's new" heading. However, you can include an introductory paragraph if necessary&mdash;for example, if you want to state that the release notes correspond to a particular type of release, such as a Limited Availability release, or you need to introduce the first release of a major version.

If you refer to content in another part of the API document, provide a link to the specific section.

Use the following guideline when creating items in each section:

### What's new
Use sentences to describe the new feature or enhancement. Provide details as needed, and provide a link to any section in the documentation that describes that feature.

**Example:**

IPv6 support has been added. When you create a server, an IPv4 address and an IPv6 address block are assigned. The IPv4 address and IPv6 address block are used for the public interface (Internet). The IPv4 address is also used for the private interface.

### Resolved issues
Provide an initial phrase that describes the issue that was fixed. Start the phrase with a past-tense verb. If necessary, include sentences to further explain the fix. If you list only phrases, do not use ending punctuation.

**Example:**

- Added support for Debian 8 (Jessie)
- Trimmed the Monitoring ID and Monitoring Token configuration variables to ensure correctness
- Fixed the Xen Server 6 package repo

### Known issues

Use sentences to describe the issue. If a workaround is available, explain it. 	

**Example:**

The create a service operation does not support Classless Inter-Domain Routing (CIDR) for IP address restrictions.

### Documentation changes
Provide an initial phrase that describes the issue that was fixed. Start the phrase with a past-tense verb. If necessary, include sentences to further explain the fix. If you list only phrases, do not use ending punctuation. Provide a link to the relevant section in the documentation. 	

**Example:**

Clarified the descriptions of the alert policies to include how the polling window affects the alarm state. See [Alert policies](https://developer.rackspace.com/docs/cloud-monitoring/v1/developer-guide/#alert-policies).

## Editing existing release notes
In cases where existing release notes were not accurate at the time of publication, change the content to make it accurate. You can make the following types of changes:

- Fix typos
- Correct links that were wrong at the time of publication
- Correct incorrect statements to reflect what was correct at the time of publication
