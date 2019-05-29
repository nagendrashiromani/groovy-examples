def sites = ["eenadu-nonworking":"https://www.eenadu.ne/","eenadu":"https://www.eenadu.net/","http-200":"https://httpstat.us/200","http-500":"https://httpstat.us/500"]
for(site in sites){
 try{
 	responseCode = site.value.toURL().openConnection().responseCode
   if(responseCode!=200){
     println("Unable to connect to $site.key, error code is "+responseCode)
   }else{
     println("Connection successful for $site.key")
   }
  }catch(Exception e){
  println("cannot connect :"+site.key) 
 }
}
