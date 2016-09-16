# JSONParser

This Library aims to simplify the code needed to be written in order to make a HTTP GET/POST request.

Step 1:

add
JSONParser.java to your Android Project.

Step 2:
Make HTTP POST/GET Requests as follows:

```

        public JSONObject makeHttpRequest(String url, String method,
           List<NameValuePair> params,String headerName,String headerValue)
         
```

this method is used to make HTTP requests. A simple demo of its usage :



```

          //Put your Key - Value Params here
          List<NameValuePair> nameValuePair = new ArrayList<NameValuePair>(2);
            nameValuePair.add(new BasicNameValuePair("key1",value1));
            nameValuePair.add(new BasicNameValuePair("key2",value2));
              
              //Creating a instance of JSONParser
               JSONParser jsonParser = new JSONParser();



          //making HTTP POST request 
            JSONObject json = jsonParser.makeHttpRequest(SERVICE_URL,
                    "POST", nameValuePair,"headervalue",headername);
          
          //Perform operations on JSON object.
                  
 ```  
 
 
 to get Status Code as return use  StatusCode() method
 Demo:
 
 ```
 
  
              //Creating a instance of JSONParser
               JSONParser jsonParser = new JSONParser();

             JSONObject json = jsonParser.makeHttpRequest(SERVICE_URL,
                    "GET", nameValuePair,"headervalue",headername);


           int statusCode= jsonParser.StatusCode();
           
           //Perform operations according to status code
 ```
 
 PS:

To pass multiple headers, modify the JSONParser class accordingly.
 
                    
