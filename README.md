# Using a RESTful API for a Beginner

The [Facebook Graph API](https://developers.facebook.com/docs/graph-api/overview) allows developers to receive data, post data, or rearrange items on Facebook's web pages. The API categorizes Facebook pages into three areas: 

<table>
  <col width="50%">
  <col width="50%">
  <tr>
    <th>Name</th>
    <th>Description</th>      
  </tr>
  <tr>
    <td>Nodes</td>
    <td>Nouns or objects. Often something<br> that can be seen visually on a page</td>      
  </tr>
  <tr>
    <td>Edges</td>
    <td>The connections or linking between<br> the nodes or objects</td>        
  </tr>
  <tr>
    <td>Fields</td>
    <td>Available data on the nodes</td>
  </tr>
</table>

<br>

Similar to other social media RESTful APIs, data for a specific page, or even node, can be requested through a web link. For example, place the address **`graph.facebook.com/comcast`** into a web browser. A page with numerous return results should appear. Pictured below is the data received from the API call and actual Comcast Facebook page:

![Graph API Comcast](https://raw.githubusercontent.com/techwriterjoe/restful-api-apis-beginner/master/comcast.png)

Notice some of the Graph API's results and compare them to the actual page:

- Listed on both is the number of likes, 352
- Listed on both is the company website
- From the API's results, Facebook has categorized Comcast as a company

##RESTful APIs Typically Have Four Actions

1. GET: to recieve data from the source, already demonstrated with the Comcast Facebook page
2. POST: sends completely new data
3. PUT: updates existing data
4. DELETE: deletes existing data on the source
  1. Stay away from the term "request" when describing any four of these actions
  2. GET is similar to the traditional "getter"
  3. POST and PUT are similar to the traditional term "setter"

> Facebook's Graph API has SDKs for many CS languages. To start examing what a RESTful API call looks like, examine
> the JavaScript below:

```javascript
var xhr = new XMLHttpRequest();
xhr.open("GET", "http://graph.facebook.com/comcast", false);
xhr.send();
console.log(xhr.status);
```

This article will be lengthened in the future. Hope you enjoyed the read so far. 

