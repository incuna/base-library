# `base_library`

A copy-and-pasteable base set of files, tests, and so on that allow quick setup of new libraries.

Contains:
- A top-level package with a `tests` folder.
- A `test_project` folder from which tests and the Django server are run.
- A base user factory (using `django.contrib.auth.get_user_model`) and a `RequestTestCase` derived from it.
- A makefile that handles tests, migrations and running a server.

There are a number of `TODO`s in this project that mark the holes that will most commonly need to be filled in.  Searching for the string `TODO` (not as a whole word) should find them all.  The most notable are:
- `TODO_PACKAGE_NAME` - replace this string everywhere with the name of the top-level package of your library.
- `TODO_PROJECT_NAME` - replace this string everywhere with the name of the repository.
- `setup.py` has a `TODO` in the description field.
- `requirements.txt` may need updating to use latest versions of dependencies.

Once that is done, check whether you need any particular component and delete it if necessary.

After setup, make sure to do the following:
- This base library doesn't install Django for you, so in order to run it you'll need to manually install whichever version of Django you need.
- Activate the library on Travis (then make a push to the repository).
- Replace this readme with information about your project.
