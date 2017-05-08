# MD resume instruction

## html

resume.html: curriculum_vitae_Kai_20170507.md
	pandoc --standalone -H style.css \
        --from markdown --to html \
        -o resume.html curriculum_vitae_Kai_20170507.md

## PDF

wkhtmltopdf -T 20mm -B 18mm resume.html curriculum_vitae.pdf