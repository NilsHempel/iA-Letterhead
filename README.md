# iA-Letterhead

## Idea

* Create letters within iA Writer on a printed letterhead with recipient for
   * private correspondence
   * business correspondence
* Output is in PDF and printed PDF.

Ideally, this correspondence template can then be filled with `Content Blocks` and `[%Frontmatter]` to quickly create a letter.

## Proposed Solution

Looking at the [template documentation](https://github.com/iainc/iA-Writer-Templates) the best approach isn't fully obvious to me.

The sections of a letter (as numbered) should go

1. head of the letter should probably go in the header.html.
2. Recipient's address - header.html or document.html
3. Re / subject - header.html or document.html
4. content - document.html
5. footer - footer.html

![](https://github.com/NilsHempel/iA-Letterhead/blob/master/Letter.png)

## Available Attributes

These are available as-is:

|attribute|comment|
|:-|:-|
|author||
|date|[Unicode formatting](http://www.unicode.org/reports/tr35/tr35-31/tr35-dates.html#Date_Format_Patterns)|
|title|might be useful as reference/ subject|
|page-number|footer on pages 2-n|
|page-count|footer on pages 2-n|

## Other Attributes

Some attributes will probably have to be added via frontmatter.

|attribute|comment|
|:-|:-|
|Recipient's name||
|Street and No.||
|ZIP and City||
|Subject|if the document title isn't fitting well as a subject|

## Specifications

* In the beginning I would be happy to have a functioning letterhead
* Then I would want to modify it to comply with relevant national standards such as [DIN 5008 in Germany](https://www.edv-lehrgang.de/din-5008/).
* This means setting up both a personal and a professional template.

## Collaboration

I'm sure quite a few people have a similar use-case; I'll be uploading my attempts to GitHub at [https://github.com/NilsHempel/iA-Letterhead](https://github.com/NilsHempel/iA-Letterhead) and would love to work on this together.

## Possible Roadblocks

There are a few issues that I can think of:

1. Attributes are not available in other parts of the document
2. frontmatter attributes don't work in other parts of the document
3. fonts need to be embedded to send PDFs electronically
4. Not possible to create a first page differently than the following pages
