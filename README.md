# metaverses-nft-creator-economies-on-blockchain
Metaverses, NFTs and Creator Economies on the Blockchain - SP22

- [Editing the Syllabus](#editing-the-syllabus)
- [Editing the Guest Speaker List](#editing-the-guest-speaker-list)
- [Editing the Course Site](#editing-the-course-site)

## Editing the Syllabus
Open and edit the text directly in the `syllabus.yml` file. Below is the format for a single row in the Syllabus. _Please note the indentation_.

### Syllabus Row Format

```yml
- date: String
  agenda:
    title: String
    recording: URL String # Optional
  homework:
    # -- Optional Entries --
    - i:
          title: String
          link: URL String
    - i:
          title: String
          link: URL String
    ...
```
### Ex. Syllabus Row

```yml
- date: 2/23
  agenda:
    title: Business Validation
    recording: https://www.berkeley.edu/
  homework:
    - i:
        title: Homework 1 of 2, due Feb 23, New Version of Team Slides
        link: https://www.berkeley.edu/    
```
### Ex. Multiple Syllabus Entries
```yml
- date: 2/28
  agenda:
    title: Functional Validation (Problem Solution Fit)
    recording: https://www.berkeley.edu/
  homework:
    - i:
        title: Homework due Mon, Feb 28- Individual Video Blog
        link: https://www.berkeley.edu/
- date: 3/2
  agenda:
    title: Execution
    recording: https://www.berkeley.edu/
  homework:
- date: 3/7
...
```

## Editing the Guest Speaker List
Open and edit the text directly in the `speakers.yml` file. Below is the format for a single row in the Syllabus. _Please note the indentation_.

### Speaker Row Format
```yml
- company: String
  speakers: String
```

### Ex. Speaker Row
```yml
- company: UC Berkeley
  speakers: Levi Kline # Text following the ':' can be left blank
```

### Ex. Multiple Speaker Entries
```yml
- company: UC Berkeley
  speakers: John Doe
- company: RDI
  speakers:
- company: Xcelerator
  speakers: Jane Doe
...
```

## Editing the Course Site
**Please contact the RDI team for any site changes.** 

If you would like to edit the site yourself, you can edit `index.markdown` 

For customized style changes, edit `/assets/css/style.scss`

For changes to the site header, edit `/layouts/_default.html`

For changes to the Syllabus or Speaker list tables, edit `syllabus.markdown` and `speakers.markdown`
