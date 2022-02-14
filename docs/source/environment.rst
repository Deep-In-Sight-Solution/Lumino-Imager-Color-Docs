Skip to content
Search or jump to…
Pulls
Issues
Marketplace
Explore
 
@iamjy 
iamjy
/
dtk4412-doc
Public
Code
Issues
Pull requests
Actions
Projects
Wiki
Security
More
dtk4412-doc
/
docs
/
source
/
building.rst
in
main
 

Spaces

4

Soft wrap
1
Installation
2
============
3
​
4
Install the package (or add it to your ``requirements.txt`` file):
5
​
6
.. code:: console
7
​
8
    $ pip install sphinx_rtd_theme
9
​
10
In your ``conf.py`` file:
11
​
12
.. code:: python
13
​
14
    import sphinx_rtd_theme
15
​
16
    extensions = [
17
        ...
18
        'sphinx_rtd_theme',
19
    ]
20
​
21
    html_theme = "sphinx_rtd_theme"
22
​
23
.. seealso::
24
    :ref:`supported-browsers`
25
        Officially supported and tested browser/operating system combinations
26
​
27
    :ref:`supported-dependencies`
28
        Officially Supported versions of Python, Sphinx, and other dependencies.
29
​
30
.. note::
31
​
32
   Adding this theme as an extension is what enables localization of theme
33
   strings in your translated output. If these strings are not translated in
34
   your output, either we lack the localized strings for your locale, or you
35
   are using an old version of the theme.
36
​
37
Via Git or Download
38
-------------------
39
​
40
.. warning::
41
​
42
   Installing directly from the repository source is deprecated and is not
43
   recommended. Static assets won't be included in the repository starting in
44
   release :ref:`3.0.0`.
45
​
@iamjy
Commit changes
Commit summary
Create building.rst
Optional extended description
Add an optional extended description…
 Commit directly to the main branch.
 Create a new branch for this commit and start a pull request. Learn more about pull requests.
 
© 2022 GitHub, Inc.
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About
