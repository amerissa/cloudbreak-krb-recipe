# Cloudbreak Kerberos Recipe Generator

## Introduction:
The script generates two scripts to use as Recipes to enable Kerberos on any existing blueprint.
1. Preinstall Script to be run after Ambari install and before cluster install
2. Postinstall Script to be run after cluster create

The script runs through a questionnaire to generate the proper parameters.


## Modes of Operations:

1. Install local MIT KDC on the Ambari Server and run Kerberos local to the cluster
2. Connect to AD Server and attach hosts to AD using SSSD
3. Connect to an existing MIT KDC server.


## Usage:
> wget https://raw.githubusercontent.com/amerissa/cloudbreak-krb-recipe/master/generator.py > generator.py
>
> chmod 755 generator.py
>
> ./generator.py
