<h2>Steps:</h2>
<ol>
    <li>Install Python 3 (I have used v3.8)<br>
        to check the version of installed python type the commnad:<br>
        $<b>python3 --version</b>(GNU Linux)<br>
        ><b>python -V </b>(Windows)<br>
        </b>
    </li>
    <li>Create a virtual environment using the command:<br>
        $<b>python3 -m venv virtual_env_name</b><br>
    <h6> Note: Give any name, in this case it's <i>virtual_env_name</i> </h6>
    </li>
    <li>Navigate inside the virtual_env_name by using the command:<br>
        $<b>cd <i>virtual_env_name</i></b><br>
    </li>
    <li>To activate the virtual_env_name type the command:<br>
        $ <b>source bin/activate </b>or <b>cd bin && activate </b>(GNU Linux)<br>
        > <b><i>virtual_env_name</i>\Scripts\activate </b>or <b>cd Scripts && activate </b>(Windows)<br>
    </li>
    <li>To installed required libraries inside the virtual_env_name type the command:<br>
        before installing libraries check the contents of virtual_env_name by using the command:<br>
            $<b>pip freeze </b><br>
        $<b>pip install -r requirements.txt</b><br>
    </li>
    <li>Now verify the installation by again typing:<br>
        $<b>pip freeze</b><br>
    </li>
    <li> Unzip the folder and copy the folder GyStaQ inside the virtual_env_name<br>
    </li>
    <li>To run the project follow the below steps:<br>
        $<b>cd GyStaQ</b><br>
        $<b>ls</b><br>
        after executing ls command your file system should be something like this<br>
            ->accounts<br>
            ->classify<br>
            ->GyStaQ<br>
            ->home<br>
            ->templates<br>
            manage.py<br>
        Run the following commands:<br>
        $<b>python manage.py makemigrations</b><br>
        $<b>python manage.py migrate</b><br>
        $<b>python manage.py changepassword</b><br>
            It will ask you to change the password (current username and password are admin)<br>
        $<b>python manage.py collectstatic</b><br>
            This will create a new folder called assets which will contain all the static files used in the project<br>
        $<b>python manage.py runserver</b><br>
        And that's it. If everything went well project will be up and running<br>
    </li>
    <li>Also change the email settings in settings.py<br>
    </li>
    <li>Also give the absolute path to the pickled_model.pkl file inside classify app<br>
    </li>
    <li>To deactivate the virtual_env_name type the command:<br>
        $<b>deactivate</b><br>
    </li>
    <li>Run the server again and again, keep correcting the errors and have fun using GyStaQ Classifier<br>
    </li>
</ol>
