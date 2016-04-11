Testing proof-of-concept for using CSS (and perhaps less?) to define
the rules necessary to do collation (and numbering) of "raw" html
to a "cooked" html form.

Test code is contained in the command-line utility 'poc.py'
This takes 1-3 arguments:

a required css file, then optional html input, and html output

example rule set is in poc.less.

convert to css via 'lessc poc.less > poc.css'
requires lessc >= 1.7

## Install

Install less (which contains the lessc tool):

```npm install -g less```

Install the required python packages:

```pip install -r requirements.txt```

## Usage

run test as:

```./poc.py poc.css poc-raw.html poc-cooked.html```

## Book assembler

```fullbook.py <bookid> mybook.html```

bookid may be any id that defines a book: long uuid, shortid, with or without @version.