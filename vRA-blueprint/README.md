# HPE SimpliVity plugin for VMware vRealize Automation

Using the SimpiliVity-VRA-Package.zip file, creation of vRA XaaS blueprints and resource actions for HPE SimpliVity are automated.

The detailed procedure to import vRA blueprints is availble in the VMware vRealize documentation. [Click here](https://docs.vmware.com/en/vRealize-Automation/7.6/com.vmware.vra.prepare.use.doc/GUID-43E01B1E-3C01-4F25-961C-F5554D15F7A5.html)

## Steps using vRealize cloudclient

The steps to install blueprints using the vRealize CloudClient are mentioned below:

1. Download the VMware cloudclient and extract the compressed file

2. Browse to the bin folder and run the cloudclient

3. Login to the vra using cloudclient

``` vra login userpass --user <vra-user> --tenant <vra-tenant> --server <vra-server> ```

Replace vra-user, vra-tenant and vra-server with actual 

4. Copy the SimpliVity-VRA-Package.zip file to bin folder

5. Using dryrun, check if there are any issues in importing the SimpliVity vRA packages 

``` vra content import --path SimpiliVity-VRA-Package.zip --resolution SKIP --dry-run yes --verbose yes ```

If there are no errors in above output, proceed to next step. If there are any errors, fix them and repeat this step again.

6. Import the SimpliVity VRA package using the below command

``` vra content import --path SimpiliVity-VRA-Package.zip --resolution SKIP --verbose yes ```

7. If the command is successful, vRA XaaS blueprints for SimpliVity is automatically created.
