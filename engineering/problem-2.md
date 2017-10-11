# ClusterTruck Take Home Problem

The following is a test designed to ensure you have a fundamental understanding of building applications. The point of this problem is to qualify your skills and open a conversation during the in person interview.

Please write the code in whatever environment you are comfortable in. Use a github or bitbucket repository and provide the link to the code with some documentation on how to run it.

## Application Requirements

Your task is to build a socket server that responds to the protocol described below. The server can be written in the lang of your choice (c, ruby, python, etc), just please write your own code. Do not pull in any third party libs, the standard library of the language is perfectly acceptable (eg: Net::HTTP, not Httparty).

## The Protocol

The point of the socket server is to accept UPC codes in a line oriented fashion, lookup the product and return information (price and name) about the product using the Walmart API described below. Unfortunately Walmart is the only API I could find that provides this for free.

Given the following input:

```
012044038840
811571013579
012044038840
```

the server should respond with the following:

```
[$2.54] Spice High Endurance Fresh Scent Men's Deodorant, 3 oz.
[$35] Google Chromecast HDMI Streaming Media Player (2014 Model).
[$29.96] Back To The Future: 30th Anniversary… (truncated)
```

## API Endpoint

`http://api.walmartlabs.com/v1/items?apiKey=<API_KEY>&upc=<UPC>`

## API Key

028400003001

## Testing

The way I will test this program is hook a barcode scanner up as a keyboard to my MBP and just go around randomly scanning things. :)

Please have fun with this and let me know if you have any questions.

## Example cURL Request

`curl 'http://api.walmartlabs.com/v1/items?apiKey=4qzgg8q6ek593kdjf6wwxn73&upc=025192275753' | python -m json.tool`
