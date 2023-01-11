# RT Las Palmas

make a Python virtualenv

    pip install -r requirements.txt
    nodeenv -p -n 12.13.1 --prebuilt



Start Docker first

Open VSCode in dev container mode
    code .
    # inside VSCode command pallet
    > remote-containers.openWorkspace

Install dependencies
    pip install -r requirements.txt

git pull / or in the "source control" on the menu left do sync push-pull

Make Changes then:
Save all

Any changes y media: git add .

Build site

    python build.py

Preview changes in browser (outside of container, separate terminal)

    file:///Users/randysmithphd/Documents/Archived/Websites/RTLasPalmas/build/index.html

git commit -am 'comment'

git push

Publish to gh-pages

    ghp-import -np build


Deploying to the Live Site
--------------------------

Follow the standard workflow.  Make changes, `python build.py` and preview locally from `build/`.
When ready, `ghp -np build/` & `git commit -am '<comment>'`.
Preview on GitHub (http://drrandal.github.io/BransonTablerockOasis/).
