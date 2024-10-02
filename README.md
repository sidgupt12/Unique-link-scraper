# Unique-link-scraper

This project is a simple web crawler written in Go that retrieves unique URLs from specified seed URLs. It leverages Go's standard library along with the `golang.org/x/net/html` package to parse HTML and extract links.

## Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Example](#example)

## Features

- Extracts unique URLs from the provided seed URLs.
- Concurrently crawls multiple URLs using Goroutines.
- Parses HTML to find anchor (`<a>`) tags and their `href` attributes.
- Displays the count of unique URLs found.

## Requirements

- Go 1.16 or later

## Installation

1. **Clone the repository:**

   ```bash
   git clone <repository-url>
   cd <repository-directory>


2.	**Install the required package:**
The project uses the golang.org/x/net/html package. Install it with the following command:

go get golang.org/x/net/html

## Usage

To run the web crawler, use the following command:

go run main.go <seed-url-1> <seed-url-2> ...

Replace <seed-url-1>, <seed-url-2>, etc., with the URLs you want to crawl.

## Example
For example, to crawl URLs starting from https://example.com and https://golang.org, run:

The output will display the number of unique URLs found:
Found X unique urls:
 - https://example.com/link1
 - https://example.com/link2
 - https://golang.org/doc
 ...