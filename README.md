# ssl_generator


### Clone

- git clone

      git clone https://github.com/marcus-sds/ssl_generator
      cd ssl_generator

### Domain modification

- vi ssl_generator.sh

      [alt_names]
      DNS.1 = *.${domain}
      DNS.2 = *.test.${domain}

> Can add multiple DNS

- additional information modification if required

      [ req_distinguished_name ]
      countryName = KR
      stateOrProvinceName = Seoul
      localityName = Seoul
      organizationalUnitName = CloudOperationGroup
      0.organizationName = SamsungElectronics


### Run script

bash ./ssl_generator.sh [domain]

      bash ./ssl_generator.sh test.io

> Result shows the ssl information 

### Results file

- key file - private key file 

- csr file - cert request file

- crt file

