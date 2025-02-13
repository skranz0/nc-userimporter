# About nc-userimporter

[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

This tool creates Nextcloud users from a CSV file, which you exported from some other software or created with a spreadsheet software.

## Instructions

1. Download and extract the zip-file
   * in the repository: click "code"--> "download zip"
   * OR: [here](https://github.com/t-markmann/nc-userimporter/archive/refs/heads/master.zip)

2. Insert data:
    * __config.xml__: Insert your cloud-admin credentials into file _config.xml_. The user must have admin permissions in your Nextcloud.
    * __users.csv__: Insert the user data into the file _users.csv_ or recreate it with the same columns in a spreadsheet software.

3. Start the tool:
    * __Windows__: doubleclick _nc-user-manager.exe_.
    * __Linux__ / __Mac__: install all [dependencies](https://github.com/t-markmann/nc-userimporter/wiki#install-dependencies-for-running-py-script) and run: python3 nc-userimporter.py
        * __Troubleshooting__: Make sure the file is executable (Help for [Linux](https://www.qwant.com/?q=make%20file%20executable%20linux) and [MacOS](https://www.qwant.com/?q=make%20file%20executable%20mac)

4. Follow the interactive commandline instructions. Check output.log ("logs"-folder in script-directory) and your user overview in Nextcloud.

## Output

Screenshot output example:

![Generated PDF file with user credentials](https://github.com/t-markmann/nc-userimporter/blob/master/assets/screenshot_pdfoutput.png)

---

## ToDo

* improve documentation of features in the [wiki](https://github.com/t-markmann/nc-userimporter/wiki#todo-documentation)

Open features, not yet implemented (help appreciated):

* read config from CLI-input if config-file is empty; update config.xml with input values?
* add other userdata
