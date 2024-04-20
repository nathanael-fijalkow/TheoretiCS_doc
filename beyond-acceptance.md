# TheoretiCS Helper for what happens once a paper is accepted

> Authors: Antoine Amarilli, Nathanaël Fijalkow, Mikaël Monet, David Purser

Once a paper has been accepted (i.e., it appeared in the previous digest as
recommended for acceptance and no editor reacted to it), we start the
publishing procedure below.

We have an internal spreadsheet to keep track of which papers are in which
stage of this process. The process is:

1. The editor-in-chief accepts the paper (changed its status) and communicates
   to the author with the latest reviews and comments.

2. *New (was EiCs)* Managing editors, in a separate follow up email to request the sources.

2. The author sends their files for final version (in some non-TheoretiCS
   style).

    - Managing editors send reminders if sources are not received in a timely manner.

2. Managing editors ensure the sources go to Chief Layout Editor (currently: Thomas) to upload to Overleaf.
    - Provide submitted/revised/accepted dates?

3. The layout editors work on the paper on Overleaf, then hand it over to managing editors

6. The managing editors change the volume (to "Volume XXX" (one per year)) in the
   platform. This has the effect of creating an "article number". This number
   cannot be changed after publication without emailing Episciences.  
   **Log this number in the spreadsheet to avoid clashes.**  
   Last few days of the year, might not complete all steps this year? Consider waiting until next year.


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
    * \ThCSrevised{}: already pre-filled by layout editors. This is the date
      that we received the last revision version of the article that was
      accepted (not the date that we received the sources as in step 2). If there was
      no revision throughout the entire reviewing process, we comment it out.
    * \ThCSaccepted{}: already pre-filled by layout editors
    * \ThCSpublished{}: here we guess the day it will be announced on arXiv: <https://nathanael-fijalkow.github.io/TheoretiCS_doc/timezones.html>

8. Upload to arXiv

    1. **Option 1**: Authors upload to arXiv 

        - Send an email to the authors asking them to upload to arXiv.   
          Recommend the time zone tool to get the publication date correct: <https://nathanael-fijalkow.github.io/TheoretiCS_doc/timezones.html>

    2. **Option 2**: Managing editors upload to arXiv (still slightly experimental)

        - Send an email to authors asking for the paper password.  
          Maybe attach the current version to confirm exactly what will be submitted.  
          Clarify the author name/email we will use (in the proxy field).   
          Clarify that by sending the password, we have permission to upload with CC-BY licence.

        - Claim ownership on arXiv: <https://arxiv.org/auth/need-paper-password>   
          Check you're on the TheoretiCS account, not your own!   
          Are you an author of this paper? No

        - Fill the publication date in the TeX: <https://nathanael-fijalkow.github.io/TheoretiCS_doc/timezones.html>  
          Prepare the zip file, don't forget the .bbl, no need to upload the guide and some other files.

        - Submit an arXiv replacement:
            * Pick CC-BY licence
            * In the proxy section, use the authors name and email (seems reasonable to take this from the previous arXiv version, or use the corresponding authors information)
            * Set the meta-data according to the standard:   
                Title, Authors(s), Abstract: Fill these out normally as you would for any other article (check if the title/abstract has changed in the latest revision)  
                Report number: Leave this field blank.  
                Journal reference: TheoretiCS, Volume N (20XX), Article YY, PP-PP  
                DOI: 10.46298/theoretics.XX.YY  
                ACM class, MSC class: These are optional but leave them be if the authors set them in a previous version.  

        - Download the arXiv generated preview and check (at minimum):

            * The references are present
            * That ?? does not appear (unless appropriate)
            * Dates and DOI are present

        - Once submitted, send the arXiv preview to the authors, asking them to get in touch very quickly if it is wrong. (We have at least 5 hours to retract it, but it will delay publication by one cycle.)

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
    on the platform, managing editors leave a comment in the spreadsheet
