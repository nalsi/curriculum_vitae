# MD resume instruction



## html

resume.html: curriculum\_vitae\_Kai\_20171207.md
	pandoc --standalone -H style.css \
	    --from markdown --to html \
	    -o resume.html curriculum_vitae_Kai_CHN.md

## PDF

wkhtmltopdf -T 20mm -B 18mm resume.html curriculum\_vitae.pdf