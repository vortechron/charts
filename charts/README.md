How It Works
I set up GitHub Pages to point to the docs folder. From there, I can create and publish docs like this:

$ helm create mychart
$ helm package mychart
$ mv mychart-0.1.0.tgz docs
$ helm repo index docs --url https://technosophos.github.com/tscharts
$ git add -i
$ git commit -av
$ git push origin master

From there, I can do a helm repo add tscharts https://technosophos.github.com/tscharts

helm package charts/laravel && helm repo index . --url https://vortechron.github.io/charts/
