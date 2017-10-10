# ClusterProblem - Front End
The following is a test designed to ensure you have a fundamental understanding of building applications. The point of this problem is to qualify your skills and open a conversation during the in person interview.
						
Please write the code in whatever environment you are comfortable in. Please provide a link to your github/gitlab repo as well as a link to the hosted version of your app to engineering@clustertruck.com.

## Application Requirements

Your task is to design a single page application that utilizes the **ClusterTruck kitchen API** and one of the freely available **weather APIs** to build a page that predicts ClusterTruck demand for each kitchen based on forecast. The demand can be represented any way you would like (numerically, colors, high/med/low, etc). It is your job to figure out the best way to present the information. 

The following statements describe what factors influence demand:

* Monday: 1
* Tuesday: 2
* Wednesday: 3
* Thursday: 4
* Friday: 5
* Saturday: 3
* Sunday: 3
* Raining: 4
* Snow: 5
* Nice weather: -2
* Last day of month: 5

## ClusterTruck Kitchens API

The following describes the kitchen API endpoint that will get you the `location` for each kitchen.

```
curl -sH"Accept: application/vnd.api.clustertruck.com; version=2" https://api.staging.clustertruck.com/api/kitchens | \
python -m json.tool | less
```
