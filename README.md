# alfred-convert-csv-to-xslx

This is an Alfred Workflow that lets you convert CSV files to XSLX (Excel) format. This tool is very useful for data analysts or anyone who frequently works with data files and needs to convert them to a more user-friendly format for editing and visualization purposes.

The conversion process is done by a Python script which reads a CSV file, converts it into a DataFrame (a two-dimensional tabular data structure with labeled axes), and then writes that DataFrame into an XLSX (Excel) file.

## Installation 

### Step 1: Install Python (if not already installed):

Open Terminal and type:

    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    brew install python

### Step 2: Install the required Python libraries:

We'll need two libraries: `pandas` for data manipulation and `openpyxl` for Excel file handling.

To install these libraries, type the following command in Terminal:

    pip install pandas openpyxl

`pip` is a package installer for Python. You can use it to install various Python libraries.

## Usage

Use via Universal Actions in Alfred. Alfred's Universal Actions allow you to select a file in Finder or on your Desktop and apply an action to it, like converting the file format.

In Environment Variables you can change the default encoding, delimiter, and quote character.

## Changelog

**0.3**
- Added conversion parameters as variables: This enhancement allows you to set specific parameters for the conversion process as variables, giving you more control over the output.

**0.2**
- Added autofiltering: This feature automatically applies filters to the columns in the Excel file, making it easier for you to sort and filter the data.
- Added freezing of the top row: Freezing the top row allows you to scroll down in the Excel file without losing sight of the column headers.

**0.1**
- Initial version: Basic CSV to XSLX conversion functionality.
