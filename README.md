Writing the wrongs, and reading the writes.

Source for read.murrielgrace.com 

# Running
Note to self:
- Clone repo `git clone git@github.com:murriel/read.murrielgrace.com.git`
- Enter directory `cd read.murrielgrace.com`
- Create branch `git checkout -b feature\some-name`
- To launch and view site locally, run `bundle exec jekyll serve`. This will launch a local web server, probably at http://127.0.0.1:4000/ Using this URL you can view and test changes to your site.
- Alternatively, and to avoid dependency hell, test using the jekyll image like so: 
JEKYLL_VERSION=3.8
docker run --rm --volume="$PWD:/srv/jekyll" --volume="$PWD/vendor/bundle:/usr/local/bundle" --env JEKYLL_ENV=development -p 4000:4000 jekyll/jekyll:$JEKYLL_VERSION jekyll serve
- Update the version number as needed

##################
Forked from Hydejack
The "Best Jekyll Theme by a Mile".
##################  
A sentiment to which I am inclined to agree.
