https://docs.djangoproject.com/en/3.0/intro


### Run
`python3 manage.py runserver`

runs the polls app at http://127.0.0.1:8000/polls

Throw an error by visiting http://127.0.0.1:8000/polls/sentry-debug

### Release

Current sentry release: a0bd33447a44cca2dbc637d3c05f2f9a0de1e73c

+-----------------------+--------------+
| Repository            | Revision     |
+-----------------------+--------------+
| slohmes/bb-py-project | c9558f4a3784 |
+-----------------------+--------------+

##### To create a new release:
1. (If you haven't since last commit:) `cd .. && cd bb-py-project` to re-evaluate $VERSION to latest commit hash
2. Create release: `./node_modules/.bin/sentry-cli releases new -p python $VERSION`
3. Associate commits with release: `./node_modules/.bin/sentry-cli releases set-commits --auto $VERSION`
5. Finalize release: `./node_modules/.bin/sentry-cli releases finalize "$VERSION"`


### Sources
* https://docs.djangoproject.com/en/3.0/intro
* https://docs.sentry.io/platforms/python/django/
* https://docs.sentry.io/workflow/releases/?platform=python