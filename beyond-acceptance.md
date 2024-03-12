# TheoretiCS Helper for what happens once a paper is accepted

> Authors: Antoine Amarilli, Nathanaël Fijalkow, Mikaël Monet, David Purser

Once a paper has been accepted (i.e., it appeared in the previous digest as
recommended for acceptance and no editor reacted to it), we start the
publishing procedure below.

We have an internal spreadsheet to keep track of which papers are in which
stage of this process. The process is:

1. The editor-in-chief accepts the paper (changed its status) and communicates
   to the author with the latest reviews and comments

2. The author sends their files for final version (in some non-TheoretiCS
   style)

3. The layout editors work on the paper on Overleaf, then hand it over to managing editors

6. The managing editors change the volume (to "Volume XXX" (one per year)) in the
   platform. This has the effect of creating an "article number". This number
   cannot be changed after publication without emailing Episciences

7. The managing editors check that the following macros are present in the
   latex file and fill those that need to be filled: 
    * \ThCSyear{}: already pre-filled
    * \ThCSarticlenum{}: the article number from above
    * \ThCSdoicreatedtrue: this is commented out when we receive the file and
      needs to be uncommented to create the DOI string on the paper. The DOI is
      of the form https://doi.org/10.46298/theoretics.year.number (for instance year
      = 23 and number = 10), and it needs to appear on the bottom-right corner of the
      first page
    * \ThCSreceived{}: already pre-filled by layout editors
    * \ThCSrevised{}: already pre-filled by layout editors
    * \ThCSaccepted{}: already pre-filled by layout editors
    * \ThCSpublished{}: here we guess the day it will be announced on arXiv, see
      [here](https://info.arxiv.org/help/availability.html). (The email we send
      to authors ask them to update this date in case they submit later)

   They then send an email to the authors to ask them to upload the Overleaf
   version to arXiv, using the template email.

8. Once the version is on arXiv, managing editors check whether it's correct,
   and import the latest arXiv version of the paper in the system:
    * either from the management page by clicking the edit icon next to the
      article version, or 
    * by answering the request for the final version from the public page of
      the article

9. Managing editors add the DOI in the platform (click "request DOI" and check
   that the DOI assigned is the same as above)

10. Managing editors click publish

11. Managing editors check that the article shows up in the "latest articles"
    page (there seems to be a small delay of a few minutes)

12. If the publication date on the pdf does not match to the publication date
    on the patform, managing editors leave a comment in the spreadsheet
