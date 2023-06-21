# Surveying-GPS-based-Machine-Learning-Earthquake-Alternative-Routing-Detector-in-Automobiles


<b> Research and Development (R & D) Proposal | Surveying Global Positioning System (GPS)-based Machine Learning Earthquake Alternative Routing Detector in Automobiles </b>

<b> Developer - Carl Vincent A. Reyno </b>
----

[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/mathworks/jupyter-matlab-proxy/run-tests.yml?branch=main&logo=github)](https://www.mathworks.com)

<!--![Matlab_Logo](https://user-images.githubusercontent.com/79138019/236503435-3328be99-f523-4b4b-9039-269bbf6a5ca9.png) -->

<img src="https://github.com/Eevalice/Surveying-GPS-based-Machine-Learning-Earthquake-Alternative-Routing-Detector-in-Automobiles/assets/79138019/c098e9a6-6545-4687-9ed3-b45d9d5ca342" width="200" height="200" />

<img src="https://github.com/Eevalice/Surveying-GPS-based-Machine-Learning-Earthquake-Alternative-Routing-Detector-in-Automobiles/assets/79138019/e70e2339-c4d8-4874-b3bd-fab5a14b2dfc" width="600" height="300"/>




---
This application displays a list of recent earthquakes and alerts the user of the automobiles which instructs an alternative paths or routes for safety precautions, this application is developed to prevent casualties and avoid dangerous paths or routes in the Philippines.

<b>Developing/Coding In Progress</b>
<i>Jupyter/Python/Django Workspace</i>

```python
import os, sys
PWD = os.getenv('PWD')

PROJ_MISSING_MSG = """Set an enviroment variable:\n
`DJANGO_PROJECT=your_project_name`\n
or call:\n
`init_django(your_project_name)`
"""

def init_django(project_name=None):
    os.chdir(PWD)
    project_name = project_name or os.environ.get('DJANGO_PROJECT') or None
    if project_name == None:
        raise Exception(PROJ_MISSING_MSG)
    sys.path.insert(0, os.getenv('PWD'))
    os.environ.setdefault('DJANGO_SETTINGS_MODULE', f'{project_name}.settings')
    os.environ["DJANGO_ALLOW_ASYNC_UNSAFE"] = "true"
    import django
    django.setup()

