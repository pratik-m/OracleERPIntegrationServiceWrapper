[![PyPI license](https://img.shields.io/pypi/l/OracleSaaSApiPy.svg)](https://pypi.python.org/pypi/OracleSaaSApiPy/)
[![PyPI version fury.io](https://badge.fury.io/py/OracleSaaSApiPy.svg)](https://pypi.python.org/pypi/OracleSaaSApiPy/)
[![PyPI pyversions](https://img.shields.io/pypi/pyversions/OracleSaaSApiPy.svg)](https://pypi.python.org/pypi/OracleSaaSApiPy/)

A simple lightweight API to interact with Oracle ERP integration Web Service.
The common operations used from the webservice are exposed as methods in the API. The parameters are kept to mimimum so that the user has to worry about the mandatory parameters to be submitted. 



Usage:
```
    >>> import OracleSaaSApi
    >>> erp = OracleSaaSApi.ErpServiceApi(url, username, password)
    >>> docId = erp.upload_file_to_ucm(file, ucm_account)
```

# Installation
```
   pip install OracleSaaSApiPy
```

# Methods available 
- upload_file_to_ucm: Uploads a file to the Universal Content Management server based on the document specified
- submit_ess_job_request: Submits an Scheduling job request for the specified job
- load_interface_file: Submits an 'Load Interface File for Import' job for the specified job
- process_interface_file: Execute the import process for the specified job
- get_ess_job_status: Obtains the request status of the submitted scheduled job
- load_and_import_data: Uploads a file to the Oracle UCM server based on the document specified and submits the scheduled job to import and process the uploaded file.
- download_ess_job_execution_details: Downloads the output of Enterprise Scheduling Service job and logs
