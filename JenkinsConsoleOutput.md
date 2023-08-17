Started by user ty sand
Obtained Jenkinsfile from git https://github.com/Sameen-k/Deployment1.1.git
[Pipeline] Start of Pipeline
[Pipeline] node
Running on Jenkins in /var/lib/jenkins/workspace/Sameen_K_1.1
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: git
No credentials specified
Cloning the remote Git repository
Cloning repository https://github.com/Sameen-k/Deployment1.1.git
 > git init /var/lib/jenkins/workspace/Sameen_K_1.1 # timeout=10
Fetching upstream changes from https://github.com/Sameen-k/Deployment1.1.git
 > git --version # timeout=10
 > git --version # 'git version 2.34.1'
 > git fetch --tags --force --progress -- https://github.com/Sameen-k/Deployment1.1.git +refs/heads/*:refs/remotes/origin/* # timeout=10
 > git config remote.origin.url https://github.com/Sameen-k/Deployment1.1.git # timeout=10
 > git config --add remote.origin.fetch +refs/heads/*:refs/remotes/origin/* # timeout=10
Avoid second fetch
 > git rev-parse refs/remotes/origin/main^{commit} # timeout=10
Checking out Revision c05ee1f9ffd174ca069c0ef2feb5528cc05024ee (refs/remotes/origin/main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f c05ee1f9ffd174ca069c0ef2feb5528cc05024ee # timeout=10
Commit message: "Add files via upload"
First time build. Skipping changelog.
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Build)
[Pipeline] sh
Requirement already satisfied: pip in ./test3/lib/python3.10/site-packages (22.0.2)
Collecting pip
  Using cached pip-23.2.1-py3-none-any.whl (2.1 MB)
Installing collected packages: pip
  Attempting uninstall: pip
    Found existing installation: pip 22.0.2
    Uninstalling pip-22.0.2:
      Successfully uninstalled pip-22.0.2
Successfully installed pip-23.2.1
Collecting attrs==22.1.0 (from -r requirements.txt (line 2))
  Using cached attrs-22.1.0-py2.py3-none-any.whl (58 kB)
Collecting click==8.1.3 (from -r requirements.txt (line 3))
  Using cached click-8.1.3-py3-none-any.whl (96 kB)
Collecting flask==2.2.2 (from -r requirements.txt (line 4))
  Using cached Flask-2.2.2-py3-none-any.whl (101 kB)
Collecting iniconfig==1.1.1 (from -r requirements.txt (line 5))
  Using cached iniconfig-1.1.1-py2.py3-none-any.whl (5.0 kB)
Collecting itsdangerous==2.1.2 (from -r requirements.txt (line 6))
  Using cached itsdangerous-2.1.2-py3-none-any.whl (15 kB)
Collecting jinja2==3.1.2 (from -r requirements.txt (line 7))
  Using cached Jinja2-3.1.2-py3-none-any.whl (133 kB)
Collecting markupsafe==2.1.1 (from -r requirements.txt (line 8))
  Using cached MarkupSafe-2.1.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (25 kB)
Collecting packaging==21.3 (from -r requirements.txt (line 9))
  Using cached packaging-21.3-py3-none-any.whl (40 kB)
Collecting pluggy==1.0.0 (from -r requirements.txt (line 10))
  Using cached pluggy-1.0.0-py2.py3-none-any.whl (13 kB)
Collecting py==1.11.0 (from -r requirements.txt (line 11))
  Using cached py-1.11.0-py2.py3-none-any.whl (98 kB)
Collecting pyparsing==3.0.9 (from -r requirements.txt (line 12))
  Using cached pyparsing-3.0.9-py3-none-any.whl (98 kB)
Collecting pytest==7.1.2 (from -r requirements.txt (line 13))
  Using cached pytest-7.1.2-py3-none-any.whl (297 kB)
Collecting tomli==2.0.1 (from -r requirements.txt (line 14))
  Using cached tomli-2.0.1-py3-none-any.whl (12 kB)
Collecting werkzeug==2.2.2 (from -r requirements.txt (line 15))
  Using cached Werkzeug-2.2.2-py3-none-any.whl (232 kB)
Installing collected packages: iniconfig, tomli, pyparsing, py, pluggy, markupsafe, itsdangerous, click, attrs, werkzeug, packaging, jinja2, pytest, flask
Successfully installed attrs-22.1.0 click-8.1.3 flask-2.2.2 iniconfig-1.1.1 itsdangerous-2.1.2 jinja2-3.1.2 markupsafe-2.1.1 packaging-21.3 pluggy-1.0.0 py-1.11.0 pyparsing-3.0.9 pytest-7.1.2 tomli-2.0.1 werkzeug-2.2.2
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (test)
[Pipeline] sh
============================= test session starts ==============================
platform linux -- Python 3.10.12, pytest-7.1.2, pluggy-1.0.0 -- /var/lib/jenkins/workspace/Sameen_K_1.1/test3/bin/python3
cachedir: .pytest_cache
rootdir: /var/lib/jenkins/workspace/Sameen_K_1.1
collecting ... collected 1 item

test_app.py::test_home_page PASSED                                       [100%]

- generated xml file: /var/lib/jenkins/workspace/Sameen_K_1.1/test-reports/results.xml -
============================== 1 passed in 0.14s ===============================
Post stage
[Pipeline] junit
Recording test results
[Checks API] No suitable checks publisher found.
[Pipeline] }
[Pipeline] // stage
[Pipeline] }
[Pipeline] // withEnv
[Pipeline] }
[Pipeline] // node
[Pipeline] End of Pipeline
Finished: SUCCESS
