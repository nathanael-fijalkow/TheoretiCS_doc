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

3. The layout editors work on the paper on Overleaf

4. The layout editors hand it over to managing editors

6. The managing editors set the volume (to "Volume XXX" (one per year)) in the
   platform and check that the article numbers are correct. This cannot be
   changed after publication without emailing Episciences

6. The managing editors figure out:
    * the number in the volume
    * the DOI, which is a function of the above: 
      https://doi.org/10.46298/theoretics.year.number
      for instance year = 23 and number = 10
    * publication date: the day it will be announced on arXiv, see
      [here](https://info.arxiv.org/help/availability.html). (The email we send
      to authors ask them to update this date in case they submit later)

7. The managing editors input the above information in the Latex file, i.e.,
   they check that the following macros are present and fill those that need to
   be filled: 
    * \ThCSyear{}
    * \ThCSarticlenum{}
    * \ThCSdoicreatedtrue
    * \ThCSreceived{}
    * \ThCSrevised{}
    * \ThCSaccepted{}
    * \ThCSpublished{}

   They then send an email to the authors to ask them to upload the Overleaf
   version to arXiv, using the template email.

8. Once the version is on arXiv, managing editors check whether it's correct,
   and import the latest arXiv version of the paper in the system:
    * either from the management page by clicking the edit icon next to the
      article version, or 
    * by answering the request for the final version from the public page of
      the article

10. Managing editors add the DOI in the platform

11. Managing editors click publish

12. Managing editors check that the article shows up in the "latest articles"
    page (there seems to be a small delay of a few minutes)
