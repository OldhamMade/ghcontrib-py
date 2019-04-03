# ghcontrib

Small python script which calculates a user's contributions to a
github-hosted project based on PR details.

# Dependencies

* Python 2.7
* A [Personal Access Token](https://github.com/settings/tokens)

Note: this script relies on [grequests](https://github.com/kennethreitz/grequests)
which in turn relies on [gevent](http://www.gevent.org).

# Installation

Note: we recommend using `virtualenv` when installing python dependencies.

    $ git clone {repo.git} ghcontrib
    $ cd ghcontrib
    $ virtualenv .venv
    $ . .venv/bin/activate
    $ pip install -r requirements.txt

# Usage

    $ python ghcontrib <user> <project> <repo> --token=<authtoken>

The script also accepts an `--exclude=<id>[,<id>...]` parameter for
any PR numbers you wish to have excluded from the final tally.

# Licence

[MIT](https://choosealicense.com/licenses/mit/)
