https:- 

1. Generate a keystore that exposes your server’s credentials.
    For example, run the following command:

      keytool -genkey -keyalg RSA -alias <key-alias> -keystore <keystore-name>.jks
    Example:- 
        keytool -genkey -alias https-keystore -keystore keystore-https.jks -keyalg RSA -storetype JKS
  
  
  
  
If you want your certificate signed by a Certification Authority (CA), follow these steps:

2.  Export your certificate in the standard CSR format. To do so you can run this command:

      keytool -certreq -keystore <keystore-name>.jks -alias <key-alias> -file <certificate-name>.cer  
   Example:-
        keytool -export -alias https-keystore -keystore keystore-https.jks -file keystore-certificate.cer
