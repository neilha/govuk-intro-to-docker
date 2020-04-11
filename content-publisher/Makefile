content-publisher:
	docker-compose run content-publisher-demo-lite rbenv install -s
	docker-compose run content-publisher-demo-lite sh -c 'gem install --conservative --no-document bundler -v $$(grep -A1 "BUNDLED WITH" Gemfile.lock | tail -1)'
	docker-compose run content-publisher-demo-lite bundle install
	docker-compose run content-publisher-demo-lite bundle exec rake db:setup