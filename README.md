# po-auto-translation
Process to translate PO files automatically for FREE using google translate, the script is written using JavaScript

1. convert your PO file into csv file
    ```shell script
    node index.js YOUR_FILE.po > untranslated.csv
    ``` 
1. upload ```untranslated.csv``` to Google Sheet
1. use 
    ```
    GOOGLETRANSLATE(“Hello World”,”en”,”es”)
    ```
1. convert translated columns to text
1. export file to csv ```translated.csv```
1. convert file to PO file
    ```shell script
    node index.js file.po translated.csv > translated.po
    ``` 
