# RT Las Palmas

make a Python virtualenv

    pip install -r requirements.txt
    nodeenv -p -n 12.13.1 --prebuilt

To build:

    python build.py

Built site is in build directory.

    open build/index.html

To push to gh-pages

    ghp-import -np build
