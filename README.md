# Script Task 01

This is a repo for the Endava´s Script challenge for internship 2024 - 2. This script is written in Javascript and generates a JSON and PDF report of Artworks from [Art Institute of Chicago API](https://api.artic.edu/api/v1/artworks).

## How to use it

Make sure to have installed [NodeJS](https://nodejs.org/en)

Clone this repo and install its dependencies with npm

```
npm i
```

Run the script and get the first 12 artworks

```
node index
```

Inside the script´s folder you should find two reports with the format _Report [current date]_.json and _Report [current date]_.pdf

## Flags

`--id` Gets the report of one specific artwork
`--page` Generates a report based on the page number selected
`--limit` Sets a different limit of artworks for the report (default is 12)
`--search` Sets a search value for matching artworks
`--email` Defines a email to send both .json and .pdf report

## Examples

    node index --id 565

Returns a report for the artwork with id 656

    node index --page 2 --limit 50

Generates report for 50 artworks on the second page

    node index --search cats

Generates a 12 artworks report for content related with cats

    node index --email jonathan.buitrago@endava.com

Generates a report of 12 artworks and send it to jonathan´s email
