# po-auto-translation
Process to translate PO files automatically for FREE using google translate, the script is written using JavaScript

1. convert your PO file into csv file
    ```shell script
    node index.js untranslated_XX.po > untranslated_XX.csv
    ``` 

1. upload ```untranslated_XX.csv``` to Google Sheet

1. use the formula
    ```
    =GOOGLETRANSLATE(A2;"en";"ar")
    ```

1. convert translated columns to text using: 
    - Copy the column then paste values only

1. export file to csv ```translated_XX.csv``` (download csv)

1. convert file to PO file
    ```shell script
    node index.js untranslated_XX.po translated_XX.csv > translated_XX.po
    ``` 
