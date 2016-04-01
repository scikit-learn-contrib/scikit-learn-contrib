scikit-learn-contrib is a github organization for gathering high-quality scikit-learn compatible projects. Each project's team is responsible for maintaining the project. This includes fixing bugs, reviewing pull requests and making releases.

# Why moving my project to scikit-learn-contrib?

* Visibility: be part of a growing ecosystem of scikit-learn compatible projects
* Collaboration: volunteers from around the world can join you in improving the project
* Quality: benefit from scikit-learn's experience in producing high-quality machine learning software
* Transfer: most popular estimators can eventually be promoted to scikit-learn
* URL: http://contrib.scikit-learn.org/project-name
 
# scikit-learn vs. scikit-learn-contrib

In scikit-learn, we are pretty selective on the algorithms we include: notoriety (number of citations), general usefulness, no external dependencies. See scikit-learn's [FAQ](http://scikit-learn.org/stable/faq.html) for more details. In contrast, these conditions are not necessary for inclusion in scikit-learn-contrib (although we do have a few technical requirements, see below). scikit-learn-contrib is the ideal choice for cutting-edge algorithms (e.g., the latest ICML or NIPS paper), domain-specific algorithms, library wrappers.

In addition, pull-requests on scikit-learn tend to take from a few weeks to a few months to review. In constrat, if the requirements below are satisfied, projects are expected to be accepted to scikit-learn-contrib within a few days.

# Requirements

* **scikit-learn compatible** ([check_estimator](http://scikit-learn.org/stable/modules/generated/sklearn.utils.estimator_checks.check_estimator.html) passed)
* Available on github
* Open-source license (BSD preferred but not mandatory)
* Documentation (guide, API reference, example gallery)
* Unit tests 
* Python3 compatible
* [PEP8](https://www.python.org/dev/peps/pep-0008/) compliant
* Continuous integration

To satisfy these requirements, the easiest way is to start your project from 
[project-template](https://github.com/scikit-learn-contrib/project-template), although this is not mandatory.

# Workflow

1. File a [request for inclusion](https://github.com/scikit-learn-contrib/scikit-learn-contrib/issues/new)
into scikit-learn-contrib.
2. The project undergoes a simple review by scikit-learn or scikit-learn-contrib members to check
that the above requirements are satisfied.
3. A team is created in the scikit-learn-contrib organization for your project.
4. [Transfer your project](https://help.github.com/articles/transferring-a-repository/) to the scikit-learn-contrib organization (transfer retains branches, stars, etc).
5. Fork the project in your account (this way, the old project URL is still valid).

# Project maintenance guidelines

1. Project name on pypi is sklearn-contrib-project-name (e.g., sklearn-contrib-lightning).
2. Upload documentation to your [gh-pages](https://help.github.com/articles/creating-project-pages-manually/) branch.
3. When changing the signature of a public function or class, the old signature must be supported for two releases.
4. The options of all estimators must have sensitible default values.
