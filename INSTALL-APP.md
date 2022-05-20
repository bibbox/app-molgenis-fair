## Molgenis & FAIR Data Point Installation Instructions 

### Start Molgenis

Be patient this can take up to 5 minutes (its a huge app). The last message in the log should be something like this

`17-Sep-2021 07:24:16.134 INFO [main] org.apache.catalina.startup.HostConfig.deployDirectory Deploying web application directory [/usr/local/tomcat/webapps/ROOT]`

### Log in with the username admin and the password you specified in the installation. 
The default admin user name is admin. The admin password is set during the installation within **BIBBOX**.

![Screenshot01](assets/install-screen-01.png)

### Make all further configuration steps within the Molgenis app.
Further information can be found here https://molgenis.org/ and https://molgenis.gitbook.io/molgenis/.

#### Add and manage user permissions in the Admin/User Manager Menu.

![Screenshot02](assets/install-screen-02.png)

#### Upload data (template in /data/molgenis_fdp_template) using the Molgenis EMX format.
Other fromats like `.csv` and `.vcf` are also supported and can be nativly uploaded.

![Screenshot03](assets/install-screen-03.png)

#### Navigate through your data using the Navigator.

![Screenshot04](assets/install-screen-04.png)

#### Set up FAIR Data Point.

Execute jupyter notebook (/data/jupyter/fillFDP.ipynb)

    - sets up FDP using environment variables set in docker-compose.yml.template
    
    - sets User credentials (Mail: "albert.einstein@example.com", Password: "password")
      PLEASE CHANGE DEFAULT PASSWORD!

    - creates FDP data from imported molgenis data points (added to molgenis by uploading)

#### Change default password

Default username is "albert.einstein@example.com" and password is set to "password".
Log in at FAIR Data Point and change the password (top right corner: "edit profile")

![Screenshot05](assets/user_page_fdp.png)

## After the installation
Have a nice ride with the Admins youngtimer.

![FINAL](assets/install-screen-final.jpg)
