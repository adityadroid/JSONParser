# JSONParser

...

          List<NameValuePair> nameValuePair = new ArrayList<NameValuePair>(2);
            nameValuePair.add(new BasicNameValuePair("key1",value1));
            nameValuePair.add(new BasicNameValuePair("key2",value2));
           




            // Note that create product url accepts POST method
            JSONObject json = jsonParser.makeHttpRequest("http://www.adityagurjar.esy.es",
                    "POST", nameValuePair,"headervalue",headername);
                    ...
