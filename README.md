
UPDATE --- Switching to GitHub pages for their repo-based hosting with custom domains and TLS. Much cleaner and faster.


I'm using this project as a start: https://github.com/mszep/pandoc_resume

I like that the two packages, pandoc and mactex, are in Homebrew. 

I like that pandoc converts to and from github standard markdown and HTML4 and 5. 

I like that Tex is used because it's designed specifically for elegant and page-aware typesetting. Some other options cut off lines on page breaks or require Ruby Gems, yuck. This runs from simple make commands in local context or Dockerized.

To run, copy this resume.md file into the cloned repo in the pandoc_resume/markdown/ directory. Then `docker-compose up -d`

Other options are problematic, "The suggestion is to use the wkhtmltopdf tool, which takes the pandoc-generated HTML and uses the webkit browser engine to generate a pdf. While this will preserve the look and feel of the resume, the pdf output is suboptimal, as webkit is not a typesetting engine. Most importantly, it does not handle page breaks well -- in some cases even putting a page break right across a line of text."
