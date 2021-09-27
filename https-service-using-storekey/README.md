https:- 

1. Generate a keystore that exposes your server’s credentials.
    For example, run the following command:

      keytool -genkey -keyalg RSA -alias <key-alias> -keystore <keystore-name>.jks
  
  
  
  
If you want your certificate signed by a Certification Authority (CA), follow these steps:

2.  Export your certificate in the standard CSR format. To do so you can run this command:

      keytool -certreq -keystore <keystore-name>.jks -alias <key-alias> -file <certificate-name>.csr  
