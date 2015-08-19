AngularJS Smartbank patch
=========

Repo to patch angular issues while waiting for upstream.

Bumping version
---------
Use rebase to bump the angular version. Assumes `git remote add upstream git@github.com:angular/angular.js.git`
Eg.

    git fetch upstream
    git rebase --onto v1.4.5 v1.4.4
    git push --force

Building AngularJS
---------
[Once you have your environment set up](http://docs.angularjs.org/misc/contribute) just run:

    grunt package


Publishing patched version to Smartbank/bower-angular
-------------
    ./scripts/bower/publish.sh --action=prepare
    ./scripts/bower/publish.sh --action=publish
