# po-auto-translation
Process to translate PO files automatically for FREE using Google Translate, the script is written using JavaScript

## Requirements

- Node.js (10+)

## Steps

1. Clone this repository
    ```shell script
    git clone git@github.com:naskio/po-auto-translation.git
    ```

1. Install dependencies
    ```shell script
    yarn install 
    # or
    npm install
    ``` 

1. Convert your PO file into CSV using the following command
    ```shell script
    node index.js untranslated_XX.po > untranslated_XX.csv
    ``` 

1. Upload ```untranslated_XX.csv``` to Google Sheet

1. Use the formula
    ```
    =GOOGLETRANSLATE(A2;"en";"ar")
    ```

1. Convert the translated columns to text using ```Copy the column then paste values only```

1. Export file to CSV ```translated_XX.csv``` (download CSV)

1. Convert the CSV file to PO file using the following command
    ```shell script
    node index.js untranslated_XX.po translated_XX.csv > translated_XX.po
    ``` 
