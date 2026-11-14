# College of Staten Island Math Department Website

The website is built using [Quarto](https://quarto.org/), a technical
publishing system authored in markdown and converted to html via Pandoc.

To build preview in a local browser:
```sh
quarto preview
```

To build without previewing:
```sh
quarto render
```

Primary maintainer [@seragunn](https://github.com/seragunn).

## Directory Structure

* `/ADA` contains notes on ADA accessibility compliance as it affects the Math Department
* `/Courses` contains learning goals for each course
* `/juliabox` contains links to all of the Juliabox courses (hosted on a separate server)
* `/news` contains news stories for the front page
* `/people` contains faculty and staff information such as email addresses and phone extensions. Please do not directly edit the `.qmd` pages (see below)
* `/Resources` contains pages useful to instructors
* `/Undergraduate` contains pages useful to undergraduate students
* `/WeBWorK` contains links and info to the WeBWorK courses (hosted separately)

## Example tasks:

### News

See [news/readme.md](/news/readme.md)

### Announcements

Edit `_quarto.yml` for a quick announcement. Shows up as a blue bar underneath the nav bar.

### Editing Faculty info

**Please do not directly edit the faculty `.qmd` pages.**

`people/faculty/faculty.csv` contains email addresses, phone extensions, office numbers, titles, faculty interests

`people/faculty/faculty-bios.jl` contains faculty bios.

Edit these files and then run
```sh
julia make_faculty_pages.jl
```

### Frequently updated files

* `/WeBWorK/courses.qmd` with WeBWorK course links
* `/juliabox/index.qmd` with Juliabox course links
* `/Undergraduate/Tutoring/index.qmd` with tutoring schedule
