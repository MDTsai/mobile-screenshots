### Running the script

`python make-screenshots.py`

### Getting fresh urls.txt

Run the following command:

```
curl -s -O http://s3.amazonaws.com/alexa-static/top-1m.csv.zip; \
unzip -q -o top-1m.csv.zip top-1m.csv; \
head -200 top-1m.csv | \
cut -d, -f2 | \
cut -d/ -f1 > urls.txt; rm top-1m.csv*
 ```# mobile-screenshots
