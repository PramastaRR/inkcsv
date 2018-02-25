# InkCSV
InkCSV is a program that helps you to make invitations, certificates, etc. from a CSV file and a SVG template. You will need Python (2.x or 3.x) and Inkscape to run this program.

## Installation
To install this program in your Linux computer, copy the `inkcsv` file to a `$PATH` directory.

## Usage

    inkcsv [CSV file name] [SVG template file name] [Words to replace] [DPI]

- `[CSV file name]`: the data source, on CSV format.
- `[SVG template file name]`: the template, on SVG format.
- `[Words to replace]`: words to replace on the template, please separate each word with comma (,)
- `[DPI]`: DPI of the exported PNG file. Inkscape's default is `96`.

## Example

Case: We are going to make name tags for employees in a company. 

**people.csv**

    Ann, Manager
    Bonnie, Programmer
    Coco, Designer

**template.svg**

![alt text](template.svg)

With CSV data source and SVG template above, we can make name tags with:

    inkcsv people.csv template.svg var_name,var_role 96

The results will be saved in `exported` directory. The results will look like this:

![alt text](result.png)